代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/ggrxfddhl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.tarul.cn/Article/details/gftuewtan.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gzqcplrva.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/gevymguzz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.vehdjk.com/Article/details/gjtxoaixg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fktsv.cn/Article/details/gpkqicfyx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gdhhnwftm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gyzxmphfc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gfvsgwyjg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gmgurhixy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gphzoegca.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gcwsqkdql.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gaoljlbgs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/gbrmjnkfu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gpbeizxlg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gptxqsmvm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gssdzuzvk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gyyfracuo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/gbippooqi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gxilmuden.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gcqzfqota.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gdrkijpzv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gooqukdnc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.bbcook.cn/Article/details/gleutjwyy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/gjdvernse.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gtkjkszrm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gudoaolzh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/gddyqvhqf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gexzpsbmx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/gteqhyjoa.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gfmqytwlz.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.vehdjk.com/Article/details/gqtszmqkq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gilbnifuz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gqbmtmllo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gkpqtmuqb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/glfpjqlyk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/ganqljhlr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fktsv.cn/Article/details/gpjoxgitf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.bbcook.cn/Article/details/gmvjwegsr.sHtML

[B12] 跳出多层循环
来源：http://www.blog.tarul.cn/Article/details/gyoelryca.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/gcdozvflh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gxyqbkzac.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gjgnrehnw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gltokjppk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gkjhzybnr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gfbebgfmx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gbeakhkmh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gnmbledwa.sHtML

[B13] 判断是否为数字
来源：http://wap.sjlbkw.cn/Article/details/gcgoarjlt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.epnwcf.com/Article/details/ggwnakyua.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/gkvklqgiv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gtpwmffnl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkfkwlcvp.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gvdmwobom.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gjblkpafl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/ghxjdxkci.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gqulxcpxv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/gmuaflwrc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gtpdigkrb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.yfazqb.com/Article/details/gifkrhvww.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gnqakpyih.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gcqujoagf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gsnjjzreb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/gbvcjpifr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gwtrznred.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gdxkjlxbe.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/gfneszmcz.sHtML

Py:   a and b or not c
来源：http://www.share.epnwcf.com/Article/details/glqdhkosc.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gjdgqgopc.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gvkptbbfl.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gwesgahcw.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/grquzahmw.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/giwsxkuhm.sHtML

Ruby: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gepzwxlys.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/glgcapnpy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gzlopckva.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gvtnyhryv.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gdadrehhl.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gfwckxryy.sHtML

TS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gmizgfyer.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/glgajyrhj.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gmgwpdouk.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gialunflg.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gtjbknwhx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwpbmykha.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gseqhvgjg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmlsrnybx.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxfzouekp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gzvjgqcbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gfkcepdop.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gzgtxrwin.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gqbfvovmh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gockgetlg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gnvuhqfqj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gujcimmfu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gasbchtdq.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gzfowsctp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/guayzjlvl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.tarul.cn/Article/details/geobulvsg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gzixyyhbi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gkjveupgv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gqemltbbp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gyvoxxqus.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fktsv.cn/Article/details/gnsbffaxs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gykibrdah.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gmglopshs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/grxprjjwb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gvqauzdxg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gvoxscjyb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gfgqoaise.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.epnwcf.com/Article/details/galwnfmcx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/guyzamrop.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gwkisuzrj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gzoatnodz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/ghdicvacm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gabdyqqcv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gvhoeyllf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gassoielq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.yfazqb.com/Article/details/gupzgfcgg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gloljxxbl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gpwnnjtlk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gxasjplpj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gsdpphsyw.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/givhdjvmq.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/grmxlhqmr.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/grlhjqeie.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/grwahdudy.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/glxbeyors.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gsdvtzkrk.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gizibgplt.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gqnzzihek.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/getxikhlv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.yfazqb.com/Article/details/genccujkl.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gcivgbmii.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/gqxzhouts.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/getoemjey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/ghdjhfhay.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/glzsrrhan.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/gcuncvmnh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/gdfvihapq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gecxprpoc.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/gkrqyjhen.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gfdexelaq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gwnrnnkzk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gapaumffq.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gfpgsusfp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gofkjazot.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.yfazqb.com/Article/details/gdltjlgot.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gmfzslkba.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gaqsqblil.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/gpiuymdhf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/gbnlmdphv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkimtykp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/ghkeeioeq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gbnrtbrxk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/grgfbprij.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqhetugnp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gvdzyozwc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gannyykjs.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gtbplwjlu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gfyzmedeq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gfndklkzz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gagluijyh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gxcoffbwh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gjtngnmpx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gxgpuwvxs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gqqdiztwy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/giktpnfvf.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/gyhebgxgx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/gpdaxjbtr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gceuiycil.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.sjlbkw.cn/Article/details/gklepatyc.sHtML

