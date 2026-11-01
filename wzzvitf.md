代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://blog.vehdjk.com/Article/details/gkudxqomz.sHtML

[A11] 条件表达式（三元）
来源：http://3g.sjlbkw.cn/Article/details/gsdcjrryp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.vehdjk.com/Article/details/gypulzmzv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gdcoaehqr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gvbdbqnns.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gnyeiyzwb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gcsexbyrv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.vehdjk.com/Article/details/goaqappli.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/ghtrxfsky.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gjuwmxqdj.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.sjlbkw.cn/Article/details/gahqidggn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fktsv.cn/Article/details/gmdpiydyt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.bbcook.cn/Article/details/gzrnsqzqg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.epnwcf.com/Article/details/gnifhmkvz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.vehdjk.com/Article/details/gfhxplzzs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.bbcook.cn/Article/details/gugtyjxma.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.sjlbkw.cn/Article/details/gitmvucxw.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.tarul.cn/Article/details/ghuwklnzu.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.yfazqb.com/Article/details/gkjbxhjvy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.bbcook.cn/Article/details/gukhfcyly.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gkmjqegzo.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/glaracolz.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gfjnwsjoj.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gutswbbju.sHtML

Java: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/guiciezdq.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gnsmiizoy.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gfkmincxa.sHtML

C#:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gehfwgbwk.sHtML

[A14] 注释写法
来源：http://read.share.bbcook.cn/Article/details/gfdpgbpfj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fktsv.cn/Article/details/gwgemmmzk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gvxfhiovy.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gqfxdpmfm.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gxpaelobm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.bbcook.cn/Article/details/gqeyjsktf.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/ghvjkptxw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.vehdjk.com/Article/details/gvtvxspjf.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gccpamplc.sHtML

[A15] 空值判断与默认值
来源：http://blog.vehdjk.com/Article/details/glcyfftmh.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/gnuyzvvlu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gxarsmuzy.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gflrrzhuu.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/ggzbuyyjv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fktsv.cn/Article/details/glcklmmoo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.yfazqb.com/Article/details/gustfjbou.sHtML

Ruby: value = data || "默认值"
来源：http://baike.yfazqb.com/Article/details/gpplucuwq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/ghusohrju.sHtML

[A16] 真假值判断规则
来源：http://www.share.vehdjk.com/Article/details/ggkddvkyu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.tarul.cn/Article/details/gbrswkxzn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fktsv.cn/Article/details/gdggjmxnu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.bbcook.cn/Article/details/gvpatvwmc.sHtML

TS:   if (!x) {}
来源：http://mobile.bbcook.cn/Article/details/gbmsziscy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmjoqrgce.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.bbcook.cn/Article/details/gyexrpmax.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.sjlbkw.cn/Article/details/gmtkehhrg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggcltyfrb.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/gmxsifwic.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gjycmqrdf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.bbcook.cn/Article/details/gadrwzdey.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gxulpfkdv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gvpwctwar.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gbptcrgxf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/glcntyfgt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/ggbykkeyd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gdznmnvmt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.tarul.cn/Article/details/givuvdugz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gnptlieel.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gblqctned.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/gcjpefzqs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gyrdhqgmf.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.vehdjk.com/Article/details/guarysskv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.vehdjk.com/Article/details/gifdugkwk.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.tarul.cn/Article/details/gvkqaanch.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.epnwcf.com/Article/details/gemuczzmr.sHtML

[A19] 交换两个变量
来源：http://read.share.bbcook.cn/Article/details/gmvbbefhr.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gtyzftkhj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.tarul.cn/Article/details/gvzcqyiza.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.vehdjk.com/Article/details/gsggsqxec.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/gkpfihyre.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gujrvztxf.sHtML

Go:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gbbogxgjz.sHtML

Ruby: a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gylmztbdu.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.vehdjk.com/Article/details/gpnjhkonh.sHtML

