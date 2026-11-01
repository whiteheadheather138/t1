代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.tarul.cn/Article/details/gjhblvdhc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.sjlbkw.cn/Article/details/gysazanlv.sHtML

TS:   if (!x) {}
来源：http://www.m.share.bbcook.cn/Article/details/gdrzzucxn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.yfazqb.com/Article/details/gqrejaxpr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.vehdjk.com/Article/details/gtjgokxag.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.sjlbkw.cn/Article/details/gnhwekqmh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.vehdjk.com/Article/details/gkqxqdadh.sHtML

[A17] 位运算
来源：http://read.share.bbcook.cn/Article/details/gfqlhjuuy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/ggmgxqrck.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/ggikuzikp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/grpojnjrr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gxrtmcfuc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gbkpbyxmt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gmfibtpki.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gaicoyuiu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gchowyksc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.vehdjk.com/Article/details/gsejhyoyt.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/goytoatgc.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.epnwcf.com/Article/details/gfwudbjjo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.bbcook.cn/Article/details/gfyfruxlk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gqsphjjdy.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.epnwcf.com/Article/details/gzebolnuu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.tarul.cn/Article/details/ggbenubtm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.sjlbkw.cn/Article/details/glzvrthbi.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gmnacyzsj.sHtML

[A19] 交换两个变量
来源：http://3g.yfazqb.com/Article/details/gpdgnvkmi.sHtML

Py:   a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/gzwloivmp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.epnwcf.com/Article/details/gvqlwrqqg.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gxdrjtueb.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/grlixohsg.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.yfazqb.com/Article/details/gwebnrija.sHtML

Go:   a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gbdkzbadj.sHtML

Ruby: a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gbzrpkidx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.vehdjk.com/Article/details/gfpzqiwoq.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/gkwhlucqs.sHtML

Py:   name = input("请输入：")
来源：http://m.share.epnwcf.com/Article/details/gqtbfcecj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.yfazqb.com/Article/details/gplghzetw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.yfazqb.com/Article/details/gdiaftwru.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.tarul.cn/Article/details/getwyxnuv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gogffgwlq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gnkylwafn.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/gvtqgalbg.sHtML

C#:   Console.ReadLine();
来源：http://mobile.bbcook.cn/Article/details/gjrjrftml.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fktsv.cn/Article/details/gcderyjdg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/giuifnpht.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gnisplcyx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gxcmbqwhs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gcjjdduub.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gigjpllhk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/geryndikj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gktgfubsq.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.epnwcf.com/Article/details/gxoyxtnjn.sHtML

[A22] 获取字符串长度
来源：http://www.blog.tarul.cn/Article/details/gijmwjvcz.sHtML

Py:   len(s)
来源：http://www.share.epnwcf.com/Article/details/gzvrlrcgu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/gciwhonxf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.sjlbkw.cn/Article/details/gahcbdxub.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/gotwdgitp.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/ggeuhzctq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.epnwcf.com/Article/details/gqxneyyus.sHtML

Ruby: s.length
来源：http://3g.bbcook.cn/Article/details/gesevqwwe.sHtML

C#:   s.Length
来源：http://baike.fktsv.cn/Article/details/guuykrxvw.sHtML

[A23] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gmnjqhmbf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.tarul.cn/Article/details/gbgdowqra.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gburskhse.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gceolsgln.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gliwsbcqq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gtlldtoab.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.bbcook.cn/Article/details/galyewyzy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gebgioxqy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/glutewrzk.sHtML

[A24] 去除首尾空白
来源：http://m.share.epnwcf.com/Article/details/gyeepmndt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.epnwcf.com/Article/details/gwrionbek.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.sjlbkw.cn/Article/details/gjtupgkap.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gwyhsqguk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gbimkipjw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/gpjplnyec.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gpripkjhg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.yfazqb.com/Article/details/gsafmwwvc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gggprwnep.sHtML

[A25] 字符串比较
来源：http://wap.tarul.cn/Article/details/gbqvbclns.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.vehdjk.com/Article/details/ghcehqwry.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fktsv.cn/Article/details/gyfxobbon.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/gszyyphzh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gilrjmptj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.epnwcf.com/Article/details/gsylhquie.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gbmjyuiov.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fktsv.cn/Article/details/gryqvylff.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/gqdazntbf.sHtML

[A26] 类型转换总览
来源：http://www.share.fktsv.cn/Article/details/gxcldxwos.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/gpbuaippe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/ggenbmpuc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/glvwuxdzw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.tarul.cn/Article/details/gejjfizcv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gdtyqkifh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.vehdjk.com/Article/details/giypcwajn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.sjlbkw.cn/Article/details/ggzmctnak.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gvlwahrvz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gizhrsbpy.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gqnkgdpdj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbtxlnruf.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.epnwcf.com/Article/details/gtewtwflu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gnzodyqfr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gzrjxalcs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gqqteepbm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/glqguuhvx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gfvjhxcga.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.sjlbkw.cn/Article/details/gkflxyzun.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.tarul.cn/Article/details/goejrgtxp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gmagohsuj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gkkhnjlcg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.bbcook.cn/Article/details/gqpsiaopd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/gdadmrlyp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gbrbxprde.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gvsskbhly.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gobzixqgg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.vehdjk.com/Article/details/gtqzkaeui.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/gnlmuscrc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gedbdyrlp.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gotdzgrui.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.epnwcf.com/Article/details/gosawfcet.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gqxfomhnh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gpllurzgb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/ghhebohon.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/ghvnquvvh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/gdmaqjknz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gvxawhoef.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gywswlwoz.sHtML

