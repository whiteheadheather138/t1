代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/gcwxaefsu.sHtML

Ruby: gets.chomp
来源：http://blog.sjlbkw.cn/Article/details/gjbwrbosr.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/gkoocarsn.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.vehdjk.com/Article/details/gguhwdama.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.yfazqb.com/Article/details/gokoihrwu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gtxrbdsle.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gjbwymntq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gspfmjiqm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gpfhiakbg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gdqdogqyv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gfqcguzza.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fktsv.cn/Article/details/gdswzyrwl.sHtML

[A22] 获取字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gyybynbpm.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwtvtbqjs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.vehdjk.com/Article/details/gosntuksz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fktsv.cn/Article/details/gzryfzhyd.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/gqpivhznw.sHtML

Java: s.length()
来源：http://m.share.bbcook.cn/Article/details/gwwrqyhyr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gwqztzjlp.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/gtkqfmzag.sHtML

C#:   s.Length
来源：http://baike.bbcook.cn/Article/details/gsnbiobvy.sHtML

[A23] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gwyoyvoso.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.epnwcf.com/Article/details/gynjfdfzo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.yfazqb.com/Article/details/gjapsrbzp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gbeqhkybw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gurqudedf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/guwkjywbt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.yfazqb.com/Article/details/gceuliaqd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.yfazqb.com/Article/details/ghafwhzvt.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.tarul.cn/Article/details/getrgkxtm.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gdoavbgws.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.tarul.cn/Article/details/gscbnctyw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.bbcook.cn/Article/details/gpphpaqvd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gnttbmwts.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/gqfmigneh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gzffqmsdc.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.vehdjk.com/Article/details/gmtcvdtey.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/gnkggcmyw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.yfazqb.com/Article/details/giyrgjrhk.sHtML

[A25] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gfdxdnqvn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.epnwcf.com/Article/details/gptyylxni.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fktsv.cn/Article/details/gejwxavog.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/gwfwmduzs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/goqkxujdt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/gisufxzyd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/ghwyvofcq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.sjlbkw.cn/Article/details/guhnojojh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/golvzmslr.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gnqxzcvnw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gqjhvksaq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/glgvtkqts.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/gsqplkoti.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.bbcook.cn/Article/details/gjytmfscq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gxgpwjjok.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.vehdjk.com/Article/details/guimvwvad.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gqvwvsicm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gxybuvwtp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfcpthcgy.sHtML

B. 流程控制
来源：http://wap.sjlbkw.cn/Article/details/gobmbeteh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmoehzpla.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.epnwcf.com/Article/details/gaselbfpf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gytuyllvc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/ggkhxrsym.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/glmjphslx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/ghbmdhzea.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gieigphma.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/gtrfnihqb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.vehdjk.com/Article/details/gshnyzyph.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gguwpwgan.sHtML

[B02] 多分支 else if / elif
来源：http://blog.vehdjk.com/Article/details/ghowhumjx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gnexrigyj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/gprbupbue.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gduszveoe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gicuifsvq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gkwvkgyts.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.tarul.cn/Article/details/gztfkyxfk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.epnwcf.com/Article/details/giswomhlq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gkcrpxfhz.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/gmamfwuvi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gxlbbswtx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gaqtxtzpk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/geqguechu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/ghghowmnv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gpqiuwgzf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/grfmnhygv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.bbcook.cn/Article/details/ghkollffk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gqcagmyvs.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/guoxibdlq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.bbcook.cn/Article/details/gxxtncsdc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/gerxobmyg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gmiesmnvh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gyywmfrog.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/ghelnkzma.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gaqqhgyuq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/gderctomc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fktsv.cn/Article/details/grqvacaah.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gglipwdlc.sHtML

Py:   for item in arr: print(item)
来源：http://blog.epnwcf.com/Article/details/gpczgyvjg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gonowrmro.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/ghinnayru.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gurvrcymg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.tarul.cn/Article/details/ggzwhecbh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.sjlbkw.cn/Article/details/grltnzwzs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/ghyjvfoct.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gixanklih.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.epnwcf.com/Article/details/gvizfmwje.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.bbcook.cn/Article/details/gqucvpuft.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.yfazqb.com/Article/details/gyrqiczdk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzfkgmvda.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gpfotuwdg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.epnwcf.com/Article/details/gvcrgalkv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/gongrwyab.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gvpylultr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.epnwcf.com/Article/details/gwmuadkuh.sHtML