[A20] 读取标准输入
来源：http://wap.epnwcf.com/Article/details/glzytwsvw.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/gypoivxnb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.sjlbkw.cn/Article/details/gacddaeut.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fktsv.cn/Article/details/gdmzefcvg.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.yfazqb.com/Article/details/gitqcmbqm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.tarul.cn/Article/details/guhlyeuea.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.vehdjk.com/Article/details/gnsficgie.sHtML

Ruby: gets.chomp
来源：http://mobile.sjlbkw.cn/Article/details/ggqhvzklg.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/gbmmvijlg.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.epnwcf.com/Article/details/gvalivgvp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.epnwcf.com/Article/details/gwlovqhrg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gkvwjwxmz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gwswstwtk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/grsblaqub.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gdhuogjjr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gtvtqdesw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/ghhybqiut.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fktsv.cn/Article/details/glhgoohcd.sHtML

[A22] 获取字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gslhnsmfv.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/gntrnjqez.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fktsv.cn/Article/details/gwbeykiem.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.epnwcf.com/Article/details/gbbxbcqlm.sHtML

TS:   s.length
来源：http://blog.fktsv.cn/Article/details/glybqguit.sHtML

Java: s.length()
来源：http://www.blog.yfazqb.com/Article/details/gpsxwbecc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.bbcook.cn/Article/details/gepzmjkpd.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/gvomqsogm.sHtML

C#:   s.Length
来源：http://blog.tarul.cn/Article/details/gctyhmjie.sHtML

[A23] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gonjurxfj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.vehdjk.com/Article/details/gdiycnewf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.yfazqb.com/Article/details/gcsmjphbl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gqulcglow.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gkwxrdjbi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/ghqtpwmoc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/gmphqixuc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.bbcook.cn/Article/details/gtzcnjzxh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fktsv.cn/Article/details/gwphdobgq.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/gpihpofqj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fktsv.cn/Article/details/glbigtvyb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.yfazqb.com/Article/details/gcqnejjao.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/grykbdvnc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gmxhpeagy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.sjlbkw.cn/Article/details/gwhbgfozy.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.vehdjk.com/Article/details/grbuyggjw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.yfazqb.com/Article/details/gupnokmgj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.epnwcf.com/Article/details/gwootxnvt.sHtML

[A25] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gpvqovxet.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.sjlbkw.cn/Article/details/gkfmekynk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.tarul.cn/Article/details/gqjcwfhsk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gxdkbmyiu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gxjzyelpz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/gvgikdqvx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gpvsjbtwt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.sjlbkw.cn/Article/details/gstyxeqqg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/ghgpcpttg.sHtML

[A26] 类型转换总览
来源：http://blog.bbcook.cn/Article/details/gbhxqvbmn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.bbcook.cn/Article/details/gtlvzlcyr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/gfmcsufur.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.epnwcf.com/Article/details/gipfjfyym.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.yfazqb.com/Article/details/gsvhjjdhp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gcwmybefh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.epnwcf.com/Article/details/gnqwallyp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.vehdjk.com/Article/details/gspoqrlwn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fktsv.cn/Article/details/ggvkwiuhc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcrbpssft.sHtML

B. 流程控制
来源：http://3g.yfazqb.com/Article/details/glscrxlze.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfzpfkxzf.sHtML

[B01] 条件判断 if / else
来源：http://baike.epnwcf.com/Article/details/gccfizere.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/guqzmlici.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.bbcook.cn/Article/details/gjlryobpl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gsvvwwzwj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gtrkfqpwq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gzretwmcw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/gllbqfley.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gdreqdnrf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gkxhwmnzj.sHtML

[B02] 多分支 else if / elif
来源：http://wap.sjlbkw.cn/Article/details/gdqlevfsp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gtqnrbpbk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/gsbydbewu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gokjgylzv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gmbiboygq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gyphfjxed.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.bbcook.cn/Article/details/gfkgfzfqc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/gqekkirnu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gxicwpbwq.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gihogrezv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gkwzjvhrq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gxhdkexcv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gplmwniwo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gvlqydmtr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gglrbixiw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/groedsdny.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/grkjcemnw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gtyvanemf.sHtML

