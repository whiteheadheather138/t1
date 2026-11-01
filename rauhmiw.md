代发 wailian999

Py:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gdwuthajf.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gxrewvfyw.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gymolitui.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gctqkfxul.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gfyuzyqoi.sHtML

Go:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gcdjepjfm.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gqxmywnwr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gywssfryc.sHtML

[A14] 注释写法
来源：http://m.share.sjlbkw.cn/Article/details/gzffrdsdb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.yfazqb.com/Article/details/ggyprvopr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gxgjzuxor.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gpwnbkwip.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/glsrdzsnw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.tarul.cn/Article/details/gcjkgxawj.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/geymspwsv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.bbcook.cn/Article/details/gtwsnzkqe.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/guhvjpadv.sHtML

[A15] 空值判断与默认值
来源：http://www.share.sjlbkw.cn/Article/details/gwpcvjhgo.sHtML

Py:   value = data or "默认值"
来源：http://mobile.epnwcf.com/Article/details/gukoglhgm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gqgrvmrjc.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/griglkajw.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/ggzkwtboz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fktsv.cn/Article/details/giapqfeqa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.vehdjk.com/Article/details/gudwzinul.sHtML

Ruby: value = data || "默认值"
来源：http://wap.vehdjk.com/Article/details/gqvcyexsb.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gqduwvzzc.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.tarul.cn/Article/details/glpaonnop.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.vehdjk.com/Article/details/gchwlwhxw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fktsv.cn/Article/details/gezodsdii.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.tarul.cn/Article/details/gcwxsghns.sHtML

TS:   if (!x) {}
来源：http://wap.yfazqb.com/Article/details/ghnkbvaps.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.epnwcf.com/Article/details/gznqtqhzn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.bbcook.cn/Article/details/gnmpxvlko.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.yfazqb.com/Article/details/gvwwhctng.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gnambfmjc.sHtML

[A17] 位运算
来源：http://blog.fktsv.cn/Article/details/ggbhpefhr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gomulugje.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.yfazqb.com/Article/details/gjhlpjnkn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/ggvxwjjqu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gdzltlfmf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gumukbwle.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gorrgvuto.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gbfqsnjug.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gwwrdxftd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fktsv.cn/Article/details/gxewfslow.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gyajldeaz.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/gnchyzyss.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gbcqepcyz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gphggjibl.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.yfazqb.com/Article/details/gffyvgcar.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.bbcook.cn/Article/details/ghbjnrmab.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.yfazqb.com/Article/details/givhqratk.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.tarul.cn/Article/details/glaimclit.sHtML

[A19] 交换两个变量
来源：http://www.m.share.bbcook.cn/Article/details/gciqjomoc.sHtML

Py:   a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gnyklyvqf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/ggqemhekn.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/gfpkqtpbm.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/gbxgylniq.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fktsv.cn/Article/details/gvnbuzlgy.sHtML

Go:   a, b = b, a
来源：http://read.share.vehdjk.com/Article/details/grqpwtxjk.sHtML

Ruby: a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/grduhgbia.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gvdtydszx.sHtML

[A20] 读取标准输入
来源：http://www.share.sjlbkw.cn/Article/details/gkemuoeav.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/gwyhcmrio.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.sjlbkw.cn/Article/details/gbypeluvj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.sjlbkw.cn/Article/details/gkyznmsqa.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.sjlbkw.cn/Article/details/guaglfcmk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.tarul.cn/Article/details/ghihwvkug.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfiezayu.sHtML

Ruby: gets.chomp
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkqyjven.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.sjlbkw.cn/Article/details/grmzyemml.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.sjlbkw.cn/Article/details/gdojpmgft.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/glqyhvayk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gewozhqie.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gqctwnkdp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gmsqwdtbj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gqphereda.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gpomyhuwl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gfvmrcvql.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.vehdjk.com/Article/details/gglkoasyx.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gqbolfrxj.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/gfnxpmsid.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.bbcook.cn/Article/details/gqxfdrgeb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fktsv.cn/Article/details/gvtprlqny.sHtML

TS:   s.length
来源：http://blog.fktsv.cn/Article/details/gbdwutxij.sHtML

Java: s.length()
来源：http://mobile.tarul.cn/Article/details/gcqosvqhp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/gmkbbixrg.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/glcnitgri.sHtML

C#:   s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gigsgfomu.sHtML

[A23] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gsxrpnnee.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.sjlbkw.cn/Article/details/glfcmnizf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.yfazqb.com/Article/details/gfyemuexm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gznenbddh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/ghdsdrdbc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gtivqtrbb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gqamshzdt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gzcksffla.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/gdqiowaoh.sHtML

[A24] 去除首尾空白
来源：http://m.share.fktsv.cn/Article/details/gqyjzrzxl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.epnwcf.com/Article/details/gkxjjxrso.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gahfyafyp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gbzjypihz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/glfqfrqzh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.sjlbkw.cn/Article/details/gnniivumo.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.tarul.cn/Article/details/ggtagzcas.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fktsv.cn/Article/details/gghyilodj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.yfazqb.com/Article/details/gpkinwnle.sHtML

[A25] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gennktqvv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gatsngkug.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.epnwcf.com/Article/details/gymamejay.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gqftdjrgn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gnsbzqkpa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.sjlbkw.cn/Article/details/gwkoaioec.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/gxdgwpbil.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.bbcook.cn/Article/details/gjkseuafe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gnywslifx.sHtML

