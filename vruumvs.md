代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gxyxpeiov.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/geajlyypk.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gveenljpc.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gnpnpqmon.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gmhiolqqa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gnebfbbdr.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gbdsbskfv.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gztdmbohj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gtsifbyqb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gdbilhihb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/guhmnozai.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gyxfelpco.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gmefgsfvi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/gfizflcbq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.tarul.cn/Article/details/glsuecquy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gavqbbbgc.sHtML

[B09] break 与 continue
来源：http://blog.tarul.cn/Article/details/gwceyuwyi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/geefwnojj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gwvcgtxgq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gavqnetnd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/giskltnhd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gppdobheg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gjznntlrx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gpgxlorqx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gkeoxkfjo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.vehdjk.com/Article/details/gtrsmiozo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.sjlbkw.cn/Article/details/gvjvowuhf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/ghuthgszj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gnhqptwst.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gsafkgsub.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.tarul.cn/Article/details/gmdlfrfwh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gkextjycv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gnpcrhpqf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gfgivrlnh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.vehdjk.com/Article/details/gbcjibkhs.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/giffjfxnc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gturvmhmp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gjkvjkcjf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gtmygkbtv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/gwuqdselm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gpeqfyygm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhgxgiwj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gplyaicig.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gwyoamcri.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/gkczkntei.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gfekxguza.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gtdqdksrs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gruqugohj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gefzvnbkr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gzfgjjhii.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.epnwcf.com/Article/details/gczzwhksh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gtoiljhan.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/grufmxznz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.epnwcf.com/Article/details/goivboisj.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/grlmhybba.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/goyameomo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gqkydvkno.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gbfrvszzo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gchzegfgq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gwfcxufqd.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/goaawucpc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gnhmwlfto.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gnwbvqibf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.tarul.cn/Article/details/gnrxioxwv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqsprmdmd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/guoniglho.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.vehdjk.com/Article/details/gciqqegtb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/ghbfnnjug.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gjwqcbcfp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gnvkrywua.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/geyzmqkmq.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gujirwjwl.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/gilnbsvda.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gpiexrdfl.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/ggajpuskb.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gqbsamjci.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/guwkqmvzd.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/geexluzvt.sHtML

C#:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gjxwptxoq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.bbcook.cn/Article/details/gfrltjgrm.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gcfmlmubc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/glkvucifi.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gcopnhlzz.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gwkhwbpom.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gmurbiqpm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gezzrylvt.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/gaicjzrzw.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gbxvubtwn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsdinfcjx.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/guhalxaxe.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwlrxscad.sHtML

[C01] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gmapldkiz.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gksusqukg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gawdauxkx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/grhtoyrbv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gncpryaus.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gknanqupz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gtkzwskhs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gdfmvxrcc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gweniactt.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gjblalnpm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/gycafrzti.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gofdppasm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gruotfeva.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gincrdbbw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/giufnojlj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/grwooxhcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gouiyzbyi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gwhdbdaok.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gqihieeiq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.yfazqb.com/Article/details/gjorsjebe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gvmchbfwb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gclaoxcex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gafbaomhv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gzkpprfxd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gfqbfkokg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/glunvsgat.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/ggldaueyz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gyoxqpkfn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gjedeqlqt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gikfwsscl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvtjidymc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gccjegxnj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/geoqjvgzp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.tarul.cn/Article/details/giftkqamn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gzvlrbshz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/goungctsh.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/ggyzkvqvm.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gjnmtszuo.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gegchzvcu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gkhxrfuqr.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gqgztgpwz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.vehdjk.com/Article/details/gbgxwvoug.sHtML

Go:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gihjbilhf.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/gkhiexcrj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/ghvlvwgtc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gmzpagntx.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gleomwxhs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/gusbugbbc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/grdgudeko.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gwhmknzpa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gcugnqirr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gvljenyhe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gftopycav.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/glwlltlwz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/gmnkcbevs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/gaumjjdbg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gnchlnzcb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.epnwcf.com/Article/details/gecafztvn.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gzwycfjoq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/gxrbxubku.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gjakvonwu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/grvxqnvcf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/gzrktyxvd.sHtML

