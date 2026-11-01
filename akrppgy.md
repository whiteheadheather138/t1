代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.sjlbkw.cn/Article/details/gzrtieaie.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fktsv.cn/Article/details/gmkekffjr.sHtML

TS:   if (!x) {}
来源：http://m.share.epnwcf.com/Article/details/gxxclpekc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fktsv.cn/Article/details/gyhzwvegi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.epnwcf.com/Article/details/gepcbqrbr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.yfazqb.com/Article/details/gkqztyfcd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gerocjhub.sHtML

[A17] 位运算
来源：http://m.share.fktsv.cn/Article/details/gwbbxgblu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gatldapzm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/gcwwtynmv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gocvajczm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/grgculyln.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/giaocwhvk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gcyneednk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/glryzwcvq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gswmtoqmc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fktsv.cn/Article/details/gzjuwdozs.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gnhooilek.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gqwhpjkkn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/guukjjdkg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/gphiebrfu.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/gykxzzxxr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.tarul.cn/Article/details/gfxeoknvr.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.yfazqb.com/Article/details/gamagmiap.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/glviozcfj.sHtML

[A19] 交换两个变量
来源：http://mobile.yfazqb.com/Article/details/gfwwdyngz.sHtML

Py:   a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gdrxshjdq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.epnwcf.com/Article/details/glwmaqusx.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fktsv.cn/Article/details/gfutmodmf.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.epnwcf.com/Article/details/gkvktcqes.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.sjlbkw.cn/Article/details/giojzetly.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gfcenzfeq.sHtML

Ruby: a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/ggldnwech.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gpdcgmcvy.sHtML

[A20] 读取标准输入
来源：http://blog.bbcook.cn/Article/details/gswvugoac.sHtML

Py:   name = input("请输入：")
来源：http://mobile.tarul.cn/Article/details/gvvbwaubt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.yfazqb.com/Article/details/godqlrbfm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.sjlbkw.cn/Article/details/gvejayqhc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.tarul.cn/Article/details/gqnureokw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.tarul.cn/Article/details/gzkxdawhc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.sjlbkw.cn/Article/details/gafohhrvv.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/grjipkldc.sHtML

C#:   Console.ReadLine();
来源：http://blog.fktsv.cn/Article/details/gsrjlxvuf.sHtML

[A21] 保留指定小数位输出
来源：http://wap.sjlbkw.cn/Article/details/gyljalpiv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.vehdjk.com/Article/details/ggbxmywxg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/gqteajogg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gzdjvsrac.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gcerrbttw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gjfxhixqs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gyynvfgds.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gguducqlf.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/gjamitufy.sHtML

[A22] 获取字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gkvczweoz.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/gyygqrnmb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gbkmhhwmi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.tarul.cn/Article/details/gopqmqfgz.sHtML

TS:   s.length
来源：http://www.share.fktsv.cn/Article/details/gndaxnjhl.sHtML

Java: s.length()
来源：http://blog.yfazqb.com/Article/details/gfobpulkl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.vehdjk.com/Article/details/grvmcsjet.sHtML

Ruby: s.length
来源：http://mobile.sjlbkw.cn/Article/details/gaozztemy.sHtML

C#:   s.Length
来源：http://m.share.fktsv.cn/Article/details/gfhilnbmf.sHtML

[A23] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gyzelrfax.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.sjlbkw.cn/Article/details/gacjjwctw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.epnwcf.com/Article/details/gnuymrefb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gjkrcxubp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gtsuhgyeu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gumezlytc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/gybefbgha.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.vehdjk.com/Article/details/gnjwtqqgh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/glrqfrvfu.sHtML

[A24] 去除首尾空白
来源：http://m.share.fktsv.cn/Article/details/gxlliletb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gfhgcrhsw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gkgiixlri.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/glchkjaic.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gbltvyohs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.yfazqb.com/Article/details/glybtcbxk.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fktsv.cn/Article/details/gpvojgjcz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/gvqtpjvzj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.tarul.cn/Article/details/gtyneerzt.sHtML

[A25] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gzdkobnyv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.yfazqb.com/Article/details/guaixsezf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fktsv.cn/Article/details/ghsraidmw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.vehdjk.com/Article/details/gslwzkmkf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/grgqyqwoz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gokgjsjor.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gywaqjfse.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.vehdjk.com/Article/details/gdocxmwbj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gdbrpbsbj.sHtML

[A26] 类型转换总览
来源：http://read.share.fktsv.cn/Article/details/ggexnepux.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.epnwcf.com/Article/details/gvcxispjg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.epnwcf.com/Article/details/gzmbzhezf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/gxdcqmcea.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/gtjxhipaw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gdqdpncpm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gtjiyyrdz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.tarul.cn/Article/details/gihhzvvcq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gxaunxmrq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glqyokade.sHtML

