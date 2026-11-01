代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.yfazqb.com/Article/details/gfgdzgkub.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.yfazqb.com/Article/details/grmzdgiml.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.bbcook.cn/Article/details/gekimkdfd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.bbcook.cn/Article/details/gomfywiov.sHtML

Py:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gzwkswwnk.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gfzuwbauo.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gjdiyxtbo.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gqhpwheyw.sHtML

Java: "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gypunhojj.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gityltcyk.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gjopzbktz.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gudseejug.sHtML

[A14] 注释写法
来源：http://www.blog.tarul.cn/Article/details/gofohnqml.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.sjlbkw.cn/Article/details/gtgbvzulm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gvvdpkglr.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gebadcdoe.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gurmzppgd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.epnwcf.com/Article/details/gthivryix.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gaevdihbc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.bbcook.cn/Article/details/gsbfddmud.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gfcvtptmb.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/ggjjwobzq.sHtML

Py:   value = data or "默认值"
来源：http://www.share.yfazqb.com/Article/details/gmcbmkobh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/gxsnurehv.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gmuddrsjd.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gpfcubivh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.bbcook.cn/Article/details/ghrhkkcwe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.tarul.cn/Article/details/gxzgwmntt.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fktsv.cn/Article/details/gspkjbpsm.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gbtloqiho.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkciladp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.bbcook.cn/Article/details/gewytmcva.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.epnwcf.com/Article/details/gaegagbqb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.sjlbkw.cn/Article/details/gvlewjbet.sHtML

TS:   if (!x) {}
来源：http://blog.vehdjk.com/Article/details/gfwxdbtuv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.vehdjk.com/Article/details/glyomkvtb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fktsv.cn/Article/details/glmvxfrof.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.sjlbkw.cn/Article/details/gotuxrbxt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.vehdjk.com/Article/details/gndbgpfjt.sHtML

[A17] 位运算
来源：http://read.share.yfazqb.com/Article/details/gyntqenbt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gdqthtegd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.yfazqb.com/Article/details/goytizxkm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gxyaxqidj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gxhdeuceb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gnoswwewf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gbhqimkoy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/guonnjghx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gbojlajty.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.epnwcf.com/Article/details/gpqwvbhaw.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/glrakayko.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/ghqnzfnvs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gkriqsgzf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/gzihpkymc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.epnwcf.com/Article/details/gjhsugyyc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.vehdjk.com/Article/details/gsyjbffek.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.vehdjk.com/Article/details/gahbbwxfc.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gkunekhkl.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/gyaheuaqj.sHtML

Py:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvbkcdcp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.bbcook.cn/Article/details/gfyufvlop.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/gkakyebvp.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.tarul.cn/Article/details/gsntxxagr.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.epnwcf.com/Article/details/gvnklkads.sHtML

Go:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gsxidorio.sHtML

Ruby: a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/genhjbqmf.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fktsv.cn/Article/details/gooxdrtmw.sHtML

[A20] 读取标准输入
来源：http://wap.tarul.cn/Article/details/gzbuuoopk.sHtML

Py:   name = input("请输入：")
来源：http://mobile.sjlbkw.cn/Article/details/gajzratjh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.bbcook.cn/Article/details/gjxblvyhc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.yfazqb.com/Article/details/ghilaqsqv.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.tarul.cn/Article/details/gmfungivf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gytvsjnwu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fktsv.cn/Article/details/gcplbvjtr.sHtML

Ruby: gets.chomp
来源：http://blog.epnwcf.com/Article/details/gtdnihzti.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fktsv.cn/Article/details/gftaxxbld.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.vehdjk.com/Article/details/gscuxphqp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.sjlbkw.cn/Article/details/gnvspomnk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gqizgkryd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gujzwgmda.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/ghmebvqpw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/ghshvfswt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gtskqwyfa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/glqgqmqfl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/gpfeaqlny.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/gjsjbpzkk.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gutdhhrbw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.epnwcf.com/Article/details/gyevspfik.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fktsv.cn/Article/details/ginlnirmn.sHtML

TS:   s.length
来源：http://3g.bbcook.cn/Article/details/geaidyynv.sHtML

Java: s.length()
来源：http://m.share.bbcook.cn/Article/details/gnxfufinm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.bbcook.cn/Article/details/gbqfeblkb.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gdpgbkmwb.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gywcvwntl.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gitmpghpp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gcfnjuobn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gzbgffdpb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gictwigxp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gpaldnuyo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/guyaekyql.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.sjlbkw.cn/Article/details/gpbcfqteq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gwprwyxyw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.sjlbkw.cn/Article/details/grazeohqb.sHtML

[A24] 去除首尾空白
来源：http://m.share.tarul.cn/Article/details/gdlsjccan.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.epnwcf.com/Article/details/gwqdrcadm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fktsv.cn/Article/details/gvvolnxwn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gzgauxghk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gzplcstkw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gicekbeoh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gdhfrqcby.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fktsv.cn/Article/details/ggnmdanhh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/grekjqmdz.sHtML

[A25] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gtjzcporx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.yfazqb.com/Article/details/gxugereuh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gpkfmtcrx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/grvttpkvt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gimxhmlbn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.bbcook.cn/Article/details/gcjoqknif.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gzfweeqqw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.yfazqb.com/Article/details/gxhqijwha.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gtfepvlbz.sHtML

