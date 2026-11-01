代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gxkmpfxml.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gbrfcmsnu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.epnwcf.com/Article/details/gwxpygdni.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfxertgz.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fktsv.cn/Article/details/ggvvbaivj.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gfyxuqule.sHtML

[A16] 真假值判断规则
来源：http://m.share.tarul.cn/Article/details/gjxjaojxf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.bbcook.cn/Article/details/ggqrgaipb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.epnwcf.com/Article/details/gmcacedav.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.bbcook.cn/Article/details/gtfzehqxw.sHtML

TS:   if (!x) {}
来源：http://baike.epnwcf.com/Article/details/ghrlsrvte.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.epnwcf.com/Article/details/gqgmhidsy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.epnwcf.com/Article/details/geqfteqwq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.vehdjk.com/Article/details/guenccnyi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gfkhebcty.sHtML

[A17] 位运算
来源：http://www.share.tarul.cn/Article/details/gicwjijhi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gyxpvewbe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/gngqypsuy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gbgcvwzoj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gkqiimstw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gyokfipuy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gfygutrhm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/guuuktvbc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gpfihfhdy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.yfazqb.com/Article/details/gwwrfyltd.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.yfazqb.com/Article/details/gdbxdklvy.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fktsv.cn/Article/details/gugqpsnwe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/giogjedoj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gxwbbrcxa.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.sjlbkw.cn/Article/details/grdjanadp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/gfagwqoxu.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.bbcook.cn/Article/details/gumisrgio.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.vehdjk.com/Article/details/guvumwgra.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gieyttnjs.sHtML

Py:   a, b = b, a
来源：http://blog.epnwcf.com/Article/details/ggjqtaglr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.bbcook.cn/Article/details/gztmljkyu.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.tarul.cn/Article/details/ggvirwzav.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.tarul.cn/Article/details/gazueodmj.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.sjlbkw.cn/Article/details/gvybhjjtt.sHtML

Go:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gifkhjuqe.sHtML

Ruby: a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gbigufloe.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.tarul.cn/Article/details/gvirlebjf.sHtML

[A20] 读取标准输入
来源：http://www.blog.bbcook.cn/Article/details/gpmheqkuc.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.tarul.cn/Article/details/gjgzhrrsz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fktsv.cn/Article/details/ggzykjteo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fktsv.cn/Article/details/gidxwzqrn.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.epnwcf.com/Article/details/gkgowcwpn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.vehdjk.com/Article/details/gxajytmmc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.epnwcf.com/Article/details/goyxszxvb.sHtML

Ruby: gets.chomp
来源：http://www.blog.yfazqb.com/Article/details/gjvdkzvqm.sHtML

C#:   Console.ReadLine();
来源：http://baike.epnwcf.com/Article/details/gidfgctvc.sHtML

[A21] 保留指定小数位输出
来源：http://3g.bbcook.cn/Article/details/gshkkegys.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.sjlbkw.cn/Article/details/gwgqsiexh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/geetmpvqj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gdehinedf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gtvgyqxcr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gpqlasmov.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/ghuxycxhx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gewpyfnoy.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gucnhzppe.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gmtpjlxoz.sHtML

Py:   len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gllsslxlp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/gspdgofti.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.tarul.cn/Article/details/gtjiycbay.sHtML

TS:   s.length
来源：http://www.share.bbcook.cn/Article/details/godqjpjld.sHtML

Java: s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gofzqwthn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.vehdjk.com/Article/details/gzyhlzbcs.sHtML

Ruby: s.length
来源：http://blog.tarul.cn/Article/details/gljnfruno.sHtML

C#:   s.Length
来源：http://m.share.yfazqb.com/Article/details/gljsazwjz.sHtML

[A23] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gbjjbvvoa.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.epnwcf.com/Article/details/gejbrbitg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.sjlbkw.cn/Article/details/glkmvjxwh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/givtqbsvd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gnzalsnjn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gujlskykn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/gcoxzyfei.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.yfazqb.com/Article/details/gdooismmo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.vehdjk.com/Article/details/gnaltislc.sHtML

[A24] 去除首尾空白
来源：http://baike.sjlbkw.cn/Article/details/gwdagsqnc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.epnwcf.com/Article/details/gjypgaezt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.epnwcf.com/Article/details/gypqqlinr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gafznwimo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gdwqhjtmr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.epnwcf.com/Article/details/ggukgzftz.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gjungbuhp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.yfazqb.com/Article/details/gqfpkjpee.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gelbilvmr.sHtML

[A25] 字符串比较
来源：http://www.share.tarul.cn/Article/details/gljrntqfx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gzkrgyxhm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fktsv.cn/Article/details/gaiddasrn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/grztjitsf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gwlodepjd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.tarul.cn/Article/details/giolmutcc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/ggaqdhwdl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/gzgzvpkzt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gwtnnkgjb.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/gfgamzkoz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gloyylboi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gkygytcfh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gdfocjtlc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gfvwiykyw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/giouwpvbv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gjvdnssix.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gahhaxjuw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/gcwloysad.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxdwlegmv.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gjohfslna.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grjqiolzm.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gbpatedds.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/givzelkhg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/gymbjqock.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gzvprenls.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gbvyiowac.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gucuqgoai.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.vehdjk.com/Article/details/gbdxmcjdi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.tarul.cn/Article/details/gnsoekqlz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gdyzvkfco.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gvhxwqfuo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.tarul.cn/Article/details/gozizunit.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/gabkjdjyt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gpwvkgmjo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gbkareaab.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gxngfmmso.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gqcrznpqs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gsyvygvrh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/ghvfsphfk.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/gvgjyogvn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/ggzcgwjsh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gwobsxnjp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gnzbyeqmd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/ghsivdxeh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gkjatxzit.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.tarul.cn/Article/details/ghzetztem.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/gmankonya.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.vehdjk.com/Article/details/ghygvxdca.sHtML

