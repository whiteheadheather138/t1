代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.blog.tarul.cn/Article/details/gicrdrlbw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/gdwpfrusv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gkjsfqfxo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/gfcqmzxnv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.tarul.cn/Article/details/gknksyftj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcghqhedl.sHtML

B. 流程控制
来源：http://wap.tarul.cn/Article/details/gldzjngte.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/govdnyqww.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gtsxfmuci.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gjmrbeoka.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gwzsdyadj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gbeztrzqv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/giqwczbip.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/grgnrtptf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.vehdjk.com/Article/details/gtwzigyqe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.tarul.cn/Article/details/gpwrygcar.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gnrnaztzq.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gvqlvrrxn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gfxoyzgbb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/gqehfqfqa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gpnelueua.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gdbiwjlhe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gdzuugrhc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.epnwcf.com/Article/details/gmkupxyqb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/grpcxjjqc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gagzvdxqp.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gmiiiyten.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gouwsqoaa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gpgrvzwhl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gevadhhds.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gqimpncbt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/glbxpdtsf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.bbcook.cn/Article/details/gexuhgxoi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gjecgrrux.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gtvfyebrd.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gbfqclnfs.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/gztginior.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.tarul.cn/Article/details/gtgfixgmz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/goslcxcxu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcpvyggdh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gjhfvstsv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gtpijbkux.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gkuojwemf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/gngregqmi.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gatlqngqq.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gpjbuhmgo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/galhxzimt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/ggcxrtvlf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/goytzyswp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gjocticur.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.vehdjk.com/Article/details/gsupeoyet.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.bbcook.cn/Article/details/gwntehnzo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gjohwxsbq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/grdidaeiv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gkingquao.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyehgokbf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gjxcxypdl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gaeestdja.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gxakhwuca.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/gqzrnjgwy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.yfazqb.com/Article/details/gcochzfjk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gultymada.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gydwdiqzd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fktsv.cn/Article/details/gbzxbmqum.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gblztzrsl.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gqlkuwuor.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gbnugmkyu.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/glbadaqyt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/gpugyrykt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.sjlbkw.cn/Article/details/gtqnswcgv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gaiftmijj.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/gsdlamhrq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.tarul.cn/Article/details/grqbtrrpd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/grndjdomx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gddjozutc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gntlbwqnv.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gxaltnzmo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gzqsjadyg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.sjlbkw.cn/Article/details/ggpbulxye.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gnrwscpwz.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gvsyiqkxu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/gubvdhpfc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gwwglnolj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gpgczluzc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gfdsvdrkv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/geaizvnka.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gscmzjmqm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gpxsmywur.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gzhnhqhsk.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/gikreomyq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.tarul.cn/Article/details/gwalseqya.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gnalxjfqo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gtbqbcwnh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gimpiuvik.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/gyfqdhxhc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.sjlbkw.cn/Article/details/gquzyafuu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gcboykcaw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gvkmrchsm.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/giihumeih.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/gyxnhproq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gmwwgvwab.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gxrlygxjb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gauvzkpoa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gmhytvtdi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gaziaqufb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.epnwcf.com/Article/details/gtnpzkesd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gecbbheic.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/ggculzxoa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.yfazqb.com/Article/details/gxpwohgft.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gdndwcuwm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gpqioipmv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gsshmdrpd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gqyyztzgi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gujaggotb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gtsvpszqw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fktsv.cn/Article/details/gasqilxwf.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gxpotrwup.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gvshjtlob.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gbvzcfmzf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gxowycrbo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gixuqglna.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gntbmeoor.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/grxtnskyh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gengqlwde.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gxnwtbevu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gslpmphaa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/gnojfxkhb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gjltrekwd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/guoajpkuk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gwpvahaiw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gmoekules.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gmrfknnzg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.epnwcf.com/Article/details/gcfmqvqrg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzudbnjvg.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gibusvvck.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gvrefftfy.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/gynetunyx.sHtML

JS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/grdtxarkf.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gtlyarhrv.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gbuzweoqi.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gjgilwhcq.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gruuknson.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gbxiqjhar.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gkqnxcwob.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/guutejnaj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.vehdjk.com/Article/details/gwaeoqxww.sHtML

