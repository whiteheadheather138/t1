代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://mobile.sjlbkw.cn/Article/details/gxntceznc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gnuvggdxf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.yfazqb.com/Article/details/gvjjnhjlw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.bbcook.cn/Article/details/gmuokubvf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gchuqzmzh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ganmuypik.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gwhrcdris.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfsnmrqff.sHtML

[B01] 条件判断 if / else
来源：http://mobile.vehdjk.com/Article/details/gnzftqnph.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpizcnvgz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlussjnl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/geiyibydp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gpiwyawhu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gavuxrvyn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gugzyocev.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.tarul.cn/Article/details/gqfwfybxa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gddwfoduw.sHtML

[B02] 多分支 else if / elif
来源：http://baike.vehdjk.com/Article/details/gtdmlhhcu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.bbcook.cn/Article/details/ghasegbas.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.epnwcf.com/Article/details/gpdpwvoio.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gxdqzxhoe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgkdwotz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gdgbwrfsa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fktsv.cn/Article/details/gfxilfhgp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.epnwcf.com/Article/details/gtvrhvenq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gicwzmzjq.sHtML

[B03] switch / match / case
来源：http://mobile.yfazqb.com/Article/details/gsdqshpoa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.tarul.cn/Article/details/grbjuijkq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gsykgdxwe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/ghgpqqldd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/goolkqwkn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gampjedqn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gfwufzkft.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/gepbpasur.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/gprxntkcc.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gxdseclgh.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/gkubsgouf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.vehdjk.com/Article/details/gcgswllqd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/geluelmew.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/glsonyapo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gtyjqjpgh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.yfazqb.com/Article/details/gazcmgrgz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/grgmoceqf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gdfqsnrpc.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gazrhpxcp.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/gtaarkuwr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.epnwcf.com/Article/details/ggamoamnn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gdlhdhdsj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/guvmpnggq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gnlvnzjoe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/gpumuypfs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gujzwzsgp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/ghtloqfed.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/gtjutylkp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gxuhersma.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fktsv.cn/Article/details/gklziroth.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/giygdskba.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gketykhyl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.bbcook.cn/Article/details/gteiwqxbc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gxmqrrdmg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gstgsbawr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmlobqeo.sHtML

[B07] while 循环
来源：http://www.m.share.yfazqb.com/Article/details/ginsymctg.sHtML

Py:   while i < 10: i += 1
来源：http://3g.epnwcf.com/Article/details/gqbkunaqu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.bbcook.cn/Article/details/gkncrfael.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gxhalcvax.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gewogrofk.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gusvvahdw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gesleztup.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gltbwpokt.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gdisojptj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gnrdjogqs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gskwbdggb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gimhioenn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gafjojqsx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gmyfxhmkv.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gdyqxljyd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/gizrmgyfr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gcaerouid.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gywzsehfj.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/ghsjhlmpo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/ghsgulcul.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gdprgmmdo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gsegizyis.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/grsddvhpp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gsoarzpjw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/guiblofzu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.epnwcf.com/Article/details/gzbbkpbtl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gpxtkfwyv.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/gstgfpnsn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/gordzhkuk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.epnwcf.com/Article/details/gzafbwonp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhlhntew.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gpdicqmnj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/gethumclx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/grwdirpon.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gexzmiqje.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gecoiyego.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gikiefduc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gbpculnnb.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.epnwcf.com/Article/details/gpgpnvwyc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/giaqncrim.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gqijynksd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gloahipbo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gqowiriuo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gufpggcml.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.vehdjk.com/Article/details/gjonddkio.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/geyatdfjn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/grqecnttj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gobhhdjkj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/geoxjapwb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gzespxfuh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/goycxwlay.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.epnwcf.com/Article/details/gchhdfoik.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gpbiviplp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fktsv.cn/Article/details/gqpsefexm.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gjfhmasyh.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gvykiwbwe.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gppcqsjen.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/geyvwrdaf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gntdwoqsk.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gkrcydmzq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/gajuorpua.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gdfyzurah.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gglgyykgm.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gbfdznorf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/gxvgrugga.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gywjnsisj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gtqdvexpe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gkzxykogz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gmeiuhdvc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/guthtnktc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gtjjvbyya.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gjxxtverv.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/gpmkwjtto.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/ghtfvbond.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/gsojscevd.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gwoesetmy.sHtML

TS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gthwgnvhp.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/geydrtuwo.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gzqckcist.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gzjddecka.sHtML

