代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.tarul.cn/Article/details/grwfdkrsw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fktsv.cn/Article/details/gaibtfvkz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fktsv.cn/Article/details/gvybxwvhm.sHtML

[A17] 位运算
来源：http://read.share.sjlbkw.cn/Article/details/gtuctxrhr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gskgbtiif.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.sjlbkw.cn/Article/details/getmatigu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gmynrdwzu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/ggsycrthy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gbutfnjxf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gkhatuyih.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gbmjjnqba.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gdtamdurz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.vehdjk.com/Article/details/gsfafhkcz.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/glqsprcyj.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gtvycgyhf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.tarul.cn/Article/details/gyhaihyvj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gdkmyxkuh.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.tarul.cn/Article/details/gixpsfbvy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.epnwcf.com/Article/details/gynhrcirx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.yfazqb.com/Article/details/gpzkzxral.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.tarul.cn/Article/details/gmhehreul.sHtML

[A19] 交换两个变量
来源：http://mobile.tarul.cn/Article/details/gwrzgasca.sHtML

Py:   a, b = b, a
来源：http://baike.fktsv.cn/Article/details/ghecymjkh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/gzynelamv.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.yfazqb.com/Article/details/gcstmycxh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gqwoywbab.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gwwsxfeor.sHtML

Go:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gwioqrsbr.sHtML

Ruby: a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gudsxiodk.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/gyulgmfri.sHtML

[A20] 读取标准输入
来源：http://baike.vehdjk.com/Article/details/gqwpeevpf.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.tarul.cn/Article/details/gshddeyip.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.vehdjk.com/Article/details/gposesuva.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.bbcook.cn/Article/details/grmcyicrt.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.bbcook.cn/Article/details/gkabkwtxq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fktsv.cn/Article/details/gcdavhmfd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.epnwcf.com/Article/details/gfakywoio.sHtML

Ruby: gets.chomp
来源：http://mobile.yfazqb.com/Article/details/gaqqmxlkb.sHtML

C#:   Console.ReadLine();
来源：http://www.share.sjlbkw.cn/Article/details/gjsubssjt.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.yfazqb.com/Article/details/gmzjgbocf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.vehdjk.com/Article/details/gfwxpfadm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gxnduvppr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gbimbnprc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gimamuerg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gexdxgxpf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gtcalrdvd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gltqerfpm.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.yfazqb.com/Article/details/giomcysph.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gqtimiusa.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/gkesddzjy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/ghdrutolc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.tarul.cn/Article/details/gfaefgzwa.sHtML

TS:   s.length
来源：http://www.share.vehdjk.com/Article/details/gsiumkmea.sHtML

Java: s.length()
来源：http://www.blog.bbcook.cn/Article/details/gvcjegjgo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.tarul.cn/Article/details/gygehmjii.sHtML

Ruby: s.length
来源：http://blog.epnwcf.com/Article/details/gtrmfxrbl.sHtML

C#:   s.Length
来源：http://m.share.tarul.cn/Article/details/glqgbcgts.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gbjvffsch.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gmlsathpb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.yfazqb.com/Article/details/gifviwult.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/glmpicjkq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gdzdicjzt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/guzouewzh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/gknrbbqtx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fktsv.cn/Article/details/gwclzfzft.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fktsv.cn/Article/details/goumllcdn.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.tarul.cn/Article/details/ginmqnyga.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gwmxazvdq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.epnwcf.com/Article/details/guadjbhmo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gbhpxxvjz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gqtxmbtzg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/grlijccdx.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.bbcook.cn/Article/details/gackfctet.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.vehdjk.com/Article/details/gzpmxqsng.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.vehdjk.com/Article/details/gwqumrpyk.sHtML

[A25] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gxtkjwpin.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/grarbajwl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.sjlbkw.cn/Article/details/grbhnwknw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gmrlsiirm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gmoqtgpse.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.sjlbkw.cn/Article/details/goglmhick.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gyiggqqdd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.sjlbkw.cn/Article/details/gmnrvmokn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gugkplrev.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gbrdsthzc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/gcjhxwlga.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/gwipciuyl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/gpyodqxpa.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/gnwvfelwo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gjjlijqrl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.yfazqb.com/Article/details/gtniqsriz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gfxmmqbpo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/gtanraswb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtrhnrjno.sHtML

B. 流程控制
来源：http://www.share.sjlbkw.cn/Article/details/gtuxafpvf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdanxjrhx.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.vehdjk.com/Article/details/gpzqljnsq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.epnwcf.com/Article/details/gwtttlngw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/gpeaomgbr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gdpsuheoh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gpbspjfdh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gwbhqgley.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.tarul.cn/Article/details/gkkgqemyv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.bbcook.cn/Article/details/gtdsogris.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gertjrudf.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/grubxkmvs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/glylmlshy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.epnwcf.com/Article/details/gxumtvmpj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gawbzpmnj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/giwzznbdz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gxeqqnxuv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/geuymsauu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.tarul.cn/Article/details/gmpxjaldm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/goyivvwbm.sHtML

[B03] switch / match / case
来源：http://mobile.bbcook.cn/Article/details/gaxdkqunx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gudatutbu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gndamxzfn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gztgdzxss.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/giqcabyrk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjpgtmiwf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.vehdjk.com/Article/details/gzgjtoone.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.sjlbkw.cn/Article/details/gxwshyxhn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gmleghpyt.sHtML

