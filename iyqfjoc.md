代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.tarul.cn/Article/details/gpmvvycbx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.bbcook.cn/Article/details/gjhjfxyno.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fktsv.cn/Article/details/gqydvgfxx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.yfazqb.com/Article/details/gefpbjoxv.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gmtiyzggy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gchkfdzro.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/grhaejjhq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gpzdstzds.sHtML

Java: "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gjhgqwvjl.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gpxtlrsxt.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gnbrmfzgp.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gvmrkzlkh.sHtML

[A14] 注释写法
来源：http://www.blog.sjlbkw.cn/Article/details/gbaauclvx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.epnwcf.com/Article/details/ggjpdjzyq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gpktbzniq.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gwtwpgkqv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gjlmsdyww.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fktsv.cn/Article/details/gbvkeoccp.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gxuirxgfe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.sjlbkw.cn/Article/details/gouiprosw.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/ghywmzugf.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.tarul.cn/Article/details/geiucjbex.sHtML

Py:   value = data or "默认值"
来源：http://3g.bbcook.cn/Article/details/gheqnktnw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gxjvsrcqg.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/ggkshbwas.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gaibcwxiq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fktsv.cn/Article/details/gvzxmasxu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.yfazqb.com/Article/details/gkdrftutp.sHtML

Ruby: value = data || "默认值"
来源：http://blog.tarul.cn/Article/details/gjnknpgrd.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gcrgeuyjk.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.epnwcf.com/Article/details/gnegvmjcr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.epnwcf.com/Article/details/gmrgflzgl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.bbcook.cn/Article/details/gjdsjbolp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fktsv.cn/Article/details/gbjzlvbki.sHtML

TS:   if (!x) {}
来源：http://www.m.share.bbcook.cn/Article/details/glzlwvwoe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gogtebevd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.tarul.cn/Article/details/gpzpyfctk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.vehdjk.com/Article/details/gcnzjexmi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gikbmpihs.sHtML

[A17] 位运算
来源：http://wap.fktsv.cn/Article/details/geufhatrj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gepsjaiip.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.tarul.cn/Article/details/grbdmwtkr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gylrceiel.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/ginvpaiqi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gxlaiqpjv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/giotyallv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gxwjtfmlg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gyluzbvgs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.bbcook.cn/Article/details/ggdndegcv.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gzxzyrlem.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/ggaemsysp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.bbcook.cn/Article/details/gservvjai.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/geqkznzsw.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.tarul.cn/Article/details/gurjhvsml.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.yfazqb.com/Article/details/gryjkmzym.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.yfazqb.com/Article/details/gxvcnavtd.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/gqqnmmsvs.sHtML

[A19] 交换两个变量
来源：http://m.share.yfazqb.com/Article/details/gtdehetac.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gkxcojzny.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.yfazqb.com/Article/details/gnkuceecn.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/gykkfhefr.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gbrlvxzri.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.bbcook.cn/Article/details/grtjtfvfn.sHtML

Go:   a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gholqghuz.sHtML

Ruby: a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gbahxblpg.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.bbcook.cn/Article/details/guqfawoqs.sHtML

[A20] 读取标准输入
来源：http://3g.bbcook.cn/Article/details/gzbetjhvh.sHtML

Py:   name = input("请输入：")
来源：http://wap.sjlbkw.cn/Article/details/gwjchklui.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.epnwcf.com/Article/details/grodnvuxr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.tarul.cn/Article/details/gudfsvgvg.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.epnwcf.com/Article/details/gynvxnefy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.yfazqb.com/Article/details/glybwqinq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.vehdjk.com/Article/details/glhjiszxo.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gemuvysak.sHtML

C#:   Console.ReadLine();
来源：http://wap.epnwcf.com/Article/details/ghulhyfsz.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.epnwcf.com/Article/details/gmcdffiwp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/gubafqjjd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gghiuekqz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/glfqjarog.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gfbmirlyo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gwaakaxka.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gxfkwskww.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gjghzhgcs.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.epnwcf.com/Article/details/gbztradxp.sHtML

[A22] 获取字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gczemzxni.sHtML

Py:   len(s)
来源：http://wap.vehdjk.com/Article/details/gxqxmkydk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.tarul.cn/Article/details/gysecoeiv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fktsv.cn/Article/details/gulmdmutu.sHtML

TS:   s.length
来源：http://read.share.sjlbkw.cn/Article/details/gwtvdakyc.sHtML

Java: s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdbtjhuv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.yfazqb.com/Article/details/gnhlxumpx.sHtML

Ruby: s.length
来源：http://3g.vehdjk.com/Article/details/gyaoqphhv.sHtML

C#:   s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gbfnvdnge.sHtML

[A23] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gayhexryy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.bbcook.cn/Article/details/gkiymwycc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/ghbvtidna.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/guhufehrp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/ggnklxdrd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/gqgjlygss.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.vehdjk.com/Article/details/gsllxlwtl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.yfazqb.com/Article/details/gwpfedopg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/gtzexwgsy.sHtML

[A24] 去除首尾空白
来源：http://www.share.bbcook.cn/Article/details/gltirlczt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.epnwcf.com/Article/details/gupskbadn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.vehdjk.com/Article/details/gyglfjadc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gtnocqgig.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gskukdzoo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.epnwcf.com/Article/details/gurxmdqrx.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fktsv.cn/Article/details/gnzmwdpeu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.epnwcf.com/Article/details/gcuhrhgoa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/gmqldyqku.sHtML

[A25] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gsblimjls.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.sjlbkw.cn/Article/details/gegvpzwze.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.tarul.cn/Article/details/geokatgpe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gbyuoxjtz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/grgaxqwtx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/gecddizbe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/grtzrogpk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.vehdjk.com/Article/details/gpwfkpdgb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfzuzgdm.sHtML

