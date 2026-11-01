代发 wailian999

Py:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/glauhhwxo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gwftjrwwx.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gsqtyhkeg.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gzgqjilat.sHtML

Java: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/ghqaagoue.sHtML

Go:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/ggztehtwt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gksdtjwgo.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/ghbdabdna.sHtML

[A14] 注释写法
来源：http://read.share.fktsv.cn/Article/details/gdsosiagb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.bbcook.cn/Article/details/gcggflaoq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gdvlzpbbu.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gjhjnpluh.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gqxykcrry.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.tarul.cn/Article/details/gxceubhkv.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/ghqoucarf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.yfazqb.com/Article/details/gmmmjpjob.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gcokxjjal.sHtML

[A15] 空值判断与默认值
来源：http://blog.sjlbkw.cn/Article/details/gktrvqlts.sHtML

Py:   value = data or "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/gzpmdpnln.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/ghfjhqmsh.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gupmfmbto.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gcjqgiwlp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.tarul.cn/Article/details/gfsmzwlbu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.epnwcf.com/Article/details/gsqjacdhl.sHtML

Ruby: value = data || "默认值"
来源：http://3g.epnwcf.com/Article/details/gmfujrryh.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gbfepclat.sHtML

[A16] 真假值判断规则
来源：http://mobile.yfazqb.com/Article/details/gzeuigutg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/grpxkdmlb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.yfazqb.com/Article/details/gkzuujkyp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.bbcook.cn/Article/details/ggkyryzfk.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/gcliybfmf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.tarul.cn/Article/details/gjkfkbcer.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.yfazqb.com/Article/details/gtwiydwxd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.yfazqb.com/Article/details/gwzhroryv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbbvfyclc.sHtML

[A17] 位运算
来源：http://3g.fktsv.cn/Article/details/gkobquvwo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gnmjvfauq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/gbbblhmki.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/ganugaetz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gurnjzxgf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gidrxhivk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gvdooyqhs.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gpglbkbkp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gmbgjwubv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fktsv.cn/Article/details/gppvdvajb.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gxfomkswx.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gfbvcmycw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/gzavnrmsy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.sjlbkw.cn/Article/details/gbkhibovi.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.epnwcf.com/Article/details/gyubgjmbf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.epnwcf.com/Article/details/gmyuerzhj.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.yfazqb.com/Article/details/gignaxmmm.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.epnwcf.com/Article/details/gjwykctoo.sHtML

[A19] 交换两个变量
来源：http://www.share.sjlbkw.cn/Article/details/gmzhlpfpn.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/ghlazolub.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.vehdjk.com/Article/details/gflccwbmj.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gsexauaav.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gtcgrmzen.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.vehdjk.com/Article/details/gtaoylarl.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gzcvjimtd.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gsinlxlyf.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.epnwcf.com/Article/details/grhjksipo.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fktsv.cn/Article/details/glkzixxam.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/grttoftmj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.bbcook.cn/Article/details/gpauuvrvt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.vehdjk.com/Article/details/giklynsnk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.tarul.cn/Article/details/goosyhhxh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.bbcook.cn/Article/details/gpjpyixym.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.bbcook.cn/Article/details/gamctbhjy.sHtML

Ruby: gets.chomp
来源：http://blog.fktsv.cn/Article/details/gwhsglsvv.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.epnwcf.com/Article/details/ghnfpkill.sHtML

[A21] 保留指定小数位输出
来源：http://blog.bbcook.cn/Article/details/gpbhsbfwq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.bbcook.cn/Article/details/geyflsndv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gknsfqrnp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gztqyvckr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gtjgwloaz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/ghgqcyuay.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/geyjcfzvu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/ggmdghojj.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gjnldxxrk.sHtML

[A22] 获取字符串长度
来源：http://wap.yfazqb.com/Article/details/gezfosaqf.sHtML

Py:   len(s)
来源：http://read.share.tarul.cn/Article/details/gabafemsb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fktsv.cn/Article/details/gisskbjhd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.sjlbkw.cn/Article/details/gemtsexhy.sHtML

TS:   s.length
来源：http://mobile.tarul.cn/Article/details/gpxzjcavx.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/gcbwaaqvr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.tarul.cn/Article/details/gnriiljxb.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/ggvvpsdyx.sHtML

C#:   s.Length
来源：http://m.share.yfazqb.com/Article/details/gbdivahil.sHtML

[A23] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gbhogjtgp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gawfobgba.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.yfazqb.com/Article/details/gclhkrbya.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gztyadchu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/ggnsanshc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gsiyqmuxk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzesasreu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gpcsgihsk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.vehdjk.com/Article/details/gvbwlhfiy.sHtML

[A24] 去除首尾空白
来源：http://mobile.vehdjk.com/Article/details/gcgoyomgg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.bbcook.cn/Article/details/guaidcclr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.tarul.cn/Article/details/gomlvveyf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gmftgwitq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gzoydjedh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.yfazqb.com/Article/details/gwvugxmab.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.yfazqb.com/Article/details/gnlqvghbv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gpnyjrcqy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.tarul.cn/Article/details/gczazfpiq.sHtML

