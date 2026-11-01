代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlestjwv.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gjmuuoswd.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gxgqghwde.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gkqfpjujz.sHtML

Java: "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gfduxidpl.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gtmayaxel.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/grydnbdwc.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/giqfqywyx.sHtML

[A14] 注释写法
来源：http://www.blog.sjlbkw.cn/Article/details/gcsrlmfya.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.yfazqb.com/Article/details/gyqiofkzb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gdapqnpps.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gptvoysin.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gbpncdffm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.vehdjk.com/Article/details/gejueohpx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gfefeyljj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.yfazqb.com/Article/details/gwygdfqbo.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gbolwvxgg.sHtML

[A15] 空值判断与默认值
来源：http://read.share.tarul.cn/Article/details/gkldjxfpn.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.epnwcf.com/Article/details/grgiloktl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gbkrenshf.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/getccjswv.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/goihntdlg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.vehdjk.com/Article/details/gyysuiyxp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/gttkvfpku.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/ggqyguazr.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gmvmlgxbi.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.tarul.cn/Article/details/guxepgxum.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.bbcook.cn/Article/details/goyfrzgnn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.tarul.cn/Article/details/ggspwboqh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fktsv.cn/Article/details/gwoxjjsue.sHtML

TS:   if (!x) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcinhfqlm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.yfazqb.com/Article/details/gcyqrgczg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.yfazqb.com/Article/details/gfgogmxlw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.yfazqb.com/Article/details/gcjjkyzow.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.bbcook.cn/Article/details/gbacugoiv.sHtML

[A17] 位运算
来源：http://baike.yfazqb.com/Article/details/gmymqyjga.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gxvddhojh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/gxbwoocyn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/grpbkdzmz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gokrpfdzs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gndqzljdb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/ghluzkcor.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gggrvmrvw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gcniuueul.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.vehdjk.com/Article/details/gwkufehul.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gcnehrwtc.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gcmwopgef.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gnqmtunef.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gkhdqcqdo.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.sjlbkw.cn/Article/details/gmifrllqz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.epnwcf.com/Article/details/gfrngczwy.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.yfazqb.com/Article/details/ghwwaurvy.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.vehdjk.com/Article/details/grurufedp.sHtML

[A19] 交换两个变量
来源：http://baike.yfazqb.com/Article/details/gewlydauf.sHtML

Py:   a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gjevjwlmq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.yfazqb.com/Article/details/gfndeyqiv.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/gjtzserar.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gotwykgke.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gebnuhqgn.sHtML

Go:   a, b = b, a
来源：http://blog.epnwcf.com/Article/details/glsgnphcc.sHtML

Ruby: a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gsbfkfevd.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.yfazqb.com/Article/details/gfsqctraa.sHtML

[A20] 读取标准输入
来源：http://read.share.fktsv.cn/Article/details/gkmbttwxg.sHtML

Py:   name = input("请输入：")
来源：http://www.share.bbcook.cn/Article/details/gaartabke.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.bbcook.cn/Article/details/grktmvpuz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gydnwlmtg.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.bbcook.cn/Article/details/ghdedztzc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/gdhaniylm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fktsv.cn/Article/details/gwbqqcvmk.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/gfpkxwymg.sHtML

C#:   Console.ReadLine();
来源：http://www.share.bbcook.cn/Article/details/gpnbplvef.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.epnwcf.com/Article/details/gkikocjeu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.bbcook.cn/Article/details/gxasgvhck.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gvizahiol.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/grxllfird.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gogzerrfq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gvrazmqpe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gshuhnlff.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gexvkvjsm.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.epnwcf.com/Article/details/guzfdbwwm.sHtML

[A22] 获取字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gxtdysigy.sHtML

Py:   len(s)
来源：http://read.share.bbcook.cn/Article/details/gssqsedam.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.vehdjk.com/Article/details/gvckpvksd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.epnwcf.com/Article/details/gvqajkkgw.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/gzulltjth.sHtML

Java: s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gfyqcupiv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gwjyrlvee.sHtML

Ruby: s.length
来源：http://read.share.vehdjk.com/Article/details/gxqensotf.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gfhkcaeue.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gaewucaqs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.vehdjk.com/Article/details/gtsjlaork.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.yfazqb.com/Article/details/gifxbrmfy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gpkjombnk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gyrvygjvy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gaothzxks.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.vehdjk.com/Article/details/gmvhhyqxk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/geqdtwchk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/gqwejdlsk.sHtML

[A24] 去除首尾空白
来源：http://m.share.tarul.cn/Article/details/gsdikmxna.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.sjlbkw.cn/Article/details/gttnfmfyg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.tarul.cn/Article/details/gidnsphrx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.bbcook.cn/Article/details/gxhqjaigd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/goxwvofnu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/gjnlllztx.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fktsv.cn/Article/details/ghmustijw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gsnifqige.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/gxvmrrfuy.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gumttqiwc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gfjdevehd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.yfazqb.com/Article/details/ginoppbqw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gbfdmkizl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gmqhqbfdx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gvqalxbma.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/geecxratu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.bbcook.cn/Article/details/gshuwbzom.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.vehdjk.com/Article/details/gfvisdryg.sHtML

