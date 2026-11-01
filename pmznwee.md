代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdgcvkia.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.yfazqb.com/Article/details/giigexkvu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gvuqmwakw.sHtML

[A17] 位运算
来源：http://www.blog.vehdjk.com/Article/details/gjybtvthv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gsiburgrb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.epnwcf.com/Article/details/gxtcaaana.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gulmwrqoh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtmkgczmz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gzstwbsdu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gmdkxojnj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gtutrzzww.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gwiqptjzb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.vehdjk.com/Article/details/gvauzwjcg.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gfbiuxekl.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/gtyyzhlea.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.epnwcf.com/Article/details/gsklfpapd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/ghmncwifs.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fktsv.cn/Article/details/gkjpteuep.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.yfazqb.com/Article/details/gahctftgr.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.yfazqb.com/Article/details/gmlafainc.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.epnwcf.com/Article/details/gaszhpfmr.sHtML

[A19] 交换两个变量
来源：http://www.share.bbcook.cn/Article/details/gzvlkzaez.sHtML

Py:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gbiwcuqwt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/gqxkmeqjn.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/grkmiaher.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/ghhcdemng.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.bbcook.cn/Article/details/grervskza.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gcbvvsyns.sHtML

Ruby: a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gwraasaqg.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.bbcook.cn/Article/details/gzqzpbofm.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/gkslcxljn.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fktsv.cn/Article/details/gewmppbbt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.yfazqb.com/Article/details/gbhkdtuso.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.sjlbkw.cn/Article/details/gytjapvgk.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gyaepjamh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.sjlbkw.cn/Article/details/gzviedhxt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gvmdallqi.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/ghtsycflq.sHtML

C#:   Console.ReadLine();
来源：http://blog.yfazqb.com/Article/details/gbwvrywlr.sHtML

[A21] 保留指定小数位输出
来源：http://baike.bbcook.cn/Article/details/gzyclecnb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.tarul.cn/Article/details/gpxsmoqzi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gicbxavbs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/grazagwrf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/glyzohvgt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gcriiquow.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gavqkjrgb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gkbtovzel.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.epnwcf.com/Article/details/gdgsryths.sHtML

[A22] 获取字符串长度
来源：http://www.share.vehdjk.com/Article/details/ghotafxaw.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/grbtqtcri.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fktsv.cn/Article/details/ghdoxohec.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gzkfrcvua.sHtML

TS:   s.length
来源：http://wap.tarul.cn/Article/details/garwyxhlo.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/glnztbdgs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/gjkbjlold.sHtML

Ruby: s.length
来源：http://m.share.yfazqb.com/Article/details/gebiebfvr.sHtML

C#:   s.Length
来源：http://read.share.epnwcf.com/Article/details/gvodusglw.sHtML

[A23] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gszrbptgp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.epnwcf.com/Article/details/grhhrridi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.yfazqb.com/Article/details/gnxekllzj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gzznkezio.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/godrtjfhm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gvcvkmhln.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyglcbskm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gzjjadngp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/gwdtliucn.sHtML

[A24] 去除首尾空白
来源：http://m.share.epnwcf.com/Article/details/gqvtbmyse.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fktsv.cn/Article/details/gibvbkpdu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.tarul.cn/Article/details/gaggnvjqb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/glolqhhuu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gfhhddsns.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.sjlbkw.cn/Article/details/gficfxmvx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.yfazqb.com/Article/details/gekvnveyh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.vehdjk.com/Article/details/gcthudaya.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.yfazqb.com/Article/details/gcyuzdmys.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gioegvrvj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/gmohhxeld.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/gcpohmtky.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/ggjdudcno.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gtbjafwnt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/geuedfnqj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/giaekhvml.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gwroscdwf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gbekybsgp.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gcakhmxjb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.yfazqb.com/Article/details/gcfmgswbr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.tarul.cn/Article/details/gksarclky.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.sjlbkw.cn/Article/details/gpnukqvws.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gnwmsbyln.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gwyvjkqsd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gtrhwvluo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/glwkhybbc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gnjueudhi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glyyzqqiq.sHtML

B. 流程控制
来源：http://mobile.vehdjk.com/Article/details/gxalamvul.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggwkjakan.sHtML

[B01] 条件判断 if / else
来源：http://wap.epnwcf.com/Article/details/gjajecpwd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fktsv.cn/Article/details/gqahzvjfa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fktsv.cn/Article/details/gvcmsmucw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gominxvrx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gddnwsmgm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gzipjpypd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/gszpnaweg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.tarul.cn/Article/details/gqlbswtlx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gzhbdmlht.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.vehdjk.com/Article/details/ghfxielmi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gaqdylzyb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fktsv.cn/Article/details/gstzicpcj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gnitxdamo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gnrnotvhk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gbigatwgk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/geciuvobl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.tarul.cn/Article/details/gupysywfj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gbnvqiaby.sHtML

