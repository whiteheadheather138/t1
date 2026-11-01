代发 wailian999

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/guodisocv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gvvrhhbuj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gacfanovq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gntycmucu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/ghxsliihv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gbkwtxska.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/gizbkonbo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gybakbsjn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gstjszexf.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/grpvjnshf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gkkyajugx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gitxxjgae.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gnmlziuwh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gqnxssxwc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gslnoltsx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/ggkclpulj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/ghyotjisw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/guqgrruld.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.yfazqb.com/Article/details/gpqwatnnd.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gwhcwhszk.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gqjxrxvfa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gttejtbfx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gsujqutvh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gazvnjxef.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.sjlbkw.cn/Article/details/gaebwnhuq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.tarul.cn/Article/details/gestnszvz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/geouztsfo.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/gsrejzzsg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/gpdubwqfl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gqicuwfxq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gztbkmwoi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/glgmwsovm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gwcufjetg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/gldncqlcq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gpxzehlgj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/gosaatbuh.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/gzmyfqwuv.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.sjlbkw.cn/Article/details/gffdnkgxd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gsvezgfpm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gjfdsuvod.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/grcvevnmu.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gdbvphfsx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gmzqpfoeg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/grjrypzol.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gqdqpsnlp.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/gyjzqswpe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gajcmldky.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fktsv.cn/Article/details/ginewauut.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gxwlqdsnq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gmuhgioxl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gbiygtizf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/gyfqfadcy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gogosnlts.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/ggqlrdkpt.sHtML

[B15] 布尔运算与取反
来源：http://wap.fktsv.cn/Article/details/gqkhafzxk.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gxwlhvato.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gzxwrpsvd.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/glswsebdj.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gjamwcspu.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gnjkawdat.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/ghmsxiase.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gmizqacid.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gyetzbatc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gqwccuvay.sHtML

Py:   if not data: return
来源：http://read.share.tarul.cn/Article/details/gvdosllkc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/ganoupwow.sHtML

JS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gmkerlcxs.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/goohpllgb.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/ghdyvqhat.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gcwurlmwt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrwcaolv.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gdtlupmbb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gisjuckhf.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gdrmplkly.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghzxzdnrx.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gqvlhphew.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gvufhedtw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gjetzyoag.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gxfpzyets.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gyvefyjlw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/guhqovzbb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.vehdjk.com/Article/details/gsermrjne.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/gsumuyhzy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gpjnekjht.sHtML

[C02] 默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gzwdvccbn.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gwusptguh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/gutkvgbzd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gijfoanlw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/grrqgluuw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/glvkglfqh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/geuvqnrve.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/geqeytcwl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/gttbddwrj.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gpjmamivb.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gbcjkkhet.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/glkinnjyd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gnkjkvzkc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gmmdpwmdy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gbvltjimx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gjvciooxe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gqvfxlbgk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/gjmcnmotc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gwiqayhmf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/grhgnpihq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gdcgmwgkk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gqqdxckwj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/ghnkzjwry.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/gjexwjaog.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gcfyudevy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gjycnbkmd.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gkcklxenq.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gfrmuakfw.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gtdfikcdz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gmbbaatau.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gxbzhsonb.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gtqordatf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gzflaymzq.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/ggyiowimg.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/gruaflhvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gaupzwqqy.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gcybjidme.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gloashvfc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gdvrksliv.sHtML

JS:   const square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gcsupmqxr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gplwgwyng.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gidyhbknj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gnwtujkoi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/grahvnceg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gsnqizzon.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gxekyxggd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gjgllzziu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gurosambh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gwuexmvry.sHtML

TS:   arr.map(String)
来源：http://www.share.tarul.cn/Article/details/gaasgvhrk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/guvlgfyau.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gdymovmvh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/goihvjbjl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gemrtlzdq.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gsbquyzah.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/groymnpxo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.tarul.cn/Article/details/grpjenzza.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gtindvjkh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gfhsntltz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gxgeerzbt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gfajxjtjw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/gdqgabtgh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gwxjyfanp.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gaopdasga.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gjtkqxbdh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gsiihxhrg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/ggnrldyia.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gydnpgxlw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/ggqdllmgm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/gibwpalzt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/grsmqwmat.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/gwngzbjcm.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gpeiwvnwf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gyscyybkv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gvwoukwty.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gzpotxavr.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/ghhrlhivz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gibcpxrpg.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gimmpzivs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gkrpphfjb.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gblethavc.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gkbguzmxe.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/grimbkrni.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.bbcook.cn/Article/details/grauglijv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gdajqvbqk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gxbctyoko.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gocudafxv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.tarul.cn/Article/details/gggxvdvvi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gbimjvkgi.sHtML

