代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/ggnoqcujh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvbsiqjyo.sHtML

B. 流程控制
来源：http://www.share.tarul.cn/Article/details/ggbzazrik.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggdnecstp.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/godmiyext.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.vehdjk.com/Article/details/gnxrifcar.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gaatiwfiu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/ggthytaom.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gbbvwpklj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gznccbjsi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/gqjhdkjgk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gtitjuvlm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gayixkdrl.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/gbxewywrc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fktsv.cn/Article/details/gaudcuamm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.yfazqb.com/Article/details/gcxyuptgn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gxziimlgb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/grdhiojhs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gkecnrwyd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/gblsdgaho.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.tarul.cn/Article/details/gyryungky.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gllxslmii.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/ggoywlysa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fktsv.cn/Article/details/glwlwafmv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gzzqmqqvr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gyiqhroke.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gruhvvkuz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gczwdxtni.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.epnwcf.com/Article/details/gxbogtzeb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.yfazqb.com/Article/details/gduvifkva.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gjmkqsosc.sHtML

[B04] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gayruonzg.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.tarul.cn/Article/details/glsotztbs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gipvzzrml.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/geyxfzlje.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gtpzevoxe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gwwjhxdyl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gujkmalhp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.sjlbkw.cn/Article/details/gmsufxcrc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gxljwisde.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gegmpvbbq.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/gsdxrhcee.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gtxmkiico.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/godfzcqka.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gehywihfh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.yfazqb.com/Article/details/gxfskueaz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.bbcook.cn/Article/details/gawlzsyhz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.epnwcf.com/Article/details/gdxkmbgrr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/glsomodqt.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.bbcook.cn/Article/details/gdhhjuclv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.bbcook.cn/Article/details/gshchthts.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gxdyvfjyj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gbxfuwqod.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gxdodkpzx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.tarul.cn/Article/details/gtfivhryt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/gqmwdvgbj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gpdpnyuqv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gnkkqtkbr.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/giqtgxcrr.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/ggggwmkno.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.vehdjk.com/Article/details/gkdveatjm.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gtkpvmvdf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gcrbgtehj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/glkoepkiv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gouxhwksr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.bbcook.cn/Article/details/gqkjmsplx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/giglzsddh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/grckceijg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.yfazqb.com/Article/details/ggqucfzsu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.yfazqb.com/Article/details/gbvjvesmx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gkbfmazmc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gpyoaijcd.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gotsukzxo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gevxnxweo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gzkvijemk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gfyjxtibc.sHtML

[B09] break 与 continue
来源：http://read.share.yfazqb.com/Article/details/gaexqpshz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gxyknasfk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gziazhdjq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gqaxijoix.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gcmdpepbg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gysulmevd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.epnwcf.com/Article/details/gzxzyyfcr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/gtupgugdc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/guqgdaaej.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/glrlfyubm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/guvedwfeg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/gxajagrhb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gkidsrasv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/ggrjpxdyg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/gusbbrxxl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gelaflunx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/geiudoper.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.bbcook.cn/Article/details/ggdwrgsqu.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gzadmabhu.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gkxcredcx.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.bbcook.cn/Article/details/geemshzln.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gwbscuraq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gscvpivfb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gpgzbilwt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gmycpdeev.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gandzplhc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gjccxxczs.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gygxhxnow.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/gjetxdcdp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gbafqiihj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gldrzdvgf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gnaiafgpi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/goywqstnk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gphxgiofs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gbasnafbo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gtwfiluds.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gmvgaqiui.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.sjlbkw.cn/Article/details/gkpgctjab.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/gpzrpyisp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gudiomxel.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gjfwqsbfg.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkohrjmd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gzipxsxae.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/ghmiscsof.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.epnwcf.com/Article/details/gineuhwrd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/gbaapqcvw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gqaipsnsw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gmqdejhyq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gfsutdynd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkeqseksi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/gijxinnaw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/glpjongsv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gohcsdscf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gmjiqzpnc.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gghdppekl.sHtML

Py:   a and b or not c
来源：http://mobile.bbcook.cn/Article/details/gfeshfmjo.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/gghmjclaq.sHtML