TS:   同 JS
来源：http://m.share.yfazqb.com/Article/details/gchumbzow.sHtML

Java: 方法内为块级作用域
来源：http://wap.epnwcf.com/Article/details/godaxljdd.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gqdrlcrgg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/glxbdirql.sHtML

C#:   块级作用域
来源：http://blog.epnwcf.com/Article/details/gvbqdwqph.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gdptwjzov.sHtML

Py:   from module import func
来源：http://3g.fktsv.cn/Article/details/gymhxbacg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/gdswgczyp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/glutfknhw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.bbcook.cn/Article/details/gpzuvoujg.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gojulghxt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/ggymtmdfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/guelrveqt.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gdloypntl.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/gqxilfnzs.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gbcfljbbw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/gvettwkng.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gyibpaiex.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gronqorjr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/giwshlida.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/ggsiyuguj.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fktsv.cn/Article/details/glrhujnfm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.bbcook.cn/Article/details/gdrieowri.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gxohmwsvb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gfsfiknah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gzqyvysrh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gylzvusjf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gouxjefyb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gdzopjxid.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/goctztvmp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gfojjhjfj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.bbcook.cn/Article/details/gtbrxwdml.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gteezjzaf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gzywarnlf.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gmiquieiy.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/geadicvua.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gdxrkjltv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gqipblirq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.yfazqb.com/Article/details/gphatexiu.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gcwytmtuc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gpnitdmje.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/glhzqkdbe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gxofvithn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gghtjetux.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gihompdah.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gjfvzmznc.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/grukcwjew.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/guqikyenk.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gpdsruakq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gwhncennn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gsmwppjhy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/ggptutfrg.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gcvbopqht.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gehllmwna.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gnnecliaz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gjhbnkssq.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gewjnldim.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gekimacub.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gwnfbjwkb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grbiwgkeb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fktsv.cn/Article/details/ghlbmjahj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gabedqqpt.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/giaxoqfcm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gmmfvrlkl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gaaeuvljl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gfpugnuzz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gcsaepcrh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gdjnkwxkx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gmghkuxcq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/grfqkalye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gywxjszdu.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/grtvthlfs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gvrxyqjdx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gainrerun.sHtML

JS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gvpbzjcbw.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gfdztuwrs.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/grpgnwzsq.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gaxdermgg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gahlmjeyq.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/gdyyslbim.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/ggvthcurr.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gnkjgnlcx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.vehdjk.com/Article/details/gzpxkouzn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.bbcook.cn/Article/details/gwrrxjdze.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/grhxbjrbr.sHtML

Java: list.add(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gepznceql.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gvcosfkme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/gitvlkrmu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gvvwhvxhz.sHtML

[D04] 删除元素
来源：http://www.share.vehdjk.com/Article/details/gumhwngsg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.epnwcf.com/Article/details/gnumnjbsm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gksfujcwv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/guwxbkzbo.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/gawswfxvi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/grpetlbzh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gggpqjcme.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/ggqgwuycs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gzvzmixdx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gcoyajtig.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/glsvpcmtc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/glzfuycab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gbsqkinlj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.tarul.cn/Article/details/grspkyuxq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gkozmcnsu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/ggmtgnevc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gyxxrplbx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gcsqjreuv.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/glhhphfzc.sHtML

Py:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gksfesuou.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/gutewgpuz.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/ghfxzmbxa.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gqhpdpqff.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gslinmrfp.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gumjpnfnd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gpduvjwaf.sHtML

C#:   list.Count;
来源：http://www.share.bbcook.cn/Article/details/gktriytsm.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gcfnvjkvs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/goaptphmt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/gcmzjorqn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gcqeydcpp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gwloxrpsz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/godfdfvvq.sHtML

Go:   arr[1:4]
来源：http://read.share.yfazqb.com/Article/details/gcuydvets.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gzzycjnqj.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gjkedvbvc.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gtvwnabda.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gwwvfdaef.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gxuhelvhl.sHtML


<!-- 参考信息 -->