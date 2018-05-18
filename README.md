# Email class PHP google

include file:
<pre>
include_once 'email_class.php';
</pre>

example:

<pre>
$from = 'info@domain.com';
$to = 'ivan@example.com';
$message = '
&lt;html&gt;
&lt;head&gt;
&lt;title&gt;' . $subject . '&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;table&gt;
&lt;tr&gt;
&lt;td&gt;
Best regards, exemple team
&lt;/td&gt;
&lt;/tr&gt;
&lt;/table&gt;     
&lt;/body&gt;
&lt;/html&gt;     
';
      
      

$mail = new Mail($from);
$mail->setFromName($from);
$mail->send($to, $subject, $message);
</pre>

