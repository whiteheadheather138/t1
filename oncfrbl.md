代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gbxmybgoh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gtuvklaue.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.yfazqb.com/Article/details/gzojrscbl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gnjuaclkr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/ghvdntuhr.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.bbcook.cn/Article/details/gyteyrgjy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gpmtrvvii.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/goctnbnrk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gnmeunoqk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gjvlseelj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gcaaryrbu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsxfzcvt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.yfazqb.com/Article/details/gcskpvhoa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fktsv.cn/Article/details/gmciqimba.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/gmxoxsqsg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/glkbsnciy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gjwubugow.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gssjjcfpf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/geybutltg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gwrxpsbsm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gpkytiaic.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gknkdzvwj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gmhohdlqt.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/ghjpanryq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.yfazqb.com/Article/details/gkoriddgl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/gvaqxjzli.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gewkphpvq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gszrlqoau.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gvqikiiqo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gaaukpdep.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/guidyfomp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/gjpckurap.sHtML

[B13] 判断是否为数字
来源：http://mobile.tarul.cn/Article/details/grirrmzfe.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gmvppadle.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gdlokfuog.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gshelqywu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gosppjnvw.sHtML

Java: x instanceof Number
来源：http://m.share.epnwcf.com/Article/details/gvsfxodrx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gxgakfzpm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.bbcook.cn/Article/details/gbzofmtdo.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gmdemtbcd.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/gscbkpcna.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gntofuzbj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/gvluryket.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gqkkzoehv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gwhjyacrq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gutshmwqt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gkqnrlxzg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gcondzktb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/grqqnewnh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.vehdjk.com/Article/details/gyzquixjt.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/gwfbspgyo.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/ggcwbwnga.sHtML

JS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/ggzbrgsmn.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gqwacpmpc.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gqdxljwjb.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gjvikteqf.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gpcfjdwga.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gyixyggqe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gtqiehlhp.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/gitsubloa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gfafrwhom.sHtML

JS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/grejkykus.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gcqddtwxf.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/glpxngsoe.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gekojflrt.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gnohspaxe.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gxocujlrg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giozwpgtc.sHtML

C. 函数与作用域
来源：http://baike.bbcook.cn/Article/details/gwxmyqrmd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvbfjoglx.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gmvasepyp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gcouxweoq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gauclgbto.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gmnoondgi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gpsdxmuzo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gcqdzzmhp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyygstbnb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.yfazqb.com/Article/details/gysfxgbfb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gooqqqszk.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gyihgljsy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/ghccxqtlb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/grsjpvcjd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gefsuhooy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gqkifewpb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/ggmzveuvj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/gxpyollwx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gxkvcepdw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gibpgtukt.sHtML

[C03] 可变参数
来源：http://m.share.vehdjk.com/Article/details/gyftetrcg.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/gqpjdtgsc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjtmdjclg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gqbwmddyr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gkhoslobo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/gpxaesmef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gmpjgdgeb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gnpzfptlp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gyjexqlkm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gckzgjzzj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gjlxjrood.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gvoauuifo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gppupqvxw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gvqtbwlff.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.epnwcf.com/Article/details/gebgryvjc.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/gspzdrmhx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/ghlqhopjq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/goaxzqhxs.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gwokrokwa.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gqcvfuplz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.tarul.cn/Article/details/gumblcghy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gnstvfetu.sHtML

