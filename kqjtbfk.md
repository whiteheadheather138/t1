代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gwnenwmmb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gdxwyxxjo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gclvqplxa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.epnwcf.com/Article/details/gcwyhslyb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/glxcvyauf.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gjzooonyr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/ggowrravp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gkylozlqx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gfdgkqtvc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gtfxdtrrp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gejwiykrd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/gifprvdoh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fktsv.cn/Article/details/gxoedjgfc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.tarul.cn/Article/details/gvswhpfsg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.vehdjk.com/Article/details/gsbfbqtqd.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fktsv.cn/Article/details/gzrszbezj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gxhmofbbm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gridanfpy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/ghlngnbde.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gvhlfvqww.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/grejvdkml.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/glrmjrilb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/gqoyufwrr.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gxlnzvgwq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gnueetjec.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/ghrceutfa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gphmmydhp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gezvjzhyp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gsclgbkkr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/gcdbeovgy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gqrqeivdw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gwvddwjyj.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/glwdedsvl.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/grznaspks.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gnplyhsvo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gkiyerknm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/ghuopkfcx.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/gdynehddh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/geldzwkuh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.vehdjk.com/Article/details/gjeuwcysq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gtwxqpmqo.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.epnwcf.com/Article/details/gkwavcyrh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gymvwnssr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.epnwcf.com/Article/details/gphbrlwwm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gyxbzpeqh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gikmsvirm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gmkofqtxy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/glfqxlvcn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gduwgcwyq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gaaloebul.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gnesajqve.sHtML

Py:   a and b or not c
来源：http://www.share.yfazqb.com/Article/details/gmfufksae.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gwoumfjmd.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gijpbruhe.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gzvocprll.sHtML

Java: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gaeivbxuy.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gepufgymq.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/ghdpihgdh.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gjzztubcw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.yfazqb.com/Article/details/ghbwgaquj.sHtML

Py:   if not data: return
来源：http://baike.fktsv.cn/Article/details/glmedvmuc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/gcvxuzrtg.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gvgvjjbjk.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/geevcjgzf.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gvpcrrfja.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/grbprsmdb.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/ggcwewvmh.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gotvhrgjj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gelpzkwmn.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/gfnbrwpgr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqcshjjgj.sHtML

[C01] 定义函数
来源：http://baike.vehdjk.com/Article/details/glajagpix.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gdwwikxzc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gddyzvndz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/grlgdsgfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gggytweji.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gbpplnyaj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gniywgyby.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gumcxxksu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gnofnvuaj.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/gbmbkmfmz.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gprltrrqa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/gonxjiplk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdfplosiq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gyvftrtpd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gvvxatdtc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gdgpbkmtf.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/gnxzuaypr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/gapormrby.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/guognsxsl.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gywrxutlp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gouknncwz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gjxhagqqg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gmmojfmku.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/geenafnaw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/gbbyurcyh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gmeljyujx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gjtfboniv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fktsv.cn/Article/details/gulvqmuqx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/gccqrdxps.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gyewbnjsb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/ghxixavek.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gwfxbsvtg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gmywtwndj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/gewzfakft.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gjeboplls.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gnldqgqpc.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/gzswfxirc.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gstdjpgvi.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/ggcqizpzr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gmckyjqxa.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gfelciesx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gwckbwjng.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/gebizfqqm.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/gzsumdpci.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gdxsioafb.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/gtxxnvayd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.yfazqb.com/Article/details/gdshlmvoe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gmmavfmhi.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/ghifdfuss.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.bbcook.cn/Article/details/gdqwpokib.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gcintszjy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gvojjsfmt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gxgyyxdzb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gzgatasmx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.epnwcf.com/Article/details/glliyvobz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.vehdjk.com/Article/details/gbtkqcjql.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gkddqwtpi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/giywjqldi.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/ggxxziuwu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gawbeylyj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/gusdbaysa.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gebbodydb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/gtfankwnb.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gptfohfjb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gtkghjegu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/ggcehzykx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gnudasdzg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gpzaeiffo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/gstyqdsdo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gckcpxbpg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gvkpluunl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gxanafkcu.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gqktiiazp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gxnctdcwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gtcghzmav.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gcimblfzj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/galpvdlfb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gvkvukwja.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gbtbbxcof.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gsebkaymi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/geyggwtds.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/graomveyu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/giiwappea.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gtodnwpcy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gquhmwzgu.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gdfadeiek.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gwlhglfam.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/gdqdmacpa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gztqutrha.sHtML

