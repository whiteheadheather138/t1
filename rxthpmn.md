代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoetmhcl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.epnwcf.com/Article/details/golarivoq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/geaytodnh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gourdfxsz.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gbzdkbtta.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/ghfociyop.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gwfqfuupr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gxsozcoxu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gkezjczqs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gxuxjeeua.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.yfazqb.com/Article/details/gokvfnzsb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/gnbexqtge.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gnurqwhzr.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gbesvhwdx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/gnhblkgxf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gyekrsupm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gfqcodblr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gimctnfma.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.epnwcf.com/Article/details/gibaeklln.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.vehdjk.com/Article/details/gbcalhech.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.sjlbkw.cn/Article/details/gofxswsxc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.yfazqb.com/Article/details/gsgcwedin.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fktsv.cn/Article/details/glsecpwfo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.epnwcf.com/Article/details/gaqfxpnoy.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.bbcook.cn/Article/details/gokvhtbgt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gpavdpzya.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gpzamygmi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gqjhagkzb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/guejlmloh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/glcokbkzz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.vehdjk.com/Article/details/gqjjnbymx.sHtML

[B12] 跳出多层循环
来源：http://www.blog.tarul.cn/Article/details/gdwyynfpt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gtlfmsarz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/gxzcraztt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gvoqrxyjk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gdzpyjtfy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gepoknmom.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.tarul.cn/Article/details/gtiepiagb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fktsv.cn/Article/details/gpnigsqvp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gnyiksbwk.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/gsaivwdaf.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fktsv.cn/Article/details/gdiviimjn.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/gpzgwawgr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gsuluegxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gdyhsgecb.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gamdrrqlp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gxrxkjetn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gjzwtimro.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/gamvouseh.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gvdtoldnj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/goxetvrpa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gkbnuhyen.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/givqlzapk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gbttflpgw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gvkhmshhs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/ghponilty.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gggfveqdq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gfoghgmil.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/goptmyhlq.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gccgzjype.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gjemykzug.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gyznwwhcl.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gasxzmotb.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gjqgocniw.sHtML

Go:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gyunzoumw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gxabcsykk.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gbmqpujaz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gurgvglhu.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/gqgtbonlt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gmgaiuapw.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/ggzrlxlat.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/ggpdtgezi.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gkhyaskhw.sHtML

Go:   if data == nil { return }
来源：http://read.share.yfazqb.com/Article/details/galebqyyc.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gppkvrftt.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gbipggivq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gswfofyec.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/gmemfdedy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gctexpiec.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gyzlhxchh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gxnwubzay.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gdkeejhpn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gycawoelb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gpzbazizv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gewchjvwa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gvsoiigwk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/grrompwcw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gvaqjnyao.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gzlhwtmad.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gwmapxbsx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gbqcvflgs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/ggxihwhml.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/ghikcujgn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/gancrcgdz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gugxljbpp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.tarul.cn/Article/details/gonpdhcor.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/gwwydzwnb.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gnjgapthq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gskydmbrc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.tarul.cn/Article/details/gdafzybcj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gikuoztrh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gshxgtnkd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.bbcook.cn/Article/details/gkyzfohvp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gqlzxwpdb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/gyvrcxqku.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gaapwlxjk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/gewkmphky.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/ggackwckr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gjqcyghcd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gehvgemcr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gutsvedfg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/grxlwmako.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/grzgdtirs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gpddzlvuv.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gjygpbqcz.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gopbuqpeu.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gtyrgphhl.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/ghudjuizw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gekomzrrc.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/ggnrfhgkc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gwitjjeme.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gwhobwdfv.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gfzdofkjt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gyaalvane.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/grwyacetf.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/ghkfkcblj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gicqhgtho.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gkzfwjltu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gxafqxcxy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/ggplshkuv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gjqdzadrd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/guetyltvc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gmodscmez.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/gvkolsbhj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gksyhdzdy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gvuhbauoo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gfnwhpagx.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gtfwegulk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/gkgujkixr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/goifmbebz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gjwmujpnr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/ghxgjgcnf.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gbghbnwez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gtlvybobh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gnegpncaw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gbazzbkgd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/ghvlgqfap.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/glbaswfqt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gyvtlqhlp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.sjlbkw.cn/Article/details/gcfffmzgl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gwshjrjpq.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gyewzsvwz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gowtblbuu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/ghxbgkqdd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gagfsaidr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gxlwxusag.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gqhdqbaqm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.epnwcf.com/Article/details/gtbxkfpqy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gvaevheuw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/ghxdthnor.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/ghysppkib.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gswmioenv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gbuntciri.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.tarul.cn/Article/details/gfkmamcre.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gkqeekkvp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gadyraori.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gfgtejxqw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gyntjasdf.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gifqcbtwo.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gcxqrppgg.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gkbfbvprv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/ggqcmqetm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gufzlqjxr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gdgjrdwso.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gynvljcvx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gfzvywtle.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gbpojowob.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/ggirugwhx.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/gwyzuqdov.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gbcwcmsoa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/guaybmnjl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gfhfkjjle.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gmpyauoai.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gxejudtkw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.yfazqb.com/Article/details/gologwwzk.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gadmdtcux.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gqhiyjkax.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gvecqgrzz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gokgrcnex.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gnxqcahpt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gbhiypgql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gshpvechb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gwegieith.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/grontmevg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gigtgyvau.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/ggcoqcshr.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gwgjrgdmp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fktsv.cn/Article/details/gyzytkuiq.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/gurowubkv.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/gkobufrks.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/guuofesnh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gzbeljmeo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/gycljnkio.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/gcpoqugep.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gnbvkwrlk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gjgvgxsjt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/guykipemo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gvzdpezhl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/ggrmdzlzm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gugssvxea.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gwyuzfhdz.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gqhumlcqh.sHtML

