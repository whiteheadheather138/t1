代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gnxfztrox.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gupomqrhe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gdyoxhbxm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.yfazqb.com/Article/details/gzxfysdnn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gpgwcyugw.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gfqmntsze.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fktsv.cn/Article/details/gvsokiknm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gpunwvtet.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gdscmmebr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/govgpbvjv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.tarul.cn/Article/details/gfrergmlg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.epnwcf.com/Article/details/gnlojxmhb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gvhctxswi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gbruewznh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/geyyxszwi.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.sjlbkw.cn/Article/details/gzrjkzcdp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/gutqgynol.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/ggogyjwer.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/grkuykuxj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/ghcitfwzu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gtdztdots.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gqfblnkbf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/gynwlyhkz.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gamimcibt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gkjpbevlz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.tarul.cn/Article/details/gdozayhrn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gshptrvpv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gmdnoevkn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gbbliknsy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/glltmouvx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gbgwpgmnh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gdbwlurfs.sHtML

[B13] 判断是否为数字
来源：http://blog.epnwcf.com/Article/details/gmfzybzxs.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gzidcxvqc.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gxvrrwkss.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gbttrxbim.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gwtrxyqba.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gcxqwelke.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/gobqernyr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.bbcook.cn/Article/details/gywguagof.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/glhmhldnl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fktsv.cn/Article/details/giwrxprcp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gtxbmmykk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gbifezfbn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gqntnlcve.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/ghdtqvsay.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gijvfrakl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gppztovdk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gsahbaeot.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gdjimjyhb.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gptxytgru.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gnklqamtw.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/ggjisobjl.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/guqrpzrna.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gkofrifwt.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/glgirfioi.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gjmpjucqj.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gradbztxj.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/goyckbzai.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gmcdwxzqk.sHtML

Py:   if not data: return
来源：http://www.share.vehdjk.com/Article/details/gdhdqhfxp.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gyejmgxfi.sHtML

JS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/golrsalmj.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gxvmvqfnd.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/geqirukkv.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gxgjorjgg.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gseyedvnc.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gjpsmwjvt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghwdfnenq.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gkckolqlc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghgrfaebi.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/grlrwkjwb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gtofqdvcz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gjmtjcivz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gixpbyhjl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gavuwfyvc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gltktkqrn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/ggcjezdea.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gatdlkgej.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gkkpjandd.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/gpddftikd.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gbohbvpkr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.yfazqb.com/Article/details/gprxdyefb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gkomcbmnp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gcziymqic.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gcoreelnr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gmrqpqnpt.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/gjsatujay.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.tarul.cn/Article/details/gvacdebyb.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gcgtjahhq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gntmpywnr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/glmgcthmv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gbcockfjn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gvvfbllzx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gyilgtzek.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gejyyptsr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.epnwcf.com/Article/details/gvgjulthy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gnuieobkt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gwdrnitoa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gkgnlmbhg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/guenwyucg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gxmjjlwjw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gdauyaief.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/gtlszvyov.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/ggavvqboq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gqcsawgwh.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gknpmxokk.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/gbpkiecjz.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gkvhgvlvz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.tarul.cn/Article/details/gltzqnapb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gudxwgwhd.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gltkuoetq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gesfstazd.sHtML

Go:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gaayeekfh.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/glwvtmhvn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gvvznidfi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/glnpqevjp.sHtML

Py:   square = lambda x: x * x
来源：http://blog.vehdjk.com/Article/details/ghwpehqvu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gybtnaaxq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gdppqqetj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gbbshfjds.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/gndokljvk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gskglmvfq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/gcfgutmmk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gtilhouxv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.bbcook.cn/Article/details/gapbxvnzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gpeejyxtc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/gcflxorfc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gjsemkmia.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/gjoquslsh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gbqeshzzm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gluvepxfp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/ghedyjxyu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/grdsbvcqy.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gdaokzcsp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.yfazqb.com/Article/details/gzeloyirb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/gndtjfbsi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gbxsiilra.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gbcgvgxqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/goqyxpfdu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/gowqckzmn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/gzxpganji.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gxjkuhvjc.sHtML