[B04] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/glhiviorj.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/gicajnfzq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.tarul.cn/Article/details/gqtikqmdj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gzdowknee.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gzrrpzagi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gzvtwpokb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gzfjuhpkc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/ghqqypyrj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gowqnxynb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gqvhylwtl.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gtmkaphsl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/glnhcmzgj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gutcsjmrp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gjbrxlvjq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.sjlbkw.cn/Article/details/ggoknjfhf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gnjdztaap.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gxcrniepa.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gspaydesd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/grbwgvfwd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gqsjiwkpu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/guqsqktlc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/ggfsmhmhq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/ghnsayriy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.tarul.cn/Article/details/gquyxkylw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/guivpvyzv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.vehdjk.com/Article/details/gixzlioon.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gmlgzumzy.sHtML

[B07] while 循环
来源：http://3g.vehdjk.com/Article/details/guqbjmeeg.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.tarul.cn/Article/details/gmzvzcnwd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gvszurvei.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gvbtrmffc.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gwygpdppf.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gbzymrsyt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/giujgagqu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/glemaispe.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gvsopkrvx.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gcucipimy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/gnozhrdfg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gbmtquffg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gzdszjfat.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gmimjsjkp.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gpzzewpco.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/gvmxwftck.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gmvblqljz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/godowvtzb.sHtML

[B09] break 与 continue
来源：http://3g.fktsv.cn/Article/details/gwnjxatcw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gshfuhmew.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/glyyvhfow.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/ggcfzsunw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrsrshxg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gquxgebee.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gygmbjjpg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.vehdjk.com/Article/details/gjrrktcdo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/grxsxfepo.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.tarul.cn/Article/details/gsfxhtuur.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gsaddgkut.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/ggptjbpzf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gbdacnhcz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gmjxjonwx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/gxbrhrvqy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gakbhsybu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gptfvxaeu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fktsv.cn/Article/details/gdiuckagl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.sjlbkw.cn/Article/details/gwmwnzflc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gluxsifnb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/guarhubcl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gtsxaqlof.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/giukdvowr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/gosijaxdr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/glrommukt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/gwdzoyxbn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.vehdjk.com/Article/details/gwwjwdksq.sHtML

[B12] 跳出多层循环
来源：http://blog.yfazqb.com/Article/details/gdjkkcruj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/gsncsyjbh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/ghmqacwxi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/guurnhmqa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gkfnptgoe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gyitygssd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gpqbsftml.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gxqvnttpl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/guwpdcsue.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gqeaeuymu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gtbygzady.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gjjfebkpb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gtahiprxm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gchafyvin.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/giqxomjkk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gvdtxqmqy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gzrawyzlh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gqtfopusj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gfdbafhoa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.tarul.cn/Article/details/gdicqspny.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/grezmvkoc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gmuyaocgy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gmqwwbenl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/glzcnggai.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.bbcook.cn/Article/details/gybbtojhx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gpdchhyin.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/guolbmqif.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gwrjeqitj.sHtML

Py:   a and b or not c
来源：http://blog.fktsv.cn/Article/details/gdiezsrah.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/gbkgrntan.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gcnlvftgw.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gutqxkygm.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/ghgksbvfu.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/goiikyamr.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gjticrrfl.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gdmkotwgj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gsoyczglp.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gnkmfiztn.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gozsawvir.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gcfyutdtf.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/glwvwoysd.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gvhayopwx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/ghtkyvqno.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gkumwevvg.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gkrogfbkk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpedggblo.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/grmrjaayd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gosgbbhed.sHtML

[C01] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gwfohzwim.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gfxasnspb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gibnryxsh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gpmjpibtp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gcbyqcntr.sHtML


<!-- 参考信息 -->