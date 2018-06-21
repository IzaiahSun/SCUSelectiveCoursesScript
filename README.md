# SCUSelectiveCoursesScript

It is a brief illustration about how to just POST data to the server without browser the webpage to choose course.

## Login

POST your ID and your password to this address to login

    http://202.115.47.141/loginAction.do

<html>
    <table>
    <thead>
    <th>Parameters</th>
    <th>Value</th>
    <th>Example</th>
    </thead>
    <tr><td>zjh</td><td>Your School Number</td><td>2017123456789</td></tr>
    <tr><td>mm</td><td>Your Password</td><td>123456</td></tr>
    </table>
</html>

## Select Course

POST the following data to this address to choose course

    http://202.115.47.141/xkAction.do

Firstly, post these data
<html>
    <table>
    <thead>
    <th>Parameters</th>
    <th>Value</th>
    <th>Example</th>
    </thead>
    <tr><td>kch</td><td>Your Course Number</td><td>999000000</td></tr>
    <tr><td>cxkxh</td><td>Your Course Index</td><td>01</td></tr>
    <tr><td>kcm</td><td>Keep It Empty</td><td></td></tr>
    <tr><td>skjs</td><td>Keep It Empty</td><td></td></tr>
    <tr><td>kkxsjc</td><td>Keep It Empty</td><td></td></tr>
    <tr><td>skxq</td><td>Keep It Empty</td><td></td></tr>
    <tr><td>skjc</td><td>Keep It Empty</td><td></td></tr>
    <tr><td>pageNumber</td><td>Do It As Example Do</td><td>-2</td></tr>
    <tr><td>proActionType</td><td>Do It As Example Do</td><td>2</td></tr>
    <tr><td>actionType</td><td>Do It As Example Do</td><td>5</td></tr>
    </table>
</html>
Then post these data
<html>
    <table>
    <thead>
    <th>Parameters</th>
    <th>Value</th>
    <th>Example</th>
    </thead>
    <tr><td>kcld</td><td>Your Course And Your Course Index With A Space Between Them</td><td>999000000 01</td></tr>
    <tr><td>proActionType</td><td>Do It As Example Do</td><td>5</td></tr>
    <tr><td>actionType</td><td>Do It As Example Do</td><td>9</td></tr>
    </table>
</html>
After that you can use GET method to get the page to check whether you have successfully choose the course. 

    http://202.115.47.141/xkAction.do
