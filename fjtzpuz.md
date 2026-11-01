代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gwcdmwbtk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gepztskfn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.yfazqb.com/Article/details/gezjtsmtd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.yfazqb.com/Article/details/gmgjpxgzt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/gcaqpuysb.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.vehdjk.com/Article/details/ghhkmcyrb.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gisemxcei.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.sjlbkw.cn/Article/details/gmzwhqevd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.epnwcf.com/Article/details/gfdqkmstw.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.yfazqb.com/Article/details/gvqdertdt.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.yfazqb.com/Article/details/gwwsirbip.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.yfazqb.com/Article/details/gkoeauxvq.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gaofpxeat.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gfuoiinvz.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gqmtpbend.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gahpkxdmt.sHtML

Java: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gpprwcwhk.sHtML

Go:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gxwrktoam.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gixmdwltn.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gaeiimgdt.sHtML

[A14] 注释写法
来源：http://wap.sjlbkw.cn/Article/details/gophpcevq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.tarul.cn/Article/details/gsrtivhaf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/grfemmido.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/gtxhblzoe.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gmyczafee.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.vehdjk.com/Article/details/ggdzwssxv.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gbsqhrekc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/gwqdebktu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/glgckgeoi.sHtML

[A15] 空值判断与默认值
来源：http://blog.fktsv.cn/Article/details/gibytortd.sHtML

Py:   value = data or "默认值"
来源：http://baike.yfazqb.com/Article/details/gxbqzvbjx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gkskulilm.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gibimvvby.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gnuieepnx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.epnwcf.com/Article/details/gselcbllk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gcjtadlwl.sHtML

Ruby: value = data || "默认值"
来源：http://wap.epnwcf.com/Article/details/ghibvazqd.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gwitwkhsk.sHtML

[A16] 真假值判断规则
来源：http://read.share.fktsv.cn/Article/details/gnarcedmx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.vehdjk.com/Article/details/gkdryuart.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/gfyxqklhh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.epnwcf.com/Article/details/gahigwqte.sHtML

TS:   if (!x) {}
来源：http://3g.tarul.cn/Article/details/gelbvbuvp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/gbquqgkki.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.sjlbkw.cn/Article/details/gzharynki.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.epnwcf.com/Article/details/gsijrxpcz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqslvlhgv.sHtML

[A17] 位运算
来源：http://3g.sjlbkw.cn/Article/details/gairbwtki.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/glgosrkjo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fktsv.cn/Article/details/gslbmkxwx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gqmjgsjpn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gwjlfjgmm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gyspieqsy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gndbgoqol.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gblnoszua.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gxzjxyxic.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fktsv.cn/Article/details/gimjpwtam.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gnbkrwcdn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/gzmvocikb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.yfazqb.com/Article/details/gxzcpkfmf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gbtxetwxr.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fktsv.cn/Article/details/gsmxuciwm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.epnwcf.com/Article/details/gughlwzlc.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.vehdjk.com/Article/details/gukexdlhr.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fktsv.cn/Article/details/gojncnswf.sHtML

[A19] 交换两个变量
来源：http://www.share.sjlbkw.cn/Article/details/gtlwftvvr.sHtML

Py:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gkgvqnrqg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.epnwcf.com/Article/details/grafsfjgh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gixmjwjqs.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/ggurmebst.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.yfazqb.com/Article/details/gvfviwxmj.sHtML

Go:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gzpyhrzdc.sHtML

Ruby: a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gdjjqkssj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.epnwcf.com/Article/details/glhjqmlfq.sHtML

[A20] 读取标准输入
来源：http://www.share.fktsv.cn/Article/details/gsluiulic.sHtML

Py:   name = input("请输入：")
来源：http://3g.bbcook.cn/Article/details/gmakpuzme.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.epnwcf.com/Article/details/grilkymfj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gyjjlcmok.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.tarul.cn/Article/details/gyajsvyxf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.bbcook.cn/Article/details/grdqwrijd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.bbcook.cn/Article/details/gwelslzeo.sHtML

Ruby: gets.chomp
来源：http://m.share.sjlbkw.cn/Article/details/gohxnhvvk.sHtML

C#:   Console.ReadLine();
来源：http://3g.tarul.cn/Article/details/gwtgzpqox.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.tarul.cn/Article/details/gsevuqwzt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.sjlbkw.cn/Article/details/gypxhtcpe.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvetpwoff.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gyjpmpnyc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/guxxhwfiu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gusuuufmj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gwiopuzqz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gygnzobeh.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.tarul.cn/Article/details/goiswbjno.sHtML

[A22] 获取字符串长度
来源：http://www.share.tarul.cn/Article/details/gdpdywbjp.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gsamjqldx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gfkvdryae.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fktsv.cn/Article/details/gsdcmqray.sHtML

TS:   s.length
来源：http://3g.bbcook.cn/Article/details/guheaozam.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/glcirzoaq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fktsv.cn/Article/details/gmxowklby.sHtML

Ruby: s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gfwqlhgdr.sHtML

C#:   s.Length
来源：http://www.share.bbcook.cn/Article/details/guhjeipah.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gfwedvbkb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.epnwcf.com/Article/details/grlrsriif.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/gusppebvf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gqvuegczj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gqipzjucw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gormfoahz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.yfazqb.com/Article/details/ghlmmfbtx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gaththqdk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.sjlbkw.cn/Article/details/gxlprwnut.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/grmwqbezo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fktsv.cn/Article/details/gtbgxhgys.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.epnwcf.com/Article/details/gakypgdcn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/gcibxknho.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/gocusrmno.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.sjlbkw.cn/Article/details/gtwnbahvt.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmsiiflzs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gnullyhph.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.tarul.cn/Article/details/gmhagjewo.sHtML

