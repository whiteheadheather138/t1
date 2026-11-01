代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gztsfucna.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.vehdjk.com/Article/details/gplfndfkk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/gwbmfxxhf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.epnwcf.com/Article/details/gxzvmzamc.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.sjlbkw.cn/Article/details/gzmygwmuj.sHtML

[A19] 交换两个变量
来源：http://www.share.epnwcf.com/Article/details/gojdqenmk.sHtML

Py:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/ggyjpujmq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.epnwcf.com/Article/details/gdlclhmrx.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/guikfztmm.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gexurxgqa.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/gjmbtnusv.sHtML

Go:   a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/gsdsmkycm.sHtML

Ruby: a, b = b, a
来源：http://wap.tarul.cn/Article/details/gzanyhgiz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.tarul.cn/Article/details/gxvkoabsv.sHtML

[A20] 读取标准输入
来源：http://www.blog.fktsv.cn/Article/details/gwqsayqyh.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/gabltivpv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.epnwcf.com/Article/details/gewmrgmoi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.bbcook.cn/Article/details/gwcotfmix.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.epnwcf.com/Article/details/gvsdytlgz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.vehdjk.com/Article/details/gwpboxjya.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gfxoomapk.sHtML

Ruby: gets.chomp
来源：http://www.blog.sjlbkw.cn/Article/details/gbhdlymka.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/gjepygtqk.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.vehdjk.com/Article/details/gitedzxtu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.sjlbkw.cn/Article/details/gtufdwshu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gsxqnsuyr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gaowveqri.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyvbocwe.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gwzlpptdd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gbbkulxjj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gugkkxvll.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.bbcook.cn/Article/details/gjnebdekg.sHtML

[A22] 获取字符串长度
来源：http://www.share.tarul.cn/Article/details/glnnhtmfj.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/gyxdtfcti.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fktsv.cn/Article/details/gezfyvhlg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fktsv.cn/Article/details/ggwrereis.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/goycnjhyn.sHtML

Java: s.length()
来源：http://blog.bbcook.cn/Article/details/gvwwwkupm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.epnwcf.com/Article/details/gnmjxneok.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gauwlzllg.sHtML

C#:   s.Length
来源：http://m.share.tarul.cn/Article/details/gocteuacj.sHtML

[A23] 大小写转换
来源：http://wap.yfazqb.com/Article/details/goabsrcpg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gcakbsvpt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.yfazqb.com/Article/details/gwnualenm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/geamkgehk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/govwbqfhs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gwsxxnewr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.tarul.cn/Article/details/gnivvklln.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gppgbmlrs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gctmkxgty.sHtML

[A24] 去除首尾空白
来源：http://blog.yfazqb.com/Article/details/gsrdenimh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.epnwcf.com/Article/details/gqtaexjiz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.vehdjk.com/Article/details/gkcskfhof.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gwvwwovlc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.bbcook.cn/Article/details/gkfcrtkkb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gmgyaeazb.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gskjymnys.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gdjspbikh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fktsv.cn/Article/details/gczyiqvxg.sHtML

[A25] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/ginjneont.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.sjlbkw.cn/Article/details/gfatwasvd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gowqdhrfl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gcnzoaczv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/gklecsnbx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.vehdjk.com/Article/details/gnbgvvynp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gkkppubcy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gureycyzx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gpcbaeorl.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/gfzhzssfp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/gxmulrpbl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/gurxpaqrz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.bbcook.cn/Article/details/gondzorra.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/gtyytbesw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gmqgkfcvb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.yfazqb.com/Article/details/gclzzvsbl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.tarul.cn/Article/details/gfhtntevs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/grcgadyyj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdeadzlnv.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gaptwnyda.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gudnrorib.sHtML

[B01] 条件判断 if / else
来源：http://3g.vehdjk.com/Article/details/groirdyag.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.vehdjk.com/Article/details/gvqaqqehp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/gscsbhbjf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gfbcqjpaw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/goqcxpfwl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gxaxwhoow.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fktsv.cn/Article/details/gtlbtrnbb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fktsv.cn/Article/details/gkdbxgaau.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/ghiralxnx.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.sjlbkw.cn/Article/details/gzntotunf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/ghbkgcfai.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/gpeenqofk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gpsrtvigs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/glyayyyns.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gszwrjoll.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gmbbylsde.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.vehdjk.com/Article/details/gyqutfzjv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gpksnjsdl.sHtML

[B03] switch / match / case
来源：http://www.share.epnwcf.com/Article/details/gfhrgxhfn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gcudvtzuz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gvviekuxv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gsfukjutc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gxidjoxme.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gcttfdlqq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gnalxniuj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/grvteaalq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gyueanaov.sHtML

