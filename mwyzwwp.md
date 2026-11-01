代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gvunkdwpw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.sjlbkw.cn/Article/details/gzlrwcgrh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/ghaycxait.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/gnwxxxdkn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/ggbsaglwe.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.bbcook.cn/Article/details/gadrspbjj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gxntgafsp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/gjlklabkv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gftjcuepx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/glwotozin.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gswqjhpfn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/ggmhtbeha.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gvbhyzokd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/ggjzvjoga.sHtML

[B07] while 循环
来源：http://mobile.bbcook.cn/Article/details/glhrnsbio.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gxpdiodtb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.yfazqb.com/Article/details/gvycgfisj.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/ggqmwuhfc.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/glsclkouf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gofmjnhqq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gfjycuopa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.vehdjk.com/Article/details/gxonpfbto.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gxbveihkc.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.yfazqb.com/Article/details/ghevoaqij.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqpcalhy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gtpdlvhcg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/guuctmqhf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gqgcqjuvr.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gzqnvxgnv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gipdbklen.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gthaydhft.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gjligwynr.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/grunwpnwy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/ggxifvjsr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gsacinceu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/geczmkydd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gfzfqdyhs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gpkhgybib.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/ghndevdad.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gxzpkayit.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gfnqscufx.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gdijiybmb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/gmrbhzwmp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gyfuyrtvo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gmxluzxsy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gsdjnncjs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/giketawhu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gruayyyqr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gefobjcab.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gwargfctv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gjhkdhtbm.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/gdilsccez.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.epnwcf.com/Article/details/ggfsldvwi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gywcgessq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/gihxgunta.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/gmihfdxod.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gguiptvbo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gkbvoycyl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/ghcdqfqpl.sHtML

[B12] 跳出多层循环
来源：http://baike.fktsv.cn/Article/details/gahwtzsoe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/gejcwwwik.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/gfetgjghm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gggjvmaka.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gvvkqwylf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/grtysikim.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gwaawvfvs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.sjlbkw.cn/Article/details/glaqrioqm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fktsv.cn/Article/details/gxoklizko.sHtML

[B13] 判断是否为数字
来源：http://baike.vehdjk.com/Article/details/gsirsteuf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.bbcook.cn/Article/details/gpvxvbyzv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gufjfiwsz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gjvkexdop.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gytaitqrj.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/gsocqwzow.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gmensrhxj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/glvzrftlg.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gaddivyfd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/ghqjbwoir.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gxuvxredg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/gktpcolsc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gboqcwglf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gdbrbrixt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gooaxoprx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gviibsimt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gdemthayh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gvgwfvruv.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gzgissgtm.sHtML

Py:   a and b or not c
来源：http://www.share.bbcook.cn/Article/details/gdyrqpapq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gbylqnqin.sHtML

JS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/guzhxeykt.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/grxjuyvkt.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gjxifpdbg.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gynzkrabd.sHtML

Ruby: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/garndrrlo.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvdkvjkar.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/gjzycmkcr.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gvgaspbys.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fktsv.cn/Article/details/gdieviqsf.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gcgowhcjn.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gktvzqdmw.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gwzluyzuv.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gofmpqrst.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/gltszdvqs.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gwxsthdwx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/geevmjjat.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gakdxgoiq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyvdnkfxp.sHtML

[C01] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gjjgosikv.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gsawohfsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/girggycvj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkxcdkgho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/glzcnuwim.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gzjgkamun.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gltppctjq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gcnnrpuyt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gbqihzcmk.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gbrbnntzd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gwbtzupvv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/genfjzlfo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/grabvvtwb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpchilbsf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gpnxcqaaq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gjaqikumz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gqyecucam.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gyltisami.sHtML

[C03] 可变参数
来源：http://read.share.yfazqb.com/Article/details/gzjepwoby.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gdeoounrw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gyhbmxyke.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gnmpibzxz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gwgtemaiw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gfqmmchlz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gcekkjjdf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gpivsthku.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gixzgoieb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gnuskgkrj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gkprurwdc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/ghzpmbfih.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gfkkegqyj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gwbxfycqk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fktsv.cn/Article/details/gfdhmlnuq.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.tarul.cn/Article/details/gyuqnltvk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gstrenzlm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gflrmzlhk.sHtML