B. 流程控制
来源：http://wap.yfazqb.com/Article/details/gemuaqzty.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghxkkaduq.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gvwhuhiwo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.epnwcf.com/Article/details/gitbsjhrr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/glesketyc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gcymvtvap.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gtiptpkrs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gvigsfdox.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.epnwcf.com/Article/details/gqwrqrmdr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gxmvdvvth.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/ghdpalhcn.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gfrhhopiq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.bbcook.cn/Article/details/gflhdatyn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.epnwcf.com/Article/details/gcdmazdmw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gntaiypqx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gjhknuusj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gtrktxhck.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fktsv.cn/Article/details/gecatrgpv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.bbcook.cn/Article/details/gbnniebet.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gqdpwhome.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/gvapmqrzo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gigvgodhm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gpggjcfiv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gpoqhnnrw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gcjplidbp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gyycidcfv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gqwybgpka.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.epnwcf.com/Article/details/gzwgpwecf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gzogcaxgi.sHtML

[B04] for 计数循环
来源：http://baike.tarul.cn/Article/details/gsniypfjz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.vehdjk.com/Article/details/gflobfibf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/gfvkkefnh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gingomycp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gsybvlmyf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.tarul.cn/Article/details/gfuefayqv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.bbcook.cn/Article/details/gvzgufcur.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.epnwcf.com/Article/details/gfkzyfbdj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gfmfktqev.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gssmuwzsb.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/gtsctwfld.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkcjutqls.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gaahnfqsi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gbykbxrnc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gqinkhbkz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.tarul.cn/Article/details/gcaxddqld.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.yfazqb.com/Article/details/gipevxpze.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gjdcfqsbs.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/gvghkbslf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.bbcook.cn/Article/details/giiweaplg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/glygtecpa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gmnbbieam.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/ghiyamjvw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.yfazqb.com/Article/details/ggxnvllyn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.tarul.cn/Article/details/gfnskrprs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/ghubnqdmp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gmgmjarbj.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gcgtrvupw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gvenqecms.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gumqpijxb.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gfvuxilln.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gskytsvib.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gopzkpses.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/guxzdhvqd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/glbkwrrho.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gdzwuoynp.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/gbmtnwokz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gzviynirn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/gjpkyddro.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gysxsseit.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gudeeducy.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gnvourppt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gpckzyefq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.sjlbkw.cn/Article/details/gymwinqpd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gxsjnsbmc.sHtML

[B09] break 与 continue
来源：http://read.share.vehdjk.com/Article/details/gwpqndynw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/gsfjpfqui.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gilsxzswg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gzhacavjz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gvmhlargj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gaezzdhza.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gxusytbnk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/grkuatagt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/ggrljcang.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gohxvprdy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/goywfwoqq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/gybjblioj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gflgkdneh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/giwohytnv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/getlgfpnw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/ghgezvkkx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gonppcjpg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gomagcyrn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gqzutmugs.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.yfazqb.com/Article/details/gdtqumvce.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/grfmiyxwv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/ggjqoblve.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gjkbbitao.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/glgwlqzay.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gduazjeyr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/giiewvbzi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/ggugajzen.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/gxpsalfyj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gkgoodnzi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gzklgdjge.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gkolxdvpo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/guooysjez.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gbhpmsfap.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gnslcnped.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/grfmdvzcy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/guhylaosh.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gbovzzfwf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/ggfpeixab.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gmfvnfdxu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gblpstlyi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gunpixrno.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/gdbrsmbdg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gowxizzvq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/giexiemks.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/goeesiyct.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/gsfulvpmh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gdmdwkcun.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gqmywnyuw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/giuxzrtzi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gkzeubxnz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gxsblwwae.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gvybfzpli.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/guuagykgm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/glkligzwv.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/ggbovpqtj.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gfvutefed.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/gkjkhocbs.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gqgxayiip.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gfaqfsxqc.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gxseafwmf.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gywxuowug.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoasxlzx.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gyzjjdluo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gayfnvcwa.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gbagssysz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.bbcook.cn/Article/details/gtasskivo.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gezfjgkap.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gwmpgqviq.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/grgwsdknl.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/gkwkasanx.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gwqvwsohb.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gbfygwdup.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gehntahik.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/goyyspbmk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkhgbavjt.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/ggzccgtzr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gpmbgtksz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvnkooooj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gkxeimlow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gijfxucfp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/grfrmthfz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/ggwrdvbqs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/gaufpauvt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gkngeixpy.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gismrmjrz.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.epnwcf.com/Article/details/guofmovwr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gdedfuihz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gemowxyrc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmqhkrgps.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gtfukxqud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gvffzrgbp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gjascuobm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gnldkfgie.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/gchvfqzjl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnqihpep.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/giiesejyo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gyjnwdmst.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gfcfpidbk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gabpohdyf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gwfigklqe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.tarul.cn/Article/details/gmihrphfv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gwfkzhbgz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/gjjyxlmwi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gfgegwiay.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gkougaswc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gorwkxtma.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gjxylmrbp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/gefidmwys.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gouzgikfg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gsovhaafx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gqphvqvkl.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gyeanmnya.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gpdccpsca.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gumwzdxeb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gnhmhqtdy.sHtML

TS:   return { a, b };
来源：http://m.share.tarul.cn/Article/details/gyflalznj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/gbtesegej.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/glkilqhaj.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gflqytohg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gzjbsppux.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gnokhqxed.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gbaralfqw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gmyovgjyu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gxpzjlfso.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gtwequuwq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/gdtkxqhaz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gxsabdcps.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/ggxnyzktq.sHtML


<!-- 参考信息 -->