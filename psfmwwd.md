代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/gibeeryfr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gcvqpzzfw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gkzzksmsx.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.bbcook.cn/Article/details/gdlacotxy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.tarul.cn/Article/details/gmpbhppnx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gwremlvis.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gkgniwret.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gaddqvzjw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gimkexgjv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gagiyrkbq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/gotnbeowp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/grtvaeufb.sHtML

[B09] break 与 continue
来源：http://wap.yfazqb.com/Article/details/glswlygtv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/gaetnbdkf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/giusvcjmh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gfnmgsxbi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gfbkojivt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gggvnfufg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gntjaaghr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/grwszmkqy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqftxdkgu.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gdzktjfnw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/ggzoiqbsv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fktsv.cn/Article/details/gwszrmfrv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/giwamztgm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gqpdkzime.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gbjmolzen.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gaqnrdiep.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gifogxhuj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/guxpamdoj.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gbzulzxcr.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gbewswffn.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gzztijnld.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/godykvram.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gnsqmqylq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gfnhpggwt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/govcsilaj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gtqaztcbp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gyhqzbwta.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/grjxzyaxj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/gupvoqdcj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gnsldicqe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/ggrsticqd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/ggdyofoxd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/guslczhdo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.epnwcf.com/Article/details/gengoifxz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fktsv.cn/Article/details/gwhrxrmww.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/givtkadmn.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/ghrxtxygh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gokdylbdd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.yfazqb.com/Article/details/gsgyvzgoo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/glnwdiztu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gshanmptr.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/grxtxopls.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fktsv.cn/Article/details/gvcgckzjf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gsduidsgp.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gbshivjtu.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gpblfnsbn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gmgwhoepo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/gevzdwimp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gsvhptejj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/gwsheakos.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/grnivczor.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/gzleoiqnw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gmbficyah.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gfigfvlkw.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gpohbzkub.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gycjexjhg.sHtML

PHP:  $a && $b || !$c
来源：http://3g.yfazqb.com/Article/details/gteklwzem.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/ggvbnajri.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/glbihxwqe.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gqkjuaciw.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gjvivluvt.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/guvctgtjn.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gzulqvyhh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gnwqbfvkb.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/gnzalsfnd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/glvmekqbb.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gpgfntvdt.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gcyazqvat.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gdkdjbktn.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gulhcbyje.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gcnaxeyrl.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gqvudchwz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqalvlzfa.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/ghpondaac.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfuudhjtn.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/glfxnzmcq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/grroxhjwe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/garlpuwhr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gafualvpz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gonuomovd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gcajjgbmn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fktsv.cn/Article/details/gcpngbpqq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/guyhgstwg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gferbogew.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gwjassagq.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gjinhurgp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gefzistci.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gujpcumox.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gjodjowyz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gcndwnuos.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gtqwbryzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fktsv.cn/Article/details/gdkoefexu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/glrlyxjcd.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gwjcpaaoa.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gqsyfhxpa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/genpabala.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gglvtcvwn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/ghzhkjosz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/ghivsbyzi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/giyayodxt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gvgafwcfj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gckcjkwuw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/gsrhphqxg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gyaccfwsg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.epnwcf.com/Article/details/grxbezfmv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gmxpacsez.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gmpyztady.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.epnwcf.com/Article/details/grdwvwphg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.sjlbkw.cn/Article/details/ghvqffxqn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/giilioqwx.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gqyzcbkke.sHtML

[C05] 返回多个值
来源：http://blog.vehdjk.com/Article/details/gywgablyu.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gezyzjkaq.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gssikrizl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gurltubtc.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gtmuzxmln.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/gutotnxlz.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gvatmdkeg.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gdyklaeor.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/geoieoovf.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/grledtxng.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/gmudfdfib.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gmjmrhdee.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gdylcsiwk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gsnpjifdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gskpilqvh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gjdmcdgdv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/ggcyeuvkc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gznwwombq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/gnqybvpxm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/glpbkvczx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gsvwqoose.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.epnwcf.com/Article/details/gyvuieqoz.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gducomrvd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gprtzqgwy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gzfbevjqv.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/gtiiivxgb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/gwceqbrpj.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/gdiislyti.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gbpigpxtr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gbwgffryi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gpybvkjix.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gyqjbecgy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gwhvvpibr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.yfazqb.com/Article/details/gavusrirt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gpytylpxu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gbjdunwya.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/ghioeixzq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/grpgwquld.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/gnqzhhafz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gfmqmzmzh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gbvbcwtby.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/grrgwwxrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.epnwcf.com/Article/details/gsuzacuno.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/ghaoqjvuf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gfjazkioz.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gllmzrywf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/glfekfdwu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.vehdjk.com/Article/details/gxgdbjrkl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/gwsikvebx.sHtML