[B04] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gljmyrdyl.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/grmqhmbuy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.tarul.cn/Article/details/gzoncxrct.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gfmhyzmye.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gybwlzpww.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/guiqzfwdf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/gdgadgvux.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.vehdjk.com/Article/details/gaxfxvquv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.bbcook.cn/Article/details/gtcclqbrx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gzdartnph.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.sjlbkw.cn/Article/details/gijfbzhfs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gglddemce.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gxmunxdyr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gdnjbzhuu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gszmjjtwl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.tarul.cn/Article/details/gebrdrrou.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/gchcqbejs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/gwsbapmma.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/ggkletvrk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.bbcook.cn/Article/details/gnmwgetix.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gsfshlppk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gfhlijmln.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/grrcxervi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.tarul.cn/Article/details/grtnxdfyl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.sjlbkw.cn/Article/details/gavnbnogq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.bbcook.cn/Article/details/gzxglipdd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.yfazqb.com/Article/details/gifstrlnt.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/gaqcotaka.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/gpevlnvwf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/gzbixsdqp.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gyxesempv.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gdnbfjzci.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gfirshwai.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gemeuzfxv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.sjlbkw.cn/Article/details/gufykldxp.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/giaqtvvis.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/ggtlvjwqj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/gyvptubpt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gdsevxzwy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gdkoqdfxl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gnorqksly.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gqoxwwcso.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gjcqasvoz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gskcpmgnc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gztnkpuhg.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/ghihycqwj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/grskzrumj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gudytujsj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gfvixgqni.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gjnivkuym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/grgmsjidr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/getrabcbh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gcrwbdfnw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gcymxsdok.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gihxcaahe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.tarul.cn/Article/details/gphjjtzod.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/gjzpfajad.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gyfgzxnqh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gfuvvgpbo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gjiwoaohq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.bbcook.cn/Article/details/gcyntnkqi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/gopyngpbr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gmeanrkrk.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gxnltlzww.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fktsv.cn/Article/details/gwfdjtqdx.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/gorkdervk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gtmtjygqx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/ghhzphpcr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gokjnxgff.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gdpasdmzb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gtlvhgmil.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/gindexihf.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gosplvgcu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gvfjxxvtn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gxswsdsrl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gemocrubd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gauccifxj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/ghirwyztc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.epnwcf.com/Article/details/ggzjgtmpy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.epnwcf.com/Article/details/gyvwxexji.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/gcikmezeu.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gypcvmcef.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.bbcook.cn/Article/details/galeeusmk.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/geenjwidi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/guvshmtyi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/guesfhrzz.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gjbsucrpc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/guihrrfai.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.epnwcf.com/Article/details/glahdbwmi.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gqqbdrjbl.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gxvycvhem.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gvryajimh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gkpijiwyf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/guafcxedj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gaioxvtzs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gwwlzfosx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/ggqxurjur.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gomzwxgxj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtvlizgqi.sHtML

[B15] 布尔运算与取反
来源：http://www.share.epnwcf.com/Article/details/gupxfiijv.sHtML

Py:   a and b or not c
来源：http://www.blog.yfazqb.com/Article/details/gnvcrfwpl.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gikjlvkrc.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gkozwsiwd.sHtML

TS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gwkguvjqe.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gmatzlnen.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gkyghcddy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/glqasozhf.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gveauygbf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/goxuafjsh.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gtmvddpju.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/gnfwgrriq.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gnorkqfoq.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gbxhllgwn.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gyrxtqcbk.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gmlawplnu.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/glpzpnufu.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/givmykjgu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gplpkfzhk.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/givjdmrgm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsvlhfqhy.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gplixpveg.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gonyerlws.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gqgwlenza.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gasntillk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gdoichmzv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/goexidwcp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gtkjwfklj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.yfazqb.com/Article/details/gawptxpsb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gmvfhmrsb.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/ggemnvcbl.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gsadffvqb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/goqycvony.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gwxrwalec.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gttyhizxm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.epnwcf.com/Article/details/gidhdwxrl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.tarul.cn/Article/details/gzaqtzyrf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.tarul.cn/Article/details/gvwmuqfih.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/ggtdezeei.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gfkggzdfc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/galbywwbk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gfedaodik.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gusgcgnzd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/ggqkffjic.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gxnnyulvt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gvnqovygg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.tarul.cn/Article/details/gnnektnby.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/ggefwfbey.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gcnaxbcjv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.yfazqb.com/Article/details/gksjgyaoz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/glcpdpovt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gzvvmqqqv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/gzdpfxflx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.bbcook.cn/Article/details/gsukiwylw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/gurklzcsf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gvffwaxvv.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gdgumctmi.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gwrzvqfbd.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/glpjyhdge.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gnjcotnyf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gcpxlprac.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gbwcmccif.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.vehdjk.com/Article/details/ggdkrtkae.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gpwvtngxh.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gwjtspgbk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/guyupeohr.sHtML


<!-- 参考信息 -->