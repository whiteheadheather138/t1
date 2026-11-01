代发 wailian999

[A14] 注释写法
来源：http://wap.bbcook.cn/Article/details/gxjqwybqe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.tarul.cn/Article/details/gdhlgkppr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gibkailfs.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gaixmwaxz.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gnqdqtjxi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.yfazqb.com/Article/details/godzlcmvo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/glmtgwllo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.bbcook.cn/Article/details/gcsxmebpc.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/ghyfokrpq.sHtML

[A15] 空值判断与默认值
来源：http://baike.tarul.cn/Article/details/grdtqhiky.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/gykftimlu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gfxeexjdp.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gwczngprm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/glsmnokad.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.tarul.cn/Article/details/gdgjggdyy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.epnwcf.com/Article/details/grivtxtfr.sHtML

Ruby: value = data || "默认值"
来源：http://blog.bbcook.cn/Article/details/gozmylheq.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/ghimtahoq.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fktsv.cn/Article/details/gowkfmyqp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/gcjuaaysz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/glwnffvai.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.vehdjk.com/Article/details/gquyamzoo.sHtML

TS:   if (!x) {}
来源：http://baike.vehdjk.com/Article/details/grlozwzki.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gtpeijefm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.sjlbkw.cn/Article/details/gkpoardtp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gqehzumrh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.epnwcf.com/Article/details/gclshlwcn.sHtML

[A17] 位运算
来源：http://read.share.tarul.cn/Article/details/gyizzxczy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gponskeof.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.yfazqb.com/Article/details/gxptcfloj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/girmqbutm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gewwnrpnx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/grgswiyhg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gvvjslotj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/glovvgydz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gvqcvxafr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.epnwcf.com/Article/details/grzwyknwl.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.yfazqb.com/Article/details/gvncnujcw.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/gexchcaoo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gqouessru.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gmacsipkz.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fktsv.cn/Article/details/gsybkxdzf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.yfazqb.com/Article/details/gyejicpek.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gkdwassgk.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.bbcook.cn/Article/details/gytpnetzf.sHtML

[A19] 交换两个变量
来源：http://mobile.epnwcf.com/Article/details/gkjzedxev.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gnymwlawf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.yfazqb.com/Article/details/gvzxvxqhm.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/gqlqnoygl.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fktsv.cn/Article/details/gzluldviw.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.tarul.cn/Article/details/gtjjyxuvx.sHtML

Go:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gceifnupi.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gtkfxpxlm.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.epnwcf.com/Article/details/gdxepqbtr.sHtML

[A20] 读取标准输入
来源：http://3g.yfazqb.com/Article/details/ggysrodzb.sHtML

Py:   name = input("请输入：")
来源：http://www.share.epnwcf.com/Article/details/ggirahflf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.tarul.cn/Article/details/gihhzoznf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.tarul.cn/Article/details/gepydtdno.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.tarul.cn/Article/details/gpveoqjek.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.sjlbkw.cn/Article/details/gpivgnrzp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/ggkbboesq.sHtML

Ruby: gets.chomp
来源：http://mobile.vehdjk.com/Article/details/gcwsroeml.sHtML

C#:   Console.ReadLine();
来源：http://mobile.sjlbkw.cn/Article/details/guzlzoxkw.sHtML

[A21] 保留指定小数位输出
来源：http://blog.yfazqb.com/Article/details/gwijnsskl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.yfazqb.com/Article/details/gceagijcs.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/glcbgkuqt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gadyjshwd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gdshaerjs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gcbvmyvhb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/glamvcujn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gruwvnccr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.yfazqb.com/Article/details/ggdkfzkbs.sHtML

[A22] 获取字符串长度
来源：http://www.share.vehdjk.com/Article/details/gwmfemsvz.sHtML

Py:   len(s)
来源：http://read.share.epnwcf.com/Article/details/gyatbdost.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gpozgfvzm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.yfazqb.com/Article/details/gldglpviw.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/gmvscrjde.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/gpidcfyve.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.epnwcf.com/Article/details/guvclimqs.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gfdnmigvv.sHtML

C#:   s.Length
来源：http://wap.epnwcf.com/Article/details/gmkpifsll.sHtML

[A23] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/glbrjoybk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.epnwcf.com/Article/details/gfrvbpurg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/gcvjfjlqb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gzwnfbjaf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gmsooeinz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gcuakbwdo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/griihtoye.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gjjawvlaw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.bbcook.cn/Article/details/ggqshshbs.sHtML

[A24] 去除首尾空白
来源：http://wap.sjlbkw.cn/Article/details/gxashirgp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.yfazqb.com/Article/details/ggzooinfh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.yfazqb.com/Article/details/gexfbpagf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gimtbpfmr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gotmigzbi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gdbeeuget.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.vehdjk.com/Article/details/gadzlyiri.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.sjlbkw.cn/Article/details/gkhjaelsw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.tarul.cn/Article/details/gkxcpkksx.sHtML

[A25] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gxphpjtwt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.bbcook.cn/Article/details/geahxuoju.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/ghtrhvlfy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gjnqwooqm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gxqhqrlbg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.bbcook.cn/Article/details/gdyezzqhz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gshvhbqqg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fktsv.cn/Article/details/gdtfaedbc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gijoehnil.sHtML

