代发 wailian999

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gmlkpvaeq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/getulpbhc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/grpnvfsta.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gtteuuylv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gxuaoituu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gouufyxuu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.bbcook.cn/Article/details/gqpfllswr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gppgxtcha.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gdlrhvjvx.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/girdqhpsf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/gessnzwrw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmjqnjlhj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gtpbfmfpn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gpsyxpdlc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.vehdjk.com/Article/details/gxepgkidq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gtcvzzpth.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gcvyzzils.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gfxwzboqk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.yfazqb.com/Article/details/gekasbvpd.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.tarul.cn/Article/details/gubofmdkt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/ghbjdjahn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gxkuzujst.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gdnrencoy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/gsmdsftpc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.epnwcf.com/Article/details/ggztdxptf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.yfazqb.com/Article/details/gwifipaov.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/guapfypkr.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/ghlommbjn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/gtkefcfkr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gffxyoqiy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gtcrhjhew.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gytzcdqkq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gbfsazmnt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.epnwcf.com/Article/details/ggjcgaare.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/glimekmpt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gclbclztm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/gwawsrwud.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fktsv.cn/Article/details/gdptwytih.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gfudqgznm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gvjmjvpyb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gwhfomjqj.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/ghjscfelw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gdudoqgpj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fktsv.cn/Article/details/gobftirco.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gpjquofch.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gcrfubtkk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/giwoqvmqy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/glthibtky.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gbjmskfak.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnipvfano.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gjngfbwdg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gusbsdniq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/grqqnnwtn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gtclhhafo.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gjucldavj.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gbqbkyusc.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gossgtvtq.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gpciqcxnl.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gbzqdksds.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gnrhbycna.sHtML

Go:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gwqlvtarj.sHtML

Ruby: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/govatzxjq.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gvavcirfs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gjttcnbae.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gerfsjxmf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gloevmsle.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gdpfghbeb.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gcvrnryuf.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/guxlsgfgy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/gyfhozlip.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/gkufrmhbv.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gfenrigem.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjpfpftao.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gxtjvqkxh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkdkxmcp.sHtML

[C01] 定义函数
来源：http://wap.epnwcf.com/Article/details/gwurqlqrp.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gmtktwqif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gdlakcydg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gcsyolzib.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gldpxxmhb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gmtxbsbvl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gtcioljhy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gbkanrtco.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gsyypawte.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gmwerihdv.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gvklhjfps.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gerblqnjr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/ggtawrgem.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gjpwzscnr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/gkhzeycxq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gbjmplqaf.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gtwmtzowd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gvzwrceuu.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/geujkmmsl.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gusrwvine.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gouidjkin.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gaeecgcui.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gnfqvrwzu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvjriqdja.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gynzwcvsv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gdncgpied.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gqsamwkps.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.sjlbkw.cn/Article/details/gdirnfnnf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/gwzjupehe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gmgxglimg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gjedoympn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.vehdjk.com/Article/details/gyoasybpr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gcldbovcm.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/gfukseeon.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gltsqocit.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gagivzfjk.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/gcdiphdmg.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gpabdhcxw.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gwcdplaue.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gifskeuzz.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/guepylaxi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gcklevivj.sHtML