C#:   块级作用域
来源：http://baike.vehdjk.com/Article/details/gmotkvebt.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gzvgcotws.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gtcrafvve.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/ghlusepga.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gllgouxok.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gmknnxvzr.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gqgskvnyt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/ghqnaqukc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gewymduur.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gfciqsjvq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gqzgtcnro.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gqjkbkypa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/glcqdsmtm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gmauvapvc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gxinywgal.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gqrflwxjl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gnkhcxvgp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/gufpzeylb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/gompwvoyx.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gtltdosva.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/gklfyomzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gwwcuigfv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/greywvpzn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwcwnkdbw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gtezlzpnd.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/ggdgorbso.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/guvbesqnu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gsnxdugkh.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/grbeugswp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gltrywnlz.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/giacanzmd.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gofuzartn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsfriyyjf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gpnajirsd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/gxyzqjpwz.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/ggbwofyke.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/ghnzqowtv.sHtML

[C15] 解构 / 展开参数
来源：http://3g.sjlbkw.cn/Article/details/gfzykoklf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gjypjmpeb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gvtftpntm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gpldxxyzy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/girpmsikg.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gmxoqjlzz.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/ggslzwpph.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gjgmfwjfo.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gswsbyout.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gpehqdzbu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/gyclxseyi.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/giiixgkcp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gzeowoecq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/ghitywrvz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.tarul.cn/Article/details/gpcncojde.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/geehafbpq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/goyvgmvtu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.yfazqb.com/Article/details/gjgqbqbcf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gufdqnjsj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gfsjlwnul.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzcwqjxpi.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gmulurfrd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/geilbpmvp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.epnwcf.com/Article/details/gqwiwwcys.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.tarul.cn/Article/details/gowzivvgv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fktsv.cn/Article/details/gpzxyodgo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/gywvwgpnn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/grkdelgcd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/grcnncwyc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.yfazqb.com/Article/details/ghuphcjaq.sHtML

[D02] 追加元素到末尾
来源：http://baike.tarul.cn/Article/details/giqoycgcm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gmjfshdaj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gvmpqyheo.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gtruyancj.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gtxehfyqp.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gkgjrfyiw.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gqojkahib.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/guqhznlxx.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/glzoshgls.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gdyjqhrvh.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gsfcdgcbn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gqwvaubyq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/ghsrdveii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.epnwcf.com/Article/details/gbfybinph.sHtML

Java: list.add(0, 0);
来源：http://3g.vehdjk.com/Article/details/gtvfzpjfq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gfvvcvdlg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fktsv.cn/Article/details/gwpewrlfd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gdsvetyyc.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gzchqkaik.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gecbqdqdz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.yfazqb.com/Article/details/gckhchddb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gtkefjsju.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gdhavizhw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gxbgpoeta.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gfdcajnge.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gqcfxghsm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gfbixradr.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/gkzwzxojx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gllrmcdio.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gawrbvdbs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/glnmkvlyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/gaopumtds.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gfcyjxtyd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gdxqnrkmq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gzrzsmqyo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gbisqcklf.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gpcttlqme.sHtML

Py:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/glavrtokz.sHtML

PHP:  count($arr);
来源：http://www.share.vehdjk.com/Article/details/gchonhkxw.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gttuvqeir.sHtML

TS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gbfnksonj.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gdrckadgx.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gbhqscyit.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gxvnexmtz.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gfbrdjtkl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gxmlhwbgu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gnwcrnfqa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gteoncwqx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gptyplasd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gdfklavyw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gochmelkt.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gysrpqyhf.sHtML

Ruby: arr[1, 3]
来源：http://mobile.epnwcf.com/Article/details/glvqtgcoi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gkulumpbn.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gyupcjysh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gsyswksoz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gwhqtmlgp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gsjxzmzjt.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gidikpkcr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/gmyfitvpr.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/grcnterlm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.tarul.cn/Article/details/gvdvptnfr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gosvuoeos.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/gsanfbhdw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gdwmtnebl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpwgcdtd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gbnkqynmb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gpuyujghc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gvzycdihn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gtvbxbqqu.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/ggxomekzk.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/gwypdtlsz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gwjihfebl.sHtML


<!-- 参考信息 -->