# Stringcom
<html>
	<head>
	<meta http-equiv="Content-Type" content="text/html; charset=gb2312">
	<script>
	function strcmp(s1,s2)
	{
	  len1=s1.length;
	  len2=s2.length;
	  while (1)
	  {
	      if (len1==0 && len2==0)
	          return 1;
	      if (len1==0 && len2!=0 || len1!=0 && len2==0)
	          return 0;
	      if (len1>0 && len2>0)
	      {
	          ch1=s1.charAt(0);   // 取字符串中的第1个字符
	          ch2=s2.charAt(0);
	          if (ch1!=ch2)
	             return 0;
	          else        
	          {
	             s1=s1.substring(1);  // 取第2个字符开始到字符串结束的所有字符
	             len1=s1.length;
	             s2=s2.substring(1); 
	             len2=s2.length;
	          }
	        }
	   }
	}
	</script>
</head>
	<body>
	<script>
	  str1=prompt("请输入一个字符串1:","");
	  str2=prompt("请输入一个字符串2:","");
	 
	  res=strcmp(str1,str2);
	  if (res==1)
	     document.write(str1+" = "+str2);
	  else 
	     document.write(str1+" != "+str2);
	     
	</script>
	</body>
	</html>
