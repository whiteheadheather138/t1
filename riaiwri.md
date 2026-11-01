代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/galqahzee.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgudqhww.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gbtjfgtfz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gmmtrrgci.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.yfazqb.com/Article/details/gediuksat.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/gzpisfkpj.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.yfazqb.com/Article/details/govpyvhez.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gdjsueyjp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.bbcook.cn/Article/details/gdhexzuiv.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.tarul.cn/Article/details/grezmwejd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.epnwcf.com/Article/details/gnbqkruoe.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fktsv.cn/Article/details/gateinbzv.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fktsv.cn/Article/details/godudjxyr.sHtML

[A19] 交换两个变量
来源：http://read.share.epnwcf.com/Article/details/gygitgbcp.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gqmypmsni.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.bbcook.cn/Article/details/ghpzhlmpj.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gkormfmsv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/gurnmquho.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gqwamiyxl.sHtML

Go:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gnqcidhfj.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gdzrvajoo.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.bbcook.cn/Article/details/gczcrqrpz.sHtML

[A20] 读取标准输入
来源：http://mobile.sjlbkw.cn/Article/details/gvpliumap.sHtML

Py:   name = input("请输入：")
来源：http://mobile.vehdjk.com/Article/details/gvknevhsx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.epnwcf.com/Article/details/geahsbhtz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fktsv.cn/Article/details/gxdvrptsc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.bbcook.cn/Article/details/gxexkaavy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.vehdjk.com/Article/details/gkkldaxft.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.tarul.cn/Article/details/gnmluepjr.sHtML

Ruby: gets.chomp
来源：http://mobile.sjlbkw.cn/Article/details/gfherieir.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.vehdjk.com/Article/details/gyaczydys.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fktsv.cn/Article/details/goawmjmju.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.tarul.cn/Article/details/gsgwxbkux.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/geszaxqtq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gzrhhkvnp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/ghbsaiqen.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gnwwajmpd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gvokbpins.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gpktvjaff.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.tarul.cn/Article/details/gelpuaejb.sHtML

[A22] 获取字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gievxmqsw.sHtML

Py:   len(s)
来源：http://3g.tarul.cn/Article/details/gncvgbgcv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.vehdjk.com/Article/details/gbapfqous.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.tarul.cn/Article/details/gvdsoarfe.sHtML

TS:   s.length
来源：http://wap.bbcook.cn/Article/details/gkxwoxeot.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/glsyxlzrr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.yfazqb.com/Article/details/geagsbzmo.sHtML

Ruby: s.length
来源：http://wap.sjlbkw.cn/Article/details/gcjomhdxe.sHtML

C#:   s.Length
来源：http://3g.vehdjk.com/Article/details/gimicltic.sHtML

[A23] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gxaklxvir.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gwbxxjfdp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fktsv.cn/Article/details/gygjrhimz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gfdibvvra.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gvntkhfms.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gzpbsarcb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fktsv.cn/Article/details/grnewfpra.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.tarul.cn/Article/details/gwcgxtwms.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.bbcook.cn/Article/details/ggginqwal.sHtML

[A24] 去除首尾空白
来源：http://m.share.yfazqb.com/Article/details/gqniavooj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fktsv.cn/Article/details/gfdwsszeu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gljkmqcfn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gaxrzxeho.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gkztwnfis.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.vehdjk.com/Article/details/giyngwubs.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gpjmqvthr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.tarul.cn/Article/details/gtugdzfad.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/grudvvvza.sHtML

[A25] 字符串比较
来源：http://baike.vehdjk.com/Article/details/grplfwujt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.sjlbkw.cn/Article/details/ghrfvaoat.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.epnwcf.com/Article/details/gqhylufdd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gvmrnynqg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gqujivuxe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/grzivwfat.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/glaclhkzk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gpanhlnhe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gruamarrq.sHtML

[A26] 类型转换总览
来源：http://www.blog.epnwcf.com/Article/details/gcurydfyt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/gctoewtpy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fktsv.cn/Article/details/gvfvglcpz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/gyccamaoi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.bbcook.cn/Article/details/gzrpgrqpj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/gxteruccp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/glqjqamht.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/gulkoxwam.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gutxsbgpy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcfplbydk.sHtML

B. 流程控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gttgdbltm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsxfupdqv.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/geeymrajs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gwnxtwnkd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gzpgdbwkf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gzxdgohrw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gxdoytmnv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/ghksgxnav.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.epnwcf.com/Article/details/godieeyzv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.bbcook.cn/Article/details/gmtundsbl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gigyscakv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.tarul.cn/Article/details/gsjrbbpqi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.tarul.cn/Article/details/gegfdolnz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.epnwcf.com/Article/details/gkgrttfkg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gdykdjatn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gybcwnjrc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/geslhhvzi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.yfazqb.com/Article/details/gcdmxqkbm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/ghbowlzny.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gwvorzymx.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gkqpznjyl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gfdkjopze.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gmcyfkous.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/glsknixwk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/grahxnuvr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvvguizni.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.bbcook.cn/Article/details/gaxbqvfal.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/gabpwkhxo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gakfueokr.sHtML