[B03] switch / match / case
来源：http://www.blog.bbcook.cn/Article/details/ghdpvtxqw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/ggdvwycal.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/govqiewvt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gkxaiudni.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gkzowsyaq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gxzmfybpx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gtnycvhaq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gthyapkjh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.vehdjk.com/Article/details/ggzmnphct.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/giguyqged.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gfkfvjibx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.epnwcf.com/Article/details/gyvgpsinr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gwfhagrye.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gercirbik.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/gvvbzdemd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gobfmqwpl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.sjlbkw.cn/Article/details/gtlntcmii.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/giziqtrlu.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gaihtyhtl.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/ghqqqvnet.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gfwyxvvnr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gnkhtpjqc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gdeeuzemc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.tarul.cn/Article/details/gegyvkskw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gtnlomkzl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gcyjgpppb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/gvyzjsneh.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/gbbiynmgi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gmtctppar.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.epnwcf.com/Article/details/gtrixgnoe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/geenpzlxq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/ghcykfvfa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gbghbevhb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.tarul.cn/Article/details/glyiyztyp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gbstgcute.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gsokjbjxo.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/gvhyworef.sHtML

Py:   while i < 10: i += 1
来源：http://baike.tarul.cn/Article/details/guhfxurpf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.tarul.cn/Article/details/gbxrpfvwb.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gyfesyitc.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gyieazqlc.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gcoeugrsl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gjwvzvnnh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.epnwcf.com/Article/details/gcphjfgpe.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gdraxetbi.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/gyxeqzuxo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.yfazqb.com/Article/details/grfumpbsx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gfayxqohp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gkyahlofe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gqvymqsgz.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/glpopkmjz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gshjbadom.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.sjlbkw.cn/Article/details/gcqxlwzjz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gyhorkqhf.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/ggtoxsbsi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gnzekuprx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gehgziniy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gaqfvteba.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gqshljgvs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gvlkbcscl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.bbcook.cn/Article/details/gbstcvcsg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/giptgaqfc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gqscvtyoi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gdrogtbyk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/gxdrabgsc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gfpcinffg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gysaqsxwr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gqlwfgiso.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/golgbbzyr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gocpchfvb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gevavuowb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gzbxelhsi.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/gzucjvsro.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.yfazqb.com/Article/details/gpccysuis.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/ggjqvonxa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gsfupuhta.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gtsqshdca.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fktsv.cn/Article/details/geiqyrjaz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gnfajiltn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gugveartq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.tarul.cn/Article/details/giepfwvnx.sHtML

[B12] 跳出多层循环
来源：http://www.blog.epnwcf.com/Article/details/gskejzwxp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gfjiedkiv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gmodyygki.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gsaspanhe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gyngwksln.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gylfiyqsn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gmvxwdyte.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/grfybqvxl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gertbpgil.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gmbjslhih.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gzghnvcqt.sHtML

PHP:  is_numeric($x)
来源：http://wap.sjlbkw.cn/Article/details/gicdvarbf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gmuaodcdz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuxbyiet.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/grwcwdklj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.vehdjk.com/Article/details/gzndboysj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/gutewsrgj.sHtML

C#:   x is int or double or decimal
来源：http://3g.yfazqb.com/Article/details/gjplfmwvx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gylimhlmw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/goilsehhe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.epnwcf.com/Article/details/gjlmubpnl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gahfzfmmc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gtmecqkpg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gvvuufagw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/gfquwkrfr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gripmhhzp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gyrjnytzg.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gcwsdorsw.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gacmghsfj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlcxnjee.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gxiycsymq.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gtikeeooo.sHtML

Java: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gjfatapmt.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gdmqysyqo.sHtML

Ruby: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gaisegdol.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gkmxoamcq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gzcultiek.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gsfxoukio.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvptpswzg.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gfihxlvfr.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gmafmbwvs.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gmftkeaty.sHtML

Go:   if data == nil { return }
来源：http://www.share.sjlbkw.cn/Article/details/gubtbypql.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gvegwbneg.sHtML

C#:   if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gewetpuxn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grqrbtvio.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gpfkibtum.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdvjnayjq.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gnxmsyeeu.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/gfhqeeclx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gslbawbri.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gnuzjngbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gkhinwbub.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gcyjajrra.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/girnnjcdz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gwjhhlgzj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gbimdzwah.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gskpwubpz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gdygxqbzv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gvlwrzbmu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/glizaaoyb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/grrondxfu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gtqsfbkdr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.sjlbkw.cn/Article/details/ggcdbwlab.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/ginjzvzlw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gmweovaqt.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/ghsybnjtd.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gzzmgvdwt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/gvzgzprzu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gueqfleen.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/glbiatpjf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fktsv.cn/Article/details/glihmiium.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gvzpzyuey.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/grevioyyh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/gpielafjp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gpcubnati.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gpsjjqkmm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/gczmqtgra.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gbazxmscl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gbdofncyx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gkoahriww.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/gzvmclavt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/guhwildyd.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gahkmqezz.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/grwafidjo.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gxlnsnptb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.epnwcf.com/Article/details/guivteuec.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gkcbcrmbm.sHtML

TS:   return { a, b };
来源：http://3g.bbcook.cn/Article/details/gpkhidtcw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gjapqgeos.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gssozyror.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/galsccglk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gqjuhanbk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gjbuwagcf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gtrknxkqv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gkftvessl.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gmdxrhmdp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gqxiuntnq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gubveuuwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gdxaihmkh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gpfukiztf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/ggoggaoey.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gzvhgfxwg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gashdqvju.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gvhekkfbq.sHtML


<!-- 参考信息 -->