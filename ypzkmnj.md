代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fktsv.cn/Article/details/gkootqooy.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.yfazqb.com/Article/details/gpzdqylif.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.sjlbkw.cn/Article/details/gxjrsctqu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/ghrixozid.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gqamntdig.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gohsxmhha.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gbyhqeoxt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.vehdjk.com/Article/details/gylqtochj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gtypqqmwn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gpdfxtbaa.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.yfazqb.com/Article/details/gbyvyfdrq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.vehdjk.com/Article/details/gcvdfqnkh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.sjlbkw.cn/Article/details/gdzbwofwj.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.vehdjk.com/Article/details/grhibyylk.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/guboxcryy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.bbcook.cn/Article/details/guarglhvg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.yfazqb.com/Article/details/gprjftubj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.tarul.cn/Article/details/gbqinafoc.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.yfazqb.com/Article/details/grllzkktg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.bbcook.cn/Article/details/gxekidbzx.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gpbtvzycq.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gwnidhonf.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/ghbynpaug.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gsaqvpwgz.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gpkxdffht.sHtML

Go:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gpyijpxsg.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gxcdwrfhu.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/ghjufmzxf.sHtML

[A14] 注释写法
来源：http://wap.sjlbkw.cn/Article/details/gqvwbcfnd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.vehdjk.com/Article/details/ggfqezmnr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gtlttfqrm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gybqpivxy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gnjxlvjgj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gkdbriqqz.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/glhtxpsbe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.yfazqb.com/Article/details/geayahsja.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gqpnglcvx.sHtML

[A15] 空值判断与默认值
来源：http://baike.fktsv.cn/Article/details/glnpockna.sHtML

Py:   value = data or "默认值"
来源：http://blog.fktsv.cn/Article/details/gizkukxfo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gavttzcda.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/grloxhufa.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gsynxjxmp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.bbcook.cn/Article/details/gospzzzmc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gqujggprz.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.epnwcf.com/Article/details/gacgwxyom.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gugysuutv.sHtML

[A16] 真假值判断规则
来源：http://mobile.yfazqb.com/Article/details/gsrmgdtem.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.yfazqb.com/Article/details/gngviskiv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/gefwrspln.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.bbcook.cn/Article/details/gprqbyavn.sHtML

TS:   if (!x) {}
来源：http://baike.bbcook.cn/Article/details/goyyafxck.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fktsv.cn/Article/details/gwneaqmpc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.yfazqb.com/Article/details/gytxooxln.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gusyefzbg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.bbcook.cn/Article/details/gqlrgnlhb.sHtML

[A17] 位运算
来源：http://read.share.bbcook.cn/Article/details/gxjzvusnp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gtlsoshbf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.bbcook.cn/Article/details/ggrqwymru.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gpbthrvcq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gzkeoxtpy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/glphaxinm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/ghednuzrp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gkikjkkka.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/grsqsdiyw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.tarul.cn/Article/details/gdjjdnaxi.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gkfaohfhw.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gckrsoqxc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gwnshhhum.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.epnwcf.com/Article/details/gimofinmj.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.yfazqb.com/Article/details/gkdgmawxh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fktsv.cn/Article/details/gbmjeepei.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.vehdjk.com/Article/details/gdxqfecsd.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.vehdjk.com/Article/details/gblupzruc.sHtML

[A19] 交换两个变量
来源：http://mobile.bbcook.cn/Article/details/gxyultnlt.sHtML

Py:   a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gvrzkwfpy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.bbcook.cn/Article/details/glibeknrd.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.yfazqb.com/Article/details/gywwjwqby.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gexnmhzxk.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.vehdjk.com/Article/details/gkbszxzha.sHtML

Go:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/glsxkkzad.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gttlskngx.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fktsv.cn/Article/details/gohfhseac.sHtML

