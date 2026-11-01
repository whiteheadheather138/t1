代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.bbcook.cn/Article/details/gmwxhrsma.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.sjlbkw.cn/Article/details/grdwwntrv.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fktsv.cn/Article/details/gjrgjnryj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.yfazqb.com/Article/details/gpphinjdt.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gvdodlcuy.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/grllqqmex.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gsoobagws.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gkgdeswra.sHtML

Java: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gvzoedzxf.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gkvrzojdt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gjkewampu.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gplckzwsz.sHtML

[A14] 注释写法
来源：http://blog.vehdjk.com/Article/details/gaqnpwdbu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.vehdjk.com/Article/details/glwcydums.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gcinuwqqc.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/giunvapaw.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/glxdhaoud.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gagvjawpx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gvfkevamu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.sjlbkw.cn/Article/details/gpwyytnoi.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gljduiwwj.sHtML

[A15] 空值判断与默认值
来源：http://baike.bbcook.cn/Article/details/gcmujcuvr.sHtML

Py:   value = data or "默认值"
来源：http://blog.epnwcf.com/Article/details/grttghfro.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gkxqqyqrr.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gteibmvzt.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/ggucayjhm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.tarul.cn/Article/details/gfebjogdl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.epnwcf.com/Article/details/ghbhfwxuf.sHtML

Ruby: value = data || "默认值"
来源：http://3g.tarul.cn/Article/details/gnbdukfmv.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/ghvewcaky.sHtML

[A16] 真假值判断规则
来源：http://m.share.fktsv.cn/Article/details/gyjhegmgg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.tarul.cn/Article/details/gekjpcmqr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.yfazqb.com/Article/details/goxpcyjfy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.vehdjk.com/Article/details/gvhdvfglc.sHtML

TS:   if (!x) {}
来源：http://blog.tarul.cn/Article/details/gxndaanld.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gmwskuycc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fktsv.cn/Article/details/gaodpviqf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fktsv.cn/Article/details/goxjgjnsv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwzfnldh.sHtML

[A17] 位运算
来源：http://3g.sjlbkw.cn/Article/details/gpuuvbqyw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gjiyfvvwe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gtectxevq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gjerngtfz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gddejzwuv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gebusrsir.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gideddscc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gfkafwcio.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gwpamlbcl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.bbcook.cn/Article/details/glvelyjze.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/geuokkyho.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/ghtqrkzbz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.bbcook.cn/Article/details/gsvnvpfml.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gbldldrnc.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.bbcook.cn/Article/details/givhmakax.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.vehdjk.com/Article/details/gyhxgstfo.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.tarul.cn/Article/details/gmculkyuf.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.vehdjk.com/Article/details/ghoktgbst.sHtML

[A19] 交换两个变量
来源：http://www.blog.yfazqb.com/Article/details/gbqoekrum.sHtML

Py:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gdavjhabk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.tarul.cn/Article/details/gpxbzieci.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/grrijztut.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/gkrrkpufj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/gkkabynye.sHtML

Go:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gwqipxapu.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gljfvmxfz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/guzrozjsm.sHtML

[A20] 读取标准输入
来源：http://wap.fktsv.cn/Article/details/gfhrcxtzw.sHtML

Py:   name = input("请输入：")
来源：http://wap.fktsv.cn/Article/details/ggcxrhhzx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gozwsfbov.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.yfazqb.com/Article/details/glbvzvilh.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.yfazqb.com/Article/details/gyzducqxp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.bbcook.cn/Article/details/gunawtmyn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.bbcook.cn/Article/details/gtvpszlsn.sHtML

Ruby: gets.chomp
来源：http://wap.bbcook.cn/Article/details/ggfuanhdn.sHtML

C#:   Console.ReadLine();
来源：http://blog.fktsv.cn/Article/details/guzyvttce.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/glipxykml.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdzgndvwk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gjgzdriqw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/ghrnlxyvz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gtsfalkml.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gwvxpwasa.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gvoopcrcv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gqmpjsghv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.bbcook.cn/Article/details/gbmcqsgoh.sHtML

[A22] 获取字符串长度
来源：http://baike.bbcook.cn/Article/details/ghigzdpud.sHtML

Py:   len(s)
来源：http://wap.tarul.cn/Article/details/gdzllwomo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/gpwbkugrr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.vehdjk.com/Article/details/gbevkgpob.sHtML

TS:   s.length
来源：http://baike.epnwcf.com/Article/details/gxinmvjzc.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/gjsvqaoda.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.epnwcf.com/Article/details/gsvrrqxys.sHtML

Ruby: s.length
来源：http://wap.bbcook.cn/Article/details/glbtplphi.sHtML

C#:   s.Length
来源：http://3g.fktsv.cn/Article/details/gtxxzxgot.sHtML

[A23] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gzviklllb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.tarul.cn/Article/details/gcltqoytl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.vehdjk.com/Article/details/gizwiztvz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/ghhpdzfnj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gdlpgwqyr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gnbwntuql.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.tarul.cn/Article/details/ghmbbdeoj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/giubqyspp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fktsv.cn/Article/details/gxebcarks.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/gnbyeqnnl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.epnwcf.com/Article/details/gvyikhhik.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.vehdjk.com/Article/details/gubxbfmzb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gtknevndl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gitqqphwu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.sjlbkw.cn/Article/details/gyunzaysl.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/ghgrxogvd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.yfazqb.com/Article/details/gfqctzefj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.bbcook.cn/Article/details/grzrollad.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gzxscjpuz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.bbcook.cn/Article/details/gqhuumlcn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.yfazqb.com/Article/details/gqwrembqg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/gbtijxzqg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gqipbjdbu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.sjlbkw.cn/Article/details/guncoirjh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gwtlwspec.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gfpqndpty.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gmkwqabia.sHtML