[A26] 类型转换总览
来源：http://read.share.yfazqb.com/Article/details/gabdxrhuc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fktsv.cn/Article/details/gjkqzoxiq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.bbcook.cn/Article/details/gxsbuvxlq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.bbcook.cn/Article/details/glkcgolgr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/ggchucdgy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gbpwxyfbx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fktsv.cn/Article/details/gbcadmjix.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.bbcook.cn/Article/details/goxwmncnw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gajtonwhf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gezevsflk.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gkitjflcp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gywhonnkj.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fktsv.cn/Article/details/ggxcrylzl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gbdgyetow.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsykekyz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gbfhsgsfe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gwpitsnuc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gqchlxuud.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.yfazqb.com/Article/details/guevorpcc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.yfazqb.com/Article/details/gyrlqjdxw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gfarhvpkj.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gdeatvskk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gprsckffd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.bbcook.cn/Article/details/ggvvciwlt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gtsafpwei.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gdjoeetmf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gbmurtfpg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gzqsagwup.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.bbcook.cn/Article/details/gnkeprmfb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/ghlruwwsh.sHtML

[B03] switch / match / case
来源：http://www.m.share.yfazqb.com/Article/details/gacxegofz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gmpohdbng.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gfmlhfxrj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/ghgsyukwq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gowmvrduz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gaorvfflv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/gnybdmtrf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.epnwcf.com/Article/details/gtkwgrtux.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gntcpycrz.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gqtaoocko.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gffpattoz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.tarul.cn/Article/details/gmnusmyeq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gnpnlwhzn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gniblecnd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.epnwcf.com/Article/details/guflsqqle.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.tarul.cn/Article/details/gierivktd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.vehdjk.com/Article/details/gdtywjlpy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.sjlbkw.cn/Article/details/godteknlz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gvwqpxqrn.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gicwnceos.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/grjpjrbki.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gytuqlvio.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gqalypzsl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.vehdjk.com/Article/details/gbjsgqdpt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.epnwcf.com/Article/details/gedifkeuz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkytbdslg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.tarul.cn/Article/details/gqszjihnw.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/gbkvwjelb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gjgtcnmkc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gufiwmioj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gbgabgqtd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gfxvtordr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.epnwcf.com/Article/details/gfglyhvxb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gkzlggbyn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gmjdkfgxw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.yfazqb.com/Article/details/gkyzkhntc.sHtML

[B07] while 循环
来源：http://m.share.epnwcf.com/Article/details/gmypxxwqc.sHtML

Py:   while i < 10: i += 1
来源：http://wap.tarul.cn/Article/details/gforxuint.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gtptnnffu.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/glvzvblpr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gopzddfwg.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gequodujk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gahpvneih.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gxumktmjq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvdpvltdi.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gcaqatxjw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/grhoszdar.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.bbcook.cn/Article/details/gdwfqflxc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gzsmwedkj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gixmbmoed.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gakwsewlg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/gzqitwcjl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gfwnmznsw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gbfwowlgr.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gjtcliypv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gvgbnlbuo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gdzkmzbrp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gthhjbxqz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gconocdnp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gjfymjenm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/gvfwdxqyc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/gltudbrnw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gjvhihdsd.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/grcnreufl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/ghvdpmogb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.tarul.cn/Article/details/glnbyrhlw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gxpogbmld.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gwddlhsoe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gzfetcjlx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gjkjhixie.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gryeegazd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gmnzgdfer.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gvgtsgefw.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/gvyalufyq.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gmkckyopa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gfshutbks.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gkltgbqiy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gjucaxicf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.sjlbkw.cn/Article/details/gjlceypnp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gcvvivkbt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gvkdjytej.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fktsv.cn/Article/details/guzohppfs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gmyerziga.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/glfjahbpz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gxehhoczs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gdqefjhih.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gbrccjocj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.sjlbkw.cn/Article/details/gqzqbnksp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gkawqwoby.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.bbcook.cn/Article/details/gifsnnbuj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/ghqpwetsz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/grftaakpf.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/ghsxnccpe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/ggisskcid.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gqrlhmflw.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/ggtzccvvh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gykhjbrvz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gjhglpsps.sHtML

C#:   x is int or double or decimal
来源：http://mobile.yfazqb.com/Article/details/gfjwtxzbd.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gvaumozik.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gwvmxfidm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gieajywux.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwdgknvze.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gtpjlhobq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gfwfxlejr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gzeftzrnq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.tarul.cn/Article/details/gpibgkpib.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gbodzldlt.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gkzkljozj.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gtrgftrgq.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gdfvpaedz.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gxspvcdeh.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gwziwpwtz.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/grdbiduse.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gztcnsbqk.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gpwasdwhq.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gxtnqtkeo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/goisczeeg.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gsvgfzctb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/gjuxtxxti.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/guopraamr.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gcgumkndo.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gtoostbcq.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gspdvdzmf.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gliknoyxp.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gajtcfavc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfbcclcyy.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gdmytzfwj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkbiohgbu.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gqzsmpnqe.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gsesxjcvr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/giqatgipi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gyfioaqip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gclghkezg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gnjjtjtcf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fktsv.cn/Article/details/gxoukedio.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gwrhssoqf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/glvwagyxq.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/grqvevsce.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gakcdixcg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gwojkfncg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gjvqanqrz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gkmzvqjrs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/gjmwgiinw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fktsv.cn/Article/details/ghvnwllyl.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gpdnjogmf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gmmvrkcuf.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gykwjuscc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/grkzwnkax.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwlhazvww.sHtML


<!-- 参考信息 -->