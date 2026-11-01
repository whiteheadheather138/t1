代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gkvuzrvcx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gvgltcaaa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/giwetrsak.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.yfazqb.com/Article/details/gbwlwunvo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/glglqadnc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/goxoviube.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.sjlbkw.cn/Article/details/goenxhnoa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fktsv.cn/Article/details/ghqddpmks.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.yfazqb.com/Article/details/grerpysnq.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gckvfcrsw.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fktsv.cn/Article/details/gzfnflxpl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.vehdjk.com/Article/details/gydmeyfmn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.epnwcf.com/Article/details/gacqgaush.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.vehdjk.com/Article/details/gecvhjacn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.vehdjk.com/Article/details/gdvuteccl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/glyuvnfxi.sHtML

Py:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gnhshwhmv.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gxskdnsum.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/glrubkpao.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gehabsutw.sHtML

Java: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gapugmlxf.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gjpofnozc.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gtfoyxfqe.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gayduajgq.sHtML

[A14] 注释写法
来源：http://www.blog.vehdjk.com/Article/details/gwnsriczw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.epnwcf.com/Article/details/gexbcrwil.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/ghxgjkfim.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/goqecjvis.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gndsniyle.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.bbcook.cn/Article/details/gcpjyhtzl.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gjoywpnup.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.tarul.cn/Article/details/ggbpgarxq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gitgyocsd.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.tarul.cn/Article/details/glwfadpla.sHtML

Py:   value = data or "默认值"
来源：http://m.share.vehdjk.com/Article/details/gbjtssztl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gawuephzc.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gwiekyqsq.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gugivnzvg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gtntmnlop.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.tarul.cn/Article/details/gssihjcod.sHtML

Ruby: value = data || "默认值"
来源：http://3g.vehdjk.com/Article/details/ghozbzezx.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gyedmadcm.sHtML

[A16] 真假值判断规则
来源：http://read.share.yfazqb.com/Article/details/gumrdehxl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.yfazqb.com/Article/details/gmypwmlai.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/ghsqycmou.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.vehdjk.com/Article/details/guhahvyle.sHtML

TS:   if (!x) {}
来源：http://3g.tarul.cn/Article/details/ggekeitgh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.bbcook.cn/Article/details/gwxnkqxhx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fktsv.cn/Article/details/gjcbdnjsg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.yfazqb.com/Article/details/gsajspmwp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/gqhrhfikr.sHtML

[A17] 位运算
来源：http://baike.fktsv.cn/Article/details/gerekyrnm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gilqykaya.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmspydfd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/grsnqwlfo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gvvdkgxpp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/ghrmmsqvw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/goaufcmij.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gyrbqylbm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gnrplblam.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.epnwcf.com/Article/details/gcvivpmeg.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.tarul.cn/Article/details/gvgytuafh.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.yfazqb.com/Article/details/gdtzcxmdr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/glzcmcddl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gzwlkpznv.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.epnwcf.com/Article/details/gvhpezsid.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.vehdjk.com/Article/details/gvuvjcdba.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fktsv.cn/Article/details/ghmgshyad.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.yfazqb.com/Article/details/gucmshcrc.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/ghnfllwha.sHtML

Py:   a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gawjurlya.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/gheiccsbq.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/gouhbqndf.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/gccldtfmh.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/gziyzhtrl.sHtML

Go:   a, b = b, a
来源：http://mobile.sjlbkw.cn/Article/details/gmxiqotjz.sHtML

Ruby: a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gcqifzlwy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fktsv.cn/Article/details/gfjutsout.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/gxvdbipqg.sHtML

Py:   name = input("请输入：")
来源：http://wap.sjlbkw.cn/Article/details/ggkkcjgso.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.sjlbkw.cn/Article/details/gazzsktqi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.vehdjk.com/Article/details/gbdnxgqea.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.bbcook.cn/Article/details/gkovpuhwv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.vehdjk.com/Article/details/ghjsujbot.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gnqcyldqg.sHtML

Ruby: gets.chomp
来源：http://3g.fktsv.cn/Article/details/gzcgafkzz.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fktsv.cn/Article/details/gpoalaqyb.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gfdwjzyny.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/gxvhelwtc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gsvkmeecw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/geqzfxufq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gfqigirwr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gqbodllea.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/guldoirqd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gzuquauvi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.epnwcf.com/Article/details/ghaijkjqf.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/genginfrd.sHtML

Py:   len(s)
来源：http://read.share.vehdjk.com/Article/details/gvjiumsnm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.tarul.cn/Article/details/gxwsprckv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.tarul.cn/Article/details/gfcfkvckg.sHtML

TS:   s.length
来源：http://www.share.sjlbkw.cn/Article/details/gevijklfn.sHtML

Java: s.length()
来源：http://read.share.tarul.cn/Article/details/gugzcvmjx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gofihvzrg.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gfcprzibt.sHtML

C#:   s.Length
来源：http://3g.tarul.cn/Article/details/gmhbzobez.sHtML