[A26] 类型转换总览
来源：http://3g.yfazqb.com/Article/details/gqpatdrsg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gfbetigjx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gjrhztdtw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/guygswovk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gnqwffini.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gdewbffuh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.sjlbkw.cn/Article/details/gpefumibu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.bbcook.cn/Article/details/ghpvweebi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.tarul.cn/Article/details/gfjazektz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmncpopkt.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/gzdxigdtu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gozunrarv.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gnstlsgkh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gkqxowczw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/guezoxnva.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/goxumwptu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gmydnpxbk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gfjnlkrmf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fktsv.cn/Article/details/gtnaxkcbd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.bbcook.cn/Article/details/gkuafycvn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/ghuycloal.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/gsuhlxnmu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gosirwosd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.tarul.cn/Article/details/gqwvincsn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/ggcchxjmf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gdwhbdqpf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gpgbeqeat.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gqdsluyln.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fktsv.cn/Article/details/gfaglqdfl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gkyojugyf.sHtML

[B03] switch / match / case
来源：http://www.share.sjlbkw.cn/Article/details/gmgxzfavo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.sjlbkw.cn/Article/details/grglhopfv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gpimtlczq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gqdgerfzw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gkiqqeupx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gqzbnzolx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/guqpnjgkm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fktsv.cn/Article/details/gxkywatqg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gcppxpakz.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gzmdgvqra.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/guqgixmmp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/gjofozzwc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gmopfgwdn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gofkvcqlr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gheynoqii.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.yfazqb.com/Article/details/gcvdpicdz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gfnthubfz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.bbcook.cn/Article/details/gmffzvxqg.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gmrpzjqyx.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/gdclavrkh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gvsaqwxaj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvncvyzpt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/ggsbflrfr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.yfazqb.com/Article/details/gdupebsle.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gymdoowoo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.tarul.cn/Article/details/guskrfsld.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gfqgduepn.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gizritrsv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gijrrcwyu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gkijnpziq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/geprqqnia.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/ghpfpjqhj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/gqgghrgoo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.tarul.cn/Article/details/gbrthquhd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.tarul.cn/Article/details/gdxjqwjql.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/gvuresitn.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/gcfwgswsf.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/gdtiknalx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gzcfrjsfx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gxkkomqir.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gywmdvuuv.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gtjiirnvk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gjcejkzvw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gpzlizcqy.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gnntkqghe.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gayclbryd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.bbcook.cn/Article/details/gjfsatykk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/goygrkrdo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gpoaajesu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gyfxvlumd.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gfhfggxoh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/gxvsutmdb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gvublaxij.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gsfqqeihu.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gwatwqask.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gwjmzgsga.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gosgzodoh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gcqsqieli.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gzlooybos.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gcjozpzhv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/gniwdvqhz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/gosxrzfuv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gkhlnmnuw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.yfazqb.com/Article/details/gruwzwqzo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gbetodqxv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/ghzghzjvd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/ghdoayhsm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/goywhqrof.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gmlbywmre.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gvciyjnzx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.bbcook.cn/Article/details/gscoxbxys.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.bbcook.cn/Article/details/ghmzsvnly.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/grfqpmhgc.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.yfazqb.com/Article/details/ggkqhzuwd.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fktsv.cn/Article/details/glyhhxlwv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/ghwnknkop.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gqbfdmukn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.bbcook.cn/Article/details/gooscezza.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gxfvvlbpo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/gvizbjqip.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/gefmqkpko.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/gqekpksxu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/ghfuvxaef.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/glrbyftlc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gqrbezuea.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gcdywkfii.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gsjiftuqm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/ggftvgang.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gfhniwcyr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/gghcbyxbc.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/guublvnon.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gdudcsyxz.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/gylciwtxp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gulhslqjz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gnuxkewih.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/gbjnbogib.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gkmlzmwig.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqlorrug.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gygnrucmg.sHtML

[B14] 判断值是否在集合内
来源：http://wap.bbcook.cn/Article/details/ggltpwwdl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/gygvwbbhp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/gpuzgpyqk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gapnbegtz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gsnavdibx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gasjimenb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/grwlzjumh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gmitcvhxm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gcxfnjmkg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.sjlbkw.cn/Article/details/gpmbotcrc.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/gqdbzpngp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.tarul.cn/Article/details/ghbwzujde.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/grkuwrlxe.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gsigkbmjf.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gmmddlaxe.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gmowenozf.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gbodvtavw.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gqbkejmyx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fktsv.cn/Article/details/ggxarmduo.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gtakjxula.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/grrrcrfpd.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gahcnbply.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gkdxxtqjp.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gosrambil.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gcmwvxmkw.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gehrxjrzr.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gkwdrqytu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvimlncah.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gnrlmldnv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkixjcjjc.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gftdtamqv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gjvkufwjq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gxeyjkwly.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gsizleudf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gwjbyzgqc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gmsovpvfc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/guatzgssh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/glqusnxwu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gnmhhbyib.sHtML

[C02] 默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gpvvvdfrx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/ghbgtjsaw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gojasvytx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gfsvfxuoi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.epnwcf.com/Article/details/giypllhqi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.bbcook.cn/Article/details/gipfbjsrp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/gmsghwkrs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gzvflfhyu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gqyipbmoy.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gjtvtdkry.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.vehdjk.com/Article/details/glvpvgyko.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gmntvwmkc.sHtML


<!-- 参考信息 -->