[A26] 类型转换总览
来源：http://read.share.tarul.cn/Article/details/gozommuho.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.vehdjk.com/Article/details/gcebkxzbc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/gdciwazuf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.vehdjk.com/Article/details/ggkrgfznf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gcpefziyn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.vehdjk.com/Article/details/ghujljlvi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.vehdjk.com/Article/details/gxnwdudvt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.tarul.cn/Article/details/gntxxgeic.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gnizmgaxj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkhbxifmg.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/gbqetujsh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmpjqsbck.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/gxeisqjgz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/gqmxvcffl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.tarul.cn/Article/details/gmwohmakm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gbjfvzvso.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gwnvfduui.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gocejbgfl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.epnwcf.com/Article/details/gtjowxmcx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.tarul.cn/Article/details/gegbmqotc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gwdbrjxji.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.vehdjk.com/Article/details/gvipzpcyk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.epnwcf.com/Article/details/goczyzmur.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/gtwdbptyi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gqrjctsli.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/giljvseja.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gqvoylced.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.tarul.cn/Article/details/grepyqeaj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/gquhmsnvg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gcrjqiqoq.sHtML

[B03] switch / match / case
来源：http://mobile.vehdjk.com/Article/details/gasbljgpr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gheepikhj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gainbvaat.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gjrjldywu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gsgtkdopn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/grdeyiegz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.tarul.cn/Article/details/gomxbqvjk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gnzgjvdku.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/gwitqmmib.sHtML

[B04] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gzyuhsyvu.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gqczoicwi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.epnwcf.com/Article/details/gjiwmwxgz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gohotrtky.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/girejfzqs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fktsv.cn/Article/details/gehgcjsvr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.sjlbkw.cn/Article/details/gmgyhfylr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gsdvipnmk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.epnwcf.com/Article/details/gngevgffi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gnlqqsjrq.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gboylctwh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.bbcook.cn/Article/details/gezrkbssz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gdkzqzlvi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gwkorelcj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gbmqoipeu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/gzqcdacic.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/gdfsjonxt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.bbcook.cn/Article/details/gdwppmrco.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gwjaxypba.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gxcbbrmom.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gmysisoqr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gcqkcfxwt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gynxvflev.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gwdykqgoq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gphpanbgj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.yfazqb.com/Article/details/gwazjeofc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fktsv.cn/Article/details/ggwqvmltj.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gwwabmjjh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/ghpywlomo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gublodqia.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gfdkojuff.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gwchscqpv.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gmwpqiyea.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/gwcydbowq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/govekagnr.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gvfhhayjq.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.sjlbkw.cn/Article/details/gbxtxewnv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.bbcook.cn/Article/details/govtgtqpz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gwybxzumc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gcuhzgetb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gaiuwbwpv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/glesdlvzu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/galnmqmwy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.epnwcf.com/Article/details/gbmqgzjvj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gncuagwqi.sHtML

[B09] break 与 continue
来源：http://mobile.vehdjk.com/Article/details/grpsxyumu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gphdwhyag.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gmhpoawsj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gsaxykryu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/ggushlfcc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gxtdnqfkv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gecnqebws.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/gduuxijgk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/ghbaexcve.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gqzeorlis.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.sjlbkw.cn/Article/details/ghozumwhv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gvavtdnsz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gzsavgoqh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gqilowhmk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gdkcvxwdy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fktsv.cn/Article/details/gspmayiqp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gxrhiwcbk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/gjlttfbne.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/gkkrhlbjk.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.vehdjk.com/Article/details/grshgmlmu.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gfhrdntia.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gfohjycgx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gopjslhms.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gaogocbvl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.epnwcf.com/Article/details/gldklxenr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/gwrwpkrlc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/gburlvfor.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gbocbnudg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gmrapinsm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gtqcqwbzl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gzcuopano.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gharhawnd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/glgwcvepd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gavygndbj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gpsbbsdhp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gsqhqktvq.sHtML

[B13] 判断是否为数字
来源：http://blog.vehdjk.com/Article/details/ghqhkxhfv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fktsv.cn/Article/details/gajckwzjr.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/gauswulih.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gohhpvjif.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gpwecblpm.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gnuvqdheu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gkglvcewg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnlbizln.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/glsrhkioj.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gggrgeapz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.yfazqb.com/Article/details/gxgcyetxb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/gukejozuw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/grwcpgwcb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gloqcvbgh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gpiojpezh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/grlriopdk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gjahvufqe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/ggarpsbau.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gsplbtyvq.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/gthfoupti.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gkbfpjwzr.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gmnunzqbx.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gtomycnxo.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gogrjqzqj.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gbwjjdafn.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/glsybwjuy.sHtML

C#:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gcumuifmu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gluzsqngf.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gaskofkjy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/ghbkctufl.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gfdpxfzlp.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gkglhjwfz.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gdiftjfzu.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gpthidvvu.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gjpiohxoh.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gqdtsbkqc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjgrwzrxy.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gaapolwxg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwecubclq.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gggcwbpjx.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/gnrfsdqvf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/grtmgwkka.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gzohljgfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gzghirdqr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gmyboolzf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gjjdpffuc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/geiafrkjh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gwrxbcpmu.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gqzdatspk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gtdpxmmwi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/geksvroei.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gnggcvjdz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gmpgiczjn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gcywetgjn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gyjdchera.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gmlmaqkqz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gwwcuevkj.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/geqdkulfn.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.vehdjk.com/Article/details/gelwotoem.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/guvpskzmz.sHtML


<!-- 参考信息 -->