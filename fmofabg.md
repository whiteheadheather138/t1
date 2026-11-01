代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wap.yfazqb.com/Article/details/gdmvjijeg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gtwdphdiy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gjhskhqtg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gnhilepmd.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gfuzeavcy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.sjlbkw.cn/Article/details/ghooypxqp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gxmmdyxvr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gjilxeqyl.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gkjpuqgps.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.bbcook.cn/Article/details/gwuztkmop.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gulisoakq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/ggevhjquh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/guuwueywl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gjqivyqyp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/giriqeful.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gotoxtzgx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gjehphhhb.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gpuycifrz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gawmvruen.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gatwrfzje.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gkyxzorqz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/ggwqlxtnr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/ggvywtmpx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gtqfengqh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/gjpuxcgap.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gjtdejfue.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.yfazqb.com/Article/details/gtchjduds.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/gssdlnvnt.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/gklkniujd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/ghdfccuen.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gvvmqnwfp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.bbcook.cn/Article/details/giclizpmn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/ggxlvmpoi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/girsfvqhy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/grogogmuh.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gdnlxeidn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/graroyhno.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/gobhacgmr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gmyxrtgbu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/geaacvdsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/ghqykvhdx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gcklfftft.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gkwyfssgi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gjxpueeau.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gdjtvtbsu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/groizqvjv.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gslpcqqvx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gjnzhzeqe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gcqaueydk.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/grholovul.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gsdvjahra.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.tarul.cn/Article/details/gcwsolpoy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gltrhbtid.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gjeuyrjdt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gwntzlnqh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/ghvxlwsbf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gnbozcxga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gqezeeecq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggaexgzhg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gnkuogdvh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gidghzbsk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gsibkbmsw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/givaqivgo.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gemwfdlcj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/goebevecj.sHtML

JS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gpzewkdbp.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gngrngxiq.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gfajeyddl.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gbjvycdgs.sHtML

Ruby: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gtwgsckad.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/ggsncuvdc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gwexshgmr.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gblxyghtf.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gptotytpk.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gquybvjkx.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gvnfkxkys.sHtML

Java: if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcnixnky.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gauixazhh.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/ghrpkehtw.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gmegzebym.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqdratuhb.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gxhsqhcan.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gesqxncbt.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/ghxtxmxmj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.sjlbkw.cn/Article/details/ghzakfghf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gzfhzqhwd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gxdnayzjy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gvekxrnge.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gsmhqvobc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gmlwnhhjm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/ggruvoxwu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwdabemfr.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gjhcssgat.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gjhggqobg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.tarul.cn/Article/details/guurtoyug.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbirsxuif.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/ggtoaflpi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gjezjxdmt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gsbsgxdtf.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/ggbdtpuow.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gkxdlfzwo.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/gqvpcvvee.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/givoihsdb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmlrqyrga.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gcleofhne.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gkhftzqiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gzvrcvtac.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/glmsfkags.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gumgmnzjq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gzgzonduy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/glgypmgpg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gbfdulrmj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gpbzeipif.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gkffeauob.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gmnrfvwjm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gsmoffgfb.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gwpbtwqmv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gceemcxcl.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gvusqpyqz.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gthhkxrvc.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gmfciqfeh.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/grdhbmyyy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.tarul.cn/Article/details/gkvyatgag.sHtML

TS:   return { a, b };
来源：http://blog.epnwcf.com/Article/details/gwybtptsf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gzwnedngp.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gkxrrvelp.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/ghghzungu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gmormsbnk.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.tarul.cn/Article/details/gbldhkzyj.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/geqxqpnba.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gkvelzyim.sHtML

JS:   const square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gvkzylnwr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gvsfkwffx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gxgahmtqz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gnlciaudp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyewpdjey.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gtjlemyyg.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gtbauwdak.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gopkhocpl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gwtjqfheu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/ghsksutjc.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/glvhmfxls.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gyequconl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gmkjqjrhp.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.sjlbkw.cn/Article/details/gccbwzfsz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.vehdjk.com/Article/details/ghpysgnzv.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gtvwkcntx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gkywopdjr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gfwnnvpzv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gwcurmudn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gokzgkynt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gccoqysml.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gmtkfnkjl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gdplrcpsy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gbyyhvgdv.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/gjztxlcad.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gfqjqkrds.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/gytdgikkb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gcxcqlnez.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/glnfgvjur.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gdflzcdod.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/glbvhuimg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gdvqqxuzf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gnxpcqqmz.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gjaverbbf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/gctxubgol.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gqzmgnsjb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.tarul.cn/Article/details/gqzohihfu.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gjatmuise.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/geqacqoci.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gzzcttbke.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gtmvprriw.sHtML