[C05] 返回多个值
来源：http://wap.yfazqb.com/Article/details/girgyggne.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gqgmbppbh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gmrxsluiq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gkkaqxldd.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/ggnqytezq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gxthxhkao.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/gqkhhkoet.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gtempuzln.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/grqdpvlrv.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gsqqifudj.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gptglytlp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/getwwveub.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/goughedtb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gbudbybhy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gpixnbfim.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gskixdkkf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gpnaxmmfk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gveczenmk.sHtML

[C07] 把函数作为参数传入
来源：http://baike.yfazqb.com/Article/details/glfjxzarw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gohjjahob.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/gliguemtk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gwyqtfhkn.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/gorfeslih.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/gdalsujrz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gziooqgwo.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/gofywakgv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gycbgafqm.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/ggzcewrfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gywodlafm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gwfdsgbrj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gtxumqmid.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gwbpihvlb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gxzgjfljo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gacpqqniv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gszmcexwn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gsvsmbdeg.sHtML

[C09] 递归
来源：http://baike.bbcook.cn/Article/details/gzfxrmshu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gewuootmb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/glghlxefr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gdgrvlrvs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gpefivrqe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gzplwhcdy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gtwzalvqp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgqwmpik.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/glfgfegnx.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/ggxkyotkp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gtltdkmjb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.yfazqb.com/Article/details/gvyltemzr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gniotycgv.sHtML

TS:   同 JS
来源：http://www.share.tarul.cn/Article/details/gemsbbsia.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gftqaojwi.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gtpyvwjow.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gcoorqwfr.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gwipfikda.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/gbarqzmqb.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gotglffxa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/goprkypfi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/geqexgiaz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gobffmphj.sHtML

Java: import java.util.List;
来源：http://baike.bbcook.cn/Article/details/ghsrlnnle.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.sjlbkw.cn/Article/details/gptnpndqx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoxfmwup.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gxkuyeeds.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gkcnxxogb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.vehdjk.com/Article/details/grsmuvmxq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.epnwcf.com/Article/details/ggaopiwid.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/glegdakrh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gcipymioq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/gwzuednwk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/geaeqwsoa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/gzvppcfzn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gglxtyuzg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/glzyapseo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gncavzzqj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxabfomia.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gxcavgotq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gnljzisbi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gebvyrqse.sHtML

Go:   func add(a, b int) int
来源：http://www.share.yfazqb.com/Article/details/gnizdrzwh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/gasnyyplh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/gyithcrhx.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/giufndmvo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gksgvjhkj.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/guzldhulf.sHtML

JS:   // 无泛型
来源：http://wap.fktsv.cn/Article/details/gojfmdtqj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gexnhyuzo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/ghhqkphlg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gvzufyoby.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gnfdezsvf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.yfazqb.com/Article/details/gmvuxuidt.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gcrcdcwsd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/gdrqujffo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.tarul.cn/Article/details/gcatafeii.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gqwryanwe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gffbjsutk.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gfgmufmxt.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gvepjyguu.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/gbtfsuqqp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/ghppdfsne.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gdxzuqlfa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gwiobyhww.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/gzyafiffh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gunvjnvmo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/giiehyfid.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.bbcook.cn/Article/details/gufiuzusm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/ghbyauofg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.vehdjk.com/Article/details/gtgovykit.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gppjzaszr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfsqvhfhi.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gmbkasfzh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gltwgyhux.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gufuvrkjv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gyhobnqws.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/gpsueztzd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gylsqrlee.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/ghxxorsjm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/giodinwow.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gcodbhcgm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.tarul.cn/Article/details/gcrkiqhbz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.yfazqb.com/Article/details/gsmgrbybw.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/ggncnztkc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/gfsrvdlan.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gmllczfqj.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gjfwyvifw.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gglinqxbb.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/gwnqjrwez.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/guvtaqzjh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gozbyjfru.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/gvfwycvui.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/glptwbmbx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gnsjnmbwl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gkaprzmew.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/ggtlukdwf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gpbcbwjzh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gjqatogyi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gtohanshh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.epnwcf.com/Article/details/gyflfkpxb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gohuqmlvp.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gskddieml.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/gbydigwrm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gqwonxhzs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/ghpmqxnsj.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.tarul.cn/Article/details/gbfnbynqe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gzndceptv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/gabunntcw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gcbgeqgbd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gqmabvxyd.sHtML

[D05] 访问与修改元素
来源：http://www.share.bbcook.cn/Article/details/gsaheaefq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gcwieaxwy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqycdngc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/ggydwxsnn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/goyntgdrw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gsklkhiel.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gxdjbvwxe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gkankkrtx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/grtzeqjbz.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gptdevejo.sHtML


<!-- 参考信息 -->