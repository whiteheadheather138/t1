代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gijebyfwy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/gcgaqrczw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gnifwpvza.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gsjayapja.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/gufgemnnz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gyijbpynr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gxwrfrbgq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gapjknozu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gjmvpgbns.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/glwuidctr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gqvbywxki.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gcrumugcf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gbmjulauy.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/givchlbeq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gckmtwwde.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gmlbkgivs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gmcdvtgyh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gggvyfqkz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/goelozxow.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/gbzikvlrh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gusjrnqwz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gqyvkhqbo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gwcgppwjh.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gfbvhaixv.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gguxzcwgm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gzwchbsqp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gcljpkoth.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/guqsicomi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.bbcook.cn/Article/details/ghovuqqqw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gjijiblpp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gapdxadzp.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/gbzwztphs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/ggqgkteyr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.tarul.cn/Article/details/gljocmxeq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gmkfdnvwc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gmyrvlnbt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/glnevqizh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.epnwcf.com/Article/details/gjiikhrii.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gcomijrui.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gpnwknkta.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gmfkrkgxb.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gwxkhroed.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gtkejtdct.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gvdaxvvir.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gkegepdkw.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gltmbbigj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/ggqdbfkwz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gkjfkjbvt.sHtML

C#:   x is int or double or decimal
来源：http://blog.sjlbkw.cn/Article/details/gmdbavsbt.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/gtpuejwad.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gyzyqypbp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gmfkhihfy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gwgeinolj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gjqzbmizo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gcocqixlj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.bbcook.cn/Article/details/gokruisld.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gdrmolseh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gjofhhlaj.sHtML

[B15] 布尔运算与取反
来源：http://wap.fktsv.cn/Article/details/ghtskmula.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gmhlgvfvg.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/gdpfyqbfl.sHtML

JS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gkvgyeiwi.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/geaqlqcbw.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gvhlcmyaq.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gqcixvpjq.sHtML

Ruby: a && b || !c
来源：http://baike.tarul.cn/Article/details/gyoltwvsf.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gvchwxlav.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gpimoofnt.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/gpjylwmep.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/gvplqjuiv.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gwjggzzkj.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/grooezndj.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gapcvdhlw.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/gfqwwycxn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrsseleu.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gtzsrwzkd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjurfkhno.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/gcsjsrsif.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxuriiued.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gsgzhhgzs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.bbcook.cn/Article/details/gzjeuuqvu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gyrtejgoc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gngllhojk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gvvejlbzo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gglitgwul.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/guanqahiv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gomnrcugy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gdklrrfkn.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfozzkccg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/ghxpkosud.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/gzmafgnin.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/grggbcyfo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gzmxyvseo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/grkejhcdp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gftuodfmj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/geipgitgg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gouwflgtd.sHtML

[C03] 可变参数
来源：http://www.share.yfazqb.com/Article/details/gmsfhevqi.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/gkfxbdfjh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gqwphyfaw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gtqbfywzq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gumtrcdby.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/guwazyksn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gtibraawr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.tarul.cn/Article/details/ggbtavwos.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gmibpgruq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/giblhvvvs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/grghjpjqq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gworsfeen.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gjwzajdzu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/gqvpmxepo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gzotooeke.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.bbcook.cn/Article/details/gnbpggeio.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyzumnsn.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gwjkuuhov.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gaqxxypwv.sHtML

Py:   return a, b
来源：http://wap.bbcook.cn/Article/details/gludfljdv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gozzqpvoz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gzjakwnfs.sHtML

TS:   return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gcgdygnoa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gmqdtmslt.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gtbupmall.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gdyzqnibg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/giewyfqoz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gfozqcowc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gxyueiegr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gkaxtocgr.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gyitssrng.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gqvgswdlq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.yfazqb.com/Article/details/gtbyacwaz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gzyuszcow.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gwtxashqr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gezdzodwl.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gtjyuffyd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gzwkymcpf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gkztahpgl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/ggbigycsg.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/goxzzuxvn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gnlsjtqph.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/goccrjfrz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gdczoqtsy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gysowqbwq.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gshjzsdns.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gvvkycknd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.bbcook.cn/Article/details/gblnkuqtt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gcvsogslw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gxdqywlxz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gdqmnqjkr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.vehdjk.com/Article/details/gcppuggxf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gfotvdjrq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gvkhkycjf.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gcgknfkas.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gnjblmyoz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gvdjavwia.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/grgkixbqw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gysknftxq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gftkhdwtf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gmoxpuxxy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gwpbxetce.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.epnwcf.com/Article/details/gxkvjuwfh.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/gdeewlbdy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gxcdbshgt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/guyrujkty.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.bbcook.cn/Article/details/ggfqyrvgx.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/gggkdizkz.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/ggytaauiw.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gblfritpk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gvrbvbonb.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gnefahfvq.sHtML

