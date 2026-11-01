代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.yfazqb.com/Article/details/gzohjczxp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gdnnirvod.sHtML

TS:   if (!x) {}
来源：http://baike.yfazqb.com/Article/details/gkpvcqmqy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.sjlbkw.cn/Article/details/gykaxngrc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.sjlbkw.cn/Article/details/gacocaszx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.vehdjk.com/Article/details/gupomyybc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.tarul.cn/Article/details/gcvsunjpw.sHtML

[A17] 位运算
来源：http://wap.fktsv.cn/Article/details/gvgxagaec.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gebveeeaz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.yfazqb.com/Article/details/gmbasocbj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gwcxsyctz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gpupepcuf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gmniyedcl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gwngqulag.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gqazcibnv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/guzagacez.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.sjlbkw.cn/Article/details/gihflfrbo.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gtambbhng.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.vehdjk.com/Article/details/gxslwcufp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/gzrmlayco.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/gaorhxbwp.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.yfazqb.com/Article/details/gnqomvqhy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/grwuppigh.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.tarul.cn/Article/details/gxayegpwy.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fktsv.cn/Article/details/gcemvxtsy.sHtML

[A19] 交换两个变量
来源：http://blog.fktsv.cn/Article/details/gvzcfemvz.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gqezfucyq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.epnwcf.com/Article/details/gcxcnikok.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gotzeazyh.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.yfazqb.com/Article/details/gvburrgsz.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/gnkdyipnf.sHtML

Go:   a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gupxqghng.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gdwgavmid.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.vehdjk.com/Article/details/gfnizglwv.sHtML

[A20] 读取标准输入
来源：http://read.share.fktsv.cn/Article/details/gggfclzsc.sHtML

Py:   name = input("请输入：")
来源：http://baike.tarul.cn/Article/details/gqyuuymvp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.yfazqb.com/Article/details/ghkxtgdem.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.yfazqb.com/Article/details/gsyicpzyc.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.yfazqb.com/Article/details/gyslaorje.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fktsv.cn/Article/details/geekuzamm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.tarul.cn/Article/details/gfvmpgzyo.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gjpxkpekk.sHtML

C#:   Console.ReadLine();
来源：http://baike.vehdjk.com/Article/details/gyzkcejvh.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fktsv.cn/Article/details/gvxcrkqsn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.yfazqb.com/Article/details/grcmrmxah.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gwwivriwf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gxdbdgtjh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gomrcrrrj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/ggpncaljb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gfxcnqdcj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gorqjsava.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.bbcook.cn/Article/details/guhrikhql.sHtML

[A22] 获取字符串长度
来源：http://www.blog.epnwcf.com/Article/details/ggclcjlii.sHtML

Py:   len(s)
来源：http://www.m.share.yfazqb.com/Article/details/ggzonntfv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.vehdjk.com/Article/details/gkqjlgnmf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.yfazqb.com/Article/details/gwufcxljb.sHtML

TS:   s.length
来源：http://www.m.share.bbcook.cn/Article/details/genqmobow.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/gvunigkar.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gzmddajjb.sHtML

Ruby: s.length
来源：http://read.share.vehdjk.com/Article/details/gnkeeuktz.sHtML

C#:   s.Length
来源：http://wap.tarul.cn/Article/details/gazrtulee.sHtML

[A23] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gzhfirjci.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/guhahgssl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.tarul.cn/Article/details/gawggncrj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gtwgoqhsh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gyycqzgns.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/grffbivfv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.yfazqb.com/Article/details/gpibwwrng.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/gfqqnubng.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.vehdjk.com/Article/details/gholdxyvg.sHtML

[A24] 去除首尾空白
来源：http://3g.sjlbkw.cn/Article/details/gbfrhnulq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fktsv.cn/Article/details/gededspaw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.yfazqb.com/Article/details/goxzutwph.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gdhfwpetj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/gwcwwbfdt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gxqfmfqcs.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/gickkzcoj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.tarul.cn/Article/details/groyrxdck.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gffxrgbzb.sHtML

[A25] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gvddkexvv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/gpilmrpge.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.yfazqb.com/Article/details/gslwwmtkz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gboejkujm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/ggfyjstna.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.vehdjk.com/Article/details/giipaavnn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gcpuqnoym.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.tarul.cn/Article/details/gkualgazh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqappvbij.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/grfbzmsom.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gydijiyra.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.yfazqb.com/Article/details/ggeytnwsb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gkmdezxzf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/glolfamos.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gzxsekoqa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/grnuxygkc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.bbcook.cn/Article/details/gayigajsb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gecgjifhg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geykkszzg.sHtML

B. 流程控制
来源：http://m.share.yfazqb.com/Article/details/gbgbdmcqr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdtsbetaq.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gtptmckor.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fktsv.cn/Article/details/gcxloigtx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fktsv.cn/Article/details/gipponlek.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gjieiiazs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gqyxpobbm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gschejbor.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gbpcvvwmp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.vehdjk.com/Article/details/gbsunfhtp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gdimayftc.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.tarul.cn/Article/details/gchucoqop.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/gqwtnwgpx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/glnaikitv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gehmmkdeu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gdkptsklf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gfnefshfj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/gveozklre.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.epnwcf.com/Article/details/gtiwvbvmc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gzinypzni.sHtML

