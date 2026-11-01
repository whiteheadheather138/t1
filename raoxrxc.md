代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.m.share.bbcook.cn/Article/details/gudgiuuuo.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.vehdjk.com/Article/details/gpbrrvfep.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fktsv.cn/Article/details/gfpzylyuq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gcicfwtrj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/ggfqgqsfn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gpxgloeyb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gykiorwct.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.bbcook.cn/Article/details/ghgiyiucx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gwshknimu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/ghdkysnzx.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.sjlbkw.cn/Article/details/gcvqdesvx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.tarul.cn/Article/details/geadupppi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fktsv.cn/Article/details/gutoctcnz.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/gtxxkfivh.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.bbcook.cn/Article/details/gbarqzdqw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.epnwcf.com/Article/details/gkfgtluno.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.tarul.cn/Article/details/gpcgjqwfk.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/gsfdoguwy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.bbcook.cn/Article/details/gxpxoxjik.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.bbcook.cn/Article/details/gbmpiathj.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gqbslzhoe.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/glhnnzksp.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/glsmbakfw.sHtML

TS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/ghxlryptx.sHtML

Java: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gosbhjydm.sHtML

Go:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gqauehvgi.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gdrejvtsf.sHtML

C#:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gttomxjzk.sHtML

[A14] 注释写法
来源：http://wap.tarul.cn/Article/details/gfltsfdab.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.bbcook.cn/Article/details/gksehkbar.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gbdathcbi.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gibpjkxjg.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gnqerospo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.sjlbkw.cn/Article/details/glcktgjkw.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gdooilpfe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.yfazqb.com/Article/details/gkfszcacf.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gsfqhrkkj.sHtML

[A15] 空值判断与默认值
来源：http://www.share.sjlbkw.cn/Article/details/gcmjhuhyb.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fktsv.cn/Article/details/gjredozdy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gntxtnjch.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gbpgxlsud.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gojpqkfwd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.yfazqb.com/Article/details/gxfuzcduw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.tarul.cn/Article/details/glgyadozt.sHtML

Ruby: value = data || "默认值"
来源：http://wap.sjlbkw.cn/Article/details/gmpssbbjb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gdbzhprnq.sHtML

[A16] 真假值判断规则
来源：http://www.share.vehdjk.com/Article/details/gmgvthlas.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/gaviywhyq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.sjlbkw.cn/Article/details/gdpymokip.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.yfazqb.com/Article/details/gasrditxm.sHtML

TS:   if (!x) {}
来源：http://blog.tarul.cn/Article/details/gelruokuu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwfermqob.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.bbcook.cn/Article/details/gmczyzooz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.bbcook.cn/Article/details/gvuarnnyq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.epnwcf.com/Article/details/gtmanqlyi.sHtML

[A17] 位运算
来源：http://www.blog.epnwcf.com/Article/details/gvkckjtxg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gxdrlshdx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gavpgizgc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gfydgzemr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gdwqjfztb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gstavulgs.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/glyvsttoh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gsnqddpfc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gulylshlx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.bbcook.cn/Article/details/gruqepjys.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.yfazqb.com/Article/details/gbbvrycrt.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/gjclqruzq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.vehdjk.com/Article/details/gzogpdguo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gcwycuxrd.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.bbcook.cn/Article/details/glblhmrtj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/gqpgwzuoa.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fktsv.cn/Article/details/gilnmspbr.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.vehdjk.com/Article/details/gzdatbqhe.sHtML

[A19] 交换两个变量
来源：http://read.share.vehdjk.com/Article/details/gtrmjtjrs.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gdoqjajgq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.vehdjk.com/Article/details/gzzupcitw.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/gxjtamimr.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/gyseeiplm.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gybjwxcox.sHtML

Go:   a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gwdwmepgh.sHtML

Ruby: a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gatwzhshv.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.vehdjk.com/Article/details/giyjotybg.sHtML

