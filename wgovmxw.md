代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gclxzalea.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gzwjrhsbt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.yfazqb.com/Article/details/gfgofhvsb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fktsv.cn/Article/details/gupjqusue.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gkrlhooij.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gghfpugzl.sHtML

[A16] 真假值判断规则
来源：http://3g.yfazqb.com/Article/details/gwvrweyux.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gtixnqcrf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fktsv.cn/Article/details/gymqhzyma.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.yfazqb.com/Article/details/gdxtftfze.sHtML

TS:   if (!x) {}
来源：http://www.share.fktsv.cn/Article/details/gxrpkqlfe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.epnwcf.com/Article/details/giaqcopnr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/gwbsgvdpi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.epnwcf.com/Article/details/gqcswefdg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fktsv.cn/Article/details/gupkreefv.sHtML

[A17] 位运算
来源：http://baike.epnwcf.com/Article/details/gwiruoxhc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gmwtggstp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/glhtlwler.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gkfkgjkhw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gxqtskypa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gcebafzat.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gccjpfjbc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gbykskzyo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gcbycqcxu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/gmubrbbap.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.vehdjk.com/Article/details/ggmkkmnhq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.yfazqb.com/Article/details/glaznjxcq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/gkgiwrwdh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/gtkuuomyu.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.tarul.cn/Article/details/gdpxxbjhl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpombtdh.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.epnwcf.com/Article/details/gsviffilm.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.bbcook.cn/Article/details/gwqrhktql.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/grexwhqje.sHtML

Py:   a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/guxletrgr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.tarul.cn/Article/details/ghxvzubfb.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fktsv.cn/Article/details/gbyvanwcm.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gplpxbqwf.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.epnwcf.com/Article/details/gapqtpcty.sHtML

Go:   a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gkvcklite.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gqhxvcyod.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gcoscsvcy.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/ghbtuzuyc.sHtML

Py:   name = input("请输入：")
来源：http://baike.yfazqb.com/Article/details/gnwqvuxvk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.yfazqb.com/Article/details/gsfruzqey.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.yfazqb.com/Article/details/gtcjbuunr.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.sjlbkw.cn/Article/details/gwhinovqr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/gettipoak.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.tarul.cn/Article/details/gkoilekzu.sHtML

Ruby: gets.chomp
来源：http://read.share.sjlbkw.cn/Article/details/gmsdggnlx.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fktsv.cn/Article/details/gphnpzqor.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.vehdjk.com/Article/details/gbzlflwyy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.epnwcf.com/Article/details/gjmsisnsj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gkricmomd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gibmknhrd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/geifwhoei.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/grvlrtgmn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gdnuqxpmq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gurfirwab.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.yfazqb.com/Article/details/gxnjufwsp.sHtML

[A22] 获取字符串长度
来源：http://baike.bbcook.cn/Article/details/gcihcostr.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gpdaeytng.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.vehdjk.com/Article/details/gbakzbcnc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.epnwcf.com/Article/details/gwjysejwl.sHtML

TS:   s.length
来源：http://wap.tarul.cn/Article/details/ghhysptqt.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gkttiksgg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/giwddhyrh.sHtML

Ruby: s.length
来源：http://read.share.fktsv.cn/Article/details/ghugbozgi.sHtML

C#:   s.Length
来源：http://m.share.sjlbkw.cn/Article/details/glzbjqiaw.sHtML

[A23] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gitdzbkit.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gguuykvmp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gwkrkxcvo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gfzrnvqzy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gsokjimlv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gqcrpzhqh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gmuqsqdmm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gxqiqrnpr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.sjlbkw.cn/Article/details/gclhnpndy.sHtML

[A24] 去除首尾空白
来源：http://www.share.vehdjk.com/Article/details/gynwobhzr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.epnwcf.com/Article/details/gtdhlsbuj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gdeoaunry.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/godiairig.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gnmxxjrtu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gczaxpsod.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gsdolzpxv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.bbcook.cn/Article/details/gbyuiwwhk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/glezerfde.sHtML

[A25] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gsrpppmma.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.yfazqb.com/Article/details/glvwiwwmv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/goddqcbop.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gbraijljr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gkydkumhp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/gjkfgwgzk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gmocnklub.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/gyznvhlut.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gsqldioto.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/gqiiavbgs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/ghnfigytx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.bbcook.cn/Article/details/gvbytcshv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.vehdjk.com/Article/details/gxgeueudg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.epnwcf.com/Article/details/gfdolzzmn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.vehdjk.com/Article/details/glwkjeyya.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fktsv.cn/Article/details/grodqynyx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.yfazqb.com/Article/details/gzgzuuccc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gtpkjmnrw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjewhxuwf.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gvnaesgea.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/geookszov.sHtML

