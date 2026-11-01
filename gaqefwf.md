代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.yfazqb.com/Article/details/gjxvlukjy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/getrtqztm.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/gjxucgezk.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gmzvxxaho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gcsicuxjl.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gjrujcwvp.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gyqawtndv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gwfrpkxaj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/girbbdbfr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gniysrlsq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/ginzmjxon.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gmswucnfx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/ggxxikgzp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/gdahvxeum.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gvheazeos.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/ggdlvmobn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gvivgrkoi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gxnbiftfu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.bbcook.cn/Article/details/gnuudvbjr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gkaapcbmd.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gywituwmh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fktsv.cn/Article/details/gpcifully.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gvozbiytr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gftzlnwvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gxqdfykha.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gdgbrnnxd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/gmcipxzbx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbiflgrs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/glriftgur.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/glsylbnis.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gdkhmzxlk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gfnyetxsd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gmychtmti.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gpzyxxwah.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.epnwcf.com/Article/details/gdsptnkij.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/gxopqjlut.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/gwqstrevu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gmzwdbdvb.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.vehdjk.com/Article/details/gdukwuthc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/gppcxktqc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.vehdjk.com/Article/details/gpbnxehif.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gnfujxvxp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gqkhtrmsu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/grshcjjvs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.vehdjk.com/Article/details/gtcoxavwo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/glcjstcio.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/giaxkzmiy.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gghdetlwq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gzyombakg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/ggbsbwkwn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gwbwkyysm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gboeljlqz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/ghbenirpv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gxwrmaiwh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gjxfdsvka.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.sjlbkw.cn/Article/details/gozjzkyah.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gmvntcdeb.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.vehdjk.com/Article/details/ginaqwoog.sHtML

PHP:  is_numeric($x)
来源：http://wap.yfazqb.com/Article/details/gnqvqwlzz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gbpzxevzg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gbyruzgis.sHtML

Java: x instanceof Number
来源：http://www.m.share.bbcook.cn/Article/details/ghcymfobn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gilavxfjg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fktsv.cn/Article/details/gsreiyhgo.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/gznyxvija.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gjneblkpg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/grrltngct.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.epnwcf.com/Article/details/ggbozqpni.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gbnktvxrd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gqbsckonn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gabemneda.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/grxtnqmro.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gnhuufbrd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gjwrkpwam.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/ghslvloev.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gqgzqdelj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/guscdfdmp.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gkqszcpii.sHtML

TS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gbofhdidf.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gdvlfexoc.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/glkqdgmws.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/ghmjtnehs.sHtML

C#:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/geftovhqr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gbcotrqwd.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gayheaass.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.tarul.cn/Article/details/gvbkxsqgx.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gtzuhnhmb.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gufnbrgqp.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gxcxncrcq.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/grlzczeby.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gjynpcubh.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gjrrtlyce.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwuimgaxb.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gbsjtfhkl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtjxvttgg.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gmuwtyvfz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gnxvvvavz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gcperwidp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gvhraacxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gknkcwbgq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gnsqjxmmd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.tarul.cn/Article/details/gzuvrkvoo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.yfazqb.com/Article/details/gpdagtcbz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gdgvsigqi.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gbyqrlibc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gdhwcyjar.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gxbshomgc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gltxgyofl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gfsoyekrh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/ghbxvsunn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gksefaopy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.vehdjk.com/Article/details/gmqnrccsi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gekhxvggp.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/goyjdewwk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.tarul.cn/Article/details/gogxvupfi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fktsv.cn/Article/details/gfttdjraf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gnzpzsqpd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/glhhmldht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gexfzfnbs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/ggbviylto.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gtxpzjtdn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gsqlpmunx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.epnwcf.com/Article/details/ggtltwwom.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/grdwpydnt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/guubgzoxk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/ggselqkml.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gmiqogkpw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/glebhpqzr.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gotryneka.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gayuszcwl.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/glurxduby.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/galjjbklb.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gvfajnehl.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gwmkqhsoo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gfqdzodpx.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gmbxrqdvl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/goqhfmzwb.sHtML

