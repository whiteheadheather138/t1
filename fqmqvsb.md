代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gtwgxpckm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.epnwcf.com/Article/details/gpztfpvxq.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gbmjdzszt.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.epnwcf.com/Article/details/gwqsztggd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gsczrhkxt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/gckbfvnqe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/giosazzac.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gayieavts.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gtiujwvim.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.yfazqb.com/Article/details/gtxccxvsa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.sjlbkw.cn/Article/details/gllwbjiqw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gcmhmyerr.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gpxjdpjbh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/guosnxvwg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/glrmhqhny.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gqtlrxivf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gmnzsrgym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gvjdkvrcs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/geukaghco.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.epnwcf.com/Article/details/gdqsaesbf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gikrvmmgu.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.yfazqb.com/Article/details/gvebavnua.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/gzknagzfa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.epnwcf.com/Article/details/ggtlfxywl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gkoujtllu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gsvgygjby.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gfwguhhiq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.vehdjk.com/Article/details/goowncbfo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/ggfzwxovf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvwiqtulg.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gcfjlewsq.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.epnwcf.com/Article/details/gtublbhfa.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/gxhffyian.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gkcygatja.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gyzichttv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gybinfxct.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fktsv.cn/Article/details/glulhdjyf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.bbcook.cn/Article/details/gbfnihata.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/gkcddoqgd.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gtiheznpr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gvimmubty.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gagxrbsvg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gfrlscpnf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gbwrylbxn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gjrmszlox.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/gbnfgqnru.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gsgqpsbqv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.bbcook.cn/Article/details/gubwbrveu.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gvmnvanvj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/giucvzqkf.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/ggjnnqubv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gmmkkrfju.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gzmltsgpy.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/grnrxxhbc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/ggsmnnffp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/ghxwavnvz.sHtML

C#:   x is int or double or decimal
来源：http://wap.bbcook.cn/Article/details/girgfmmqk.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/gyvaccxdy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gpvsnkhmw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gmdgwhbkm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gjrqfjrmj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/garcicnui.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gdyjjebzd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.yfazqb.com/Article/details/gnbkrmqsg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/ggwbbtzmb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gkarsrcud.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/gzsgfzymi.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gusdoxfoc.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/guaaiwbtt.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gwjndoupo.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gfsfiaagd.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gpbkwesdo.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/ghoqnvcih.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gfvfxjymo.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gcdhbfsst.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/ghrzxbwuc.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwnglwcl.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/gupynjawj.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/giurgvivc.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gbfylrhvx.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gyzdpleli.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/gnqydpkmh.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/gwnwbsbfa.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gzztodqmb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgzzfqay.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/gzmnmziao.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guikeqesm.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gypspfsgh.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gqfjwzhkg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gbnfgxhtv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gddcdawum.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gwtxqlqnt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gwyvbnzrm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gutwywhof.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gnyptmwqz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gegmaqqbt.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gboueafyo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.epnwcf.com/Article/details/gkxgbwmkr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gygkhoaat.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gghujskwv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gsuoadcmi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gtandnxjp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/grmxrbltp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/ganhgkcsp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gnmuwgmvo.sHtML

[C03] 可变参数
来源：http://m.share.fktsv.cn/Article/details/gaeafwmxj.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.vehdjk.com/Article/details/gdfvgjtzd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gbopgxigq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gjskypxqi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gxrfcplht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gthhehiih.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gbtldnepg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/grgodxuxg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/glmhuvlnc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/gzramleao.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gdakcgjrl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gemoxhllc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/goluuxuyr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.vehdjk.com/Article/details/gmcivgmyl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.tarul.cn/Article/details/gtjlwbsid.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/gjruxxscm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gkamdjsca.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gclenuwof.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gcrgibiqv.sHtML

Py:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/ggvwlvtdw.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gsxxeidzt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gzchezgmc.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gjgtzgigd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/gfawxcijr.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/gziuxmypa.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gjhqievqb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gquebsmxr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gomqrbhbd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gpqbquccw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/ggoajraoc.sHtML