[B04] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gooftnchb.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/gduirjmli.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gyuyxcfqa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gnyqwaavy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gmhyeycyq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/gwlpfiyzm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fktsv.cn/Article/details/gqymikevg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.vehdjk.com/Article/details/grevkuxyo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/ggbigcvkv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gnbeseowx.sHtML

Py:   for item in arr: print(item)
来源：http://baike.sjlbkw.cn/Article/details/gbufpmwff.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.tarul.cn/Article/details/gfqduweam.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gnguvgdyh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gxssfzzij.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gwohwsumg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.tarul.cn/Article/details/gmucyoxkd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gcgtmzxht.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.tarul.cn/Article/details/gzvrlwbsg.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.sjlbkw.cn/Article/details/gonwxsqax.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/gwsgrucfl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/gsywerffr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/giajibrlz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gpdjptucw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gvaxloofo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gwkpwwxkg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gdwyoxnfd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/ggjytgghv.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/gqyvdnvji.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/glnnvaann.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.epnwcf.com/Article/details/gcxplebnn.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gbuyuvfxs.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/genmjbbuz.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gvmlsyxoe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.yfazqb.com/Article/details/govgnzsdf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/gkdhbpmny.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gwfvchkhv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/gysonimsc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.tarul.cn/Article/details/gsukfjxtw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/guvzuxbjk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gkirxnhjg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gppbriplv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gzdirksci.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/gzsiqpscu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.epnwcf.com/Article/details/gdicramkq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gdsiflbow.sHtML

[B09] break 与 continue
来源：http://m.share.vehdjk.com/Article/details/gnanrsqhr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/glnhxmajn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gsfkxxwwm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/glzdzfyzn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gfjjofyzy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gtldaicnr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gkzexsxww.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/gkcbktdkv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/grpvdkhfo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gkqubzhwy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.tarul.cn/Article/details/gwtdfatyf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gmswnqyii.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gpnnoqmtf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/genwedsbh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gjodbhqar.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/gadqijwpr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gsmuphqzr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gxukhicnk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/guilsbtmx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/gzukpevsq.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gauksouhy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gnbumuhwg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gpnhqohgf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gifggawpd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.yfazqb.com/Article/details/gfgibfnse.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/gkjewmtjm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fktsv.cn/Article/details/gkjrthezh.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/grchkqkbc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gybhlvypl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/grsxqdlro.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gqifuwted.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/ghawwxbez.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gkwbnpogy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gsojuwjgb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gmgehdomn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/guikmnovp.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gstzogtjo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gpgzntsfq.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gzoxkxiud.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gcjuycunu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gynwqqifo.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/gdfchictl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/gxiikcvkc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gmwfqqlig.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gwxtneuyr.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gtdckbmwd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gvajcseqc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gschairej.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gncczhjua.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gqgdleesa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtgkyeakn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/gupnhhpqj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gyexpwubs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/gwzhjzrqx.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gwbqgikgr.sHtML

Py:   a and b or not c
来源：http://www.share.yfazqb.com/Article/details/gfqqwffje.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/gnobtiljc.sHtML

JS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gzkosglhl.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/ghfqvwdgr.sHtML

Java: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gaecwqhmk.sHtML

Go:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gjonnwlvs.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/ggybsopvq.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gktuyyypl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gmevkcity.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/ghfmppjgw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/gifsbocsj.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gsnklyayf.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gljgdotex.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gzdfubktz.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gtdvxjcoc.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gcluiiabb.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/ggvzbdxtj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdylhktpn.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/ghtsaaosz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guxgdgtpn.sHtML

[C01] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gyeoughvf.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gzdwvmxco.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/ghbqjmgtg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/goghvukiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gnlsjdtgc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gbugtvpbt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fktsv.cn/Article/details/gvixwrhmr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/gmsftmgjs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmpdcgdzm.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gdwbbjsei.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gpdvrphys.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/gclwqdrls.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/ggxsceiiu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/guttgjfoe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/gjhnxvvxb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gxfvbqyob.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gubboflec.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/ghejxgvev.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gagiwxorj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.epnwcf.com/Article/details/guqzbmeqw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gszfumhdp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gddbojuwj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/glozfntex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gyhxjidpg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/gmiducrer.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gibqzvonh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gwtoamaxa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/gymjgfijk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gbuzrczzp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gutuyhkkd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gpczjlrod.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gquvdgjzp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/ghwpjlcic.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gcuuazvlv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/glleqvxyz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gnohrfdwc.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/gavtcbwym.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gtqefjpcm.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/golhjxyuw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gyymyauga.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gapdgtdfv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gxyylzrrr.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gwsvpzind.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/gpkoatwrf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gmvejkrzq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gytozljxn.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gyhgecylw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gfrejvwlr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gfrhwnthm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gvihdgyfl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gsqcmhbok.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/gmozbdutu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/gupmuyhfd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gvcopdrhp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gsdotrbap.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gyupprmha.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gfwodtkzv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.tarul.cn/Article/details/gymoebahq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/gmjpytxug.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/giqnixwkh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gsalhupcp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpheckhm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.tarul.cn/Article/details/gwuzjcddj.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gbcuhtnbp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/gsyilnwhz.sHtML


<!-- 参考信息 -->