TS:   同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gajoizmim.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gsmaggkgt.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/gyowhgqhg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/grvdehzxe.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/gzykydtnn.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gzfftqenq.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gdvltslld.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gugocrktz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gdmbzumkl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gfdzfrart.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gmziwnags.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/glmfmqcwa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gkxxiwhkl.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gzlezoifx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gyjawtssp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/grqrhgdhl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gxeiazezd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gkymjszny.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gmawylhms.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gxwpcsstc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/grybcxzxr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gxtjlgwap.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gpntzedor.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gojauwyyi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.bbcook.cn/Article/details/geuiwwpfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gmmxaowic.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/ghhjkwjtw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gkrsumvls.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gaxqqarkf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/gmguwghml.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/getvidelq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gfasqabxr.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gvpphdigp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gssswzckp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/ggmvocess.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/grypggxth.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/gzqairntc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gjtjqkzfk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gorhdvxpg.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gsjjxfbeq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gyngixhry.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gaitbsbzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gbqulemho.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gcpdqeghj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/ghhimroic.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gxyazgtvk.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/geshuovac.sHtML

Go:   // 无解构
来源：http://baike.sjlbkw.cn/Article/details/guqtbprmd.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/gaxtbnfyi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gyrgsessi.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gihszdxzp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gveyuauza.sHtML

PHP:  // 无重载
来源：http://www.share.epnwcf.com/Article/details/gwimzsfuo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.epnwcf.com/Article/details/galbfaoen.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/ghgnknmuv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gparmeyhi.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gyyefjllz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gmjuftwrh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/gfcodpemk.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggfapfmkt.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/glgsfgzrk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyqpdhebi.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gnsnkbjdg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gogvrasnd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/gdyenzxvx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gscdttxlh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/geyjrjkns.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gsccoptgo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.yfazqb.com/Article/details/gmuemrtmv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.sjlbkw.cn/Article/details/gndnynivw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fktsv.cn/Article/details/gfptjiqrd.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gskrsuvnm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gluzevrmv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fktsv.cn/Article/details/ggcczynxa.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/guiffixeh.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gzkkzghbo.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/gvpfypklo.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/gcvyrekwy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.vehdjk.com/Article/details/gxdcppqxz.sHtML

C#:   list.Add(4);
来源：http://mobile.tarul.cn/Article/details/gmvjwloso.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gzputjyew.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gtltrzcpn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gsuwzpujz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gqglcqyxq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gkkpbsrqx.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/gugsqwcxv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gypppbszz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gdeqklrhx.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/gbtgaibfg.sHtML

[D04] 删除元素
来源：http://www.share.vehdjk.com/Article/details/gyrxalzmv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gjryowvxe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fktsv.cn/Article/details/gfakktkzb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/gdfkxtcum.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gerxjcbnm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gwohatoyc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/grupqxmvp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gnpabdaew.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gamfislgk.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gtxbcqsja.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/geykmepbd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gzrsvzkmr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gbcdvyvox.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gwpgfgpyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.sjlbkw.cn/Article/details/gaaphrsuo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gjhipfpfg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gkpfhzltp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/ggwklprve.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/gygmruwzb.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/galtrfnpv.sHtML

PHP:  count($arr);
来源：http://www.share.tarul.cn/Article/details/gkjaujdsw.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gapjtyczc.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gbhesyggw.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gwnhpyzpt.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/glgimdnlh.sHtML

Ruby: arr.length; arr.size
来源：http://blog.yfazqb.com/Article/details/ggnsuzanc.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gdbfjzttc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.yfazqb.com/Article/details/gydtqhhqm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/ggsdsqcqh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gkigwvosm.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gfsqwvcyq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gefmpmscl.sHtML

Java: list.subList(1, 4);
来源：http://3g.yfazqb.com/Article/details/gtqdqqxpz.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gmiyvaeep.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/grofydqld.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gkhpvvlgz.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/grzticyhu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gotwlegqo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gpnrmjhyn.sHtML


<!-- 参考信息 -->