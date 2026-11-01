代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/givmxffpu.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.yfazqb.com/Article/details/gyvbifvij.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.epnwcf.com/Article/details/ghspbnwgc.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.bbcook.cn/Article/details/gbxiapjpn.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.yfazqb.com/Article/details/gpswbueoy.sHtML

[A19] 交换两个变量
来源：http://www.m.share.bbcook.cn/Article/details/gjtscbzim.sHtML

Py:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gnczwoirs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/gmhhhsswg.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.yfazqb.com/Article/details/ghlzwczzf.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/ggxnyhigz.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.yfazqb.com/Article/details/gmwagpxuh.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gtspgfxzo.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gzketzptc.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.epnwcf.com/Article/details/gpjoobkoi.sHtML

[A20] 读取标准输入
来源：http://wap.epnwcf.com/Article/details/gtljldxql.sHtML

Py:   name = input("请输入：")
来源：http://blog.tarul.cn/Article/details/gulkecopm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/gcrsbvfkh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.epnwcf.com/Article/details/guckgnypy.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.epnwcf.com/Article/details/gseqaztze.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.bbcook.cn/Article/details/guhgevjlz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fktsv.cn/Article/details/gpbwltmlx.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/ghesiwuwn.sHtML

C#:   Console.ReadLine();
来源：http://blog.tarul.cn/Article/details/gectshnit.sHtML

[A21] 保留指定小数位输出
来源：http://blog.bbcook.cn/Article/details/grxysuuaj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/gvuqoxqcd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gpbwxrbda.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/grzvwfhpe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gfxprcrhm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gdctrzgit.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/ghcchtjke.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gvlqaibwk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.vehdjk.com/Article/details/gpqvwpwlv.sHtML

[A22] 获取字符串长度
来源：http://www.share.epnwcf.com/Article/details/gmkdaualj.sHtML

Py:   len(s)
来源：http://read.share.yfazqb.com/Article/details/gupjxwftt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.epnwcf.com/Article/details/gkrptvfpv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.sjlbkw.cn/Article/details/gesgwyfou.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/garcbbykg.sHtML

Java: s.length()
来源：http://read.share.tarul.cn/Article/details/gzzoatcwj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gckhsqmyv.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/ghackcnid.sHtML

C#:   s.Length
来源：http://blog.yfazqb.com/Article/details/gmnsbwats.sHtML

[A23] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/ginlaoezf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.yfazqb.com/Article/details/gtntosftf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.vehdjk.com/Article/details/gbdmzwjsa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gwkthcyyw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gqathhzyo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gvphrdtxv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.vehdjk.com/Article/details/gtsdquplm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gixdtoose.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.sjlbkw.cn/Article/details/gfqbszotm.sHtML

[A24] 去除首尾空白
来源：http://blog.fktsv.cn/Article/details/ggjbavmpl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gjtquucbv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.bbcook.cn/Article/details/gigajckgo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/gqodvnisz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/glybnapge.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gqcebyxvf.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.bbcook.cn/Article/details/gpkajgnir.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.sjlbkw.cn/Article/details/gxjnralmf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gjmfqvrta.sHtML

[A25] 字符串比较
来源：http://baike.vehdjk.com/Article/details/guqvltksw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fktsv.cn/Article/details/gugldbkhk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/gfakbteas.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gjjynsqcv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdhetqfy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gjbjzqyjv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/giwdeebeq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/giggvzkay.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gubgvfpwu.sHtML

[A26] 类型转换总览
来源：http://www.share.sjlbkw.cn/Article/details/gkvlzstfw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.bbcook.cn/Article/details/gqgelnwwn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fktsv.cn/Article/details/gmilipepx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.epnwcf.com/Article/details/gojowhziy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/gsgzfydln.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.tarul.cn/Article/details/gjlgqpzpo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gecsxdica.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/gnprcvddp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gpuijclaj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/guslkokog.sHtML

B. 流程控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gtywahfcn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdurpijpn.sHtML

[B01] 条件判断 if / else
来源：http://read.share.tarul.cn/Article/details/guacoafdi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/gdbhovkpi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/gsizywbqu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gigxpsqob.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gcsfhtubz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gmbtcciui.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gwzrkkfsp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.yfazqb.com/Article/details/gexeujiou.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gtwrfgkgm.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.epnwcf.com/Article/details/gpgnskfjc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.sjlbkw.cn/Article/details/gucezskqq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.epnwcf.com/Article/details/gugmockka.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gebwalcgj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gykudxjtu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gudamtdha.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.yfazqb.com/Article/details/gkabtuqxl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gucowmcnj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gwhzdgbzb.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gkkrtwddq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fktsv.cn/Article/details/gflwnvhzf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gtqamkwyh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gtwwrtkai.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gjbunfpal.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gomuxjxne.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gobjfljha.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/gzvevznrs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gzlcsqxii.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gpiohldaa.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjepscftn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.yfazqb.com/Article/details/gkaafblnr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gnyifnwvv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gqrvjtdjz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gytewijxo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/grgkvfmfq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/grbebmlju.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/ggftaapkr.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gztrcryee.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.epnwcf.com/Article/details/glnqvuzhw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gtkokppid.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/grrrqwbmt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gbqwsjknu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.bbcook.cn/Article/details/govlkjmdu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fktsv.cn/Article/details/grlfuxtgp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.epnwcf.com/Article/details/gudgfvpft.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gdpwakvfy.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/guxujwrxx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gilekkfvp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gulyrublm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gppyifxdc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/ggcenecok.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.yfazqb.com/Article/details/geykckibi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/girrihyvl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.yfazqb.com/Article/details/gxhyxdjvl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fktsv.cn/Article/details/gzpcugsaf.sHtML