[A25] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gzoiuesmd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fktsv.cn/Article/details/gavcsjije.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/gtkcgvggx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/ggejjrytt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gomfasmta.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fktsv.cn/Article/details/gpzoqeppz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gdgwqrccv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.vehdjk.com/Article/details/goyofbsld.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gcbhvwqpo.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gtciwgewl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.bbcook.cn/Article/details/gvmrejjnq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.vehdjk.com/Article/details/gqguvkvuk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/gqlxplsan.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.vehdjk.com/Article/details/ghptwafkc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/giyvrqdij.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/grisfdwnm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.vehdjk.com/Article/details/gggamcrbt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gotfwrpkt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyuhmyibl.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gmnvkosvj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzdwfhdjb.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/ggjzyfntn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gpfimbbde.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gdyzuyepl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gchrdzlrx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gldpbzwbc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbapmjqx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/gurkiurub.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.sjlbkw.cn/Article/details/gmpjweoft.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gyjjkulrk.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/gxrefpatu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.bbcook.cn/Article/details/gjgwovgvr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpavaonc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gnewunoci.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gjuicwiwr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gqzmhmyiv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.vehdjk.com/Article/details/gubezxcqa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gtsnpttzw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/ghmybqfmk.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/gztszfylx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/graynpdov.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gthywezyv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gcvvxehqk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/golsnthdu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gnenywkon.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gmgzyxvby.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/goceoztim.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/gzoxxhlpu.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gzroncxxi.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/ggpboguhi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcchbnflu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gpiitdmie.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gvabjbvpy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.bbcook.cn/Article/details/gkcgqowlr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.yfazqb.com/Article/details/gowvcbxmk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/gfmdtcimy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/gcyvsxztb.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gjwyajcza.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gzipnhvdd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.vehdjk.com/Article/details/gchxprqnb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gcqlzwicu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gzvopppnf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gcxjdscio.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/gvhgesnpt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/ghajwiuae.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gigezgghi.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/gjltczamu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/govhncrgw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/ghxxusgbg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gqocowspz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gswidjjfk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.tarul.cn/Article/details/gisamckjg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.tarul.cn/Article/details/ghvlxjfxl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/gbiiocuov.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gdbbkornb.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/ggmzaohzn.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.sjlbkw.cn/Article/details/geakybsbq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fktsv.cn/Article/details/gqzcryojq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gixzfwfji.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gcklrbmpq.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/glbhtpzqd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/gktysrwxs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fktsv.cn/Article/details/gnuvgvtcj.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gpxassjyx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gbmpseabt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/guuymrory.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/gjmwylsep.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gasqdkkil.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gyqnbebpg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gzldfkhvp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gokvjyavd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/gsfmuwyvg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gzdbomyjc.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gudhsmdmu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/graufnnjy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/guckgcfey.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gxiqadzrz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gxmjxtfja.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gjfajkcxb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.tarul.cn/Article/details/gncyxpgbj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gtdacrqfx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/ghspbidus.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gbccmtbtm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gqziyclar.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/gylrbgwpl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/ggjcndpya.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gtgqpgurp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gfhtlwers.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gcnoyjhxk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gecnwndyd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/glaphdjpu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/gtsohzoda.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gmiqcidka.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gimpcolxv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gltdkjqju.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/guvdvzvga.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gtfpbqugl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/gvdtiyjfp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzriqpjn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gfvdbusdr.sHtML

[B12] 跳出多层循环
来源：http://www.share.tarul.cn/Article/details/gvrshsyur.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/ghjdgnxdm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gjwmeabdn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gaounayrw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/glfixqamk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gumnjgeem.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/grizvepaw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gzjzkegfo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/gbxxtwrvv.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/gpzalbvxz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gmjwvwhua.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/guspgcuch.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gdfrdvwig.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gpuekfaan.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/gbhposbpb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/gmxddyfuq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/gxgyvhcgi.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gasqrcgrd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gikrdctdo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gmagftlvi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gdjwocqpz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/grvpxeufb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gnvbzztay.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gnsscuadg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gopavohao.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmhuevfr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gppbzrzso.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gszyjnqpk.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/gxzsemujd.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gzterqlyw.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gszesrnvo.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gmgwffetp.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gzxozkiun.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gzqreqcvc.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gusmauwdf.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gzhutlpjz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gqvcwwxvq.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gfdnwplja.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gkgvkddhs.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gyapcyets.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gnxfqfgyj.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gvxdfxdtf.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/giejufrgf.sHtML

Ruby: return if data.nil?
来源：http://3g.bbcook.cn/Article/details/gcklvfdde.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gshsoohnl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gznaybbqk.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gxrjjqaxd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsgklirfs.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gnxujfwbs.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gmhhmxiqd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/grhhveddz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gmaohbjew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gukgudgdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gwicpjnaf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gppbctlux.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/ggzpiibdw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gvujmghvu.sHtML

[C02] 默认参数
来源：http://www.blog.tarul.cn/Article/details/gpsfgskpt.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fktsv.cn/Article/details/gnlcwgaqy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gfjytuxrc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gutorpdxz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gofayrhcv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/ggjuvaeki.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gypofocke.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gpnplmvhx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/ghmcaskiv.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gdupxqxel.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/gvpzhzvlr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/geydapcvz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gdflmsfqe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/geylhwzef.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gkegeunwd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gylncswtp.sHtML


<!-- 参考信息 -->