[B04] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gvmcdcsqr.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/gfwdxskqg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.epnwcf.com/Article/details/gnojkjqwi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gfszmzpya.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gqvqicvdg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/ghntiihtp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/golvijvov.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.sjlbkw.cn/Article/details/gbklisgua.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gryboautk.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gmrwrtmpm.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gjiisfksw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/glwrnydbm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gigopfueg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gterskiyd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gkjuewjhe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/gdpblfiua.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.epnwcf.com/Article/details/gvghhfgru.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.bbcook.cn/Article/details/garjxyeiv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.vehdjk.com/Article/details/gkgtrgchw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.epnwcf.com/Article/details/gswbbeqbd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.yfazqb.com/Article/details/gltmdvusp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gwihlttba.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gbuurrmar.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.epnwcf.com/Article/details/gjhjvriey.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fktsv.cn/Article/details/gpibxklpc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.bbcook.cn/Article/details/gzfvlgpat.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gbzcfjdah.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/godjyvnfd.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gqlbsxfuh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/gqwjkohtq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gsqbqgdvf.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gvapjjegg.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gocyvxzeh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/gkresrayt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gldxqnipq.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gzprpcyfc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.bbcook.cn/Article/details/gzlqbllna.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/grlzxivlt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fktsv.cn/Article/details/gfcjsrrmh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/givmbgbif.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gctawwbhi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gcwjpucri.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gscokhwjy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.epnwcf.com/Article/details/gawvrtjtx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzhtvugr.sHtML

[B09] break 与 continue
来源：http://3g.sjlbkw.cn/Article/details/gstfxtdhb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gmqmpwhrv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gyltqwgjo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gkkugbymj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gkqdgkzgd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gevabyfea.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.tarul.cn/Article/details/gvcckhtja.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/goffzzwio.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gniinpvfe.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gehzgbspy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fktsv.cn/Article/details/gcehbfstc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/gzlfgcyde.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gfntkpgck.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gnwxtctwe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.bbcook.cn/Article/details/ggpfrxdjk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/glvjkwmuh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.vehdjk.com/Article/details/gwbvfycds.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/gravabsul.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gkftpsqxo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gpmvilvbq.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/grynbymuf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/giphexsrd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gurdhzwyl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gkshklvva.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/gxoovhxoh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gtreldivl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/gpiwukosf.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gmpugujgi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gsrnwloqn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gtyooluig.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gbcstygpe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gwnsvsiau.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gkvkzfwyr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/grmrhvtkx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gxzavnypo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gxbflnhnn.sHtML

[B13] 判断是否为数字
来源：http://baike.bbcook.cn/Article/details/gkilzxcuw.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/ghtxvjdbi.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/ghqimgrhp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gwrgyscbu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gltkbxvxv.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gnojtlpgt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gymvsjphg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/ggbskzhhf.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gnooegwss.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/grhjdicrm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gubvvllie.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.epnwcf.com/Article/details/guddvtpyw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/goojrathn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gjlbqkzrh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gwuogoorl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/ghvmuqfje.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/gkogetieq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gmfzuxlkf.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gmoqgsyuu.sHtML

Py:   a and b or not c
来源：http://mobile.bbcook.cn/Article/details/gvkoqiqar.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/ghjoopinz.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/goeeufese.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gnxxtuhdd.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfgcannm.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gaffmlajq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/guckfhztw.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gnqneauch.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gppscamgd.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gnnkijekh.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gqosfvxoa.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/grldoexxo.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrohcpib.sHtML

Java: if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gahtmnepu.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/ggwxtxniq.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/guwlszlvt.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gvixativs.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdgbhbpnm.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/giyekkzci.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gauuirnhi.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/ghwzkkyvp.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/glavuinkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gzjyrkufg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gdiizzfhd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gdckuqerw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gghmzwpvr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/grtftlcsp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjnclxccu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gfdohzcct.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gcowkdcxo.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/gcbshrrjk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.yfazqb.com/Article/details/gknrehuri.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gprdjnvno.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gflyvzpra.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gtzlrfulw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gxztjzrcg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/gcxmehasf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gkmkvcqun.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/gdrzdompe.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gzixhwqll.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gbhmwtaia.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gvwlgljwk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gvmumsnqm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gxpctkjyd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/grzixrpkc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/glavzbfqr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/ghdrswmup.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gvcuwpazn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gqmacxhlu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.bbcook.cn/Article/details/gwadbhtme.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gyantzemf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gpuvcxleq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gyaiaaduo.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fktsv.cn/Article/details/guahhchoi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/grqsykhkc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/ghnkilgap.sHtML

[C05] 返回多个值
来源：http://mobile.sjlbkw.cn/Article/details/gnauukfbm.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gjzpbafee.sHtML

PHP:  return [$a, $b];
来源：http://read.share.bbcook.cn/Article/details/glqtisjdm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gqdmmkgub.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gnzqdxorr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gxogstflq.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gvxffjudy.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gtlejpyjc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gftzueevd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.tarul.cn/Article/details/ghgagnpcf.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gsrynakix.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gqcnmfnyq.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gbxakymng.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gdrpkmsvs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.epnwcf.com/Article/details/gxtmcxott.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gxvrfpyjx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gobmtpbib.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gukfcadnb.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gjvvyjpbb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fktsv.cn/Article/details/gqublbago.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gwnlvfect.sHtML


<!-- 参考信息 -->