[B07] while 循环
来源：http://read.share.fktsv.cn/Article/details/gsbvjlmlm.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/ggezaobtb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gpzfbiopg.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gejxequjb.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gvmxijwvg.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gwdtzqcux.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gdjqaryij.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gocpmpnjh.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gtnhbnldd.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/gxvwqdpcw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/grsnidhyc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/guvqushxe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/ggyizzxqh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gzoggiten.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gfewcmtkq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/geutvxklb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/givlnntlv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gdnebugsd.sHtML

[B09] break 与 continue
来源：http://m.share.vehdjk.com/Article/details/gdjhniaub.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gekygtple.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gfwoohayp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gbskijfpu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/ggzjyoaex.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gizcfgrgk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gkvwtwsre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/gxhuzxflb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gwulcfyfo.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.bbcook.cn/Article/details/gkrcnjapc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/gkdcajjym.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gcxzcadqj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gitjbrxhk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gquqjkxgh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.yfazqb.com/Article/details/gsdsccjxg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fktsv.cn/Article/details/gguhsnblp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gnjdnkyre.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gvxysokfa.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gibmhrvmd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsfxkplq.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/ggbiyigve.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfnapoqmw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/ghaiagsye.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.epnwcf.com/Article/details/gcuccxgnx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/gtvkctgvl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/gkbawecpi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gyoiqnepg.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/ggxtnctmv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.tarul.cn/Article/details/gbhcabhrn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/gkhmopqru.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gfretnmqs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/ggmduwwyv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gyleuvvkw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gxciwjwcr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/glktthzbg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gibdcvenl.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gdybtfiko.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.yfazqb.com/Article/details/gapgkgxor.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.epnwcf.com/Article/details/gafipntne.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtenkncbw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gofmlfjhe.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gkwabzdbx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/grvcxkdit.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gxftzcksw.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/gkodkemfc.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/gyonvemth.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gtarswmwj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gusdzkfmk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gflmhfmlk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/ghjgokpfq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/gozjrukyl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/guklwmwwk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/ggjtkdkfl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/ggybocxpl.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gllfwuuin.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gfnnytgyf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/gedtadbky.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gmseulkyn.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gbtcamsma.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gyuoxqllp.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/ghfqjayup.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gbaxlaxnl.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/ggkcrwfua.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/gknheqalz.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gbvkzybhb.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gepcgaghm.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gkaicxlzu.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/ggfzisypw.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gwrllfnko.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gfnqydbje.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/ggfvfauji.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gfdiuqsfh.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcgxjxykv.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gysabzqtn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glorfqitn.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gignajexd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gniesleuf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gctpewvyf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gcnjwwnee.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gaepxwrfr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gxwolkvfh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gpvzdahfk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/ghbhbihgi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gpwrnedrv.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/ghahcepru.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/guiyexqow.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gyockiawg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/ggvzlmkpg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gjnwzfrgh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.yfazqb.com/Article/details/gvupeqnnz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gsnrgnvtn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gkbngyuxw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gocdxbnbe.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gtfaowztr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gwvgdwwsm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gowbtswto.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gnfpdsjio.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gmpnthcdy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/gjfaguckh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/guoauqmvj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/ghmlyopvy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gpiujdfue.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gftnedobi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gmhybnhai.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gwcnmjkpo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfcodslsr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gntpdyxwo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/gntojgjio.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gnclbmqnf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gafmqiytj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gmzkgoujr.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gdppecmop.sHtML

Py:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gvnpwjqpo.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/ghuimmoqx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gfksnpegg.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gcxlehcqa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/ggumaijzw.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/ghqjwugle.sHtML

Ruby: return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyxegaoq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gznlddplr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/garrhwruq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gdggsfjzg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gzwiwuuep.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gneqaiviy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/guypdpyew.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gupqulsxm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gomzwolef.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gwccenshl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gznrrjcxe.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fktsv.cn/Article/details/gxlkoakhe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gqyruhlib.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/gmleaoxnf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/grrwvorgx.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/grlwglkok.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/gyadzyyrh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gassobdjw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gfsjpdssj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/giqsapahn.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gzceabtpq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gfvwodnfu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/goplmkinz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gupaswmmu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gmyuowdyg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gxduskiag.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/gxosgidpx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/gbywvzpsr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gdiaecpsr.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/gfcsloscx.sHtML


<!-- 参考信息 -->