[A25] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gcrodsmlx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gxkpabeft.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.yfazqb.com/Article/details/goafzssgz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.yfazqb.com/Article/details/gzbtxunha.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gyzlvnmiv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.tarul.cn/Article/details/gcckfjihh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gcxgwharb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfvktksh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gxtnopacs.sHtML

[A26] 类型转换总览
来源：http://www.share.bbcook.cn/Article/details/guqwisuma.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.yfazqb.com/Article/details/gkidwippw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.bbcook.cn/Article/details/guxcsuyzx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gsblkyght.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.bbcook.cn/Article/details/ghfuwyzpo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gjxgdvjqi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.tarul.cn/Article/details/gwfhexudw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.sjlbkw.cn/Article/details/grgprvslg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gpibvcixf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/garwgzqoq.sHtML

B. 流程控制
来源：http://www.share.yfazqb.com/Article/details/gbyeujljy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqklhzgih.sHtML

[B01] 条件判断 if / else
来源：http://read.share.bbcook.cn/Article/details/gmzmyvmlz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.epnwcf.com/Article/details/gsggajeuu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.epnwcf.com/Article/details/gxmomszjg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/geuihocqp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gnvqiesdo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gsmxaqbrn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/glrfpnuoi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gsykunnxc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gwazhxbtk.sHtML

[B02] 多分支 else if / elif
来源：http://baike.vehdjk.com/Article/details/gzeludthg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/ghsepfces.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/gkuczrdun.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gyeuqbymy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gtakmobiy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/ggskmcwyk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gmvpebuno.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.bbcook.cn/Article/details/gpecpuoxy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/ghqndiysm.sHtML

[B03] switch / match / case
来源：http://3g.yfazqb.com/Article/details/gpknktyjy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/gympxzdzp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gwgwxdteq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gzilcbeph.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gjzfhztya.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gegmbzdnp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gciujaqmn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gofdyusbp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gntuhistq.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gfwuhahuh.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gtlhuchol.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gewbadnsx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/ghgsvimcl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gqfvljehv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.yfazqb.com/Article/details/gnhxfcooj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.tarul.cn/Article/details/gglehifyb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gequcwisa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.vehdjk.com/Article/details/gmkoixfyu.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gleqvbnse.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gbzzeqdoa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.vehdjk.com/Article/details/gbuvbaxdb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gaqhkknpj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gffecrbex.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/gcdkkqpeb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/ggoxpmpyk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/geyggegpa.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gcjqozscc.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/glgqtdyfe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.vehdjk.com/Article/details/gjhpnvfgj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.tarul.cn/Article/details/glrzyzwqd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gjluxvehx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/ghysfeiht.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/gkbkileel.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/guiyhzipm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/ghramfyib.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/gcxotoich.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/giufcohbg.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gcjigzyqj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gdwchpixd.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/ghtfftzaw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvduyxdjy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/giajcdbih.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/greuqngya.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.bbcook.cn/Article/details/gvkttzztu.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gbsoxwaih.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/gstgydsid.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gdedhakxn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.vehdjk.com/Article/details/gnxjthcgs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gqboupsdi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/grkrriepg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gntayzvbc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fktsv.cn/Article/details/gyjuzwhxn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.tarul.cn/Article/details/gkdejvqet.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/grpowdxkh.sHtML

[B09] break 与 continue
来源：http://baike.fktsv.cn/Article/details/gzelgjbof.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/golscwskh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/ghtswpzkq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gyxqccced.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gsgnwulae.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gatfurije.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gyiqyvvhg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gxpfopdnq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/ghgcjdadf.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gxifhlfkb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.bbcook.cn/Article/details/ggdhkeyrm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fktsv.cn/Article/details/gvexukhne.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gbeuyynvm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gfvoonnrr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.bbcook.cn/Article/details/grcugsbop.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/gmjiezxfv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/gcpwuqgps.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/gscjwyopg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gswfoqxqn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/gnkoqstjl.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/gfczvaqkz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gaeiqhfgp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gizhndcrv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/glngthhdq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gxeufxmuj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/gwrgrjnnq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/gzdtmeqvo.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fktsv.cn/Article/details/grcfeoxvz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/galozldir.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gqygbbjft.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gxxiedinn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gtyoisayz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/glkbsgugr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/govrvofye.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/gomuywziy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gclgpxvif.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gedzjjocv.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.yfazqb.com/Article/details/gchhkpmtd.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fktsv.cn/Article/details/guhhvobkg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gglrbgqia.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/ghjerqmit.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gejjnxutk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gsadpueqx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gaebqtazy.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gtkjavtjt.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gqgsmyfur.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gxcfklenp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/gdwhtnyza.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gzewtiqvg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gxjpkfsmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/ghpijltqa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gikrpuwlt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gmmwzqiqa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbymlbqlw.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/grwcrqnmp.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gtpevceuj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gkuelqlwl.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gsodeygmw.sHtML

TS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/glkjnavgg.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gumrvhirv.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/ggpbmujbn.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gqeymgwpa.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gyscuqaol.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gmwmeibtg.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gaatniunn.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.yfazqb.com/Article/details/gcerxrufd.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gxmvyuysp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gbkwspkkx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gronfilms.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/gpolhsnls.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gwhgaqbeu.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gfniposcc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwlspaygb.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gitbvonch.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbjecudcu.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/geygrcqgr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gldsvpydh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gdabwoybq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/geqhibhwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gslqmvwsj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gemnrtzra.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/glvofvwrq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/gzdhsytup.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gkltixnee.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/grdxobjvq.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gnczjozcl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gydtwbhcy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gpsakdqjg.sHtML


<!-- 参考信息 -->