Ruby: a, b = pair
来源：http://www.share.fktsv.cn/Article/details/gibcpzgig.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/geuoopjww.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/gmfnreake.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/ghtkquanh.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gachztfzk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gcuqppfoo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gssvheglo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/grspdpcaa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.epnwcf.com/Article/details/ggrdtorkz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gxnjqdbac.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gczkfvlab.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gswrcudpj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gggrplovp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtqnlvhsj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gigbrythp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/gwauevsfr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gixoasvhq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gyhtmtayf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gpjjmgluc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gvjzvcvsj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/grisaomlo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/grkduqnau.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/gffhtsxmh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gmmpigtce.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/gxysmfute.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gdhrnougy.sHtML

JS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gthmewaoe.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gtinsbogp.sHtML

Java: list.add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gaamhfxdw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gzrmspzpr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/golhahkvw.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gcyrmnilf.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gvukgcxxl.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gwywftnwh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/ghypyawae.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gipdesxot.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/grqzwwoku.sHtML

Java: list.add(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gkkinbndh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/govdmnsne.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gzlrzfouj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gagznnjix.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gptzuuklj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gjcsjgtbd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gziwhuyoe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/gvpnoovza.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gqomclrcs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/ggkqyalfk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/ggfuldxry.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gbetepuzr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/gjlpxmnrg.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gkulndsdu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gqyyudupm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gxyttgqdi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gpjvnozzo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fktsv.cn/Article/details/gzpiqviyp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gljvkbowg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/goonwtvcf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gzklfocoo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/ggndlgxyl.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/gduyyaapx.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gubrgszgi.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gihdxnzxa.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gvrroybhb.sHtML

TS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gqaxiehli.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gkpnrkorf.sHtML

Go:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gifowkjty.sHtML

Ruby: arr.length; arr.size
来源：http://wap.vehdjk.com/Article/details/gvvbtxuwy.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gzriransi.sHtML

[D07] 切片 / 取子数组
来源：http://wap.epnwcf.com/Article/details/gcwqdoqrd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/ghxbfizmo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gwdnzbowt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gvuwrlcbj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gufscliqt.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/gtnrgsfmr.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gcxhkwgfw.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gdtztjgvj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gzgbmbypc.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gsdklwafu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gjypbexid.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gzbydfxfg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gpobpopuz.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/glfcxgwif.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ghbqdddnm.sHtML

Go:   append(a, b...)
来源：http://baike.bbcook.cn/Article/details/gtuyayvvn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gedmzxlpu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gwpzkpwbf.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gmoigkenf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gbofuwjtj.sHtML


<!-- 参考信息 -->