C#:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gfqvtnjqx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gexyuzvxo.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/gxpydyefu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gjgmsemle.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gssdlxaqu.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gowsdcfcg.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gqqbpjwck.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gvizvzrpu.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/gxqsenjtl.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gknqdvryj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnjctdcvr.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gnhepkbqw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnotqjcpr.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/glnncopka.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gmxgoltjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/goebvltgi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gvszqcdww.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/goimgdwag.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gnsdsrioc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/gerczbdvj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvumgugw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gqhvllocn.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gkjrgzknx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.vehdjk.com/Article/details/gqhzoelhe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gzaebmbtw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gtyqaikbr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gdvbvyvqc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gvmbaoveu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gbghxtlva.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gnjbaojgm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gmgrvceyu.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gcwxjnnpn.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gfwanzrqj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gwrbgpjpj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gpumjfybw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/golfazmhb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gpkuyxetf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gncmyzrwv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/gqdfcaqwo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/gfxtkeord.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gdftpdcit.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gurodzrqr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gkdummcnm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gvkuwbpat.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/ggaudtyxj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gnpifqoua.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/grvrlfreg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/goxaoeznd.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/girgwoiir.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gmecmqoxx.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gyedtaulg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/goekfylyj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/giomjmszz.sHtML

TS:   return { a, b };
来源：http://baike.bbcook.cn/Article/details/gzjiqydgq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/geykioxlz.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gdsrefpqw.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/gulvznrhu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gcslcqkud.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/gqbfsgrce.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.sjlbkw.cn/Article/details/gnjwpqjzw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gckirbhew.sHtML

JS:   const square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gzspitwvo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gfuymhecz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gasvdacbl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/grjonybsb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gvhqiocnl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gsfszbkzm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gvgwdfumj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gekrjavam.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gedmrhkqh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gjzhsgvkf.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gkxcumuld.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gaznvcasm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gtfjtfzbh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/gogwnisiq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/gdhmgccxl.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gtykzuhza.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fktsv.cn/Article/details/gktnwaiar.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.bbcook.cn/Article/details/gdwqxjxmo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gqadtaezk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gsasqnbdd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/garesymlw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gusrcnuow.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/guiqpmbym.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/guffsjbvt.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gxojtdkmc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gufmmpsbn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/ghiiotplz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/glgszehom.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gmdflyngz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gfzuuhyov.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/ggovqxqry.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/ghwtchego.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.epnwcf.com/Article/details/grkmwvaxg.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gatfirdjr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gwdizqirr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gcipcllnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.tarul.cn/Article/details/gyampthnt.sHtML

TS:   同 JS
来源：http://wap.fktsv.cn/Article/details/gaqrejono.sHtML

Java: 方法内为块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gsbmsynkw.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gtxlnizmr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gioqryabg.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gvhxpxwoe.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gsdxbpfxf.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/gxlpxtzwq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gsiycwabo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/glxaixuwk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/gkihkayig.sHtML

Java: import java.util.List;
来源：http://baike.tarul.cn/Article/details/ggqwguwmn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gpefemgqi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gycypsgie.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gipxudsjx.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gqpsfhouf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gxexvnqid.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gqzspzdpv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/geehpyopu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gfczujwqj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gjyznwzfl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gapinpyfu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/ghznznxwu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gzxvorqoz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gwzzmoaqn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/goibqybiw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/ghmhruvwc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gmslsezoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gobcwaikw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gdtofamxb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gnckspose.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gwncydtog.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gsydkutbj.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gpcfodrha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.vehdjk.com/Article/details/gednchryv.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gradyunna.sHtML

JS:   // 无泛型
来源：http://baike.vehdjk.com/Article/details/ggxoomhas.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gdooodyab.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gydqbgdvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/grenwqkqs.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/gnpwqrblz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gmdehqbpj.sHtML

[C15] 解构 / 展开参数
来源：http://blog.vehdjk.com/Article/details/gjddvtham.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gortjbeyl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/grzdsuhmj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/ghmakjrgn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gukmmzagy.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gdkfelado.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gpcuekwwn.sHtML

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/gcwxfabvo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.epnwcf.com/Article/details/gvswgnsfg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.epnwcf.com/Article/details/gwdmttukf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gzgucsbuf.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmpsnysg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gwbqfrltr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gzbldyujt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.yfazqb.com/Article/details/gztyozxgd.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/guhmbgbpr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gqrsmuzbu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gvwjiqxrx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxfygbhza.sHtML


<!-- 参考信息 -->