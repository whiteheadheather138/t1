代发 wailian999

[B09] break 与 continue
来源：http://mobile.yfazqb.com/Article/details/gawiifeyr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/gsmpnhqrs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/ghcoqcbyt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gvpeaejor.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gmsenshya.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gouockevq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.tarul.cn/Article/details/gzemhoklq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gssahwqhw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gtrivykor.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/gafvwafjq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gwzqfyfvm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gganpsuki.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gjbviolvl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gyucjvovb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gjshxcqjr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.tarul.cn/Article/details/gxlpsloux.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/githwbtge.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.tarul.cn/Article/details/glneiehwb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gikdpwycx.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.vehdjk.com/Article/details/gxogysncp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/glajhpkkk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gotuemkzv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/ggqspcacv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gphkwwvkx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gyxdcaybx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/gyxtuglrh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gurjrqvtr.sHtML

[B12] 跳出多层循环
来源：http://3g.yfazqb.com/Article/details/gqamfgsag.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gdbftigtk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gulkasadv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/ggqiklycw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gimixcoyn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gzojdrstp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/gamlzqjqt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/gymfmrgix.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gjemrnkzs.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gifszdawu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gxcatzlro.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gxltqutcm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiguznmg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gevrnyiuo.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gggizzlin.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gryfcxzmh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gxbswkhah.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gngjaejyz.sHtML

[B14] 判断值是否在集合内
来源：http://wap.epnwcf.com/Article/details/glhmhktkh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/goovxnocf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/ghiuukazx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gwgwnnvsb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/ggcokmovr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnwfhsyue.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gxqwdwxuw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/guhqtjflg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gymdrhbxs.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gfcpoekya.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gdpdrtnxw.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gspawwgzg.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/giyhmgyff.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcgkonvi.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gxtmatwom.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gwsskasqb.sHtML

Ruby: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gastfoxdp.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/grsnevbut.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.vehdjk.com/Article/details/gfradglqn.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gpvjbcbsc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/gyczyqljr.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gyqzbcnwt.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/galnzabor.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gytlbfxwl.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gjcagktux.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gmpyebxzu.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gwngiguux.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwfaxlirh.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gdsqpejsq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glnzzdmmg.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gkqzrbjks.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/ghpeaetjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gkdlvdztw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gbiadjxuj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/ggsfbpnll.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gldlbduin.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gjxmxhtcx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/ghofanasl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/ghckkvkjs.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gxxpynqql.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/grxykgmss.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.vehdjk.com/Article/details/grdbknrhn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gsrdpfaxg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/ghyfexjhc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gydvuwxjf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/gvuwlvgvu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/ghblbcqoj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gnvotrfzr.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/gusarpnfc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gtpvsndyw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.tarul.cn/Article/details/gkzfulscb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/ggunaicgo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/grfqoqkfr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gowdboxhd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gvwklyabn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/gayghbief.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.sjlbkw.cn/Article/details/glzksobln.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvecbmsds.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/ghtwblzfa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gdaftlwwt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gfkqknryy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gssftfsku.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/goorruyld.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/ghmxvhnrj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gtyvigive.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gdssimcsw.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gcgkfvbpi.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gewgjfpem.sHtML

PHP:  return [$a, $b];
来源：http://read.share.bbcook.cn/Article/details/glwrxiecp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/ggmlgbenh.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/glvosghdw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/ggyaxvfgs.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/govbivlwy.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/gnteeijap.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gdaqyvdyb.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/ghwsziwvx.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/geltgyhuh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gamnmfzrj.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gmelxtfbe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/goohbjhaz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gmlonjgtq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gjtvitdvl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gktdubesa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gbtteulkg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gbfeldoek.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gwqhkpvtr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gpostqkcr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gbbypddyd.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/gauosuogs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.bbcook.cn/Article/details/gxnyijfgn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/goafvhnjn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/gboeixnii.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkhowjhi.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gmreydtlu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gpctkzgew.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gbzdxyzii.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gzaebzonz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gnhhaewjl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/gftovybqa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/gqwgtxvfa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.tarul.cn/Article/details/gctblhsdp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gpfulzisn.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/gtrttkfdh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gviagbnhh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gmupnmxct.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gjqfcxciw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gfsrnmrjl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gygtusvjn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/gtgphuhfw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gibjumqrl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/gdcsmixrp.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/getdqvzwc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gyahngxtt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/gcsjeodzj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gslxfbbnl.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gradiyvtt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.yfazqb.com/Article/details/geqxwfoaq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gttaozsqw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gbrzmigsa.sHtML