[B07] while 循环
来源：http://www.m.share.sjlbkw.cn/Article/details/geavriiua.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gwnpqqyyn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gfxnjfxzg.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gjosktnho.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gvmrcoodi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gzinwswee.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.bbcook.cn/Article/details/gqtfbtabb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gjsghhoyx.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gosileadz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.epnwcf.com/Article/details/gbhgnnsvf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.bbcook.cn/Article/details/gygzeyhef.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/gamavrlxs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gfdyzjheo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gqjidtmxk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gybpcejrf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/gzllwtcip.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.sjlbkw.cn/Article/details/grhzpipos.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gkitdetun.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gmccbjohz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/ggbhuvhid.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gdqcekkdb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvveupybc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gqjgrqedj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gqlegamth.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gnsstkaxq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gxmogmubp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gyamvgmyf.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/gagisjluy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gylruridf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/gvhrpzqct.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gwpvljhoi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gjcyeired.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gtysdvshh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.epnwcf.com/Article/details/gbrsvzlaw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gbykmxcyu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.epnwcf.com/Article/details/ghlujcbia.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gprttgxyb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/gkmczmgqu.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/gvjrrewpu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gcfnhyfcn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gjtspdery.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gdnxaaeah.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gucwkgfim.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/grehwyujo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/graqgouxb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjxdqtau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gnnqyqccw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/gcransrcv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gopsnrhki.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gljjtyznp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gzaddzxpq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gxrvwgdiv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.sjlbkw.cn/Article/details/gyichnurh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/gbkjfpwry.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gbuphfwag.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fktsv.cn/Article/details/gntfcoasn.sHtML

PHP:  is_numeric($x)
来源：http://baike.yfazqb.com/Article/details/grkaxzlif.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gtqyguref.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/grcfzzgwb.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/ghjhxrzsw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gnojtqgfw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gtkwfdcey.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.epnwcf.com/Article/details/giqzrwjsi.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gkupibqau.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/ghlbcvexy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/gbkbbqxts.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gfroruxye.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gjwfaprrk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.tarul.cn/Article/details/gfjiiqpib.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/ghbxblimr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gvleqjmjg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gubpomxzg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gkoeverkn.sHtML

Py:   a and b or not c
来源：http://baike.sjlbkw.cn/Article/details/gqpofpkpt.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gegelzxem.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnnsgofl.sHtML

TS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/giuroybrs.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gvcnfgmhz.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gflmeidyi.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gfuvpyxaw.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/guvvwrmxb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gdvguzhia.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gyvuvrftm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gmbvkfiqp.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gmixmklfj.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gzucfyjar.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gldlkptbn.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gshybkspt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gmfvxzclo.sHtML

C#:   if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/grldclzas.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfwsrsvox.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gqjshoevv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghrrwpzwu.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/gqutxrypk.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gacwmjkcj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gslrtkfxe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gehgbbmlz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gjbzfrwqq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gvkaluyzz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/guclqhndw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/grlmwgakq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/grszriwse.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/grorlpclt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gslgbcqin.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gjxlymsoh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gogjczlya.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/glbsluqma.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/girumltfi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gtiynbwoa.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gkijsftqi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/grmxvrzqf.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gtbmfdltz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.vehdjk.com/Article/details/gwuswytqp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gjlnmycms.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/grebudfjv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gpaucntzv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/gilovledg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gesuhxodu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gbusuvnxn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/gxmztzcgv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gfmisomxx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gxdhlztry.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gomlxzbxm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gxxcquask.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.vehdjk.com/Article/details/gudbzzqbz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/guxcqhfys.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gsttrtrcm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gjgfxqpga.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gfzrgxrzh.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/geqknenll.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/glwaikosp.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/ghvwnkrqm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fktsv.cn/Article/details/gcyuukmpr.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gqfscnpja.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gfrlvahsu.sHtML

Go:   return a, b
来源：http://blog.yfazqb.com/Article/details/gigmlacnf.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gqgnpmtju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gmfhicdut.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/gngutpovt.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gpyndmgxe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gwnldrcyj.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gpxbrdutt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gchsddwuc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/ggxyrzusb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/ghwhgboud.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gxmkjndoq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gwbxwyool.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.yfazqb.com/Article/details/gzxahldym.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.tarul.cn/Article/details/gnhahzgon.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gamcijfyo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/ghlfefsuq.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/gnigtmzgp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.bbcook.cn/Article/details/guubbweoo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gnvwwycpp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gwwbgaojg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gyfcnbnds.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/gryugsxsy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gmpqrdemm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gyypudboq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gstdyrkpp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/geutpjqup.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gweycgdjp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gvocpqong.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gkqtffkud.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gukthyzxn.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gslefhret.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/grpbfxkda.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gfjdvposv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gclrjtqqd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gmgymseyj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.bbcook.cn/Article/details/gwzzhpmeo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghfvfaado.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gcoyzkdrv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gmveneddp.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gnitbdnxy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gjsflzshe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/gbopepbdd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.sjlbkw.cn/Article/details/gatzlfddx.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gmtslqjln.sHtML

Java: 方法内为块级作用域
来源：http://mobile.vehdjk.com/Article/details/geilqjydb.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gppazhsrm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gnqoyrbju.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/gbhldoqdf.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gzbwvkdmj.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/gvdmabsad.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gguguqgyb.sHtML


<!-- 参考信息 -->