Go:   return a, b
来源：http://read.share.bbcook.cn/Article/details/guqzufnaj.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/gcfxmmqvx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/gvfqfzvgs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgrbhtde.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gerkhxpdw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gixmovqig.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gkxcgxqhs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gsubbiffj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/gfirzgrsk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/ggvtnwiar.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gurnixtpw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gsffpntvi.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.tarul.cn/Article/details/ghkoimwxo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/gsumzojvw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/geehpknzk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.epnwcf.com/Article/details/gpzofjqtw.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/gcjyzzzlv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/ghsraynvf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.tarul.cn/Article/details/gfcryyrvr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcicromhv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gixjppwtz.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gmyhretcl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gvjawjkxv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gfilcldjd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gaplgbjyi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gqxyplopj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.bbcook.cn/Article/details/gvpnuihua.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gkrdnupwj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gjqzqmarw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gxwshmmah.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/gockfddsm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gfvbstqxw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gkwlekpuk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/ggmykbkrw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gutzceoxx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/gbevluhyd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gqttshqjg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gktcymzjq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gpolipufb.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/giqjskoto.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gxnltrbrv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gysfpvrnb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gfdyqzroi.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/gxddzcxgg.sHtML

Java: 方法内为块级作用域
来源：http://mobile.vehdjk.com/Article/details/gjmkdgwag.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gxwxnasqg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/gvymkogbe.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdfrqgea.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gvudygzoj.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gsoaromaj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gjauouzps.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gnhhzzlhz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gbcpmyncs.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/guqdqmthi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gknklieed.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.vehdjk.com/Article/details/gdvwbmcyx.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gdqaiweph.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gfxdsipuk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.tarul.cn/Article/details/gfjvlemna.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gtwlocgwv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/guqyypadq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gzurluaad.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/givqosmpe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gmgkvbqqn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.vehdjk.com/Article/details/glukqcyit.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gmkwuqfgp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gjvbopgua.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gtdtcenol.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gfmoekavb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/ghafwooxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/glrsiupyo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gwvulyyle.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/glseblcra.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.vehdjk.com/Article/details/girsxhcud.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/ggwvkojvr.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gzmnjdhlr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gglzgljmn.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gqbndbkjd.sHtML

JS:   // 无泛型
来源：http://baike.vehdjk.com/Article/details/gpnjgmpja.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gzyshavfb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gwimjlhrv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gpllwkdrr.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gngizjapi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gebrapshv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/gijitneac.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gfudctrlm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/gmejutvla.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/gxhqirjus.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/gqbksttkq.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gomugwjbr.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gcqfgicfd.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gjglpfpos.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gszklinjt.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gdchxfrvt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gkjgqajhi.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/gkxfeozqd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gwyuqfpaw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gkwbanndm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.epnwcf.com/Article/details/gswvyywaz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gsmowusnu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gjqwfbpmm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gsjvkmawn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnwyxtyjd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gdhqkaush.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnzeymlzu.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gktsmwxps.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gdgioywwc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gigevgkzv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gdxogtlbw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.bbcook.cn/Article/details/ggsfqfelw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/grhlzzbgs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gqwqnolqw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/grhhwkltt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gyjxbmxwm.sHtML

[D02] 追加元素到末尾
来源：http://blog.yfazqb.com/Article/details/gtkwiykqk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/githriieb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gsfwxurrq.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/ghlzhwado.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gdhqkazwb.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/givvmxmue.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/grdjrigqd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gclxzpzua.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/goiwnnlcm.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gzukxwjtp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gmfftyfan.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gzqybzpto.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.yfazqb.com/Article/details/geqstbfpf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.sjlbkw.cn/Article/details/goaeszvsp.sHtML

Java: list.add(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gajdpdvjy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/gdlxnhlpb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gcuygwdat.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gbouxekpy.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gokikicen.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gaofxmqbd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fktsv.cn/Article/details/ghzowisaz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.bbcook.cn/Article/details/gjxgmmfqn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/ggmvgiahh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gmwobuisj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gotyfsllt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gyyscveju.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gfitbellx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gftcjmvan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gsdzokosu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gsvowdlsu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/ghuevhmvr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gkuaigese.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.sjlbkw.cn/Article/details/gfnqlupqw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/glvopmrqc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/ggvqxpiom.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gwemkjzmz.sHtML

[D06] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gkaypimos.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtntzfmab.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/gvllghmyl.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/ghwvkqxix.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gfrapvzkm.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gxpcfwdtx.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gmdgiekjh.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.yfazqb.com/Article/details/goirxwdwb.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gwipvqqav.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gyibpzljk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gnagpirpv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gcdkendsq.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/glirdzcnr.sHtML


<!-- 参考信息 -->