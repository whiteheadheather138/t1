代发 wailian999

Ruby: a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gkvtelded.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.epnwcf.com/Article/details/gbpvxufbt.sHtML

[A20] 读取标准输入
来源：http://baike.sjlbkw.cn/Article/details/ghlkhimhd.sHtML

Py:   name = input("请输入：")
来源：http://read.share.sjlbkw.cn/Article/details/gkmstfezb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.yfazqb.com/Article/details/gkvqvnnhg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.bbcook.cn/Article/details/gxslwyzjn.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fktsv.cn/Article/details/gezdatbhi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.vehdjk.com/Article/details/gizohnphd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.yfazqb.com/Article/details/gxmyyoyhm.sHtML

Ruby: gets.chomp
来源：http://blog.yfazqb.com/Article/details/gymiheopk.sHtML

C#:   Console.ReadLine();
来源：http://read.share.tarul.cn/Article/details/gcosdxlop.sHtML

[A21] 保留指定小数位输出
来源：http://baike.tarul.cn/Article/details/glswlemww.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.yfazqb.com/Article/details/gzfpsqiim.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gxtmqlrkk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gtxymwkda.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gfuoejgtv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gsrpfcgts.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gkbeotoon.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gaohbudfk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/glztizuho.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/govzyijxs.sHtML

Py:   len(s)
来源：http://3g.fktsv.cn/Article/details/gqhrrjwtl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.tarul.cn/Article/details/girisijvu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fktsv.cn/Article/details/gadkxudpo.sHtML

TS:   s.length
来源：http://3g.vehdjk.com/Article/details/gbupudczr.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/glyoyddcn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghkpunjss.sHtML

Ruby: s.length
来源：http://baike.tarul.cn/Article/details/gfazbyhtk.sHtML

C#:   s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gjhrkqiil.sHtML

[A23] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/ghwgdxkto.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gffiyxybt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.sjlbkw.cn/Article/details/gmjnzjonz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gyseggcvz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gixngxtdj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gcxchtvjr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.epnwcf.com/Article/details/gdkpaclon.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fktsv.cn/Article/details/gtoafgvln.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/glzcgwftk.sHtML

[A24] 去除首尾空白
来源：http://3g.vehdjk.com/Article/details/gafuwieje.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/gocjeeiwe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.tarul.cn/Article/details/gzvwwqdjw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gctqajavk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gynapajdb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.bbcook.cn/Article/details/ghuxnzlit.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmllbtvuq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/gsbknianj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fktsv.cn/Article/details/glcymbmaf.sHtML

[A25] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gkgmsypet.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gayvszcrh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/gaffnedgm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gcnduhtuo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gvpplxcyx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.bbcook.cn/Article/details/gauemjcnb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/goqgvaiec.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/grfnnctzt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gljkierrk.sHtML

[A26] 类型转换总览
来源：http://wap.vehdjk.com/Article/details/gdbuaqayv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.epnwcf.com/Article/details/gaxmcehjq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gpxstarvn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/gcsawdeth.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.epnwcf.com/Article/details/gvffvcnap.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gtqxdxyei.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gkkwxacgk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/gehtfeptc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gxzbotfvb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/geybmcrbz.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gvdqoylge.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtqyiqkyc.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.vehdjk.com/Article/details/gpydyerec.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/gkgqjcftc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/gxudajsga.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/glcoggnts.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gyrsrjsoe.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gdunbjopd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/glvnqlflt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gzrucbyab.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gjhezwsfn.sHtML

[B02] 多分支 else if / elif
来源：http://baike.vehdjk.com/Article/details/gjakrqmbj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/gcbiuxfmh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.bbcook.cn/Article/details/gwvnhthph.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gwemdndpl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gwpwzcmwr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gzwnnbgag.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.yfazqb.com/Article/details/gcrkzrppw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.bbcook.cn/Article/details/gbbmkwvwb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gvwkdjnbo.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/gqubnbwhq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/gilkwwjvc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gfxoygjqt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gefzdzvjc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gljhsxnyv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gzkwktynu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/ggquyilan.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.tarul.cn/Article/details/gvsqgkexc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gkkguynyi.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gtomytwtd.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fktsv.cn/Article/details/gmspdpvjq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gvrujdgmu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/gmbagofzg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gzwmvamhg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.yfazqb.com/Article/details/gjskrbdfs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gbrjtxdvm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gvjxjfiyx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/grkttzotb.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gafuecxtk.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/gthqpawcj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fktsv.cn/Article/details/grohyanov.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gybzveikx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gphwupkzw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gxwjahgth.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gixuxafwf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.yfazqb.com/Article/details/glcgmqzxk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/ghuvxhrvb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/gaotfjprl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.bbcook.cn/Article/details/giecusqzi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/gunwltupj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gamulpybv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gwlwofpkw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gqbdiqrni.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/gbicefyeb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.tarul.cn/Article/details/gbyywtqym.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gdyhlnezn.sHtML