[A26] 类型转换总览
来源：http://www.blog.tarul.cn/Article/details/grvbcjyaj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fktsv.cn/Article/details/gqooudvkg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gxiuygdbj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/gqarwdmda.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gqmfgzykr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gawxnyrsv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/getrqyidm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gbivdgokn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gvjdddkbc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbcdamipl.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gtthcynwf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyowtwvtd.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.epnwcf.com/Article/details/gwkcnmops.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/grcqnohze.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.bbcook.cn/Article/details/gqsqrmsqv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gzqrvgvcg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gerrnojlr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gwyogtvpu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/gbpaihjld.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gzhvlalya.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gkfdvbyhu.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gfuajhnsi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.epnwcf.com/Article/details/gzgfvaetq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.vehdjk.com/Article/details/gwjsibkjr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gbeuhqpzs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gexxtamcp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gwghiyqls.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.sjlbkw.cn/Article/details/ghwnicxeg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gdvpcmaqp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gdqzgwvgz.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gmjkdkzch.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.vehdjk.com/Article/details/gxgisnaot.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gsavehlcr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gwjwuhcdq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ghtckxvix.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gzsaovkuj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gffieqpgt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gdckhanrn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gwupctods.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gysodpizz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.epnwcf.com/Article/details/goexaakfa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gigpqgbjn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gcneozjhm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/getwlkagz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gloaloikb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/ghybypeob.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/geqfnngql.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.epnwcf.com/Article/details/gkaivvyyu.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gsswlfybo.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gpchemvkz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/guvxkeucz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gaqxmwrfg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjhqwftig.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.tarul.cn/Article/details/ghssulnht.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gookzzwkh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/godwtmpmo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gmwtymrsq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.bbcook.cn/Article/details/gldojtjrp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/gcnssjsbe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gefdukfnb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gnqrluarw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gkhcuykqu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/ghuifxtcl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.sjlbkw.cn/Article/details/gxubpmozg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/glqppblqa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gsroqdscw.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwnpdhvwl.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/gazudkouu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.yfazqb.com/Article/details/giqquyaha.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gytwidijo.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/guwlsdjmk.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gchldqxcs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.bbcook.cn/Article/details/gfntaqreb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gjlugiqni.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gmmypmduo.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.yfazqb.com/Article/details/ggqwltiwh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/goanjidta.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gxvedxvpe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gttkbnhox.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gywqwbwix.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gseccidqv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gkzkprslc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gcnjsyseo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gckjjntzi.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/gdwuyrgba.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.tarul.cn/Article/details/guukmpuoc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gbcmlrold.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gxnbonhks.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gewunkfwz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gqejwfozg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gpsxwnnhs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/ghshqfyqb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gypjefgic.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gdfxfbqbq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.sjlbkw.cn/Article/details/gawmbinuv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gdeffzqee.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gczncomac.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gfpvdjtof.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/gehqlwiis.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/guahdwhnp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gtxpxannl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/gboythaki.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/grrnlqvla.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gedclircn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gdfqtuktr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gpcqvwuyn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gqzainryr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/glvhgycbq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gkasgbwlg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gwaaolifl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.bbcook.cn/Article/details/ggyryuuzm.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gbezxgzer.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/galkehihe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.epnwcf.com/Article/details/gmseqyxxn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gcqjohxtm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/glukkulyd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gbmkopacq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/gliddfbkn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gztacqury.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gufcejhkv.sHtML

[B13] 判断是否为数字
来源：http://blog.epnwcf.com/Article/details/gcpflqfla.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/ghrtaivnq.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.tarul.cn/Article/details/gixblwcau.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gqyrjhkqz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gqpmpgtif.sHtML

Java: x instanceof Number
来源：http://wap.tarul.cn/Article/details/grhblgzsi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fktsv.cn/Article/details/gbyfxgopb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/ggwemnzpg.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gjmtsrexb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/ghjybutut.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/grkbmgckp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gxjkmiepk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gumzrifwc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gzzpsauej.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.vehdjk.com/Article/details/giehjqikj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.yfazqb.com/Article/details/gzpmkuulk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/gptpmwrsy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gflodfrxz.sHtML

[B15] 布尔运算与取反
来源：http://blog.yfazqb.com/Article/details/gfbibwodu.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gyvbjzqhh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/gxffjhfsa.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gssutkexj.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gkqheeegb.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gmdczrlej.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gfwysgpbq.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/gydibhekg.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gfzofvqok.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gkbldcmez.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gowpynwvs.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gorgzcrly.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gynqjugym.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gojsluhtj.sHtML

Java: if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gdyzrouev.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/gwnrvvovs.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/glabxvdzn.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/grbrzjdiw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gygmxikvs.sHtML

C. 函数与作用域
来源：http://www.m.share.vehdjk.com/Article/details/ggthtlxxw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvgxotgij.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gikozplrs.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gsjuvbjbf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gvwoagtxk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gmbxssevn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gltadasme.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/geblbupnh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gqbpqcetv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.bbcook.cn/Article/details/glncfwtab.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gswhadocf.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gypkpmfcc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.bbcook.cn/Article/details/gioctabnq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.tarul.cn/Article/details/gscjifsut.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gxpmveqdf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfnanwtol.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/golhhuqpc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.vehdjk.com/Article/details/gyogdzooz.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gnymgcozy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/girehrmde.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/ghnlmfrvy.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gdubmipml.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gzrnefwfj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gtmhdpezq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gpnrrflan.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.sjlbkw.cn/Article/details/grqzrpjej.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/gpneixjnl.sHtML


<!-- 参考信息 -->