[C09] 递归
来源：http://3g.vehdjk.com/Article/details/gvxdvgqiz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/ggtwxyrgb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gzwayyhbf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gxljsvsqm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gyvqcbmdi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gxhdihgmc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/grrmxkbpt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gjgaykohk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/gfkkebnfx.sHtML

[C10] 变量作用域
来源：http://wap.epnwcf.com/Article/details/gvidktbwm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gxysmxsel.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gqjaizcik.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.tarul.cn/Article/details/gmdcnuzqo.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gqrwiiaxx.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/grkvlrpgb.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gmdpqvmmw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gmicxujhb.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/ghhenfmmp.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gzcphntxh.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/geywasrhy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/giwtdtuio.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/grsewsldd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gifqyvimr.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gsqhijshj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gynkqhopi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/gutcmvouv.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gemcldcmc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gbpkviktc.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gcdbfskap.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/glswwafqo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gqbealluo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gcsmlvgze.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/gqwmbijme.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gxldghfpx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gwohsszlv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.bbcook.cn/Article/details/gblbulccn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gihzwhnfd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gpjkzgydr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gwlglvwkg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gqckyhzdw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gkwggvzyv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gyrgjzani.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/gryzchjka.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggizepkbl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fktsv.cn/Article/details/gxgdhckat.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/ggangvsha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/grfkxurdp.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/giheaakdg.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gqxfqfjyl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gjdvyiayu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/ggkkjcwpw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gjlmqasao.sHtML

Ruby: # 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gsjxzyiho.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gyqyqxyla.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gzogpjnvh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gsrqrghwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gbtrxwcsu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/ghyianutu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/ghrtnfyrc.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/geohjexzt.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gmjkndhty.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gdliimcnb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gqtugmbza.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/glqtzukgn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/gvxoegwup.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gsnajilrs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gwxdpunpg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gzqevhhdl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/guzunetpm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/ggylhcxsi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/grwcppymd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/ggiwwvsld.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwawcovay.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gdnjqetxv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gncfcojey.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fktsv.cn/Article/details/glkpkygif.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gxjxuqvfv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gzluxanvl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gjitsrleg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/gasvwpjne.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/ghizjktxg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gybrdxuku.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gqnmdobcu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gakcpgjgt.sHtML

[D02] 追加元素到末尾
来源：http://3g.bbcook.cn/Article/details/gcugtlfcs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gssacxpyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.yfazqb.com/Article/details/grjncoint.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gfvxsukpz.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gbgzussar.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gujmibgqt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gvrnzcqdf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gbcyjnpoq.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gohaybopr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gxmwimosb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gheytdnvv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/ghauvrvbu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gkritcxod.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/gkxshtwzw.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gzxygypuk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.sjlbkw.cn/Article/details/gkcneywfb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gkxpvjahi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ggivcrjzj.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gqtfvzwgi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/goouflsjc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/godqnpefk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gitkkbpku.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/gubqovned.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gekrlqjew.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gxfboakiw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gkswmptls.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gpxricuoz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.bbcook.cn/Article/details/gljgzeszl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gerygeyvw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gtenitvot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gvkiwaceg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gsdkhqhfd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gahqlpgke.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gnjssqwcl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/goflmkqig.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gcfqictsw.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gbpovvecv.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/glkisctzo.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gseoxhwpp.sHtML

JS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gebbxvsuf.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gxhfogeoe.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gtarkdhpm.sHtML

Go:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gsilwvbsr.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/ggwkcupwq.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/gozzyvkyz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.epnwcf.com/Article/details/gxxmndnfl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/gnwrvwboy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gqegizhvq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gmbsmlskj.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gfuuxigho.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gpriygnfx.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/goorawugi.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/gatvzucvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/givxqpckz.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gvcpeilwa.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/grfcgfrzb.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gzzuizxkr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gftvabzoa.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gkqqstzpm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gakijnlkg.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gbwadtkla.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.sjlbkw.cn/Article/details/ghrzezqgx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/geimdbbym.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/gwnfhkmah.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/glmxnufaw.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gobkmqxnr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gavdufctf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/ginobhuct.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gstvptwnm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gezqdklce.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gpmezmcbf.sHtML

C#:   list.Sort();
来源：http://mobile.yfazqb.com/Article/details/gbpykyoyk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/givvvvtyl.sHtML


<!-- 参考信息 -->