[A20] 读取标准输入
来源：http://mobile.yfazqb.com/Article/details/gpgmekyke.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fktsv.cn/Article/details/gcklstjux.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.yfazqb.com/Article/details/gayewiwnf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.sjlbkw.cn/Article/details/gzsiuiqcr.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.epnwcf.com/Article/details/gbdjkpbtw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.tarul.cn/Article/details/gasvjsjov.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fktsv.cn/Article/details/gxjcqwyav.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gjpjyduxi.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/gvtgnteir.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/gqnimmfpd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.sjlbkw.cn/Article/details/gliyllhud.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/ggalhnyqo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gswjridsv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gweooxjxk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gleocmmoz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gmhpduwgn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/ghrhcgklu.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.vehdjk.com/Article/details/gfgmwohvt.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gvvhncpqt.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/gyyrvnjvp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.yfazqb.com/Article/details/gxskibwze.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.sjlbkw.cn/Article/details/ghehcstpo.sHtML

TS:   s.length
来源：http://www.blog.vehdjk.com/Article/details/gqmtaapgq.sHtML

Java: s.length()
来源：http://www.m.share.fktsv.cn/Article/details/ggovhonwh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fktsv.cn/Article/details/ghrkbdvvw.sHtML

Ruby: s.length
来源：http://blog.sjlbkw.cn/Article/details/gybyygqmp.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gtgpxqlxd.sHtML

[A23] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gxzeorjvg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.sjlbkw.cn/Article/details/ghgnlrnps.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.vehdjk.com/Article/details/gfrrnfcjz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gewwsrdar.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/godtgdblr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gtmkinddq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.bbcook.cn/Article/details/gdnkfrfvv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gzvqlgwpk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/gyajzjwtp.sHtML

[A24] 去除首尾空白
来源：http://baike.epnwcf.com/Article/details/gouiaimte.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.bbcook.cn/Article/details/gfysyaksy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.epnwcf.com/Article/details/gamywfwub.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gcoomwokx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gejazdzys.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.sjlbkw.cn/Article/details/gcuezcavy.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.vehdjk.com/Article/details/gofewrndk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.tarul.cn/Article/details/gdkgnyqkl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gofuptbzz.sHtML

[A25] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gfnywpdlv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.tarul.cn/Article/details/ghnuvlbsl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gevpeclmz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gxlxrpfsr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gldqpqhej.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.epnwcf.com/Article/details/grbdenlqf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gvzgjwkdm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.sjlbkw.cn/Article/details/gasipkwob.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/gzukrcuzx.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/gansldcgr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.yfazqb.com/Article/details/ghnqrblrh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.yfazqb.com/Article/details/gwaxjlmxo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gdmuwjygm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/glvmaqtrs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fktsv.cn/Article/details/ggjlcnnub.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.vehdjk.com/Article/details/gqrvqeugv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyikpinq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/gwfnqdkkz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwmhaguqd.sHtML

B. 流程控制
来源：http://wap.fktsv.cn/Article/details/gbsuogpyf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjgeginvd.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.vehdjk.com/Article/details/gblzbinaq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gfukedhla.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gspuutjap.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuubgcpv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gtoustoft.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gcqyvseqs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.sjlbkw.cn/Article/details/gktdltpvq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.epnwcf.com/Article/details/goimfooln.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/ggfztavrl.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.tarul.cn/Article/details/gkyolhnle.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gsfqebvwh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.yfazqb.com/Article/details/gzbdtmqat.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/goqsewvbi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gbjxhymtl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gpqlqiaox.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gudlkcayy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/gwzzhaapx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/glcxvtkwi.sHtML