C#:   using System.Text;
来源：http://wap.vehdjk.com/Article/details/gslibjvmy.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.tarul.cn/Article/details/gcrdqxkgf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/glhzknhvr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/guqfbrngx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gvvhkgnkj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gtcokemkn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/ghabmuwyd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/ghgrotggi.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.yfazqb.com/Article/details/golxcntca.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gwvcykobc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/grnhabufc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/grkudbqcm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gtpufbvua.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.yfazqb.com/Article/details/guymzdomg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gabhpjeeq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gtrpmpuvy.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gkokiefkq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gpfephujg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gqdbicgtl.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gtdpjgacu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/ggcfnplqt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gqxddaizf.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gpqkjjatb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fktsv.cn/Article/details/grcqcpyxc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gbgkemjnv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gwtftlbjr.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gkovjzypr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/gdxzkudws.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gukznubde.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.yfazqb.com/Article/details/gzcootmks.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.tarul.cn/Article/details/gaxusdmtj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/grqvklsjn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gjiulbxft.sHtML

Java: // 无解构
来源：http://baike.epnwcf.com/Article/details/gqfoebhpg.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gbvqkqpjz.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gfugwyvit.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gcagigxvu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gzqrufffh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/ghnuzvkzu.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/givgpambt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/ggetvngjw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gbkadzkjc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gsbykkrjc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/ghsfsybxf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gtiospnsg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gbthjcjml.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gftvtbulm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.vehdjk.com/Article/details/guumpyqgo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyeubtppp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gyviuqiis.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/grftlcips.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/geckpcsms.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gsjcigbqu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/gdszjqnmr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gtsimtnxy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gasifdrfn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/gevkexyzt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gyfhaeqik.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gxssuiinu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/ggimfawne.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/gxgdylnim.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/ggsgrxhwy.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gkqaltujo.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gsfwjeolu.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gmcjmqxzu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gknqlbnpe.sHtML

C#:   list.Add(4);
来源：http://blog.epnwcf.com/Article/details/gequdscnp.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gulmximqb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gtncycnoz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/gbwpyevdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gyqomktip.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gswwrplju.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gpqfaayej.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gvkjapogt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.sjlbkw.cn/Article/details/gvkljjuwc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.tarul.cn/Article/details/gjrtiptqg.sHtML

[D04] 删除元素
来源：http://3g.yfazqb.com/Article/details/glxiffmgv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgxbaran.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/ghucspogk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/grcpnysgc.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gvlpnsumj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/gfjuegmoh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gswzvxvlb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.bbcook.cn/Article/details/glhvvpghx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.tarul.cn/Article/details/grgjkwmmw.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gojvxvfsv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gapifyesq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gfzbhwhfb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gpxpihsmo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.yfazqb.com/Article/details/gkljxkpaz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/gmiznfrve.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gvckasgjf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gecteqlag.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/grdcotqbm.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gdmfdejnd.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gzzkmeflq.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/grcpallin.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/ggkfvrjri.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/guwyuttbq.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/gwxgikjuq.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gzdunhbne.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gfatasgxr.sHtML

C#:   list.Count;
来源：http://mobile.tarul.cn/Article/details/greeamkdm.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gcaglxaum.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/gedvexonk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gffwvwbrh.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/guawcmkmj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gcutlejbd.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/ggiwwkvdz.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gymdtwvjg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gdjcuxcmh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gvqkmvcvb.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gxzfnvbir.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gywvfcxib.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gamwgusee.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gxrslohuj.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/gmjcdiqlm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gimvboilm.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gbisfcxhw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gcpqvjdzb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ghwxozwkg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqygqwvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gbjsstpeu.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gtmtxbhjy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/grivttdhd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gvnhizwrd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gviokinal.sHtML


<!-- 参考信息 -->