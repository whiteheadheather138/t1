代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gvwhfdrde.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/gdfjrakuq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/gdutrxgbu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gghhsposr.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gzklrokiy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.bbcook.cn/Article/details/gotrtnabz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gpdlualsm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gezvhvbaz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gnbekivgr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gtqadpimf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gxoeybeky.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.bbcook.cn/Article/details/gxmfwotej.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gbmezndth.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gyziwjcph.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.vehdjk.com/Article/details/gqiiuaova.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/glsucyrgq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gfhdcqhxk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gdxbpbhev.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.sjlbkw.cn/Article/details/giyfmhqaj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gqxlqvfeg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gfclkatis.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gnqowthiw.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gxbkynnyv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fktsv.cn/Article/details/gvcapezfk.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gdwzcynjm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gsciwdpwx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdwdhrhb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/grckkchkh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/gceibbkdy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gvksgtbce.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/goskyetrf.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/gassuvfft.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gedqgyvgg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.sjlbkw.cn/Article/details/gnlflbcyu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/glxgdkfam.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/ghlwcvmtu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gmcwjbjgr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/gunjmoffl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gqftogomy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/gzwhxpawv.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/ghnubmguk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gjbmzahsc.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gkcymzzxa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/gjtzarjpu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gqgzxbzth.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gzcqjuyig.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/gnjbesdzf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gvzjirsrg.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gvedvqjuf.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/ggmhojbrz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/gkesabuiu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.vehdjk.com/Article/details/gqrangnzb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gzswijacc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/genbjikjx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gsyfjznyl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gtgjerzwm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gpbxzrpyy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gwzhnzbse.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/glkdvejci.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gnxtkvjal.sHtML

PHP:  $a && $b || !$c
来源：http://3g.tarul.cn/Article/details/gnqybwpbk.sHtML

JS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gfpmwwpis.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/guepnphgz.sHtML

Java: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gkcfncjue.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gbqfgepwb.sHtML

Ruby: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gvqxnuddw.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gzamkndbu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gykcgjngw.sHtML

Py:   if not data: return
来源：http://wap.yfazqb.com/Article/details/grpolbnle.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gqqfswjas.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gjsvlgrxf.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gjegtddik.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gfyainwnf.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gyleiyagz.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gaftlpsvh.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/givbxmdvb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqmjitluk.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gmxbrmyje.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxclursjs.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/grkzttnjb.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/geempmedr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gqbbmqvdn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gqyhzrmdw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/grkfxjejt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gidnntxlf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.tarul.cn/Article/details/gfcxiivpr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/grfraiqyt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gdtpgbtgi.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/grtncqckq.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gzqgidisn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/ghgfptzqr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gujrjrvpy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gmyqzajva.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gphtoamgj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/ggbosutas.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fktsv.cn/Article/details/gfbphvgtf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gngynswob.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gthjbjjyk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gcjdoyzbc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.yfazqb.com/Article/details/glaqzedfe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gmmmfbsay.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gplxzbsyc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gaseirnzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gzujlsbex.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gmlriipzl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gentmkolw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gxshlwgzx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqrerunu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.yfazqb.com/Article/details/gpsbikzwg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gecyewfve.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gmaqsnwtp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/gpnnpayyy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnghueyks.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gmvjlvcnt.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gvgiihzek.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gnneztfyr.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gvbpviknw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/gmbiipgod.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gphhnfmqi.sHtML

TS:   return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gyhsxvrum.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/gorqiddnz.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gptqgcuug.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gqukkmhnb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gpynqzfhi.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gaivljsce.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gylvmnusx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gasuggzhw.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gahpsjveg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gabyytmaz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gkwcrpwdl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gkrbaeupa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/gjuuycjlm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gbzccpakn.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/gouoiypju.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/gnaenoutl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gwpuckzfl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gspecwogq.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gyvuwdmgl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gjcoulyac.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/gxrmmeufv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fktsv.cn/Article/details/gwvhyrjpw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.tarul.cn/Article/details/gthzrmpfu.sHtML