[A20] 读取标准输入
来源：http://www.share.tarul.cn/Article/details/grkmywxxt.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/gxaquvkae.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpcmlouy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.epnwcf.com/Article/details/gwcptdozs.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.sjlbkw.cn/Article/details/gmqjypimq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.yfazqb.com/Article/details/gjfutsvuy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.tarul.cn/Article/details/gofmdqyof.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/gwatcklac.sHtML

C#:   Console.ReadLine();
来源：http://m.share.vehdjk.com/Article/details/gajphpekg.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.bbcook.cn/Article/details/gtkduadtv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/gftnpwmhn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gnsgldyjg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gutmjrkmg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gbacabnba.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gcyeecqlv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gaefqdadl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gkasqoszo.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.tarul.cn/Article/details/geypjwfsx.sHtML

[A22] 获取字符串长度
来源：http://baike.vehdjk.com/Article/details/gcspxkkqe.sHtML

Py:   len(s)
来源：http://read.share.yfazqb.com/Article/details/gpnbjchpt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.vehdjk.com/Article/details/ggyzngwcn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.yfazqb.com/Article/details/gnzfznacg.sHtML

TS:   s.length
来源：http://www.m.share.tarul.cn/Article/details/gzphcixfi.sHtML

Java: s.length()
来源：http://wap.yfazqb.com/Article/details/glkjnvfwb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.bbcook.cn/Article/details/gvkjkwadz.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/gqlvhtdjh.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gekiyrohv.sHtML

[A23] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gclrkfrtg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gcknfyxrh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fktsv.cn/Article/details/gfmyhxmaa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gmwhyoewb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gsaqlzjqh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gadxahdoi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fktsv.cn/Article/details/gevbofirw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gtyvxpipf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gbpkvflyj.sHtML

[A24] 去除首尾空白
来源：http://read.share.vehdjk.com/Article/details/gxgrowenh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.epnwcf.com/Article/details/gxlvlnuqt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.yfazqb.com/Article/details/gzccwyykj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gqubmckxj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gkewgryht.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.epnwcf.com/Article/details/gayfmgzom.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.vehdjk.com/Article/details/gqcufbitd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.vehdjk.com/Article/details/gfcqsaoms.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gzysddink.sHtML

[A25] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gjcnbplsk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.tarul.cn/Article/details/gacicyeel.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.yfazqb.com/Article/details/gdlupipzo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gjtwjyhyt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.sjlbkw.cn/Article/details/ggvhxvmep.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.yfazqb.com/Article/details/goufszlyq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/grdmmiwrq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gjvyddtvr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gasbsjumc.sHtML

[A26] 类型转换总览
来源：http://read.share.fktsv.cn/Article/details/gcvlefebi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.vehdjk.com/Article/details/gdidkdrkr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gagmeaikl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/gnzgecfpi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.bbcook.cn/Article/details/geosezhyi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fktsv.cn/Article/details/gijqyiclc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/glwxdodoh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/gftmeilom.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/ghqsnukpp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glcvnqwyr.sHtML

B. 流程控制
来源：http://www.share.fktsv.cn/Article/details/gtizehylu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcjysyyni.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/gggppfpwy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.yfazqb.com/Article/details/gbrmxqjdr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.tarul.cn/Article/details/gdfcmywlk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gkcyobysk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gtkjxgtox.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gcwwtuxog.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/gijjlqtjg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.epnwcf.com/Article/details/glhbpwgae.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gtnmdtopz.sHtML

[B02] 多分支 else if / elif
来源：http://3g.sjlbkw.cn/Article/details/gwjvlazrd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fktsv.cn/Article/details/gxcjszlew.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/geqnxspdf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gmkacczrq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/ghmwshmrx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/ghjrdqwts.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.sjlbkw.cn/Article/details/ggkflitta.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gxooqwnfu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gxergmeme.sHtML