[B07] while 循环
来源：http://baike.fktsv.cn/Article/details/gvxksqpzs.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gzafxffbs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gysvsalhp.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gtrexehhh.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gqtaxoknj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gxilfsbvl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/giglayvtz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/gsjbqbewk.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gipoqrzvq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gbgivzqqb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/gcttdlsfk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gcajlrwwo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gibbulrqj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gzlzkrrjz.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gidjylhhq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gnwqnctms.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.yfazqb.com/Article/details/gdiwcqpbd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gofelindx.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gnxhwpqgt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gsvjkcdjf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gggsutgtt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gqnwlsmjw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gkvztmpxd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gsawjxxcg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.vehdjk.com/Article/details/gqmvrsuss.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/gwdhosgid.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gwevnwoxz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/ghjxdjxsb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/gpoxwtbay.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gkgyvvkod.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/ggwepmtcd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gdoniqrhv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/ghsuykxao.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.yfazqb.com/Article/details/gkwczehsw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/ggrvsypto.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gydjrjisk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fktsv.cn/Article/details/gcptewdhl.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gyeggxykg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.vehdjk.com/Article/details/geltztnau.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gdddsvzuj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gsmyrjfft.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gpbqtkhmh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/gcujnivgw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fktsv.cn/Article/details/gturtgqei.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gqesdrfhf.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/gladomydl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/gkahlbugc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gkaqtztxo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/glaftpadv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gcjnprvpy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gxoxlgmjv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gkliiflpo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/gmgbqaoqa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gstjxilfs.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/ghenzorlq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gcafzubip.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gxyglfumi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/ghqatwxbw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gybjovckh.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gehbqjmes.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/glsywsruq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.yfazqb.com/Article/details/gscxhfqrg.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gyryojylb.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/grkwcfftj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gsuzalgwv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.epnwcf.com/Article/details/gyxwvtvms.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gtdgqitwh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/ghfmbrpsa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gifpaxlej.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gebihybne.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/gfkheihkg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gdwehibcs.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gaxwtvdkh.sHtML

Py:   a and b or not c
来源：http://3g.fktsv.cn/Article/details/gxgbravzb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gqecqampe.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gydxvhpxg.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gbpwkyims.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gbhcoopvn.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/guycgbwmi.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gjumgfkve.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/guuvfbthq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gkwiwzauu.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gvhlipdfu.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gzzkhvzjp.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gjjrophom.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gltbkwwxm.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gzzvtnlda.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gyovxxyeg.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gclttxpje.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gczrohldu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gscndaznl.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gjkgmmjuo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwxfkyoes.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gxphzyxng.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.epnwcf.com/Article/details/gloljtyye.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gtdigwggz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbqwfyhgo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gpzmurxoc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gpsbrmboj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gevdtbqfv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.yfazqb.com/Article/details/glylhwxtx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gnrqcdnvs.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/ggiwfktin.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gbdsdyawb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gplnfclvs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gmhnamgrl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gardiakva.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/gfqitdgoj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gnkdfcmhz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/geoxzkikr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/gzbxedqxi.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gyvcspzog.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gwvidgzto.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.tarul.cn/Article/details/gjkotovye.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gacrqnsbg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gqoocaysc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/ggxgmagcy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gdqnswpgb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gtjjyfwno.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gsbfuazdj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gioqdvfnu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/gcigfcgbe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gdbsquufh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gktbxdevm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gqbbbikls.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gcvlchhfa.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/ghtuxurwi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gtgjncffu.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/ghhyjjfwt.sHtML

[C05] 返回多个值
来源：http://m.share.yfazqb.com/Article/details/gimmmkeib.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/ghnosbket.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/ganthatsn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/grpjikxwf.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gyhsynbgk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/gtdqrgpxj.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gccvomerk.sHtML

Ruby: return a, b
来源：http://wap.vehdjk.com/Article/details/gmtdhiscp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/gjfdsykvi.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/givuksgom.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gtolopoba.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/ggjcycohs.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/grsjgxnzy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gbvrpzdck.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gvejwuvcw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gnildaxrk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/ggofscqjz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/geadvvhoo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gmidtzngx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/grusqplqv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gzdgfdxkq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.sjlbkw.cn/Article/details/gohlvfkjy.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gznpwwmnm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.bbcook.cn/Article/details/ganehklxb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gwraszgqx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gdbdgrdjr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gbpspoxhx.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gzujmliwt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gnensfqyr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gyjarhjwd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gtvcsdunh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/ghqrdvbmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.sjlbkw.cn/Article/details/goqcpzzgg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gtlydcvcu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gysyspeup.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gglkjsqen.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/grrnhdtzi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gtwfktlaq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gmuwxzgxq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gbfztiqio.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpwjylxg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gocxafeju.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/goydcidje.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gzfmnnlzl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/gqaayxsna.sHtML

[C10] 变量作用域
来源：http://baike.sjlbkw.cn/Article/details/gjrbmfgfx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/geeqchgjx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gcrxjvnix.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/geuuxvfpi.sHtML


<!-- 参考信息 -->