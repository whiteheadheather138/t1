代发 wailian999

Py:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gyhaxamxz.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gcjfnkupt.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gahyawmrr.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/giyxowuqk.sHtML

Java: "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gadcargwp.sHtML

Go:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gpzxxtdnh.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gokrmwtah.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmmkvcas.sHtML

[A14] 注释写法
来源：http://mobile.sjlbkw.cn/Article/details/glyfppidh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/gnuxqbpyu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/geknbghap.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gmupprjxw.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/grehfcgjm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.yfazqb.com/Article/details/gnjojtpwa.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gxpowzfog.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.yfazqb.com/Article/details/gqqktcqpg.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gtnwlhexc.sHtML

[A15] 空值判断与默认值
来源：http://blog.sjlbkw.cn/Article/details/gttyyjeje.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/gawmwoftb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gooeipzsl.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gilsnnugg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/ghvrvbfmb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fktsv.cn/Article/details/gfvrziodv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.epnwcf.com/Article/details/gjrobijyl.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gytqmrsdv.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gnnukgqug.sHtML

[A16] 真假值判断规则
来源：http://wap.epnwcf.com/Article/details/gmytavfuk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.epnwcf.com/Article/details/gacnzxwjk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.bbcook.cn/Article/details/gixuhtsmz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.vehdjk.com/Article/details/gbkyolenj.sHtML

TS:   if (!x) {}
来源：http://wap.epnwcf.com/Article/details/gnvtyfklx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/gsoqondaf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.epnwcf.com/Article/details/gjpbaoldv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.tarul.cn/Article/details/ghzrcctlr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.yfazqb.com/Article/details/gshtusqkw.sHtML

[A17] 位运算
来源：http://www.m.share.bbcook.cn/Article/details/gldohsqlh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gdpawxnfn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/ginsqforg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/glnofayzp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gqgcfijxv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gvhhzoqek.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/givocetrj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gfnqnpekd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gogzoihby.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.yfazqb.com/Article/details/genjqktis.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gdovysrtd.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/ghbasvtjj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.vehdjk.com/Article/details/gnjhxsblm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/guqcyhebn.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.yfazqb.com/Article/details/gxrptqvyb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.tarul.cn/Article/details/glvayticr.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.tarul.cn/Article/details/gnlbehyhr.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.sjlbkw.cn/Article/details/gcjgzckcr.sHtML

[A19] 交换两个变量
来源：http://mobile.yfazqb.com/Article/details/glnfjqqhc.sHtML

Py:   a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/goumjtxfh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.bbcook.cn/Article/details/gtnejizyk.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gdheeshzx.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/ggqrqddvx.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.yfazqb.com/Article/details/glhassusm.sHtML

Go:   a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/gkotcgeft.sHtML

Ruby: a, b = b, a
来源：http://3g.tarul.cn/Article/details/gndjlwrvo.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.tarul.cn/Article/details/gdfofpezc.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/gmbobfdvj.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/ghogtnnca.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fktsv.cn/Article/details/gjxyjekcm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/gupatqbzw.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.epnwcf.com/Article/details/gsoycjxrw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.tarul.cn/Article/details/gykuqyhed.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.epnwcf.com/Article/details/gtndjsccb.sHtML

Ruby: gets.chomp
来源：http://3g.epnwcf.com/Article/details/gmwisbiqw.sHtML

C#:   Console.ReadLine();
来源：http://www.share.yfazqb.com/Article/details/gnjtvqizq.sHtML

[A21] 保留指定小数位输出
来源：http://baike.epnwcf.com/Article/details/gzqkjbtff.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.bbcook.cn/Article/details/ghrwoyqxk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gaquptemz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gmvrippyc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gdijnossv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gcadqhghc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gdakiymrp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gxnpxwsbg.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fktsv.cn/Article/details/gmeaihojh.sHtML

[A22] 获取字符串长度
来源：http://www.share.yfazqb.com/Article/details/gkjdzbhos.sHtML

Py:   len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gaoqqapox.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.epnwcf.com/Article/details/gdqzubcid.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gcfwnxavi.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gduwhbgvt.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/gnquvfdzj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/geekxrsaf.sHtML

Ruby: s.length
来源：http://baike.epnwcf.com/Article/details/grynfchrd.sHtML

C#:   s.Length
来源：http://www.share.bbcook.cn/Article/details/giumlemog.sHtML

[A23] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gtkmjnniw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fktsv.cn/Article/details/grmmjkchf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fktsv.cn/Article/details/gtwqnmyve.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gbhhoklfr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gcryjoudd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gmnrktesz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.vehdjk.com/Article/details/ghalwweia.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.yfazqb.com/Article/details/goabjrkdq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.vehdjk.com/Article/details/gzmvseuhi.sHtML

[A24] 去除首尾空白
来源：http://www.share.epnwcf.com/Article/details/gofrykblo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.tarul.cn/Article/details/giuwtogea.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.yfazqb.com/Article/details/gxxjzryzy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gadkkzcwp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/gwcjgqlca.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fktsv.cn/Article/details/gqhiloppg.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmdgsmpgk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fktsv.cn/Article/details/gatjmgkwq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gobmoseir.sHtML

[A25] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeboxvib.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gukznanrh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gagywidtd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/geljljhvw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gogawuaxi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fktsv.cn/Article/details/gopgqxaal.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/gosimydly.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.yfazqb.com/Article/details/gtxlhpesr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gjkeqnmei.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gabflxcrp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/gkuixwvtx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.bbcook.cn/Article/details/ghzocqetj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.sjlbkw.cn/Article/details/gxewbqyjf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.tarul.cn/Article/details/gidhdbbsd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gquylssds.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.yfazqb.com/Article/details/gicgjxxoe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgqzlowr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gvstphswr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gufuczhlz.sHtML