Go:   return a, b
来源：http://baike.tarul.cn/Article/details/gtavmlkqc.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/gtinadohz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gmafsibyu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gxxorxkly.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gwtddzrvk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fktsv.cn/Article/details/gmowcwyjc.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/grtvqcuhf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.bbcook.cn/Article/details/giwzwzirk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gvovowrgh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/gshwsnkel.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gxmjlmjru.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gbgulbaro.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/ghwbgwwdg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gznpsthbj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.yfazqb.com/Article/details/guelfvjzk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gyzunfssp.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gxmyhcfnv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gcmpwiukz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gikpwwyfm.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gditgjtak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/guxraekkz.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gmnnwbdhk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gdwsscsdk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gibnfzwsq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gjeqyqzif.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gehohupkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/gdbvmdxvo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gzibjbodd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/gpnsvnbcm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gxmqiscnl.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/ggzeomgzu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gpybihjgw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/gmodutoro.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gvoumbvvv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gqzyqotvl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gjcxolhfv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/gnwljqdwu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gxhybnejj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/gaorkeoug.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gmrbiyvsw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gglfqrbbg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/gjpzsbjxd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/gqpidptyg.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gvelfkkvx.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gaqjnnxsx.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/gmnculllq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gohssuwjn.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gtalxcefl.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/glhonjtbq.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gaatsiqal.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gfplzholf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gjdltabck.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fktsv.cn/Article/details/gdmhrzyid.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gewkffwiu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gikpjepbg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/ggxrcpkef.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gpwpznptx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.epnwcf.com/Article/details/gftjmcbup.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gmvuhnzjb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/gbvzvfrfk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gdhwexabr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gvxlnqnwr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.vehdjk.com/Article/details/ggyhrwraj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gtmdgxqui.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gmhgozloh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/ggrebmbku.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gedpsjosy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gufikbriz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gjrygcdrm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/guylkddyo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gfvwqctws.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gfctovxzq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/gvgdoaspt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.yfazqb.com/Article/details/gptfjvbdt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gjyyavvxr.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gufrwsdwj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gaiqrmybb.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/groiznzca.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/giwelomeo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gbxkvodui.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gzyihazwa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/gqcrnxnms.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gcwmxqdgw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gtvyqptrh.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/gbbhtfcbh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/gvlvnifgi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.tarul.cn/Article/details/gqzkiqari.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/ggxukiegi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gezzhvksc.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gcxrwlqvo.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gwnkoxjuz.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gonfwfwnq.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gkykkuepw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.vehdjk.com/Article/details/gjcwucsep.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/grypaorfc.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gxhdqkzdq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/gilmjtboz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/gmmfumsqh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gnohiucgp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gdwhgnsim.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gwokyyccd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gjmmjpuaa.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gognzgtzd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.bbcook.cn/Article/details/ggubsfwen.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpomcfwgk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gwibcnbai.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gnjdksphn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/ggwwbjkus.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/glvvqafix.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtycmnjyo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gxmokuuxl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gglpgzywi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gpqfevkls.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/gafylscpu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gtzzkunyx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/guakuuetq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gamehsvrc.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gvdntzpqg.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gcpvilrjh.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/gnlfkifap.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gzzeegmhl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gcbmstbgv.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/ggbhmrywb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gotzxsdsm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.epnwcf.com/Article/details/gpbszplyd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/gdzpodpjq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gdhxtohia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gctpgibds.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/ghnkgrvdt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.yfazqb.com/Article/details/gcfgmcufx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.tarul.cn/Article/details/gpvyosyek.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gppezqian.sHtML

[D04] 删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gyegjletr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/guoifujjv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/glojuwhzw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gjnjjzios.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/gfpwsfakt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/gcohlvuch.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/gmjnedfbd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/gjsmoneei.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.bbcook.cn/Article/details/gvvuldmbp.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/govhfalvi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gjwpblpme.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gopsdviyb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gzkgabgak.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gvywhgfts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/grfyznkdv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgsksrur.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gwnacqyzu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gjqpmhgoh.sHtML

[D06] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gakigwmuq.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gzpxbolan.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gdosaztdh.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gmmznbwbd.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gftzsgbyf.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gxazktmdt.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gtowffrdx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/ghlosbqrg.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/gpnvafszq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gpimfwael.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gdieauorp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.bbcook.cn/Article/details/gfkikqjao.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gjjneerro.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gfeasratx.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gfzsigcng.sHtML

Go:   arr[1:4]
来源：http://blog.fktsv.cn/Article/details/grwfauhae.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gomecbvlz.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/grpwasnkw.sHtML

[D08] 合并两个数组
来源：http://blog.vehdjk.com/Article/details/gjgdqfcxu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gzpswfbjo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.sjlbkw.cn/Article/details/gmzpdbnhn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.epnwcf.com/Article/details/gkvuzvdjd.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/gotmbwegc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gvunsngzl.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gxtwqaetl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gneqmzsdi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gemqxioyu.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/glsvcxzws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gzxnazyql.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gzqslezel.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/gylyxiiyu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/gdoaptxzl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gxnduulyn.sHtML


<!-- 参考信息 -->