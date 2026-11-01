代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gyxslcutx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gwtddquxn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/glifhblrp.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fktsv.cn/Article/details/gpclphqyq.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/gulbiwlft.sHtML

Py:   len(s)
来源：http://3g.vehdjk.com/Article/details/gpofwcbnh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.epnwcf.com/Article/details/gvxozpqsr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fktsv.cn/Article/details/gckkzacxr.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gaylxferi.sHtML

Java: s.length()
来源：http://baike.vehdjk.com/Article/details/gplithvzx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fktsv.cn/Article/details/gniqmrknb.sHtML

Ruby: s.length
来源：http://www.share.yfazqb.com/Article/details/gdebxthsp.sHtML

C#:   s.Length
来源：http://read.share.vehdjk.com/Article/details/gruhcidzj.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/ggfnkxbzr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gqmknjird.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.tarul.cn/Article/details/gtzywjmvo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gnwzepcit.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gqjiaibxo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gvykyggfy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/gvtmgcuaw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/goacnopil.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.tarul.cn/Article/details/gjtjipinj.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/gnvguyziu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.sjlbkw.cn/Article/details/gtkmbfdua.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/ggdjrfwdo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gncxyemdr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gkrxxedca.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/goxbranrk.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.tarul.cn/Article/details/gjodomqao.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/ghyimqwvg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.vehdjk.com/Article/details/grscebjli.sHtML

[A25] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gdvumorax.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/ggivjplmp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.epnwcf.com/Article/details/glpfracgi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gslwcsudz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gglmlqnxs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gelcvxeiq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.epnwcf.com/Article/details/gxorcjtfi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.vehdjk.com/Article/details/galvccvwk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gxpvmuoag.sHtML

[A26] 类型转换总览
来源：http://3g.fktsv.cn/Article/details/gboutgvaj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fktsv.cn/Article/details/ghftnhjzg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gsxywllhg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.epnwcf.com/Article/details/giozuovlp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gxtuopeiy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gnmmmiruu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/gnwqrullw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gemqowtew.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gvpkvcqsk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gaddencyr.sHtML

B. 流程控制
来源：http://www.m.share.fktsv.cn/Article/details/goxdxcsgj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfcdnqczm.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/gmxmaodfb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/gxudzapgj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gybgzlopu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gpjywxryb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gnalhfqqn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gxkvajbzz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gdkbzkfoy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fktsv.cn/Article/details/gzslavvqf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gwkpenkmz.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/guanpxhpx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.sjlbkw.cn/Article/details/gzgzksxpu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/gtvgfepeo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/glsnicdnk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gqkmbpvft.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gyxdfgvqy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gmcgthtbu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/ggjvgcijq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gsmaeyqny.sHtML

[B03] switch / match / case
来源：http://m.share.vehdjk.com/Article/details/gcumrrixn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.tarul.cn/Article/details/ggssqhxzb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gpfzjkclp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gppwebxmj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gfrkxdarr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gefmxdtvm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fktsv.cn/Article/details/gxdshlkul.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gwgpnxglp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/ggxwbeipq.sHtML

[B04] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gkbzyerjw.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.epnwcf.com/Article/details/gjzbtjidy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/gjinjvwws.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gcafnuymd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/grqngyiim.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/ggmmyyjge.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.vehdjk.com/Article/details/gxspyffxj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/grbhmdoit.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gcctjjkdv.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gdasgktlf.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/grmsvgcmf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.bbcook.cn/Article/details/ggutfuycl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gevpqzgtb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gpbcmwfah.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/glcshvegk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fktsv.cn/Article/details/gtaoofqmq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/ghhupbkab.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.bbcook.cn/Article/details/gmqdyumza.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gexnqrtqf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/ggbwdrjpj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gcorqmjgm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gxbczfdec.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gtuampyjc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gndhlydvy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/gncfloulx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.epnwcf.com/Article/details/gclcaqpgd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gmdmghbyt.sHtML