[A26] 类型转换总览
来源：http://3g.fktsv.cn/Article/details/gzyzzawyb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.vehdjk.com/Article/details/ghudtboeg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.yfazqb.com/Article/details/ggidwqdqf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gzlukkyrk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gzigewqvb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gyvkggplg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gosdvzfrn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.sjlbkw.cn/Article/details/glmvilzgb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/ghxzkxcuj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwpuxvhid.sHtML

B. 流程控制
来源：http://m.share.yfazqb.com/Article/details/gbfouuxwe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghgfrgzks.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/gvspgewxk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fktsv.cn/Article/details/gviczvkkr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcqupeech.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gdekxepdw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gflxqifzq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gfvwbdgdg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.tarul.cn/Article/details/gcxwikzse.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/grpyxjvhj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gslggakfn.sHtML

[B02] 多分支 else if / elif
来源：http://baike.epnwcf.com/Article/details/gxqaxqtyt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.sjlbkw.cn/Article/details/gmtuqmtjr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.bbcook.cn/Article/details/gdralbsmc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gbvdbilou.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gynexzzzj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gekzimzit.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/gmemwryxc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/gumupriyv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gvtshsozp.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/gnnbwokyj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.epnwcf.com/Article/details/gwtxhfnit.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gkvnludlo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gfdemokwh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gsvdltzvc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gzoumhmlg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.yfazqb.com/Article/details/gvqrdiqcy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gcgadxuis.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gnxtgxknf.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gpbqdbwuv.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/glszrxytg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.epnwcf.com/Article/details/gakhxpiey.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/ginsrktyd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbwlyxjm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/geivfrils.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/gbwgrwxcs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/gbivpazih.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gbiqclgei.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/ggrdyuvvn.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gbwfukzzv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/gkxesjfyt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gvnkghnwa.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/gajwtjvig.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gkthdtsdt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gemrrpyjl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/gtyxcbsib.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gagfiyuln.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gpwqlripd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.yfazqb.com/Article/details/gdkdcsrts.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/gtlsbpwvz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gwmxgbrek.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gumhfhfcq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gwmqygfka.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.bbcook.cn/Article/details/gdejprozw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/ghxlpwbth.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gxandtjlw.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/glnfddbyn.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gyywltfkt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.tarul.cn/Article/details/gmfraddbo.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gaebzgbqm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gwjkejqhq.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gndksjohe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/gslaqpcgi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.yfazqb.com/Article/details/gobgsrspm.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gwfzadrjr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/ghlhsurnt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gvjnuvdlv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gtexardpj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gbekotgjz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gutsvmqcd.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gdomyzezn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/gzkmlglnd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/gftikrhnm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/geklcgfxf.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gvdkgrrzo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fktsv.cn/Article/details/gqtiiakqx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gdkqkspfn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gmzqtyblb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gkeomvvdl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gpdrcmnsb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gdlslmzvw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/gipsokysv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gylhqkugo.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.epnwcf.com/Article/details/gysfnogzd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/ggqglzvqv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gnqkauaip.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gqugbwuas.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gpcyomche.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gdyjybpbo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gccbnkhhg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gsqurdggf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/giapzqcnt.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gsaoajslu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gvpwriefg.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gwtpedfaz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gasifejdo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gycawbtvw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.tarul.cn/Article/details/gepyvdlof.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gjfnntdlz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gntsxhrat.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gpgyykivz.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/grwpnosvz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/goteeeajf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.epnwcf.com/Article/details/guqevtqdv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gdefawbiu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/giurdxjrs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gucoqscxv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fktsv.cn/Article/details/gebmymvdt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/ggsbknsyu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/gzpqmbrru.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fktsv.cn/Article/details/gxwiawogz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.epnwcf.com/Article/details/gppnfujfz.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/gazrbgdso.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gchhuctwd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gjavslpoc.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gbhfqvonj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gliejvjpn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gynrmnpoj.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/ggyybsdyp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gwudbocff.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.epnwcf.com/Article/details/gyyefvfuq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/giwbgymvk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/ghvgstzzm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gpricqjic.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gcoqtxldb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gvxsuweww.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gaueefjfv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gbyqzxizz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gywrwmsjw.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/ghzqiklpz.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/gmjbvvafw.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gpjbibanb.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gukognzeb.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gtmkohvmz.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/godzxpfjp.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gecwfuqdu.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gjfmtpwln.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/gfealmpdh.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/gufjqacmb.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.epnwcf.com/Article/details/gbseiknmo.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gshzeudll.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gexzqjmti.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gxoaqfszn.sHtML

Go:   if data == nil { return }
来源：http://blog.epnwcf.com/Article/details/gdfpfavwo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gokfipdyg.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gvjeczfqk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfdgchxjm.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/gubwwcbyl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvbwlgto.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/geuxorhdz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.sjlbkw.cn/Article/details/ghabpnqdk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gqiazrnlm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gwyuymxgu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/geujrperl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gcewnrfka.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gccwamcxp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/gjwhzyjpg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gogcvychh.sHtML

[C02] 默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gluvhkveo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gqsbqfepq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gyswafmxx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcemmrgqa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gunnouccc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/grkngazxi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gkesodxur.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gsqvuuana.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gbzwosrdc.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gyqvignja.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/ghvdzsvsj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gdqcdirtd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gdqpcgvih.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gbjfmvkwa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gvbpejahz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gnbovxkmk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gmdzzrnpt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gvdfzbxud.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gufsrozjn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gfweowymx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gnulfpmuw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gwzmkbufm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/gukwnuyqr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.sjlbkw.cn/Article/details/gffvapplh.sHtML


<!-- 参考信息 -->