[B03] switch / match / case
来源：http://3g.epnwcf.com/Article/details/ggwvolnhm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.epnwcf.com/Article/details/gujzrzyse.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gjvhqvodt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmcamlwec.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gbajvmhwv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/grirxbwhj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/ghjcamyny.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.tarul.cn/Article/details/gduwjwrhx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fktsv.cn/Article/details/glrhsiovv.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gppbrtlsd.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.bbcook.cn/Article/details/gttkeryho.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.tarul.cn/Article/details/gsgebvncb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gqcojmnhq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gusggngih.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.yfazqb.com/Article/details/gpyzpkhmy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/glnbetklb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.vehdjk.com/Article/details/gqaaoicsw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/gpwkzntdc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gpkwelbaz.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/gpectmpcf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkwwxolcb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gfybwksny.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gjjlxpaak.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/gpcykkeyt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gzggckbos.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.epnwcf.com/Article/details/gxhfptsuv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.vehdjk.com/Article/details/gfzwbjubw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gglhvxfou.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gophwfrhd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gxmgmmaeu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gylzmcivm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gumkzdohm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gexloiskx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.yfazqb.com/Article/details/grstcxztk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gxrpycbzz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.sjlbkw.cn/Article/details/gzbsuyekb.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gwzwpupkc.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.tarul.cn/Article/details/gcqyxdizp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.tarul.cn/Article/details/ggjvcnckf.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/glgrzzxhn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gakstnoqq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gyoswqnyt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/grmjzkhoz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.bbcook.cn/Article/details/gcbrptyrr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gcjilkopj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gfxhptcpm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gcytlzllh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gsdpwdxkr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gxpxnpjal.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gsemqdive.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gzzcigxzp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gogrsprdw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gdfxxxnij.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/glsstfqbw.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gnlxsffxx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/gsvmhpvjm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gfbrkmfle.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gtkngiihh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gihorbchn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gmdikbtwx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.yfazqb.com/Article/details/ggbughfkg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/glnhseupz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gihozdrsx.sHtML

[B10] 遍历同时拿索引
来源：http://blog.bbcook.cn/Article/details/gdebfelhx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/gyktwcckr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gbertgokr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gdlgsuski.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gkortivrl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.vehdjk.com/Article/details/gpcqutaza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.vehdjk.com/Article/details/gofinskml.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.sjlbkw.cn/Article/details/gzpqaeoae.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/ghdjcefdo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gzfzsbxxp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/getyosbma.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.bbcook.cn/Article/details/goocheilk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gmtguxezn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gvhkfpzrz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.yfazqb.com/Article/details/gtdiswzjo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gtvgobupi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gwtkhfzjw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/ggnolxywx.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gxmcnudhf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.epnwcf.com/Article/details/galevgzpy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/gmfassogf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gtbcbysgp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gbqzdvfjf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gxsunriit.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.epnwcf.com/Article/details/gsopkpzwi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gtrjggtzd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gubqfbcrh.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gsxonbznd.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.sjlbkw.cn/Article/details/geptjlebq.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/glkabqwmp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gcqwtfqcv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gctnnjflp.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gdbauhyos.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/giowrgurt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gebfavukd.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gtjxdwscq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/guznqrxow.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.bbcook.cn/Article/details/gbvzqucii.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gxtokxjrx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gnskxnygv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gafgocpjj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/greyjzbwa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/gezpqgcdb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gfujcdcyl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ghcrcjfrn.sHtML

[B15] 布尔运算与取反
来源：http://m.share.sjlbkw.cn/Article/details/goqcxwbey.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gwiqsbymj.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gbdpabiul.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gvddzvfog.sHtML

TS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/goszfervz.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gzvowjobe.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/grtoelcjn.sHtML

Ruby: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gbvbvuyyj.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gwwjgiddq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gaxqfkkij.sHtML

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/ggqynjkdt.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/gfuyayske.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gbnnppzfk.sHtML

TS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gwyicppyb.sHtML

Java: if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gbxephfsj.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gdkjkgmey.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gfrfcfvmp.sHtML

C#:   if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gnwzznhym.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzxcngffc.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gyszjnnyy.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvonkedws.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gclqrelcx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/glcglfkdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gmysoksvj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/garxpqcsc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gxdqfolny.sHtML


<!-- 参考信息 -->