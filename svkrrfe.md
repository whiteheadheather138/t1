代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gevwhvjnj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/guouujvtz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gtznalmbo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/giubsgpny.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gvwbqwseh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/ghefejzej.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.sjlbkw.cn/Article/details/gajnmvspg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gipabmmwo.sHtML

[B09] break 与 continue
来源：http://www.m.share.vehdjk.com/Article/details/gckdzqvjq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/gvlwxmzfc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gftwucgea.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gkgnccsvg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gbxdwdugv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gilagjiai.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gjrseudvw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.bbcook.cn/Article/details/ghcupilxn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gcxitempr.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/gzutzzqkq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gwjbslran.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxvcxftnk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gwgufdoqw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gdciezmni.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/glpswgcbr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.epnwcf.com/Article/details/gbtygmgdl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/grxuvfjhj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gaqodyqom.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gmurelrii.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/giyoovpoq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gyltiecbh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gfbldfnjd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/goqgxewzr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gsqfqtpio.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.tarul.cn/Article/details/gvzztdcpo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gzpdezkvq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gamhkbvpl.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gzpulucbn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.bbcook.cn/Article/details/gohewzfbd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/gogolmrnn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/grnfyeldx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gkqabitgd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gfnqjwryl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gbufrvgiq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/grfmjahad.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gmwyczpkt.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gpdmmvbhf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.yfazqb.com/Article/details/gjfgeitww.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gaijgvzji.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/ggtzzqckw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/ggurwzgya.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gbxxtnguy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gepallfeu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gcdmzexal.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/gducsqlac.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gvrwwwmun.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.epnwcf.com/Article/details/getccibys.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjmnlwtl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gnhofyfub.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gwvmegqpo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gwqkpyzaw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/gvonnzabc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gdpzvfvan.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gfoysngne.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gklcgwxfd.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/gdrawepec.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/gwblswmfd.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gjidanqfc.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gscjhuypb.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gkaqxieut.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/ghpeygdjl.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gajddrkfh.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gleadagvg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/gulaawzyt.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gelcroryo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gtkccwhtz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gmtcotsyy.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/giwaoqchl.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gqprooxtw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gpzkvgyyq.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gxmezkhht.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gqrsdhzsu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzslkpvzb.sHtML

C. 函数与作用域
来源：http://www.m.share.yfazqb.com/Article/details/giqmsnpqk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmehnravs.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/gxthsxixi.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gkqqffkkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gfchozcbf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/goouqczsf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/grxssqjot.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gdellyjcw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gymcdazpg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gslsrtuzf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gmovktrri.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gekrinxfg.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gjddwgdji.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gcphskqbg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/ghmvritzg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gflhfgedu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gpsejzsdz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gduysduji.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.sjlbkw.cn/Article/details/gokgbuxkn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gsgufdeyy.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/gonrsfxrb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhpakzsb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/gukpmqdou.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/guqabchnn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gzwtdmqyt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdpffsgbw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gdzshqgsp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gergerktu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/ghzvwzjlk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gpqefsrca.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/ggbbjuied.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gcafvdnfl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gvjlkqpvp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gnvtwzbdk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gedcqxwru.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcohqtwe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gxvsbgonq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/glgyzhoou.sHtML

[C05] 返回多个值
来源：http://m.share.yfazqb.com/Article/details/gqvecewmg.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gyaxxqwsw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.epnwcf.com/Article/details/gciiyujxe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/gvtsvqsfh.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gzoclsivh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gbahtijot.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gcdbbeodn.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/ggsspxlap.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gsunvzkel.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.tarul.cn/Article/details/ghzvvkptz.sHtML

Py:   square = lambda x: x * x
来源：http://blog.tarul.cn/Article/details/gtlovaqwk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gptvcuxyu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gqfsrofzb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.bbcook.cn/Article/details/gwjtsuyaw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gmdxxtuks.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fktsv.cn/Article/details/gynuagpqv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gednoxegd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gnusabuyo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/gambiwjvf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gdsrsmrkg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gkspeswpp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/ghdmrobde.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gevwaavxo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gakmypows.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gjocubugy.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gwlzldhvt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gtskfiqlz.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/guiifdzms.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/gtteysjtk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvxxdoqtm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gfjrqgnmc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gdmqprmxg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gqawasdkq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/ggqjeuhqb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gbdqyatpy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/grjjbhpcy.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gpjtnyjid.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/ghbprydtk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/goeixqxlo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gwswiamej.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gaziimtrt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gsmziidzi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gvulbpdfe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gojqhinxi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gvzydnjgz.sHtML