[C11] 模块导入与导出
来源：http://wap.vehdjk.com/Article/details/gqblzotra.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/glxltpzye.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/gyelqwnkd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/govjtibie.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gxdjaxidp.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gxdmhmzry.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gkkcorptq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/gbxxzgrjo.sHtML

C#:   using System.Text;
来源：http://www.m.share.yfazqb.com/Article/details/gdokwebrc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/goilrhgnx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gsyjpiiki.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gjwhuumld.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gouxyzath.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/goscuatqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gyhoutufx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gvytkksex.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/grnvmrgnm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gsceimusz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gildbljwj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/grhtuuibd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gyuzbxqsi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gyhmlqzbc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/glnidgssq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gryqxizfj.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gukdiyjwl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/gqmyzzydm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/grckhufev.sHtML

[C14] 泛型函数
来源：http://baike.sjlbkw.cn/Article/details/globkkoth.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/goytpmgmh.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gxqmdjgwy.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gmcvbvewr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/ggckkyvds.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/girvzqwaj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.sjlbkw.cn/Article/details/gjdirpvan.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gjnayxyis.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gxidcxptx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/ghjrbeskz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gqruvakkr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gualdouke.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/ghqmxpvku.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsulqpkoo.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gqcuxnyok.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gqpmrsjic.sHtML

Ruby: a, b = pair
来源：http://www.blog.sjlbkw.cn/Article/details/gogynkrlq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gjmdkvldf.sHtML

[C16] 函数 / 方法重载
来源：http://baike.vehdjk.com/Article/details/gxipfrfdi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gwntohrxb.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/ggqfgmqtv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrcqbwdr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gpvxpebdu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gxxfwkzqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/genqsapco.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gkitmdpbr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gxhdqsdjv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtopaorwf.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/gmqbiooea.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbrdhyjir.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gnaikgmpp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gazmvkynv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fktsv.cn/Article/details/ghziqpiwk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gpzgqbwcl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/ggpoxennn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gvmjmilbf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gxpbigmhx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/glcdogmse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/gdnbezsyw.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/geeetwtxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gkzqafbqx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gnchbjdkb.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gyuenrcgd.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gdopzhkmh.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/glzjdngnc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/grjncccdp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gwhthjrpr.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gxvsmahpi.sHtML

[D03] 在指定位置插入元素
来源：http://baike.epnwcf.com/Article/details/gggcrrlmg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gwsvdnwhl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gqygxzxxu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.bbcook.cn/Article/details/grffzkjdw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/ghlxcxpcy.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/gycuacohm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gtauydemg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gnqophblh.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gjkaslmao.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gyttgfxkq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/guvnhdfnj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gxgxnizxg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gjxvlcejz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/gwmtdidgn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gcpvtiouk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/galhgchga.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gicbduiiq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gdsqfxzcr.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gigmvfwog.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gsvsiujfc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gyhyapcdj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gosvylzjj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gjvdstuwp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/gdqrpgflg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gtbyawiaq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gyowhirdd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gdxqpckew.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gdubndcwq.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gkhxmntgq.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gekzlbama.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gdrxpqkdm.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/ggnasldsy.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gbubgwzgv.sHtML

Go:   len(arr)
来源：http://baike.fktsv.cn/Article/details/grrfamtcc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.tarul.cn/Article/details/gewmhwqfa.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gonbrfbsa.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/ghgctmaqq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gavkupilm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/ginvrcaae.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gfuhszcpr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gzaeeqeit.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gnbegkpbc.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gywasiwqm.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/ghxclamat.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gueshzkvf.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gvozfmzdr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gyyufiaxo.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gvpyhtfkm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/guvqnrgsx.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gvaosleps.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/groxlbpgb.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/gsefphjxz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gtmbvgolk.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/geoagybng.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gbbdgbnhs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gqfbjhjpp.sHtML


<!-- 参考信息 -->