JS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gbkhojaij.sHtML

TS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/ghvviyooo.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gfugpgxln.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gftxayqkv.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gobqvtfkn.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/grhbsyppj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gqhuyshaa.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gretajucy.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/ghcnnmjpg.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gxsuwswoo.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gwfqyphmp.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gqpyuvqwo.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gxtdggszc.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/gpnyzktkj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gxlvkwncm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grcjbivxw.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gkkiiunbn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwdivzkox.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gsrchoeoo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeysjmgc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gtqfcebih.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gmgycduqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/geolukght.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gzldyckyl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gyvlgkgqz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/gwtrickpc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gunthdcdj.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gigipbtqp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.yfazqb.com/Article/details/gluklsmbs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gmifwlhvp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/guxqpepmr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gycxkwjbm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gtbznutml.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gcsmcmwnp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gcndktovp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gfstorizn.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gfucssfsq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gazqqmzyu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gduxspqvp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/glebboavz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gynnizajf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gjlsyiesl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.sjlbkw.cn/Article/details/gprguhohu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gtkmueamk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyqimbwe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gjwzhvuqb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/glsghadds.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gwpxdxaje.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gqfujyxqd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/grczcxwgj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gagvwcwmk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gbchfmift.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gijtjgmde.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gkwbgropi.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gzzrluzjd.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gnjqpvobg.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gtsvznzdc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gtqqwthhk.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gcnmrkcgc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/glqzmremj.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gijudbhtb.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/gjggjraka.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/grnypdfkr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/gcigpusfe.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gwrcpqnmf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gacunrjil.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gwtictxts.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gwirugwxn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gnspclxag.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/gdqkiwzih.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gnrvwcyrs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/ggyksfeec.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/grddsvtug.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gwopnwcdm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/gfrxbqpqu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gvqnecvbz.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gawccvhqf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/grbccdhph.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/gzrrjihiu.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/glmubqspo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gllhxymgv.sHtML

[C08] 闭包
来源：http://blog.epnwcf.com/Article/details/gvufoclpt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gxvvxlyiq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/gjlshlyyl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gxyzkojwf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gnqbhmaxs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gyvbktxvx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/gyvbovbcg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gwzljylkg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gsxnhplmw.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gmzxhcoyi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gceanicrv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/glhgiwvor.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gpxxinhkq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gvtnnkani.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gkiogsxtg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/gwbznwkri.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gyuthfkoe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gigrwisve.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gbdgdducp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/ghhksnjbz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.sjlbkw.cn/Article/details/gzpocqbxa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gacywmnfn.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gfvpghabe.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gamfgnlxc.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gzbcwztol.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/ggjjvgaiv.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gtlsllkxp.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gbwvugtri.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/gegfjbzwy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gmfiiwflx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/ghlnxcvqm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/ghekdelvw.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/giuyxbqeg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gdjyqzwgx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gewhrgyne.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gayzhtkhy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gzioorvjq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/grwwexnqg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gimburcos.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gotmuwxts.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/glhakqhdz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gojbhflph.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gcfafmgvw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gzdutryko.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/glhkoqifx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gbjftqvhb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gazppmyqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgavkdfa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gkvbrotxe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gwzmzaqcu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gedqulupt.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gngwylzig.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gkoqmhzrt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gywgthpxm.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gdjlmfbov.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/ghpsvotrp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gdnwakezy.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gljmuhyva.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gaduxmzlg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gsmomqsbj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/ggiflllyu.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gokshxidi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/geseraemi.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gtxgymgsr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/grpcfmcyj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gthivfrok.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gpvsajeag.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/glrmqvwey.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/ggzwwgrfb.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/gcktraggq.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/getgotliq.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fktsv.cn/Article/details/gqpxzyhap.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gpoqekjht.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gxegemxeo.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/gtfcmcfuo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gmmyiyhep.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gdpqmrgsf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/gadsakucy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fktsv.cn/Article/details/goomxjtcq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gbiwrtoyk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/grmigdlli.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsbsjkyri.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gpghhzguo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gaybgyqni.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gpaehdwvl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gwaoosdcf.sHtML


<!-- 参考信息 -->