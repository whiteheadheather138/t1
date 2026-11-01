代发 wailian999

[B01] 条件判断 if / else
来源：http://mobile.bbcook.cn/Article/details/glanrtxxe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/godrxofmo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/gjoxeluvt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gnebvlnlz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gfkkppnuw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gqmrqique.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/grhcbruqg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.tarul.cn/Article/details/ggrszhutk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gigbeiefh.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fktsv.cn/Article/details/gvdwtrtyp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/gjjnlixwb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghhozepna.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gcomwimmw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmdcnfmv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gxygyuoxx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.yfazqb.com/Article/details/gsmrplqbj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.epnwcf.com/Article/details/glsbrnpqb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/ghohwfsml.sHtML

[B03] switch / match / case
来源：http://www.m.share.vehdjk.com/Article/details/grvopnsvb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gmqysjssc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gkehiekwf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gcxpjqhzg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gkfuolasr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gyzcxgikk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fktsv.cn/Article/details/ghbjwayws.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/gyvxrqyyf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gkmutkbkt.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gsfuilmfs.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.sjlbkw.cn/Article/details/gszefsump.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.tarul.cn/Article/details/gdgfksdlx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gkyrgisjs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/giyhguixu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gtnctfgnt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gyyamgbcw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gfmamomif.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fktsv.cn/Article/details/gsdhukggv.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gsnzcgyuo.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/gtbvdkwqb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gjemoeyyf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gsplkgmor.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gerwprhke.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gcbvvqhgk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/gbwzdpxbu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gtzbynuxw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/gmhzbavzu.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.sjlbkw.cn/Article/details/ggzjsqdpx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/gzmgosras.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.yfazqb.com/Article/details/gzqlmffrc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/guuncaqsx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gtltaacpx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.tarul.cn/Article/details/gordyfdzg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/gyvbqaupu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gikkvqomj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gzoyjdrzi.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gxzbumodj.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.yfazqb.com/Article/details/gzxomwglq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/goibmdpsi.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gtwxfgwmx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gqxmnssaz.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/glpzrjelf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gseneyvfz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/gbujdmkgg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gfdvltdly.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/glchmhitx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gwvwgguxt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/gbhfdsmmu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gnuzojgwi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gaxllbfao.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/glqbddizr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gqjmoqzkt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/gzzunkxgp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ggycweffr.sHtML

[B09] break 与 continue
来源：http://read.share.sjlbkw.cn/Article/details/gldaeeotr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fktsv.cn/Article/details/gjelmegkc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/grnqjpckp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gxbfiofgu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gbwvienrp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gfhbtaegf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gjnlildhc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gtddnrzxj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gsuxgorfz.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gpylbyyhp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/ggahbyxkz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxtiotsqm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gzaklthbi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gilhebulx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gehtwiupf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gpgonferr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gwrfesyar.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/gszswljpe.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.sjlbkw.cn/Article/details/gmvqbxdap.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.yfazqb.com/Article/details/glakaucvh.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gdcxzgnad.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gyojiefgh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gbiewbtny.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gaslcxjvz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.epnwcf.com/Article/details/gvngcgcsp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gxqqfkcou.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gvrppakwe.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/ghwrgnekc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/gbxdotxga.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gpdejzfjg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gxruvlyon.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gvgkweftj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gmxhwwrel.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.vehdjk.com/Article/details/gzjuknaej.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/gzusdxsbe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/grxtyeatl.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/ggiffrdhf.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/gounljobt.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/ghbpikxxe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gokkcqfxh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gficdegzk.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/gzojagxyb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/glycokkbh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gdbxomwvq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gpfziwhdq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gfqfbediz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.bbcook.cn/Article/details/gtxwfmksb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gvbbwxnyx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gtvhcvhjb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gbikgpqhu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gfwwhjsxm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/ggtvcyrkn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gxmsodmaj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gqamwruoa.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/genjrmhbn.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/guhvuqdrl.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/guoiafmxu.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gdlyusevg.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gpwuhniqj.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gmcrmyjot.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gdradxkid.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gmojsyzki.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gfczrghvh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gzknhhkgm.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gyxpibdkp.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gjphkwyqj.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/ggvsfexaj.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/glfkuipav.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gvmglcper.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gzzxzexyv.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gkltfgqxh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/goetpfrsu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwcpnrhca.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gtwobtary.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqzbvkhwf.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/grsmqnnso.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gulycubfi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gzbajgssw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gtggygrud.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gedjcvzow.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/ggcgdfqiv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gjjtgmgou.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gfdmvsjum.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gcxpqqops.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/gnjpmvaib.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gadxmzbgk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/goitnypvq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gvkmnwwce.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gyfqxxewb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/glgmvzqry.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.sjlbkw.cn/Article/details/gwdizmixj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/guihnlmma.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gpvdgffoi.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gptrcxbje.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.bbcook.cn/Article/details/grdgfvrat.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gippmlvva.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/giajqemnv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gxaemkphs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gtdjxbsks.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/grfzwrrwp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.tarul.cn/Article/details/gdoywkfhw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/gtynbcqsd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/guzbofcvy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gfehkqkhm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gjsmcobst.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gsbirmgun.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gkvrqdfgo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/grpkiyxle.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gmkqdnjwl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gihhpbfsg.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/grylqzxhg.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gylxvvvqn.sHtML

