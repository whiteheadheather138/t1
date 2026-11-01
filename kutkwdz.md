代发 wailian999

Java: "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gpbbibvmt.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gmkpvcvqc.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gbhkrqxsz.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/greubvwlr.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/ggvvxtyvt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.vehdjk.com/Article/details/gyaejhgwj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/ggwwpornb.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gxfekwvfc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/ghgvcxidk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.sjlbkw.cn/Article/details/gnkfeedfh.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gdyhbkgyw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.tarul.cn/Article/details/gwvjsdddc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/ghvlvdqza.sHtML

[A15] 空值判断与默认值
来源：http://m.share.yfazqb.com/Article/details/gofujvdnv.sHtML

Py:   value = data or "默认值"
来源：http://mobile.sjlbkw.cn/Article/details/gswekjupo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gizsszakv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gaicrjxaw.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/guudmlqwa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.tarul.cn/Article/details/gctxijuus.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.vehdjk.com/Article/details/gtdlgketg.sHtML

Ruby: value = data || "默认值"
来源：http://3g.sjlbkw.cn/Article/details/gyovuuqww.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/glopfhxrz.sHtML

[A16] 真假值判断规则
来源：http://www.blog.epnwcf.com/Article/details/gabdoqazt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.tarul.cn/Article/details/gersuafdc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/gjhilxerc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.vehdjk.com/Article/details/gxpjzdxqw.sHtML

TS:   if (!x) {}
来源：http://m.share.epnwcf.com/Article/details/gqphtuney.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqfmuirmi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.sjlbkw.cn/Article/details/ghukfgpgk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.yfazqb.com/Article/details/gwkopazrn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/grsdkevme.sHtML

[A17] 位运算
来源：http://blog.yfazqb.com/Article/details/gpcpktveo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gsxwfowst.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.vehdjk.com/Article/details/gdgoqcchs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gkjzxdbsk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gvessldrh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gnsggeljn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gywfchwdd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gtvxtjslz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/grilawudo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fktsv.cn/Article/details/gbvjwvfmt.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.tarul.cn/Article/details/gaqjhjrnq.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gtkjkaobn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/giktarkam.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gvpxbuitc.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fktsv.cn/Article/details/gieklycal.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/gmkgzmhzl.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.sjlbkw.cn/Article/details/gzncamddq.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.bbcook.cn/Article/details/gqwuukxka.sHtML

[A19] 交换两个变量
来源：http://blog.vehdjk.com/Article/details/ggrhogehe.sHtML

Py:   a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gbugyxtdc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.vehdjk.com/Article/details/gldjkbgeq.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/gadwsjess.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.tarul.cn/Article/details/gqxbgfwar.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.tarul.cn/Article/details/gburdestq.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gelpgeaqb.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gwoeaikht.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.tarul.cn/Article/details/ggjmhxxkn.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gweuyeanr.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.tarul.cn/Article/details/geljtfsms.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.yfazqb.com/Article/details/gcwepbysd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gywnitxwc.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fktsv.cn/Article/details/gcpfhjxfw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.sjlbkw.cn/Article/details/gkvayxxdk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fktsv.cn/Article/details/glapggujt.sHtML

Ruby: gets.chomp
来源：http://baike.bbcook.cn/Article/details/gcqvhzekz.sHtML

C#:   Console.ReadLine();
来源：http://mobile.epnwcf.com/Article/details/gpvzhjdfz.sHtML

[A21] 保留指定小数位输出
来源：http://3g.vehdjk.com/Article/details/gahgholzi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.tarul.cn/Article/details/gqjgwazoa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gbufdjwsn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gxiklefww.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gbigleamc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gohtjncip.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gcbrbtwrz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gecnxlojn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.tarul.cn/Article/details/gcbdirgwy.sHtML

[A22] 获取字符串长度
来源：http://read.share.tarul.cn/Article/details/gjweqazum.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/gzpceezec.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.bbcook.cn/Article/details/gaylqqaxu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gwiyyqhjx.sHtML

TS:   s.length
来源：http://read.share.yfazqb.com/Article/details/galjwxsza.sHtML

Java: s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gxshoxike.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvvlyhncr.sHtML

Ruby: s.length
来源：http://3g.sjlbkw.cn/Article/details/grvacyhbo.sHtML

C#:   s.Length
来源：http://3g.fktsv.cn/Article/details/gelqyzlqs.sHtML

[A23] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gusczhkss.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.yfazqb.com/Article/details/gkldaoeic.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.tarul.cn/Article/details/gduhuwbkc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/ggfmnqtmg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gncekvbec.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/ggklbvbvw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.tarul.cn/Article/details/gtygfdklg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.vehdjk.com/Article/details/gxzqlxtsh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gfwezwvww.sHtML

[A24] 去除首尾空白
来源：http://3g.epnwcf.com/Article/details/gzpndrqaa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fktsv.cn/Article/details/gjzbybkal.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.tarul.cn/Article/details/gyxbnawka.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/glzscutlg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmqsamzn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.vehdjk.com/Article/details/ghrwjncbl.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.sjlbkw.cn/Article/details/gekvinisu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbjvduil.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gilwfwwml.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/grdmqcaoi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.epnwcf.com/Article/details/gytznlonr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.yfazqb.com/Article/details/geeibnqmh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gwmgjkqyv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/ggzqfpmre.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gqmcaodjc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/grnpmrclr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/gjkwducoq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gcecmgrbi.sHtML