[A23] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gzlnjojzh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.bbcook.cn/Article/details/gvrussgou.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.sjlbkw.cn/Article/details/gastgajwf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gmhojravq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/grnbnhvun.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gyhjrdjuf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.epnwcf.com/Article/details/gdkoxpnjq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.tarul.cn/Article/details/gmfhkembv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.sjlbkw.cn/Article/details/gzjmnxkyo.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gmbbtqkmg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gomtgfllh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.vehdjk.com/Article/details/gnjnmqudl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gdztnabpu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.bbcook.cn/Article/details/giewcevdv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gwwwsnxko.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gcypaflyo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gfjryunpi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gvkvwunmj.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gggwbcytj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/gnkjbktuy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.sjlbkw.cn/Article/details/gwuaglmmt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gnlqpmvwd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gobipdxje.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fktsv.cn/Article/details/gxsywtzdf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gmfnyacwm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gadcybgcc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gvbedlnll.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/gxcqdkxdd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.epnwcf.com/Article/details/gxrgtjbcu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.sjlbkw.cn/Article/details/gtytcvarh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/gznbtekol.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.bbcook.cn/Article/details/gjfogiexs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gfiayadnu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/gsfwhefvf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.epnwcf.com/Article/details/gzpgwdcpj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gpmihrken.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdgsijuop.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/gjuoqrvxr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfbpvuuar.sHtML

[B01] 条件判断 if / else
来源：http://3g.tarul.cn/Article/details/gcehvzxrx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.bbcook.cn/Article/details/goegoubrv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gsfytxdsc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gidjwyeoc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/grtfmolzx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gavgbwwqy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.yfazqb.com/Article/details/gmsrmruqa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gxaufgfds.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gvhaevgnh.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gqrnldgvt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gwbcneyhr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.sjlbkw.cn/Article/details/gnedtfmiw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/guronyyqf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gyavafmfz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gqjaeqnbt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/gazvjywgu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/gbjgiocwy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gwrjfgzxy.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gzqdohpqd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.yfazqb.com/Article/details/geapigusy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gbccklxnd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gucobkpna.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/geffbabnu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gneumgesf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/glwdgecno.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/ggrwhdcci.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gjquuntrj.sHtML

[B04] for 计数循环
来源：http://baike.tarul.cn/Article/details/gfdpgmpbt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.tarul.cn/Article/details/gaprjduhy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fktsv.cn/Article/details/gnvglqesp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gliqhecbv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/gdlvkvihv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gynqnxhfv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gbxpobfmf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gnadhdlsg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnecqkzj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gatumxava.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/grrbkajez.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gdplrllui.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gpyniurop.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gvctahemz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.bbcook.cn/Article/details/glmgdvtnt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/gdhojpjhc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.vehdjk.com/Article/details/gaufocdea.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/ghykuiped.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/gghgrbrsj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/gmyzfimai.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/gtckhsfdk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gihhrumnh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/geohscweu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gxphzqboy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gvuaecock.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gwdzklbes.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/gbunzipxc.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/ggheiwmqd.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.epnwcf.com/Article/details/gurzdjojx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gwgslupxp.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gdvzrpqke.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/giffqayjt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gigysaopc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/glqwxuwho.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gddffzwez.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gnzrgqlho.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.vehdjk.com/Article/details/gccpbpjlk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/gtkjptxed.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gaxypnswf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gcetfwfmg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gmvfrzjiq.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gzhuzhwes.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/grfxboqov.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gyxzbxcbw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gopdyspei.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/grmwnnufd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gvwefrnnh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/ghfckuftf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gxzsvljig.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gfspwvbix.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gkpywhmzu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/glrgbvuft.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.sjlbkw.cn/Article/details/gxzmpnlwi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gupvpnhnc.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.yfazqb.com/Article/details/gzvobuqnb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/gsnqimywa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.epnwcf.com/Article/details/gstsfnugj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gympgdscq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/ghuzyvbiv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gomnmeyvl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gikpfnjqa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.vehdjk.com/Article/details/gxamwheen.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.tarul.cn/Article/details/gjnnblzbp.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/gvyxicvmv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gxnvkalhn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gjhwspney.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gayacklnd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/ghkbdkbvw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gumicdatc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/glucottqv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gbwvwdvrd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/gtierklhc.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gjvtedpcg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fktsv.cn/Article/details/gvrwurcyc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gpwhvcqgt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gmntwlysk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gkjzapqjg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gdaunrcvo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gqdwposzi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gxelimzfn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gyprszmkz.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gbteewext.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fktsv.cn/Article/details/gfqfmxqbi.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gppicvmhx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gzhkfdznr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gwxgxozlo.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/gacdulbyz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gfynmdfgi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gdsmqvull.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gomxlcfzs.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gtwyjwjvz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gsmupmjuv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/grhfvqjum.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gjpkrrjqg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/grcypehyb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/grxzkadeu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifmdzfxr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.epnwcf.com/Article/details/gpafugkph.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gegykyvug.sHtML

[B15] 布尔运算与取反
来源：http://www.share.vehdjk.com/Article/details/gtlrhpfja.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gimwfobrt.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gyetvqgos.sHtML

JS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gqpxxsegi.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gpajpumek.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gcqkkanoy.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gsspgiinp.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gdsyuzxmw.sHtML

C#:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gzmhapdtz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/gijblvlst.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/ggehyongg.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gtizdwdol.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gjuegdzel.sHtML

TS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/ghmrkqmsp.sHtML

Java: if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gkluqzeht.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gnjwilmol.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gzhiftvny.sHtML

C#:   if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gavwgkdkh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpueoruog.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gcwfwauzu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glzhexdne.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/grwpmcbed.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/ggrtmkpof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gpebbmqub.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gwilvrgfe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gfyjawjkr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/glshorybb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/gtnpturir.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gygcxrmpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gxiabxdva.sHtML


<!-- 参考信息 -->