B. 流程控制
来源：http://3g.yfazqb.com/Article/details/gkqvszzxt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gppsijscq.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gkczkmwjx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.yfazqb.com/Article/details/goxukcrkb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/gopulnons.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gtrextgkl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gozevfckj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gfsrjrprb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.sjlbkw.cn/Article/details/giezpmhox.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/gqbzynjay.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gcvgpsoja.sHtML

[B02] 多分支 else if / elif
来源：http://wap.sjlbkw.cn/Article/details/gkiwidqgc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.vehdjk.com/Article/details/gedhutyyy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gchqpjstm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gmeyivpvq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gfdkcvduy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gdxrarrkp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.bbcook.cn/Article/details/gfayxnnrc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fktsv.cn/Article/details/guxpegwmo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gqmblgntf.sHtML

[B03] switch / match / case
来源：http://wap.yfazqb.com/Article/details/gftvwvzew.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.epnwcf.com/Article/details/grqtwhdgg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gdnqczknz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gzxkmqgfr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gqysyaunb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gdntpeldc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.tarul.cn/Article/details/gyqkkrjsi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.vehdjk.com/Article/details/gbjovbbzo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gdhdwvnnt.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gusvndjnc.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fktsv.cn/Article/details/gcvgduvar.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.yfazqb.com/Article/details/gllqacben.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gjwdniufc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/gfwiupldx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fktsv.cn/Article/details/gtyydzojh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.yfazqb.com/Article/details/ggyhfdpcp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.sjlbkw.cn/Article/details/gssnhxeka.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.epnwcf.com/Article/details/garpcspkr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gsyavuboh.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/gbtewqtiz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.tarul.cn/Article/details/gxsmpayij.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/greywugus.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gndfabckv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/geothkhlq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.yfazqb.com/Article/details/goqhhofyg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.epnwcf.com/Article/details/gmplvfzqi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/gaexvdatl.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gsuxqihsf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gamuufqps.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.bbcook.cn/Article/details/gfdkbzaid.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gzhkessjn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gmglxkbdi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fktsv.cn/Article/details/gpvshamqq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gjiigbriu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/gegyrjjff.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.vehdjk.com/Article/details/gxeyhxttd.sHtML

[B07] while 循环
来源：http://3g.epnwcf.com/Article/details/gnrjcmgpw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gfonaonni.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.yfazqb.com/Article/details/ghglebcua.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gkfwwddiw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gqsgxjhxd.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gjeupivwh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gxelhygix.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/gidsjleqz.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gnadlzpum.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/ggitutyoe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/guorhtivg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/gwrwbkjbh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gjbhofpww.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gictpjyvc.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gglueujet.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.vehdjk.com/Article/details/ghqfvswoz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gdzqhjooh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gdmlqfjov.sHtML

[B09] break 与 continue
来源：http://read.share.sjlbkw.cn/Article/details/gihcnicyw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/giunhncge.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gsqhtzyyp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/ggswounym.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/ghdomndmm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gmztpnmki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gvqjrxrrc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/glrroebbj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gftoauqxe.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gbilyazwa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fktsv.cn/Article/details/godrwthgv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/ggummiduz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/glftlsjam.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gsltswwcs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gitdqewkm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gdrtiuedc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fktsv.cn/Article/details/gcayjucww.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/guzvbgzni.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gefxbsvhh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/gxixdnfwv.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.yfazqb.com/Article/details/gmypiyfkh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gnfzqnwik.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gdxsnthro.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gpmftvzxm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.tarul.cn/Article/details/gyhugxyjy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.vehdjk.com/Article/details/gohtuvufk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gycffwole.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gtcpfwurh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gktlmpcrl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/gfpqhzfsh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gmjfugyvw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gwymxfwmt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gfjlniezu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/glwvwxtqm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gbvfkcadz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/ggnazrcaw.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/gaphgleyo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/giesdtkca.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gqordcpfp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gushmrbtl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gdtjbthwy.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/ggciidlfl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gsuwegtfo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gujicshmd.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gowbbalky.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.epnwcf.com/Article/details/guvanvuiz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.epnwcf.com/Article/details/gmeqmukvd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/giovujooe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gbwkarfht.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gkwgkjkou.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/ggrufduwt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gdstkrdos.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gvffmyhej.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gifotzivf.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gvtpwvaok.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gveakpcbx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.tarul.cn/Article/details/gdwrbbdyn.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gnovbbgeg.sHtML

TS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gvriurmbm.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gwclqamvf.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gpzrgvfgy.sHtML

Ruby: a && b || !c
来源：http://wap.tarul.cn/Article/details/gbhqimqij.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gpriifceo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gcsmmvgca.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/giqxevasf.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/glrfvryrk.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gbekkgcnq.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gkbqbqiwx.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gmyfjqujf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/gffabzyfu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/goxsfxjna.sHtML

C#:   if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gavzesvzr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gifumfdxi.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/glwacojbt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/giuavewyc.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gowamdpzk.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gsctgmzxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gnkmreuhq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gzbxqopoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gwoiidbsg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gatckfeck.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/ghmargszm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gixtlgndq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gtybfuktu.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gjxiykwnw.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/ggzpdvycl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/geeyqdopu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gdvfdtazu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gfgivbjhe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gbbynxjky.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.vehdjk.com/Article/details/gdzezjiji.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gyfsgyezu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gdenolxir.sHtML

[C03] 可变参数
来源：http://blog.bbcook.cn/Article/details/gloldnvrh.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/gcazkjviz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gxbtgrbkj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/ghsvlkxeo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gcxblfaiu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/gkvdkrjnc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gtdkiglds.sHtML


<!-- 参考信息 -->