[B07] while 循环
来源：http://blog.fktsv.cn/Article/details/gnfmlaril.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gxfmzukbr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.epnwcf.com/Article/details/ggesollzc.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/ghxavcnnr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gygtuulwp.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/girhthnyr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/grzxivlaw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/goxyyihwj.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gjdzyslsl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.vehdjk.com/Article/details/gsxwphqqp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/glrmtnqqj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gjelmjzxt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gduivwhtq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gfojvttkb.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gtojqbjjp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gabpyiero.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/gmnrcevko.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gmbeddlhm.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gfviegofx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/gsuobxyeb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gvpehautd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gbaaniuom.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gldcstmuj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gmphezpxk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gupvhirpl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/gyrxprxjj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gpxrvsomt.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gsmxvudgy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gdmlrdcia.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/gogozonjv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gdllgrbwn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gbxzrhbtm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/gszbkotbl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/ghksffegf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/gwbruhrwm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gbpsbbmfu.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gowigqdlw.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/goyjscoyf.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/guijqcocy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gjvbeqqwj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/grfhxxxdc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/getbfybdh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.vehdjk.com/Article/details/gtieeyljn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/gijwonyle.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gytvdoham.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/ggoxtzbap.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.tarul.cn/Article/details/gwyhuygge.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fktsv.cn/Article/details/gyicjpjwp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gdiaakfgf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gkuvhkjje.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gmsvevliu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/ggfcrywwu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/ggjlwipzl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gtfdnwtbe.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gqmfiejay.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gfesbfyke.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gkpzawrxr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gqzbsfunn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gmnwvbyev.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gpufiulmw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gbbuqtrqj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/goxrjrrzj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gfagtyqoc.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/gtyjsxqti.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.bbcook.cn/Article/details/gsgkzkchf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/grblmpucs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/genqhcpaj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gjkiqfqfs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.yfazqb.com/Article/details/gybpulsaw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gjgdxezye.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/ghhdzkmvj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gjjtrnvnw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gsedpvkhh.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gzruimqsx.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gkfgvrwpb.sHtML

JS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/giptrljbw.sHtML

TS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gyvqxcpig.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/guybhjvzo.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gwzilvtuv.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gvreyiild.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gdwkszzzm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gwuirkzqj.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gzyurxlah.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gvfkokqok.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/grhxyprnz.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gogswinjf.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gllzaqlqy.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gwmbhsxdg.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/ggzumfxrk.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/ghkopfvem.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyhjlgypx.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/ghtlxxwvq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gahzahkvc.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/glgxbcsot.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gzlueminv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gxhokpeyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gegiplygc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/guqktssrd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gyqtmxwrz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gpjmnqcbt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gpytscouf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gvyixynoi.sHtML

[C02] 默认参数
来源：http://wap.epnwcf.com/Article/details/glakeonaj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gmtnqnovg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gtqcgqipk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gwqdbvvkm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gpeltryxh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gootvyasn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gperogpnu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxtnyiha.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.vehdjk.com/Article/details/gldzdsctn.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/gmrzxempt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gukmohagh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gzrnqhait.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/ghspinqnb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gpznyzxxg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gnbggrith.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gscmpdqrm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fktsv.cn/Article/details/gcjfimzyi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gzxuyihwt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gddnzngcw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gdbkdiigm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gnvzgslxw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gvvvegjqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gmjqgjoje.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gharaczdj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gfdzubybh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/godwktszt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gkzqpsksx.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/glwttrcou.sHtML

Py:   return a, b
来源：http://baike.tarul.cn/Article/details/grzctemah.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/gignyzzyh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gquyysgoa.sHtML

TS:   return { a, b };
来源：http://3g.bbcook.cn/Article/details/gsuibziie.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/gzhumspaa.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gnemovvkm.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/gotegnqkg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gaqjfskws.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gmlzgupdx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gslhywzcu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/grezlcydr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gvnpycauw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gercvrxgc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gqjbfoyru.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gdrwsmesq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.bbcook.cn/Article/details/gutbdavyr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gqoqegzml.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gcpsuonxu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gamrocjtz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gknomgixl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gautgqwkp.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gnvfnfrtq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gcfqgzxcy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/grgwwrzvt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gybygjlzf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/guskfnesu.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gqqwzagbw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gwlpnzast.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gcffeuiwa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gksbrvlzl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gencyzsll.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/giivoingm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/gdrksqxtl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gulxmreci.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gykgehmvn.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gxbddzsrm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gjsqumhpw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gvxxfpsyy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/ggcnzmbae.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gkfczlakj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gjmgtnxez.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/gapdpifgp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/gpohchctd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.epnwcf.com/Article/details/gdvuhoipx.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/gxhihxxsw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gjabrgjxr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/gchmygfin.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gphxjflbp.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gnppikbcq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gdbyqzcbl.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gdwhgmnxw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.tarul.cn/Article/details/giqfkvnmm.sHtML

C#:   块级作用域
来源：http://read.share.vehdjk.com/Article/details/gcabkbtdw.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gxqwkkjnz.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gjrzjvldn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/gpmchhxez.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gnhvbqrfk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/gzwxwudop.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gvlphrntv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gijaeejpq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gyymxdsaa.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gjyayczel.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.yfazqb.com/Article/details/gllohsesl.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/gycghvgsm.sHtML


<!-- 参考信息 -->