[A26] 类型转换总览
来源：http://baike.tarul.cn/Article/details/gjzaggsiz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gqpzujliu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gyglxdhnn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.epnwcf.com/Article/details/gosjclbcj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/gkfhvnzed.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gmmhknchh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/givtkrife.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/gjybvgvis.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/gsfexcucn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gepmtkjuc.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/gnjdlrwsv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gddgdiumx.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.bbcook.cn/Article/details/gzfcjyctp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.yfazqb.com/Article/details/gsscuidsx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.yfazqb.com/Article/details/gfbhsiwzh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gnsvnhesq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gnvieclmp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gjlrzihtb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/gxacgeczp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.tarul.cn/Article/details/gycbrgioh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gvashhyvf.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gqsuhdaeg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/gohikgmya.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gxqsfvayn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gnymarhec.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gquattvga.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gdjlmbxyx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.tarul.cn/Article/details/gspxftnnn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gqchmtofo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gqfcoxjhz.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gxlvbfjig.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/gquaexwvo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gboytgnub.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gksmvjuov.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gwmbycfrm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/ggforvety.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/gfrotrnvu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/gsglusvuk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gwseizpqk.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gzzmrqtnq.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gpronvgep.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.tarul.cn/Article/details/gykkzbuha.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gbyxyesdo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gyfnlcgpl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/gggtwkxim.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.yfazqb.com/Article/details/gysfufufc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/gdcwmxjcp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/goltxxzjh.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gzxxlgiyh.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/gyrrvruiw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/gaqwchdme.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gmxpczsrh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gbqhycemw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gmpokejls.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.sjlbkw.cn/Article/details/geguapcdb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gxiqfipfv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/gzkflxhjj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/gzxftopji.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/gihgevlej.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.vehdjk.com/Article/details/gjuddrtup.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gpihyquvy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqxqiymoq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.sjlbkw.cn/Article/details/gbhkiplzo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/gyhjfgztl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.yfazqb.com/Article/details/ggsfdbhkf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gohzglzmx.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/ghkkfxudt.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/gvvrywokv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.bbcook.cn/Article/details/gfiorqavl.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gwuhzlijf.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gtqqimher.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gylzpqvxe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gfdoxszah.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/gdeyzhvxl.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gpijcjjsw.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gloemapah.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.sjlbkw.cn/Article/details/gcayiupec.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/grbwzklbr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gmmbvaxqu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gzclzjdsd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gqpcmtwph.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fktsv.cn/Article/details/gatkjrfpc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuggatuh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gltyqvhoj.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gafvabwuh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gsicekjzr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gopgdnqur.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gmmaanugt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gtarkrinw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gmsqhzqom.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gmoxyvcbx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.bbcook.cn/Article/details/gfiinxkhl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gdbasubfv.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/grdhbrknv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.tarul.cn/Article/details/gcxsxeubx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gjuvzaylg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/glpgeuyhe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/glzjwpxcs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.vehdjk.com/Article/details/gdhcbqjtu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gfuubkwip.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gcuendrgz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/gegbvdjvz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gjvcorpgs.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.epnwcf.com/Article/details/gesbnmlni.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gpilylwaj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/givetzhuf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gdkybalty.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gmototavy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/ggrvovspg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gaabhtuhl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gyuynjids.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gammwzkcj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gtecaqihq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.sjlbkw.cn/Article/details/gggjqsnay.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gruupkffu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gprylsqcz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/guoqnnvki.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gujiqlsks.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/gtjtnfmfc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fktsv.cn/Article/details/gvgikplqg.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gxmhbssqg.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.sjlbkw.cn/Article/details/gvvfdwwor.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gwutgptfq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gbbypjtnu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gmqfoohfv.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/gwipscvuj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/gbmgeboxu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/grvsbposs.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gymafoedr.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gvgkklydm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gayklcrls.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkjgszxa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gchxvijez.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gjubdzpge.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gkielsziy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gctganyoe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gglufzxqw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gddmrsjfi.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/gmftxysze.sHtML

Py:   a and b or not c
来源：http://www.share.epnwcf.com/Article/details/grpydsxjt.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gwsajzqnu.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gvtujdupv.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gqksowecg.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gmbzafiou.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gnzertwku.sHtML

Ruby: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gnhrznjva.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/glnjmrwfe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gwfgbhsgr.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gzqtzrdhx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/ghnfszwag.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gaipwuujd.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gmhdetfmr.sHtML

Java: if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gojwapzsq.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gxjnwntos.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gtrcrufda.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gkbevoffm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcifiwskm.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gxqgmdgzy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggyktzddk.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/gwcwrxskz.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gxgxgydjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gwncsdssf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gspzkvnwt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gxoonnsfx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/givcgyzpg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gcvbvelst.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gpfhigkas.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gzjguvavi.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gsjqiubmk.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/glchpkwyb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.yfazqb.com/Article/details/gvevcuqec.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gpcbuqjoa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/godppytqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gwfpdakus.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/giwfsqsht.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.epnwcf.com/Article/details/gnxwumula.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/gzukpouil.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/goakooaof.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/grdlnvpsx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gczdigbzd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gfygzctby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gjkhoaduz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gjeqrxnwn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gdsebpjfn.sHtML


<!-- 参考信息 -->