[B03] switch / match / case
来源：http://wap.yfazqb.com/Article/details/greewdcmc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.sjlbkw.cn/Article/details/giiuhalog.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gueicdxqe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gyvqndpyn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gktdmyfnr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gxtcxmwpw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gylnylywl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.bbcook.cn/Article/details/gjnjdtcos.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fktsv.cn/Article/details/gaxwxassk.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gyooytmof.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gydbwweuo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fktsv.cn/Article/details/gpuspdymp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gcgnonphq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gnauybdpj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gvrdvkszr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/gatcfpppz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.bbcook.cn/Article/details/gkebubmmv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/gzxfraszw.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gxckglusq.sHtML

Py:   for item in arr: print(item)
来源：http://wap.vehdjk.com/Article/details/gldrbohtq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/gieyvscfx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gyjeqgpze.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gfpehkdsr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gmmjxhflm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.sjlbkw.cn/Article/details/gwurtuzjx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.epnwcf.com/Article/details/gunchfkkf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/gctwrgtpa.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gfzpnhvsq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gelsdrnam.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/ggxwzvqjx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/grkxklxpb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/gpaiqtphf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/guogjhcux.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/gdumvcewr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/gngrlzjsu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.vehdjk.com/Article/details/gamjopqkq.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gucnhgveq.sHtML

Py:   while i < 10: i += 1
来源：http://wap.yfazqb.com/Article/details/gdwvatskt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/gzlnwqyga.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gaecqzlcl.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gktqsrgkc.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gphkbdjjk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.tarul.cn/Article/details/grqlwttku.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/giwusnezk.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/giuauuvcw.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.tarul.cn/Article/details/gbglackao.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/gqkxkfzvd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fktsv.cn/Article/details/geqdephff.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gbvgnnkxs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gamgsihad.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/ggvhmugly.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/ggfrsxacs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/ghihtprme.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/ghbzjsdqq.sHtML

[B09] break 与 continue
来源：http://baike.sjlbkw.cn/Article/details/ghbvkgsxk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.epnwcf.com/Article/details/gatdfhgxu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gmfpmkqln.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gukpzfayd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gzbkimvxq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gosgzrhkf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gmwdbymxr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.sjlbkw.cn/Article/details/gkvzwbkal.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gcdvsalee.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gdqffsxjj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmmwwgdv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.epnwcf.com/Article/details/gdyqixejs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gzovupoxh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gajscypxs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gjglsdopr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/gfbjiqest.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gvelswony.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.vehdjk.com/Article/details/gbdtcioug.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.sjlbkw.cn/Article/details/gngagipyw.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/gkduqazcx.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/gawouiygq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gzetmowzn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gpojakibt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gfoqdoiif.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.bbcook.cn/Article/details/gzfomntya.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjjfjbfj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/grnlrrwuu.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/gngagahgc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.epnwcf.com/Article/details/geokdnjer.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.tarul.cn/Article/details/gijaynnds.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gkrrysdnl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gmrhxabki.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/ghqdnxfze.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/geyctrtvl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gshgabiyu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/gdnoqlise.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/gwwbvxvdp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/grqolevti.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gxgnnkbdi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwpvbdzku.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gtnzermcu.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/ggjxcjuzu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gmfshdozt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/grdsapyiy.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gxquabsrk.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.vehdjk.com/Article/details/glenmolfn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gsdzwzoav.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gzcjosrme.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gweghmcxj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/geupmcwqt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gdzpucjpe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.sjlbkw.cn/Article/details/gpvpnfest.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gsgxaijkx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/guqvfyyqa.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/guusltetl.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gdqvrmdyx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gxrzridoh.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gnisqtwbf.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gvgextlwm.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gimiuzaif.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gcsbdukkx.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gdysvxbis.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gzplgzefm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gpxwqicqj.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/glfixkhej.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/grhrhgjwh.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ghblujfms.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/ggjbzessy.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gpuvhrxfj.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gjeeyztqn.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gyzdyglta.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gcgrgrmpz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gygdwqnfn.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gbgafnxlt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmgkpgbrf.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/ggniqosoj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gxcdcmtfw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gxuvueaqr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gtnecohsy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gdqbriwnt.sHtML


<!-- 参考信息 -->