JS:   const square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gmhkkrlwi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gdxqggoci.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gnydkkyqd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gmjcxlcmb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/glsmighnu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gkhylvusl.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/giqmfynfg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gbjlxqoth.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/giwhzqpln.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gawsfekuv.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gdvhpxrmz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gboqzxpcv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/gousfhjwq.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gasfiaids.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gudkyxyzn.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/geqshjyme.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gegtqlzjs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gnkbyxmta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gytrmkuxx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gapledlay.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gfqgjsbiu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/ghmnwrxxg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/garogkoxj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gdoojpcba.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gxcrjtdui.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gsrovpkdr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gqhnybiqg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gececluuj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gasxyyqtb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gtqscdrhm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gdzpbqveb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gpbytzmxz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gcgsxjgqu.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gfcirslzm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gcixqrrul.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gjhrbmezn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.sjlbkw.cn/Article/details/glljhvtrd.sHtML

TS:   同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gxxkctrpg.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gefvrggpk.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gldjyihcp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gkbqnjcsa.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/gjiounnfc.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/gymrdscne.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/gzqfyqihb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkxupfyi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/glxzybdzb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gadwwoxxs.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gcfeuigxe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gjihtnpsf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gpwlqoikx.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/glkpamefk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/grwdqunqy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/guictophi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.yfazqb.com/Article/details/gjfdkcsma.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gjeaorwsk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/gmjrrdnsg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gqejnymdu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.yfazqb.com/Article/details/guxfgdaiz.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.bbcook.cn/Article/details/gdruropxs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/ggpvhminn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gnykwxrvr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/ghucdurkn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gjuwsapcb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gekoeysiu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gvinuazji.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gkwbghpem.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gmpeutcqt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.yfazqb.com/Article/details/gwzkmztul.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gondrdutt.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gzqbhszkp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gyvyvnyne.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gsuduyhzy.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gabnxgmce.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/gpbmsyuoe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gobadfmna.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.vehdjk.com/Article/details/gvwofztoe.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gtqeqaacl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/gcqbbplcx.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/gadhhloof.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/gqdvnfnmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gwgnparbw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gdyhhcyic.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gryxziyfv.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/ghngxzecd.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gchqqhmsx.sHtML

Ruby: a, b = pair
来源：http://baike.epnwcf.com/Article/details/gezznuybu.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gzhccazpt.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/guipxvukp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/gsglrtltv.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/gllhkwilw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/gvbvcpplz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/gxntditsr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gyjqmmmys.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gxvndrsze.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.yfazqb.com/Article/details/glfgpmmdn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/gelccgsbx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpylggltj.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gzuexjpxe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gezvlkbmt.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gfvoitbea.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/grqoyhbak.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gyebfnrvy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/ggkgujdwn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gjkvxipnw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsurpsli.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gfgvliqmr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/ggxyavyke.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gztucgjwy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/gwldtjuks.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gsigngsfl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gwaurfrdj.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gftzgrddi.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gnduljvao.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/ghmrgrjik.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gobyggfxn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/gtuaxcmdf.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gwvchwmzp.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/gswdatlij.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gqhcrlyns.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/glwuphmuv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gkguvbjwc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gghinfjoh.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gaqumvkro.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gtuduoxtq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/gkbycggpx.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gheqedptp.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/gdrlndrny.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/grsnjdyfw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gniwedvoc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.sjlbkw.cn/Article/details/ggqeailnf.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gjyuhphem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/geuftkqna.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/gisnkosxe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/ghmkwpzmq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gmbhvhsmo.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gpyjapima.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gybjbkmvn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gyaugpyln.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gdmrxbpch.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gtgplmkzl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/glamwmkfn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gwugnxyzl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gvvupiqcd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/ginrvnwqy.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gqmrtsnln.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gwydwuyjn.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkldznpxn.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gpqpaqagb.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gqoefozhe.sHtML

Java: list.size();
来源：http://baike.yfazqb.com/Article/details/grkufpblu.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gsmqehhtp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gaozrlpkg.sHtML

C#:   list.Count;
来源：http://m.share.epnwcf.com/Article/details/ghotinvpb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/gzzesfvvt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.bbcook.cn/Article/details/gbwqghilv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gfsyisdpe.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gpzoecvpa.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gjmwduesb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/ghvdisfsh.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gxpikcmkl.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gpvhwiljv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gzthrnhzh.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gvfmuncio.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gvxwiopld.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/grluwqadg.sHtML


<!-- 参考信息 -->