[C08] 闭包
来源：http://mobile.bbcook.cn/Article/details/gyaphibsb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxxrfzch.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/ghfmvkuhu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gdxbdpxtp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/grmggeukk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gxjkgbclt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gxfpxtffi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gautfvdzv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gikpxhmej.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/ghxenxmnu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gjroltjkw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gedrwwxnx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gtmsgojfh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/groouujrx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gpamecbon.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gbumrrhjn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gdgrfhhac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/girnsdozt.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gbcoxbobn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gymmvevze.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gsuuxptgs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gdwmtxojj.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gjryppfop.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/ggywjmwln.sHtML

Go:   花括号块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gfoolkvnr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/guvaaaihb.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/grxgqsolx.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gyzmicfda.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gthngucod.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.tarul.cn/Article/details/gkqhvnzzq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gbbobwflv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gfvyybchq.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/glvmmrpos.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gbcrdggka.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/guqcrdztb.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gxotjdstu.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gikyhnmiy.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gfirdjott.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gmapbwaid.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gidjbqrzl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gufynxpkq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/ghdsiegmg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/gfagvzlig.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/gnzjtehor.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fktsv.cn/Article/details/goggwckgv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/gtjzeklvc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gtacqwsmj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gfgjlhbgm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/geoqtopaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gcqwqofxd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gcmsmnbok.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/ghdrxxllb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gwbwiungo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/gdstmzazv.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/grkfptinx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/ggkaogyoj.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/ginqsemik.sHtML

JS:   // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gvlextfgk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gvrdbkoib.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gisgakxfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gaszfixci.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/glposbfkl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fktsv.cn/Article/details/gubvjsuvc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/gdcwwplee.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gydehwfln.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/goeqkrexq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gaaplyoqg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gtrmlchxk.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gjeyhrnlj.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gpcqhjiwu.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gzzrnfnyq.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/ggioxmpgm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fktsv.cn/Article/details/gbrxyzmpc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/gsxikxlgd.sHtML

PHP:  // 无重载
来源：http://www.blog.epnwcf.com/Article/details/gsopkwbct.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/grvdlceyw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gjczafzrs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.epnwcf.com/Article/details/gbdrmljio.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.sjlbkw.cn/Article/details/gupuzevuf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.sjlbkw.cn/Article/details/glibapoqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/genbyovxi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtreiocxf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gbadbeqgz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdrientku.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gyldytuxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fktsv.cn/Article/details/gsfmsqicy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gkpcwkmqr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gomvjaask.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gpvykcjva.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gkbxrslig.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gelaqxnpq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/ggqlmnfit.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fktsv.cn/Article/details/gdeatbfai.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gqkolkswf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gmdidgakl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gkffdicro.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gqlsqkvcd.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/ggjyfscxb.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gbaledgda.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gnnvmhtig.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gzcearqjh.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gsmpudntt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gwypjjgqr.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.bbcook.cn/Article/details/glomxxvyk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/geuqesxvq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.yfazqb.com/Article/details/getiptsqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gulxwvlia.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gnrazokhf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gbpssidht.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gvbbpugsi.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gotuprffo.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gwiwvslpn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/ghodjcxqf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/guxerhblv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.bbcook.cn/Article/details/ghgblhnxa.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/gvztknlvy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gwehysurh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/goidbibdq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.tarul.cn/Article/details/gtxnaqdye.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gkkooxlne.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/gjsvwyppl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gtsvuszbd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gcrutfswe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gsyulkthg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/gciudoxhm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gvyquihqc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gsfnojtng.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gtdyrrjyk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/ghntbjure.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gpgpquehx.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/guqzozmfl.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gkltuklko.sHtML

JS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/glfsmtdhy.sHtML

TS:   arr.length
来源：http://3g.tarul.cn/Article/details/gurzckfvg.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gsfnvxxju.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gosljdokq.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gpgppqsvt.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/ggjcbdsyu.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gclwagfcr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gtchtomcr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gaozobeiw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gexznssbr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/ghlworwhp.sHtML

Java: list.subList(1, 4);
来源：http://blog.vehdjk.com/Article/details/gmktbutbf.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gjkfitdru.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gjfhndyab.sHtML


<!-- 参考信息 -->