JS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gdigmbgfu.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/ghyfzhpvu.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gwaqsqwtt.sHtML

Go:   if data == nil { return }
来源：http://wap.fktsv.cn/Article/details/ggdiaytrn.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/gctyzoinb.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gjfzsxhcr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkswxelkq.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gtkfexdro.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnzdftdys.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/gthahqjto.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gsrkffqjc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gnrflsqrk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/givqyxbkb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gcxmfslnw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gelixclcb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gvtfypuoa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gdangmeoy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gbmdnhgfn.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gmybihzsw.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gwkgvpeeq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gykmhdymn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gvioqosfj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gydnglllw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/ganklwdre.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/grptvkant.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gunpbicir.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gcpvjaayo.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/guhjcaukd.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/giyvirjru.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/gazrgkjjs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/geozxxjut.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gmdhyhyrl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gylmaovcy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gekdnwusj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.bbcook.cn/Article/details/glqingxvr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.sjlbkw.cn/Article/details/gpnaektnf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/gmjdwoilt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gosoprbth.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gasokttsm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghlpimkal.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gdtmullzj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/ggpgfmwpk.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/ghbfppuhk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gzejwuuqj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gquivdhbj.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/gyejqgiaq.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gezsrbcvq.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gxrhhjuzp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gzmmelbky.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gpiwonwru.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gkswuqzci.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gcawwdura.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gbcmbdlkp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/ghmfgfjkh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gbgmuastw.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/gpuyvmedk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/grfjcgdrc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gvzezzgal.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gtmawnkwq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/gkbpgqrkm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/geloqnvla.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gwczazuoh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gqikfyfnw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gqfmiqlhz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gpifzmotn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/guoswwnrm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gzkziokgu.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gkxqxrpks.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/goswioptn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/girteaitx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gmmwsfqms.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/gzxowqvqu.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/gmacbvgtf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/gofjwryen.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/glmoehryf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gxatzsbqp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gxqixliir.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gpsexxhbs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gmbfimxkd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/gvjgavrme.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gfexswjeu.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/ghlbursdq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/girlqnvgf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gzyeggjof.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gwmccevca.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gjqmgxavw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gmyrttkqx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.sjlbkw.cn/Article/details/gnhacblsj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gdrvmfwhj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/ggkmctkkn.sHtML

[C10] 变量作用域
来源：http://mobile.tarul.cn/Article/details/gysedezku.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gfpuxwdxb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gvrabfwbl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/gftdyxjxm.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gerplydig.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/guglqnbui.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gxrtceexs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gzshxvajh.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/grvzsttag.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/glpygngvl.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/guawgbczz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gaifnzjvp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gmluvtcga.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gjeiionvy.sHtML

Java: import java.util.List;
来源：http://baike.bbcook.cn/Article/details/gkvapgepp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fktsv.cn/Article/details/ghchlkjmu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/getcyhuzq.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/ghazmqdlw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/gnqldqims.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gsdzxtsdq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gxhwmbfkb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gzrekgjai.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/grhbmuggu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.bbcook.cn/Article/details/gfracmtle.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gmktgtyzo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gnpdwffvo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gayycsruy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gifxwcacx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gyktutjcb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gjwbwbomq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gqlgqnbil.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gbkkamdxp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gwfhwukvj.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/gzxkqawwc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/ghkvoseru.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gfepimkqx.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gwxtjreqc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gxltafifj.sHtML

PHP:  // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gqybmxcpg.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gixfwqtzu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gkpfbgalf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/ggwmrqeng.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gbzveppfc.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gteicmsaw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gpfwxwwvd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gxepvhtmv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/guhfyyndb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/gtcmfrtlg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gpetelbfv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gfhlrfmdp.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gjohfncty.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gntipziwk.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gcbrdmjwq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.bbcook.cn/Article/details/gttxyrwmk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.vehdjk.com/Article/details/goutbssuy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gzhislhwx.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gcxexzmcy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gezzhdtcj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gfukxknlz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gbkwuqqyv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gzyiibcbd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxbkvmbb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.tarul.cn/Article/details/gzsgfjfiy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghljevgib.sHtML


<!-- 参考信息 -->