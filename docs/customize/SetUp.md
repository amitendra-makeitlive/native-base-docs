<div id="themingNativeBaseApp">

    <h1>Theming NativeBase Apps</h1>

    <p>
        Customizing <a href="http://nativebase.io/">NativeBase</a> will be a cakewalk for you. That is due to the fact, <a href="http://nativebase.io/">NativeBase</a> has categorized its screens into different sections. It provides a separate file inclusive of color schemes for different sections.
        <br /><br />

        <i>
            <b>Note:</b> <a href="http://nativebase.io/">NativeBase</a> is built on top of <a href="https://facebook.github.io/react-native/">React Native</a>.<br />
            Hence with any component you can pass the style property which will be merged to the default style of that component.<br /><br />
        </i>
    </p>

    <p>
        Steps to be followed to customize NativeBase theme:
        <ul>
            <li>
                Copy the file <code>light.js</code>
                <font size="2">
                    <i>(/node_modules/native-base/Components/Themes/light.js)</i>
                </font>
            </li>
            <li>
                Create a folder <code>Themes</code> under your rootProject and paste the file here.<br />
                Say <code>myTheme.js</code>
            </li>
            <li>
                Import the file Themes/myTheme.js into your code.<br />
                Make the necessary theme changes into myTheme.js.
            </li>
            <li>
                Include prop <code>theme</code> with the component whose theme you wish to change.
            </li>
        </ul>

        Now your project is ready for theme customization.
    </p>
</div>

<div class="section" id="theme">

    <i>General Syntax</i>
<pre class="line-numbers"><code class="language-jsx">import {Container, Content, Text} from 'native-base';
import React, {Component} from 'react-native';
import myTheme from './Themes/myTheme';
​
export default class ThemeExample extends Component {
    render() {
        return (
            &lt;Container>
                &lt;Content theme={myTheme}>
                    &lt;Text>
                        I have changed the text color.
                    &lt;/Text>
                &lt;/Content>
            &lt;/Container>
        );
    }
}</code></pre><br />

    <ul>
        <li>
            The <code>theme</code> prop can be applied to any component of NativeBase.
        </li>
        <li>
            The theme holds good with all its descendants.
        </li>
        <li>
            The above code for theme change works this way:<br />
            Go to Themes/myTheme.js and modify color code for <code>textColor</code>.
        </li>
        <li>
            Similarly you can customize theme for the rest of NativeBase components by modifying color code of their respective attributes, some of which are explained below.
        </li>
    </ul><br />


</div>