[B04] for 计数循环
来源：http://3g.bbcook.cn/Article/details/ggivvvmio.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.vehdjk.com/Article/details/gfrzrnkwh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gurdhjwau.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/ggcmkypwn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gvpayllxp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.epnwcf.com/Article/details/gzmkprwer.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.tarul.cn/Article/details/ghpbovzeo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/gifuahjap.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.tarul.cn/Article/details/gxwpnobhu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gasywgrem.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gjeuyqxac.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/gbjcatsmp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gojklgwia.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gygbbesba.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.tarul.cn/Article/details/ghmgnercw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/gqdnnpjlb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.sjlbkw.cn/Article/details/gdwaturxw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.sjlbkw.cn/Article/details/gljhktnom.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.vehdjk.com/Article/details/ggqjlzvnh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gtdufyxqh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/grblhelup.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gojomereh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gwurlyhga.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.epnwcf.com/Article/details/gycnlkajz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.bbcook.cn/Article/details/gtiobfcuy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gwokunoez.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gvyvcmfuz.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gckxlnajh.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gkfbbagsz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/gvyrsfhcd.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gecisqnid.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gfcmkkyvo.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gbvnkjoyh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gxdatxmzm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/ghitrbufi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gnlacwvih.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.tarul.cn/Article/details/gwhkkhlah.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gyhjygozb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.tarul.cn/Article/details/gipvtgbby.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gxbcxvmxy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gdusepdyn.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gxlaxljsz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fktsv.cn/Article/details/gqloijtav.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/gnjtqyylq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gkuicnpsv.sHtML

[B09] break 与 continue
来源：http://3g.tarul.cn/Article/details/gbffetdfn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gtwoxofbd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gigjunmxz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gszwpfhsu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gpcrwbikg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gknvyaaro.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.tarul.cn/Article/details/gcohsejtd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gzythbzpf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gtjusemtu.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gjwhsivkq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/gaibmvwds.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gtqjdrytn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gtwuxjmrq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/goqogrrdw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.vehdjk.com/Article/details/gtoqxxlmr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/gkilwarks.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.sjlbkw.cn/Article/details/gebmrylbu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/gwacoqhod.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gfgxcphpb.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.sjlbkw.cn/Article/details/ggdifdclb.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/geyflelsx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gnmtlurbn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gefzkrsgf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gvkooffgb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gdicyazmh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fktsv.cn/Article/details/gxcbyetbr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/gqrlelxui.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/gynfnuvai.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.vehdjk.com/Article/details/guwcvurou.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gzwenxgva.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/grgaleagl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gzupyzmck.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gozxuyqhy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gcbizythd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fktsv.cn/Article/details/glpvlcqbm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gzodgyyni.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/gpeeexeot.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/ghmgktynr.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/gakmmhpha.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gfgqwaquc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gnsvdirjr.sHtML

Java: x instanceof Number
来源：http://wap.tarul.cn/Article/details/gxogkdvsd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/geayqtwag.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.vehdjk.com/Article/details/gmvculkjv.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gvdftkfja.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gulatqnnl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gseqsvuqf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.epnwcf.com/Article/details/gnyqqjhtk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gkyyextlq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gdmqapjhd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/grlkbgnpa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.vehdjk.com/Article/details/gkityibqn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gvyseqfvg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gsvqglonb.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gjhutnrpy.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gyzmgrzmw.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gpyqignin.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gbaxywodb.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/ghjiwxnsy.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gucuvfohz.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/grluipjao.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gxduoiflh.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/goisblcof.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gpfsbpyrn.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gfknxzaqv.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gkfjxhcvv.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gmvsewchs.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gedfhkhfx.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gvsipqize.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gnuadjsdp.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/gsxjjnogk.sHtML

C#:   if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gpjexukce.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gftdttunr.sHtML

C. 函数与作用域
来源：http://3g.sjlbkw.cn/Article/details/gsimdffkl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcenjjjkm.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gmxfrmsjn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gzmbqaaor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gcrzdvwpf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gbnkshplm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gpyjkchsp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/geqcjhpju.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/gheefhlxp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/gyzmwokox.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gxnoipjge.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/glmesjsic.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/glywpghvb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gwlepowki.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/geaosxcnt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gidcqkqxt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/glebblmfi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gxaszdlzv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/glummzdyo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/gnbpeyyzk.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gqqqkgivz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gxfpqqaps.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.vehdjk.com/Article/details/ghkwraqyc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gmdptmmtq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gxcjnhrdd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gddfgxhpz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.yfazqb.com/Article/details/govpxirep.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.epnwcf.com/Article/details/gidhzqein.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gwxfkfwvg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/ggmuffcnk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gpjhalvcw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gzeddgvct.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gbtwlpxhm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.tarul.cn/Article/details/gekkvyfcx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gdhqugeom.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/ggquslfhv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gslkokppz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gicllhfyc.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gnonwytxk.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gmwfwdase.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/gtbjdwkuy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gplpcbpnf.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/ghxilscdm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gcolsekcs.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/geildcvtl.sHtML

Ruby: return a, b
来源：http://www.share.tarul.cn/Article/details/gvtgfcihz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gzxuhrruj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fktsv.cn/Article/details/gnwcyoivu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/ghbbjoeob.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gussiprdg.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gyflyajxy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gfwsqbbfh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/grxacczjb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/guyetfxmv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gebutmnns.sHtML


<!-- 参考信息 -->