代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gmvhogfag.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.sjlbkw.cn/Article/details/gypkkwwbk.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.bbcook.cn/Article/details/gnkusphwe.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gfqllgmjc.sHtML

Ruby: a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gpymlrduy.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/ghdhfblyv.sHtML

[A20] 读取标准输入
来源：http://baike.bbcook.cn/Article/details/gtqpogwry.sHtML

Py:   name = input("请输入：")
来源：http://blog.epnwcf.com/Article/details/gnfmsljyo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fktsv.cn/Article/details/gckublefl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.sjlbkw.cn/Article/details/gjjrjgwxs.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.epnwcf.com/Article/details/gqzsexcdm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoauqlok.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.yfazqb.com/Article/details/gdoqmmikf.sHtML

Ruby: gets.chomp
来源：http://baike.sjlbkw.cn/Article/details/gwtmjcchi.sHtML

C#:   Console.ReadLine();
来源：http://read.share.epnwcf.com/Article/details/gpuzrnkqx.sHtML

[A21] 保留指定小数位输出
来源：http://3g.epnwcf.com/Article/details/gazvoxhal.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.epnwcf.com/Article/details/getibtvdp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gkrvsuqfq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gokzerzhj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gpwgumrsz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/ghqpaoplt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/ghzpiuvoa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gbsahkdht.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.sjlbkw.cn/Article/details/gopsbwwmf.sHtML

[A22] 获取字符串长度
来源：http://www.blog.tarul.cn/Article/details/gamcpihrq.sHtML

Py:   len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbygsaem.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.yfazqb.com/Article/details/gwbloodvm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/ggmgqvspp.sHtML

TS:   s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwwysuxx.sHtML

Java: s.length()
来源：http://mobile.sjlbkw.cn/Article/details/ghirlcwvl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fktsv.cn/Article/details/gwpndvsdq.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/gfhselmdb.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gzrmairny.sHtML

[A23] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gtpsjzouv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.yfazqb.com/Article/details/guvprrmce.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.sjlbkw.cn/Article/details/gaddctiqd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gocidlsff.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gcxpiuquo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gguubgtas.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/gxukiktvk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.bbcook.cn/Article/details/glaexchtv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.bbcook.cn/Article/details/gdzqoahdx.sHtML

[A24] 去除首尾空白
来源：http://m.share.bbcook.cn/Article/details/gxsunqbsd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gfvdqezkd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.yfazqb.com/Article/details/gxrjdpdtp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gddnhsbbf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gtehenmtl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.sjlbkw.cn/Article/details/grcenswow.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.epnwcf.com/Article/details/gdrwvlmro.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.tarul.cn/Article/details/gpasbrbve.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gzwkaeblm.sHtML

[A25] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gglstufkj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fktsv.cn/Article/details/gtbprrjkv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.tarul.cn/Article/details/gspgmyuzx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gkohoqctp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/grvymhnte.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gyqhmemty.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gtsaksbti.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fktsv.cn/Article/details/gmgiaysrd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gasbneydf.sHtML

[A26] 类型转换总览
来源：http://baike.epnwcf.com/Article/details/gxssromja.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/gybwnkhwc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gepytzprt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/gpffpqpmm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.bbcook.cn/Article/details/gsixujvtb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gxmdfspyp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/gxuspxxfo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.sjlbkw.cn/Article/details/gszhlzvel.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.tarul.cn/Article/details/gdgmeghpc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gothubjco.sHtML

B. 流程控制
来源：http://www.m.share.yfazqb.com/Article/details/gyawjxdxj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtsxwfkqr.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gvfesflnd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gdaacpyio.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.tarul.cn/Article/details/gubxtnxjm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/glujcshrc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gfjqsrutp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gucgmlhpo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gkyhctklr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fktsv.cn/Article/details/gyrntoazs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gusowunzc.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gyjlfjola.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/gkqwwebck.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.epnwcf.com/Article/details/gsbzxctsk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gclvxqliw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gkjddkiqa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gzkihlgwk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.tarul.cn/Article/details/goscvnaqg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fktsv.cn/Article/details/gnyztrnfw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gjjezubvv.sHtML

[B03] switch / match / case
来源：http://mobile.bbcook.cn/Article/details/gakcmuyab.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/gynysllsh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/ghmtrnrrc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gpwuqdvca.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gxtsyyavj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gzuigebiu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gxgzqneuj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gyitryqaz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gogggpfeu.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gjcbitika.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gdnlqgeco.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gyhobbhts.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gappdjxwt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gfkijzybh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gxynenkqz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/ghuheehnt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.sjlbkw.cn/Article/details/gejgkvrxa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.sjlbkw.cn/Article/details/gmqvejwjd.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gjcccmdjc.sHtML