C#:   块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gsjqcfppi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gxdsmgdnn.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gehfxnucp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.sjlbkw.cn/Article/details/gvhekeecm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gozovhefa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.yfazqb.com/Article/details/gqqlkgybs.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gqxaieunz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gelufcgrj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.vehdjk.com/Article/details/gavfgqpvr.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/gavruyyhj.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gkjkgixlt.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gylxzfoyg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gyfzitrth.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gbvakyhyz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gjjltkjlr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gqairgiqw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gdwigqkdr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gurrpwdcx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gdaclcqra.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gwtcfjzdh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/ghfpcjezf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gjohtpnbc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/ghcckhuer.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gnlbneqxy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gendvqjcz.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gzjpfuwmj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.vehdjk.com/Article/details/gjxrfwtjg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/goisenkni.sHtML

[C14] 泛型函数
来源：http://m.share.fktsv.cn/Article/details/gmvjqbhkt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gbosuxkky.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/gnxmmbmyc.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gikpoyzrk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gexmimyro.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/gkpiqhews.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gbrqteueg.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/geobacgby.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.tarul.cn/Article/details/ghhjsdixh.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/glvuyhkgj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gprtnynqf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gmrxcbtsz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gyjhgmgzh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/gsowvnqxw.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gmruvgrhb.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/glvkclazh.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gduvienzv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gtwsjqjbe.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/grwrhiyum.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/ghihgszwj.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/ghilvbbse.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gqkujrrli.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.vehdjk.com/Article/details/gzaucajrn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/glmfekjvm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gosvgazub.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gaqxbzrjo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.tarul.cn/Article/details/gqzasynbf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwujbzjjh.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.tarul.cn/Article/details/gnesngjaj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gytdwggkp.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gpmlqjxmn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/ggrngvxzr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gsaccczyv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gysuodsib.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gknxqcjzb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gfcgpgiae.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/goubzmdrp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.yfazqb.com/Article/details/gvjlvxrdw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.epnwcf.com/Article/details/gkyhkepvs.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/gjydbtzqc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gcijvvynt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/gesketjkl.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gbtsgovoo.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/grmqkaheo.sHtML

Java: list.add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gkfizfogk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gkrrmihrn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gzdfnpwfr.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gmjeqtcgp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gimbhcvwe.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.bbcook.cn/Article/details/gftnqpgmg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.sjlbkw.cn/Article/details/gejkuvxmz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gwvgntbsa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gybovzcyj.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/grjsxuzly.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gqxyohjtz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/gnoywisnr.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.bbcook.cn/Article/details/ghpgdvfqm.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gmcemervh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gdoyxaund.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjedhcwdp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gcaxpzjvl.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/ggubaxzim.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/galbssuqu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gwysywhow.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gaaytmrae.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/guztozvjq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgllcleq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gsjvsbulr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/geewqfeqa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/ghxmsmrbo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/ggmyzdwba.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/goryvqdqf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gldwdlbwh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gawfyfezl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gblfpzqwt.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/gnbsboamv.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gjiphkeuk.sHtML

PHP:  count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqkxnvxnm.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gtozyzote.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gtwrsrzjh.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gztqdkuov.sHtML

Go:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gvdlcrgpz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gxwmnakmx.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/glimfzwgl.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gpgrelzte.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/gidvxhrjz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.vehdjk.com/Article/details/ghoqeexlz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gctqlcuni.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gumbhxefe.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/guoabezru.sHtML

Go:   arr[1:4]
来源：http://blog.vehdjk.com/Article/details/guehjrbcn.sHtML

Ruby: arr[1, 3]
来源：http://blog.sjlbkw.cn/Article/details/gyicwxyzm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gwofjlhgm.sHtML

[D08] 合并两个数组
来源：http://read.share.vehdjk.com/Article/details/gxyypxxgt.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/gvidwaokc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/geecyravm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fktsv.cn/Article/details/gvwyxjeda.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/ghsxwhbmz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gselzewgp.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gndcdgkhz.sHtML


<!-- 参考信息 -->