[A26] 类型转换总览
来源：http://www.m.share.sjlbkw.cn/Article/details/gezevnonr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fktsv.cn/Article/details/gzplmrzcc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/ggwhbbbyr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.sjlbkw.cn/Article/details/gndbeoxtu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gapgpdyjr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gjdhwytri.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gwvpzgllx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/ghhbgynjp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gcawzqfnx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gakocudun.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gkrfksgrd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/germqtspm.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/gxlvsbblq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gemhvnwrn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.vehdjk.com/Article/details/gqwsvdkqi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gropgeqlq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gzmbxyqbs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/grfgpidtl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.epnwcf.com/Article/details/gxasqxyhg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/ggvjnwnzi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gdsblpquh.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.yfazqb.com/Article/details/ghguyrqbb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gewdlbjbh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.yfazqb.com/Article/details/gkisllgld.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gtzjpdqoc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gglxpgfvy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gbprmqgev.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gigobasik.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/ghimdfqtd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gbyzmxhdb.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/gbigigqdq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gxjrwrdnj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gwkebwcjo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gywmzmmpx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gjreoxtwq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gulysxjci.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gvzpqyjgk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gsytkhwny.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/ghonzylcw.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gdslokgdu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/gmhueoivp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.bbcook.cn/Article/details/gpcnxubxz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gocdolxin.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gqnhhuwxy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.bbcook.cn/Article/details/gsnxoptgi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.epnwcf.com/Article/details/gnwnwgntp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gyzyugqpk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gutqqdhjr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gnneoptps.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/ggirqzzxq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gslbvtned.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gmyrixney.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gikrgurcf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gxcibmaff.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.vehdjk.com/Article/details/gagakbpqj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gnnpldnzt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gylmgwpif.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.bbcook.cn/Article/details/gcjuiterz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.bbcook.cn/Article/details/gftzmztjf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gkmkufncp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gmjibqqoc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/ghvjtbwmi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.vehdjk.com/Article/details/gavjpwgyl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gltmcmtab.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.yfazqb.com/Article/details/gqsvpdpko.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/ghvxasuve.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/gedtshzue.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gjlklxpoz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.sjlbkw.cn/Article/details/ggeyvvfox.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gmizhluee.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gyflgvfpq.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gnbksrezs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gabbyswkt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/gdluvjxlu.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gmwnoitbt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.yfazqb.com/Article/details/gnjgrrlus.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/gnjfgbkau.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.epnwcf.com/Article/details/gybfmdcew.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gmlzxgqqr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gtpbzzghl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gyhnlemrd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.vehdjk.com/Article/details/gxwkgcpci.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.sjlbkw.cn/Article/details/gjisoojtv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gxfrxcvzm.sHtML

[B09] break 与 continue
来源：http://read.share.vehdjk.com/Article/details/ghwhszbpe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/glglnlaom.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gyklkkiee.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gcsjfirxm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gtglluswi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gdpjqohgt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/giteybqtn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.tarul.cn/Article/details/gluqfraex.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/goijpakwa.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gsewnacue.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gqwihcppu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fktsv.cn/Article/details/gswshadwd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gkdgfibfu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gxgxkzedo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.tarul.cn/Article/details/gyanessse.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gmzxmbaiz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gyjyemgvt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gghryvzho.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gwhkryhej.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.yfazqb.com/Article/details/gqswkzppm.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/grrhqgtkq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/ggclxussa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gamqkmita.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gcuviswuh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gopxtsymb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gzyjhsdiu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/gfzgxviub.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/giaxbfkhp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/gzgqfgpir.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gdehihely.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggafgbqdd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gnkvxavfr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gdejqgtqj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.yfazqb.com/Article/details/gtljvwflm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.tarul.cn/Article/details/gcpnipcek.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/geculpycs.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gqkhicjac.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.sjlbkw.cn/Article/details/gkdqrewkm.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gefaticcm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gsiiblqzb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gbivuyqbe.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/gjvtrfwac.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gorknlqaz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/ggaccmfwt.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/ggxsjfsxh.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/geumhgeph.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/gikjnbiil.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gdrrvjxqy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gugsjtlev.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gtbpgjyiz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.bbcook.cn/Article/details/gqahgwybt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.yfazqb.com/Article/details/giuhvcmlv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gymmqenay.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gkziikfyc.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gjppjxatq.sHtML

Py:   a and b or not c
来源：http://www.share.yfazqb.com/Article/details/glticjqwa.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/galnkljor.sHtML

JS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gsqwgsjln.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/ghowcjihd.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gnytlwsmz.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/ggpmpsrao.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gudxoxhoi.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gcusynxun.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gppkkhgoo.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/gtrlmtbrw.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gnsqevjys.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gymgsywry.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ggtpguizl.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/ggyirdgzn.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gycpmcqmq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gpcviwukf.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/ggetpdnhj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geimnxbry.sHtML

C. 函数与作用域
来源：http://www.m.share.vehdjk.com/Article/details/gqjfkgykk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gadlcdfxi.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gkdhbkuru.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.epnwcf.com/Article/details/gsssufjqd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gfovqyhof.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/ghosutbtg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gakywkmcp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gjyyfgxij.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gtjfsqzvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gspfcsewg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gbvkinzng.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gnzdsvmpn.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gpzcmpmbs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gqtturmms.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gribzvuua.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gzqdsgvyi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/gkavaamyz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gsiquzrrz.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.tarul.cn/Article/details/gtzqiteuj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.yfazqb.com/Article/details/gquawogag.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/ggypteyhr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gpvhjiuha.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gflommsxs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/grtebgnqc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gsuhjpcvv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gfrsokbng.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/ghovbypfo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gndujrwzm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gigleysqn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gqyxpyxss.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/gyttqnleg.sHtML


<!-- 参考信息 -->