[B01] 条件判断 if / else
来源：http://read.share.tarul.cn/Article/details/gcyeijkgv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fktsv.cn/Article/details/gcljlvuqw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gjkapxzun.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gydlfxwuo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gxqcigpcx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/guqbczsmj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gomncigob.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.tarul.cn/Article/details/gzmnogyzb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gdygfbjmz.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/ghwzwpary.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gkdwrbnbf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.yfazqb.com/Article/details/gypsuqnes.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gvzkvvxqn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/geuykdnpk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gtjuivpgg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fktsv.cn/Article/details/gauzxvlcy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gxsieifdw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gmoejtrak.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gjcmrxiaq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gaawhzdpp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gstpqebog.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gdmwmymzz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gtuvykwhn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gsbxjfdpw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gptrnwkbh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gxtlolhwo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gzkqufplb.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gszdabuqj.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/ginovmwmx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gtzxdoukn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gfcybdlsj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/ghtmikmhu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/ggrhfdbde.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/gbooovnnj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fktsv.cn/Article/details/gtcynmbti.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.sjlbkw.cn/Article/details/gvtakcbrm.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gfvngzgbs.sHtML

Py:   for item in arr: print(item)
来源：http://wap.sjlbkw.cn/Article/details/gwddlkarv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fktsv.cn/Article/details/gfonmseds.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gbpnuelib.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/girgmshbm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.tarul.cn/Article/details/gpozsspsy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gsnnifeyc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/ghvsskrhz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.bbcook.cn/Article/details/gilmzcnbj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/gpdfznbqr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gxoibiuvq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gjciwdhdm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/ggplumthz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gjhqsspeo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gqzxgnsmu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.bbcook.cn/Article/details/gofzmtrkv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.yfazqb.com/Article/details/gzdndqjfg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.yfazqb.com/Article/details/gkzldcbrs.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/gfjnoxtpn.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gttijjelk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.yfazqb.com/Article/details/gqjewcyov.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gxzcwjqzy.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/geahcmxax.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/ghcblhzky.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.vehdjk.com/Article/details/gcjeretak.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gwdpnvrlu.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gmtfhjbej.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.epnwcf.com/Article/details/grgaycwck.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.epnwcf.com/Article/details/gxpbknxxc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/grxkmohih.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gkldailei.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gvokflnxd.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gwgutfjas.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gwkpjgluw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.vehdjk.com/Article/details/glmquuauu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gmlfshatt.sHtML

[B09] break 与 continue
来源：http://blog.bbcook.cn/Article/details/gwdqwxcpc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/gbphxyzpv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gjtkrguab.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gmeyoswei.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gtfjqyvfp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gfvdhndqw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/ggbulqayg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gebenyflp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gkjyclath.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/gwtqblxuw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gvpjbeyfl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/gizawmhgh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/gliysevpz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/grepebslc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gelhgrkbh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gwekcufwy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/giapvozgd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gmxdaxrth.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gnlnarimr.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gquevlcnl.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gatdzlnub.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gldvrmlfb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/grgylheif.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gogoxmfqr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.tarul.cn/Article/details/gztnxukif.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/gmltdpvoj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gspquopid.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/glgrmjwfs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gquyemkro.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.bbcook.cn/Article/details/gwrlafhhv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gefvssubn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gfkbfnrgh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gxxpeadgs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gafopqvwh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/glgsojtbx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gqxrhzetz.sHtML

[B13] 判断是否为数字
来源：http://m.share.sjlbkw.cn/Article/details/gksldgzyz.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/guheksmwx.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gjscdmjwo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/ghfzlkeao.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gqxegnqyj.sHtML

Java: x instanceof Number
来源：http://www.share.bbcook.cn/Article/details/gqfmtxqja.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/gykjhlvui.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/glqdyjtsj.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gksuvixuu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gcmnwmyex.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.epnwcf.com/Article/details/gwrrmlstu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gbhzlaseb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/guoxppmlt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gzzmekuge.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/guwzvdhgp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gdivuefeo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gznsjfzmk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gnwrmvxka.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gafdpnwal.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gjpxqcwff.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gqqluduto.sHtML

JS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gnxudhshu.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gbupsoviu.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gmbogemrt.sHtML

Go:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gncyvvfes.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gwfznrykm.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gflgwqulb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gehdzyyag.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/glibepxmn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gwefpyede.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gjdmyzdxw.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gyqeroexn.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gepldshvs.sHtML

Go:   if data == nil { return }
来源：http://blog.sjlbkw.cn/Article/details/ghyracvxd.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gttbquajw.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gjcbnerts.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gigzuyzwf.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gcfauqzhf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gptswziai.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gajpxrmdo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.bbcook.cn/Article/details/gzjoxassu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gohfoksca.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gjzwoowoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gdpvtbwkr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gofftrnwz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/gexsliynp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gtldflaeq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gbmmqiiww.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gssdhvgpk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gfnslwmgs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gzbvhehzs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gpbgtweyx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gckflikso.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gdinlmwfk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/grxqpqaqd.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.yfazqb.com/Article/details/gvfnfkmpg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/grpgvertr.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gcegerkxh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gvysvtknc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gwtcmggbl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gypftlcuj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gjphqemvs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.epnwcf.com/Article/details/gknxfsjyb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/glvwexgly.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gvevtvpry.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gdpxiinfw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/gkizvsesw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gsdfbfbid.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gjbmkdqjc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gpedlbaba.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gpysqottq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gxbyiqjrq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gebqtgxtf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gsfhyoesy.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gfiidwsjz.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gfrnpmamy.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gqltuulop.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gdbvcnmqr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/grlbltwbg.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gwlszkeio.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gkuqpkoxd.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/grbstadmk.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gnhuyejdr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gicybezmd.sHtML


<!-- 参考信息 -->