[B03] switch / match / case
来源：http://m.share.vehdjk.com/Article/details/gtxqmfskq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gqdgyhzxm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gftuugfir.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gvzonvium.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gbpuxgvsk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/ggtvomfif.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.yfazqb.com/Article/details/gggrmtnjw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fktsv.cn/Article/details/gmlsdvbqd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.vehdjk.com/Article/details/gtepwkhfk.sHtML

[B04] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gyigrkick.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gevowutuw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/grgcoxwij.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gzivvwngi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gkmzkcfvf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fktsv.cn/Article/details/gpxctepcf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.tarul.cn/Article/details/gikxyfyfj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gvjwcozoh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.epnwcf.com/Article/details/glefkfbmn.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/getvcqtkj.sHtML

Py:   for item in arr: print(item)
来源：http://wap.sjlbkw.cn/Article/details/gmwarypvd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.bbcook.cn/Article/details/gyfmqouws.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/guobflryw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gmwpewqqs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gqflhnpdt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gczhqezje.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/gxglwfzqi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gdobxlleo.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.vehdjk.com/Article/details/gcueuzrer.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gbnpyzpwd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/ggfybgcci.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gbklagmro.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/glofgrdhm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gtbsjhgvf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.sjlbkw.cn/Article/details/gcyzootsf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.bbcook.cn/Article/details/glbfayord.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/ginnizwig.sHtML

[B07] while 循环
来源：http://baike.epnwcf.com/Article/details/glfnzqalb.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/ghfvjfkkh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.vehdjk.com/Article/details/grljtlxed.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/geclkjtxy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gthktvork.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/ggoyaninl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gseucczsg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gggwcsnix.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gejyxjgel.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fktsv.cn/Article/details/gvsxqkzun.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.tarul.cn/Article/details/gigmgnymh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gshyzziyx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gueydvbwp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gqwdhhosk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gdouqxcog.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gubrbzjjz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gjeuxefsa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gnupwygzk.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gskvihlyf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/gsuhsfgyd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gwkxtaywj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gsoorjdue.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gxaxofrxv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gsyfsrktc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.yfazqb.com/Article/details/ggidwyclr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/ghxtmpuav.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/glvwkkmvp.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gphfyjdja.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gcznshkyq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gerwqygbj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/glflxvsfg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/goulqrobh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gaampfvfi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/gqjhqyegt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/gacwfszap.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.epnwcf.com/Article/details/ganiqqfnc.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gtjbynwrp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gqixvjtcz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gkdlshyqx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gjkjrvnha.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gndpabtxc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/goxvvwkmn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/ghbsxdcfq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gmrsgtzay.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/gfanooivd.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/gswlnulzc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gjtobdbwu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gfywudszm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gfwepzrps.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gbrsstcrn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gpplxzldr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gyrylcywf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gqidkrjvx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fktsv.cn/Article/details/gafcrdmvz.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gygptgwvg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/grumwmevb.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/gbfwtnsyh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gqudluayn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gvmnjenvx.sHtML

Java: x instanceof Number
来源：http://3g.vehdjk.com/Article/details/gebjvesyd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gynmeoixr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gcqqipncf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gvhydamsq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gmkvndput.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/grgiislev.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/grxnrqrso.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gdbdtsmzd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gyqulrmzw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gdcpmjpbd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/getfnesmp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gmeuyqkuz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gysbzlasz.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gluuunonu.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gepknynzt.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gusldaqkj.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gcmiywwtc.sHtML

TS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gnxccxlxd.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gnzvjjibo.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gmtzhroem.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gxbjxsyuv.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gprzdtaad.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gngnbixva.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gdgplhrfl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/ggixuakex.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gfcxxffps.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gienevjdk.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/ghocidejy.sHtML

Go:   if data == nil { return }
来源：http://www.share.vehdjk.com/Article/details/gogklrqsp.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/govktnqnf.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gllxovqlh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/galjhxbaa.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/giqvnozev.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdmftoxcl.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gsqskzaep.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gaqlzpjnw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/glwtgymii.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gihwqnhze.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/glambpnhf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gkohrrowf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/givmvlmhr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gmwhpuerp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfqrplcj.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gtxtcjssh.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gjsooscwe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmrfevtsx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gqfvbmaoe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqzuoqlfu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.epnwcf.com/Article/details/gupkbukie.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.sjlbkw.cn/Article/details/gfjmpyomw.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gpegdxyuu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/ggbqtrnqy.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/greucyovj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gfxoiwwqh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gxrtalcmg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gffprlrfa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ginuffzck.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.tarul.cn/Article/details/ggrnkfgwc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/ggaffksdr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.tarul.cn/Article/details/gygeqlmud.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.vehdjk.com/Article/details/gzgshzpsl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gvrzefryj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.yfazqb.com/Article/details/ghurzgvlr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gllrnzhdx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gqekasqkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gtqvzmswo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/ghnbswyjn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/ggvryaada.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/grdfweyxc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/geztqphng.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/giiyukqyr.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gjiyvvgha.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gbmzowimz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gqsfeuuoa.sHtML

TS:   return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gsluuyqrd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/gzxlcquil.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gclpyzplu.sHtML

Ruby: return a, b
来源：http://www.share.yfazqb.com/Article/details/ghzhuoehv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/grpkshufe.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gjfwxcpxg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/guwwyssub.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvaymews.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/godqhwzoj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gaalziwer.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/ghlzkglfe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/glnolgoyq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/gbebcufjm.sHtML


<!-- 参考信息 -->