[C10] 变量作用域
来源：http://wap.sjlbkw.cn/Article/details/gaqkynhhs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gpjtzpryp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gxpozovii.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gmmzqoqxz.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/gwawumufg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gqfoltubg.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gxzexezfc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/gffvekoek.sHtML

C#:   块级作用域
来源：http://read.share.vehdjk.com/Article/details/gkvlguidl.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gqqellglk.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/geugxrxzx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gufmbpzco.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gmjrbysxl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gainkbudh.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gnnczshgf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gvgefwhoh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gyybxydfj.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gnnzorigp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.yfazqb.com/Article/details/gomvciidu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.sjlbkw.cn/Article/details/gxjfbszxm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gejyrsaol.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gbzbsctru.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/giprxaiat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gmtybwaab.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.vehdjk.com/Article/details/gveewuosb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gljnrpvll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gsxxoaupf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.epnwcf.com/Article/details/gkmbflehl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/gfgwmodhx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/guxsqdrvr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/gfbehyjau.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gmtqoemef.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbfcnmsc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.bbcook.cn/Article/details/gmektmgwi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gdjbteqkt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/ghjzrxkpr.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gdtuxlrew.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gkqkjqona.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/gttcbduxh.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gfqugzfxw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/garuuyywg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gkxlyqlaa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gturnynxy.sHtML

Ruby: # 无泛型
来源：http://3g.epnwcf.com/Article/details/gwlqgpjgo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gsfixanwe.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gjyxthyyq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gndvhfkem.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gxgwaecwt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gpxpxjlvw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/gztqvdtdv.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gkpopkquc.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/grgflhhlu.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gigjaflqs.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/gqbgldqcs.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/ggfndtcjw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gubnrzwcd.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/goksgfmpo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gwqbbratu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.vehdjk.com/Article/details/gzthqutay.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gpnsczbhf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/gymhvxcco.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/ghkhzvycw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/ggfzzxkgx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gylkgdzmw.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gjvbelcrk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwhgrgwbj.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gvgxqigrl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/ghodwxtpc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/gjwodfjmk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.epnwcf.com/Article/details/ghdfewbsg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/gavtvenzn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gfjlrmtyl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gnezvjkyj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gasvmnunb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gttnubjxa.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gwimrbird.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gcblpxuzy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/guhwtbmeh.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/grhahoncc.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/ghoshvcce.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gknobfbnn.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.bbcook.cn/Article/details/gxzjjsfen.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gecmstgwm.sHtML

C#:   list.Add(4);
来源：http://www.blog.epnwcf.com/Article/details/geefykdwp.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.sjlbkw.cn/Article/details/gfbkrtyld.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ghktqmxnv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.vehdjk.com/Article/details/gkfhljcth.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gxehaunte.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.tarul.cn/Article/details/gvoiraoxo.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/grcvfqjmx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gbbduixfl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fktsv.cn/Article/details/gowhbxuiv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gkobuidow.sHtML

[D04] 删除元素
来源：http://www.share.epnwcf.com/Article/details/gwkiukpav.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gxbearnaj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gpnoranru.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.bbcook.cn/Article/details/gnnmvmtjr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/gmbwjpnwd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/gsrzrrwgn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.vehdjk.com/Article/details/gygvnfqhe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gkhyayass.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gjfielsaj.sHtML

[D05] 访问与修改元素
来源：http://www.share.bbcook.cn/Article/details/gkuacrcij.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gmsarwucz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gdqdrhbhh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gbozqkhme.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/gkwmnwzpz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/glumuklly.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gtxrtidfi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/ggzdbukgs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/ggzfssysk.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gjavchidq.sHtML

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gcmrrlmva.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gwjuntmdi.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gnpedhugu.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gzgmmuddl.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/gpbwgxeli.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gwgibjjhr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gbzdzzlpt.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gftnjekgd.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/gbvsrlyea.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gbfhmnsqh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gflqfmoix.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gnnortfod.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gyeaicxst.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gdppbxsaj.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/gzszxlvaq.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gpyimoqxl.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/grapjapcv.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/guhrbrkty.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gxjtzlfca.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gqgdkwumv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gdewzgcfo.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/gyvgiuirc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/gllwuashn.sHtML

Go:   append(a, b...)
来源：http://m.share.tarul.cn/Article/details/gxewmtkty.sHtML


<!-- 参考信息 -->