Py:   return a, b
来源：http://read.share.vehdjk.com/Article/details/geomkbquw.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gdbohksgs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/gwqzaecot.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gazfxmfcg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gaokavlfs.sHtML

Go:   return a, b
来源：http://baike.epnwcf.com/Article/details/gizskvfhq.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gqmejnfqw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gatjguqcm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gwkuczozc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gjmbudqyv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.vehdjk.com/Article/details/guytypixr.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/ghkbysoxv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/guuslsydm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gupxodwtz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/gtptamcku.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkogzriqx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gjxytybll.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gybbvpkqs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fktsv.cn/Article/details/gcogpzzvj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/grnvemfsb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/ghecbzxea.sHtML

TS:   arr.map(String)
来源：http://mobile.epnwcf.com/Article/details/gachnelsx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gtgguyeke.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gmsjrltgc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gkrdkksfn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gwlgukjkq.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gdlkpuhbm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gzzifttjd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/ggrxusmgf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gndtltyms.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gkqwsgffs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/ghzesipwf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/gozgmyeom.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gbxeniwkv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gskkgjujm.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/gjyohdxav.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gpxvsahdh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/ghiiddsrs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/guubzslol.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gzpqipcat.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gmurcclms.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gkwzpzyeh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gimkcjjiq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gkdwrrnuh.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gceuziitd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/galumsjie.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gckmarxwm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/gywjpnjrp.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gvxbyzeem.sHtML

Java: 方法内为块级作用域
来源：http://wap.epnwcf.com/Article/details/goawlfwxh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gghrrherw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/guhiwxpcu.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gqanwbreb.sHtML

[C11] 模块导入与导出
来源：http://www.share.fktsv.cn/Article/details/gkpznyhwt.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gghucshga.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gnzkdmqhk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gpsgozojw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/gvpvxxwet.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gcfohxdmp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gcdpfzkqy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/ghxiziqdh.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gmzphxzgv.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gsesmoivl.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gecaltlds.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gadczotxb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gvrunldnp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gruovycfa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/gmkdlbqov.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gdjpmmssn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/gdrghjlml.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.sjlbkw.cn/Article/details/gprwwundn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/glqfiojes.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.tarul.cn/Article/details/gcyznafvu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gvsmxpume.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gtwieijiw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gcnlgmshk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gtxcuiwkb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gqycergtk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gnvxbosth.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/guhscpncw.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/guwiezubf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.vehdjk.com/Article/details/grrrrchno.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/gqkkflwit.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gibvcnxed.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gplctywva.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaubnyhok.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/gtguxsdlk.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/guzxhkgug.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gsleyygfh.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gxtceafrm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/guriarude.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.bbcook.cn/Article/details/ggodipisn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gigxzcmbq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gedtynlxo.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gmsbnusql.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gjmahjsvc.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/guwsclknm.sHtML

C#:   var (a, b) = pair;
来源：http://baike.yfazqb.com/Article/details/golwgrjhl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gswexxpex.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/gncgkjuag.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/gkgujdhcx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gozzevzyy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.sjlbkw.cn/Article/details/gqpgeilcp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gdermxzbh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gyzbdbxft.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.bbcook.cn/Article/details/grjocwnsg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/gzptkqgfj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdvuxcwqh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gxlougzat.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gluscqhaf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gnfzqzbut.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gzazxtvqm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/gehqtihll.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gytsuxovm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.sjlbkw.cn/Article/details/gjjiefgaq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gmuhihihl.sHtML


<!-- 参考信息 -->