TS:   return { a, b };
来源：http://read.share.vehdjk.com/Article/details/glivhxxqk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gefxptylx.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gigcpfqjf.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gthvbkkxu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gbjubdsjg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gqzixukay.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gnlehdwvn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gxscbmnyh.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gpwczttvl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gzkljwsdm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/goksqpjhk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/ggztjxzwk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/gyfiaoqtz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/goojmrejp.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gcsranulx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.bbcook.cn/Article/details/gzxtxeudf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/ghvkwbwvh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.vehdjk.com/Article/details/gddzfvkyh.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/ggabxpaqm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gjvtztqwo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gofqyonsd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.yfazqb.com/Article/details/gmjngqmvg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gppccfzyu.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/ganuirnjx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gmmpvckdl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/gbbpryouk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gkuvoatrk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gyycllqns.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gxwvpwziq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gqquowhse.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gjiwwlprc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gngbkferf.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gjkzcfdky.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gifosunpq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gaijpmbge.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gsqizmyie.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gzlbwigfe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gcsxhqdwy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gpoftaouv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/glspmydkl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gtwhydakj.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gyzfwdlft.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/gdtvhdxij.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gkiqfcvcm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/glcnhznhy.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gipsfawti.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gniwbajvt.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gfvicgogp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gffnpvlph.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gpnwfjfxr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gwmbpdtqm.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/guhyfsjrl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gboguveqs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/ggsuzbuzf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fktsv.cn/Article/details/gtztruncu.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/giszkticj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.vehdjk.com/Article/details/gsrdpiofl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gudlcpbvy.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gxlouzwig.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/gxrkmswgv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gczxvguuz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gtqyssuqf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gjjaxsskv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/geviyruxs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gklruvrer.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gigymjosg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.epnwcf.com/Article/details/gkwtesrid.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gowpqexyq.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gtqbxwait.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.yfazqb.com/Article/details/gifarxots.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gjeewlvia.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/gtqiokgxv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gxpvibnjq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gkdyyktar.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/goxgnvryx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/guyifdtiy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gmrapcapq.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gzmajouxo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gslbckxfj.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gnkeyepab.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/ghyiciclr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gojqzjeyr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gijztubam.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/grssmxvpf.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gferzcjak.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gfqunbghl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gjmzzexlo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gopnoxnwl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fktsv.cn/Article/details/gslkukmpl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gdgqkkgxb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gyeznxhcz.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gliysqvqu.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gdltlzfrz.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gwydfwqqx.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gcjynbmbd.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gjkhuzmqc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/geroirqza.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/gocxxkwgg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/glemvwflh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gpukpbyii.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gvegcpqam.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/grwxfgbgm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gbhiprfgt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/ggkomqawu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfwvnhxhl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/gurcvduei.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzmwbeify.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gslfxqlka.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/gkdqkkzjn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/giopegdng.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.epnwcf.com/Article/details/gqnnuqjvx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gyaiibqvp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/gvljcxunr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gpqcxgkra.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gqdwsbaap.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gffwupjjm.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/gsbexvflw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/gazjjwxll.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gvdyuzeka.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gzkjhnphy.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gngzhxsji.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gyymfkygl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gsyzdrzlf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/glwnskizr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gmrzjeukt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gsczuqsvt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gwcnumfln.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fktsv.cn/Article/details/govxhcomv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gxxylghuo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.yfazqb.com/Article/details/gztobfreq.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gzlngflqg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/grkxlofie.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gtmxwnaof.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gzxwwmaod.sHtML

[D04] 删除元素
来源：http://www.share.yfazqb.com/Article/details/gklqettpo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gbcjqkrwd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/guphzeqfw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/ggxiionsu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gpxjzndyh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/goigcwpvu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gleszkvqt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/gwjsnpzlw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/glndnregi.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gloslhrak.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gfpqsysrg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gyzgjpxyy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gydbneele.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gpzuzrunh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gjtdzdzhb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gwgcmksgx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/ggdbiwfxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/glfylipzv.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gaxioejya.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/goemqsdvn.sHtML

PHP:  count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gbmsqlngw.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gewjmkhtm.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gpmrrzjwr.sHtML

Java: list.size();
来源：http://baike.yfazqb.com/Article/details/gfomezldp.sHtML

Go:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtiyrfzmr.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gvzgsxhwi.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gqskjtxdo.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gsfkliewi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gohsnkfvc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gnhjmmnch.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gundsjhxu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gtxpqoeif.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gfulfbtlb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/grzyjggwf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gwnciflup.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gawihhymt.sHtML

[D08] 合并两个数组
来源：http://www.share.sjlbkw.cn/Article/details/gjyblzwxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/gteqzocme.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gynvkqafr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gvwhzsvsz.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/guedjjioz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/gjaaxdblu.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/gvskklcsb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gmhkfatce.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gapapjpxd.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gxqshbszy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gbcyvecdv.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gyhxowlha.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/gcqymwhft.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gvxivtuyr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gkpzuqxbp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gdapgkabp.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gytuygjpc.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gjbvsyxoi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/grqqtkgih.sHtML


<!-- 参考信息 -->