[B04] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gghvvawmh.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.tarul.cn/Article/details/gpmkpkcwg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gygvsiaal.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gyydohcfw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gqmckhmhc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fktsv.cn/Article/details/gizaaovao.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.yfazqb.com/Article/details/gwikpekry.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/gsasvjdru.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.epnwcf.com/Article/details/gtcfaixmr.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gumtvjsht.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gzfwmolpn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gerecmbua.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gtuxihkds.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gedsquduh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.epnwcf.com/Article/details/gozwvkimc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/ghdsfinln.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/gbcltxxne.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqhfhpqn.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/ghxcvsohi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gudbbuooy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.vehdjk.com/Article/details/gtwqsvuwt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gbasgaigi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gqwzahqea.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.tarul.cn/Article/details/gqhhzftsp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gkoenzcar.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gejksjyyh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/gezvglkjw.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/gxsxelvbg.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gizscjjck.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.epnwcf.com/Article/details/gnvzvtvvh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gdqvcqjtf.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gpmdtfxzo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gpgzmnmmm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/gmaokyixh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.bbcook.cn/Article/details/gzxachjus.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gowvtvgwv.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/guslenfrt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gqahnnglp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fktsv.cn/Article/details/gsxhsmhnt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/guastwqac.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/glcblbegk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gfhcmdfhh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/gcefsthip.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gvjqkzumr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gsjiroycg.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gvuhlgfjh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/gavencmjy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gzcqaphyi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gsdpkcnxj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/ggywenyub.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/ggdncxvgz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gvvlxzawg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/gxfamvwku.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gftnfbaaq.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/goultjsgp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.tarul.cn/Article/details/gjgaoadal.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gelklgqgf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gtmkejbnm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gmnjgjebn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/ggredhbbk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gkyvehdsr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/gaekmaufz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/glksjifje.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/geblvaaal.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gaqqdoolv.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gpatazcuk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gvbpunpgb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gzjlvqyrn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gpdzmnquz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gepvgptps.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/gcsdewmcv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gollixgkg.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gxssgovub.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/giumsvdff.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.tarul.cn/Article/details/guxiwonks.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/ggbihgxzm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/ggqiahlez.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gwzpdeqhu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gpjldleuw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.yfazqb.com/Article/details/gdbeketbk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/glorgzdac.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gchkwqpkc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gasxmxzvw.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/ggasgxped.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/grwfjcosk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/ghpsdyfxn.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/gpibynrxn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fktsv.cn/Article/details/gqctjkzlu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/gmdekjdkh.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/gqoyfjzqu.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/gbaktzlye.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fktsv.cn/Article/details/gfgjqhemu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gkfbvmson.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gyrkdyrqn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gnepxluym.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gltcryxbc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gpmkenbnu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/gawvnrbzx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gcvibfxnz.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gjwugglzp.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gopwpztcv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlaobyry.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gewbjpzub.sHtML

TS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gfwdxdywq.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gwdvxtwyp.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gvfzpdmay.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gozcjrfxj.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gtzyuzzkr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gtdngiuyw.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/gxspeohev.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/giyfeycdx.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gguomvijd.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gvusgabht.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/ggxisxkqs.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gorhwhqas.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gobdbifnj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gycqgashl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmdnrrdim.sHtML

C. 函数与作用域
来源：http://read.share.yfazqb.com/Article/details/gtptiggmt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwirpmdak.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gvygscjba.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gldkovvdn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gbcedbjcu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gfbrtiygt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gakjtgkyf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gengesqcm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gmpgkkemx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/grihpcuau.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gqpvwxzwx.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gngnwnrje.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gwxeqbdsi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gjoaclitu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gjtrlkgxy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gksuirezv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.sjlbkw.cn/Article/details/gblwhtjzj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/gznktoekp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/gyqflebcx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gdiuzvocz.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/grzbnjpjf.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/gquuqucdz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gpemywdns.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gzkjmeslz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gbqcpqfod.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gtdxldxsp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gekesdxor.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gsrhqsthr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/gpgxpfrpm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/gibullqqo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/geqcidjoj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gjfvvlstx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/ghdjebnxi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gbvjlvtor.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gqatboxtv.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/grrqiwxpe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gprwhlhit.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gctchgnqu.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gxmdmudvx.sHtML

Py:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gewkxoxgd.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/gjqmkzrvq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/ghnwftdpu.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gpsnmhyov.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/gjxhqrvxh.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/geeqiacnj.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gdeldobpa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/ghiyasktb.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gsdbsxsmv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/glntwdvtj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/gvkcdhzym.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gwillnsci.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.vehdjk.com/Article/details/gdljjsxpv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gmeuxnval.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.bbcook.cn/Article/details/gibuyynaz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/ggasmgpjc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gozvrqdos.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gpeawzdfj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.tarul.cn/Article/details/gkbeywvby.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.bbcook.cn/Article/details/gmzloobuf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gmixnkjuc.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gfpnyhrmc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/gspwuxgqo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/gofmefkzj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gjphqqbad.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/gcgodzzha.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gmywywtag.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.bbcook.cn/Article/details/ggkhaogud.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gcyqrrnnx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gznyvioqb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gvmzsjbpw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gvgkmdvuv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gmekvhdth.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gcltapcpg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gtwtundtd.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gfzdqegpw.sHtML


<!-- 参考信息 -->