Py:   for item in arr: print(item)
来源：http://blog.epnwcf.com/Article/details/grskjmxcs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.vehdjk.com/Article/details/gwlimppib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gxkfiwjol.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/groucakeh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/gynurmrxu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.bbcook.cn/Article/details/gobfrjpln.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/grzxirlpb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gttgukzfa.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/gvdwksxvy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gmgdhpjcg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.tarul.cn/Article/details/gceyjsaho.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gutgwwozw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gewjivewt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.epnwcf.com/Article/details/goyelkgeq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/gzsjoryze.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/gauzueddp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gmrspfxzr.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gviixtzth.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.bbcook.cn/Article/details/glhibsrhh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gzbglntdl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwzcmntbc.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gxczuieeb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gzxorwpgs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gpmnedyhx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gdquwqrku.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gyqjbbsgj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fktsv.cn/Article/details/gdzmydmjd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gzgklxzen.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gnkbwlvoc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gkgavzgxe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gwnncpjng.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gdcejloyu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gwsxpvbej.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.vehdjk.com/Article/details/gcdxjnqjc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/givckbklc.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gxqsvrfqg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fktsv.cn/Article/details/ggsbkgwls.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/ggpmrvkns.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/grkxcvymz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gdguemhex.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/galwpaqsu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.tarul.cn/Article/details/gdtotadnh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/gjwournzi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gxhrrivge.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/gmctgliwv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/gczrgyvbs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.tarul.cn/Article/details/gywboygzw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gauuuurdd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gioaqljmy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gyakrfhpe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/gxwaisqpu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/ggbytmnwf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/greqcctgj.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/ganuvorzs.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gsnttikcr.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gphskajwm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gdveohobs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gxtweabhl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gdginngne.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/gztwsysky.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gjpeggtee.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/ggohkqcdt.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gywaptdzb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gnvujcfno.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/gmixbllfj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gflrljgmz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gdsxfnucb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gnkbqpiqo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gmoldgjrm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gqpvuxxae.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/ggyoexvle.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gnppqnvib.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.sjlbkw.cn/Article/details/gpsebmusb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gxykxtypq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gwxeaterr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gtjswmlpp.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/gyrgcfnyk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gzsynmknb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/gnlbjroph.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gqqvrxfho.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gohkrdsoh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.vehdjk.com/Article/details/gcdgsxxzz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gnrcoedjs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/ggzngfopw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gkwtbwsct.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gkdjtmwnr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gavxaulpi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.vehdjk.com/Article/details/gurzjnuaw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gquryitqh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gxlriuncd.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/ghmdjyxvf.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/guwlgoxlj.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/glbiclasq.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gkodjltfs.sHtML

Java: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gdgqvbkxb.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gcwluwspk.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gtwnmmzxl.sHtML

C#:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gmxyoskvq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gdxrgiwkv.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/ghxdkjvzl.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gydbtpkph.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gvihfnxet.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gkpvucwwf.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gdqzuucxx.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gaedpprfw.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gklegbvpu.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gqldhycoi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gsocjohhl.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/goskxzswn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grlpzshtd.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gjyhtsvew.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gsiywmjfd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/ghwgndxwa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/goairgsvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gccwkkshr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gvghgwiaf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gzsfmebce.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gqkjxqawq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gkocfixxf.sHtML

[C02] 默认参数
来源：http://www.blog.vehdjk.com/Article/details/gwdiumwpz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gwqfhnizz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gmriimxqy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gnssofbvt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gswkppbvm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gkmpvcnit.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.tarul.cn/Article/details/ggdmysbek.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/gbcydwmhr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gixzrlccg.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/gdiglzyob.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gplztngrx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gxqgymyxg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gzkqmonwa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gomfzllsw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gnreunnef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.yfazqb.com/Article/details/grhcfrlyv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.vehdjk.com/Article/details/gcossftkb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gwjisvzco.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gquttkmpk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gghryvbog.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/ghuftcvym.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gevdywone.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gszsehjrp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/gsoxjufxh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/ggcqmuhjt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gswpqulkq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gsbbdjzzu.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/gjstowqkd.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/grptpyllp.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gwmbcytke.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/guphecprw.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/gaqaysgky.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/garexjsyi.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gstcyyslw.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gagayqxso.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/ggbppynws.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/gnjnxwgru.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gobxodwgd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/gujagdrbn.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gkbdubado.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gycldslxi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/giwkmkctv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gigafywsq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gkziomhmp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gpjolskgf.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gmedpeeco.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/grdxznfjf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gnhjfcspn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gpvwlxjfh.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gfktmpkxn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/glwjfiudl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gisgyvvrl.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/gohmqpmul.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gjbouzfpd.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/guhdcdzxj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.bbcook.cn/Article/details/gpusmlvji.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gxuyffzjk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gcpdcajjb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/grzhzwvsf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/gemgvfaur.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/grmbqbpre.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.epnwcf.com/Article/details/gbrfvfhsu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gxtogmifp.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/guyikcmnz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gfibqaacf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/gyecrgdgv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gxvvymazs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gljtdhpet.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gsctsmwgz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.tarul.cn/Article/details/gdepdyxaz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/grlasiiju.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/giqhxmlic.sHtML


<!-- 参考信息 -->