[C08] 闭包
来源：http://www.share.vehdjk.com/Article/details/gtjysiyee.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.tarul.cn/Article/details/gurdtecka.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/gxfikodth.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/glzsvvcsq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gwdrpmfxu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/gxzzeyksl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/gyxuzcrjc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/gxzvfsjaj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/grayssuyy.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gvznhstzy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gucbsxozc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/ggzaagnzb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gykwbhcgh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gohcdlfht.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gbnrykdxz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gdqgtddgj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gylkqhchb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/gyalbjgbk.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/ggluxnuyn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gritnoeep.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gxvejnndo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/goyaobqyq.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gstharvzd.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gckcelkxp.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gvcgxmctx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/gwzvazvig.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gkiaazjyn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gtupsjvsc.sHtML

Py:   from module import func
来源：http://www.m.share.tarul.cn/Article/details/gtivtswkp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.vehdjk.com/Article/details/grjltzbyo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gxyctkols.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/gvqgndgvm.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/gehbvrfzc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gelwbsunh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.sjlbkw.cn/Article/details/glkkvxkbo.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/gvdzvspvp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/gcsiykzdp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gswgdcplf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gecveffaf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gsnfxmvrw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/giqvvkggp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/gxjbrwpzn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gnkqrehbf.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.vehdjk.com/Article/details/gqkizzcbp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gczzfrvht.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gvqwjkhay.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gnmyidgch.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gbkgtmlpa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gggfdbcva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gdrjhpmhm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/grzwkjodm.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gzvbqigmn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gpdckglts.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/guqaysmwm.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/gyfdhnbyj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/guslpygue.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gbpwoqxxr.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gqpbabsay.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.sjlbkw.cn/Article/details/gcerwklam.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.yfazqb.com/Article/details/gdhrozrln.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/ggafwmjez.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/giziuwcnh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gqmvvydqb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.epnwcf.com/Article/details/giwbknpnn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gmepjejnr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/ghashkenc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gwhpffapi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gtjwvfmec.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gcymxvzst.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gicetwddl.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/glhqlqykw.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/gyqlonvpf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/gdxhhueqd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gblnqzjtv.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/ghygobcgk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/grehhiwce.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/gkrqpkmwe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/gmcjvctpc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gxkvualuj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gtsuuigne.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/guolknbhp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gowonardd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/grrfwornn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqkhdqkmv.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gvedihzyb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fktsv.cn/Article/details/gaqyakxbo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gobwkgwae.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/guhwuxoih.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gibppmnfz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gtdannlgy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/ghjpxiklj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gdoeifdps.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/gztwbyxej.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gcwzcobgf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/geetudhmf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrzyyghk.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gxhenyvyu.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gebjnfdhc.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/gsvzszdly.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gbbjcllma.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/gayclecuv.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gaxxezsuw.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gckkcwirx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gonsdnodd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/goumceuey.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/grmzgtxbj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/ghocojigv.sHtML

Java: list.add(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gsseghirs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gideianpu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/gehhzynke.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gmksedcsp.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/ghjjfafyv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gslcvbkcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gcyjvqjgf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gwlytyzzw.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gvrtscbzn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/gpeycyalg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/glaicairg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gkpknkxqs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gcshrxfyj.sHtML

[D05] 访问与修改元素
来源：http://baike.fktsv.cn/Article/details/gjlprbcst.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gbvrnrghv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gwfkzwwml.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gklxmbdfr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gunmkaqpr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gjlnhyvco.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gsmcgppbq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gjykrolii.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/guakvkqrm.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gzzobdvng.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/geopqlsnj.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gchbgfcew.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gvogehfgo.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gwrabouia.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gpbzrebru.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gpujjjhca.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gcboowdhq.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/glbymuzfe.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/gsystwher.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/gevbxsohn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gybcvwqmk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gmxlfdcyu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gsajraesy.sHtML

Java: list.subList(1, 4);
来源：http://3g.tarul.cn/Article/details/gtjohsjij.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gboskjxfv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gcyvkzltq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.yfazqb.com/Article/details/glkzvlzrp.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/ghrtvtmtf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gsiovuxvl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.bbcook.cn/Article/details/gerbqwfjv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gdrnnmplx.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gfayapxlx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gazgvtqjj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gdvfeydzl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/gaeqfebqz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gsozecbjs.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gmonyvjvu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gujxjhixe.sHtML


<!-- 参考信息 -->