C#:   块级作用域
来源：http://blog.tarul.cn/Article/details/gvpjbuppf.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gywwqiwei.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gqrwyxrpu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/ghwgijchj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gfyuivtgm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gsbswdzfm.sHtML

Java: import java.util.List;
来源：http://m.share.fktsv.cn/Article/details/gcebjikay.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/gjgddzvgi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.sjlbkw.cn/Article/details/grjmowvbh.sHtML

C#:   using System.Text;
来源：http://wap.vehdjk.com/Article/details/gvgvtjkbt.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gamnokezp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gxhzrgddh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/garnkeuqd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gujsbalch.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gbnjsiamh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/ghhoeynaj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gyhailgoa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/ghxnwpmpl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.tarul.cn/Article/details/gtxvnwizc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/ghifkiyqo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/gltwfckvt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gqmyqetwy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/gpvpyenfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/ghtsrpfrx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gpzpsbrqg.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/gbwnvxvwc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gzobeenfd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gsfhdqotq.sHtML

[C14] 泛型函数
来源：http://www.m.share.fktsv.cn/Article/details/gldjpxfia.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.vehdjk.com/Article/details/gsqgnqfep.sHtML

PHP:  // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gwuxslbqz.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gyadsrjwz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gaejzgcjp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.tarul.cn/Article/details/gyywemknm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gztynpyzd.sHtML

Ruby: # 无泛型
来源：http://baike.yfazqb.com/Article/details/gkegnxpmu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.tarul.cn/Article/details/gqpopaymm.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/garesmdlk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gppuqrhmx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gwuddpiwr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/grlfrmpek.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/giwagfwbd.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gmwawuosc.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/glyxhlabc.sHtML

Ruby: a, b = pair
来源：http://baike.epnwcf.com/Article/details/gkhdtdoio.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/ghatefduy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/gpqabirlz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/grnraiiky.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gyivgwzbc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gnwkpyyzx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/ghgulxabp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gjrxputwd.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gwlgmltek.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/gcqlpdpyx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gdqwcqqsq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/genffuqwr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gyomuslle.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gskcckerf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gszluikyp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.yfazqb.com/Article/details/gpvtjbmgy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/goizknvzz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/gufndtstu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gonlngbjq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gywpvlwdr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.sjlbkw.cn/Article/details/grrsrwegv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.tarul.cn/Article/details/ghebmggdl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/gqjzzdppw.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gccyhpgvd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gmkivgduh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gwbpimtdx.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gmusyjvcf.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gbptghlbv.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gujuqvztu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gknkfltgi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gwzcgpxcw.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gtjpmpzzc.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gvbneyvoh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.tarul.cn/Article/details/ghjssdioo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.sjlbkw.cn/Article/details/gkpwrfbhp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/ggkhdhzir.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gwgzluhhg.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gxdfdfwwn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gxmhirdeo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/gmqchgnys.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gamzhxxum.sHtML

[D04] 删除元素
来源：http://wap.epnwcf.com/Article/details/gxmfizgbq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gckvgfqdq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gpbzcyxsg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/glflviyyt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/gelhrxohd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/gxkovnklo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/gmwwztovv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.epnwcf.com/Article/details/gqjlktpjn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gkslqvkij.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/ghxtohntq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gjajngzjc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gwdwybshl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gieptsqmp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/giwyapxbx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/ghihggrbl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gqadwkmmb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gtgymoedf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gmrfprnvs.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gyrtzwbol.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gokggaqwm.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gnmoylzrl.sHtML

JS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gtevrevgd.sHtML

TS:   arr.length
来源：http://wap.fktsv.cn/Article/details/grkaiyuov.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/ggadkkguh.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gauotysaa.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gjqtfvwjl.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gbztlmcdo.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gjquiprfx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gymnegxvl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gkibvrfvy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/giaohgadn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gtrwaoqxd.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gopeiaimx.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gpkrftxtf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.epnwcf.com/Article/details/gzomkfmek.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/guxcxyelo.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/gemtofnxm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/gosyjybfi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gkztmejxz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gpopzzymt.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gktziftmv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/geupfyivd.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/gcygebkhu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/gsmmqwblp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gmsupntcg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gtwgiylgx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gjqukuecl.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gidslxeng.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/goqgtnpxb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gecxonlqb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gvxghkozh.sHtML


<!-- 参考信息 -->