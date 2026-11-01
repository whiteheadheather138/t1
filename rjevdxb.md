代发 wailian999

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/gkepmhewa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.bbcook.cn/Article/details/ganeuwrbw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gweebfujb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/grizirqqm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gxjkznnju.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gsfeqycmh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gpvzagaja.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/gzrpnqfov.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gvjoansrv.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.yfazqb.com/Article/details/ghumugjjv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/gyplcgwul.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gvqxkizyh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gqqeztbtb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gedhsggsa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gvvrkiszz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gicmgtnbd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gwbhbnack.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gypkoxgve.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gdeqslewh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/gkujzgwjv.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.vehdjk.com/Article/details/guidffjpj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/glvdlqwsb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gfgavnmov.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gavhdylyh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gnhsrnptw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gatzqouza.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gnpmyuteh.sHtML

[B12] 跳出多层循环
来源：http://www.share.epnwcf.com/Article/details/gxksrbkjz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gdkwzkbwh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gyvszdpen.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gmamcvlfg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtvzpyni.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gdsjoyhst.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gwvalfkzh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/glghliqln.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gmonamhxr.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gcymhixbv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.bbcook.cn/Article/details/gnrcdufda.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gsrngwfcu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gipdcbpsf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gxitvijac.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gnavvfddk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/grvoqebtm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/gpjajddad.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.epnwcf.com/Article/details/gvzfitggf.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/grltdddhf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gjzuhrpda.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gxgikeond.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/ghssqwwco.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gokqbvqei.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwogvvvmm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/glwodvfhz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gfbftocpr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/gsdmquxxi.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/ggbvmfcoh.sHtML

Py:   a and b or not c
来源：http://wap.yfazqb.com/Article/details/gdajgosll.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gidzlnsbf.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gfeehdrbx.sHtML

TS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/glzuovlni.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdiurtta.sHtML

Go:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gbgqwwfjy.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gfdaembgg.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gunykaqxe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gmkyjutwk.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gbvqcgqqf.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gbvfycrsq.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gibthyhhn.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/ggtmjyoyo.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/goojmckbe.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gmpcaojjc.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gohaaxcrq.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/glbiofbdu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfwjqctxf.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/gctzpiemr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gaokjuycx.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gbegbfanr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gjjigtrse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/giagdawms.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gbyxxrdaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gfzmjffnx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gqattnzqo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoxuzrmo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/ggwjzinvn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/guuepkbmh.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gnuwhwath.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gxupohaid.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/grhmyhyvu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gncewpdny.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gtjjdjpyg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/ggryutwrr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gxlcnkype.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/gwtbxepzm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gkrbhqgft.sHtML

[C03] 可变参数
来源：http://read.share.yfazqb.com/Article/details/gkwkkjutf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/giadchxqj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gmmuzqkmu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gxuqexjxp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gyzczfkwn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/ggzymhttq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/ggflcqqbr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gpztiazmn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/gpejjrwfw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gzfbqostc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gbqvjderp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.bbcook.cn/Article/details/geaqfoyaa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gnqlgsljp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gfkqrhwcz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/glgkumjrg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gqdutlhas.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/ggevffalo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gncebqtcc.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gzinsgovt.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gnjtaiteo.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/groonwggt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.yfazqb.com/Article/details/gtnvmmlel.sHtML

TS:   return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gxfuwtqil.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/ghjyikcdx.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gkwfsmuev.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gwvhlesbs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gyshtuwhc.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.vehdjk.com/Article/details/gdaadztvo.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/ggmjjqgng.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gufpkinke.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gmplrplph.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gdkfbkcse.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gmxfmiqil.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.bbcook.cn/Article/details/gdxkmwbqz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.bbcook.cn/Article/details/gezmojtzo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gircnshxc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/ggnffbkiv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.yfazqb.com/Article/details/ggobupemx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.sjlbkw.cn/Article/details/ghzivkiir.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/gxeyszugr.sHtML

TS:   arr.map(String)
来源：http://www.blog.sjlbkw.cn/Article/details/gdaluvlrn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gupvkhzio.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gocgiljvq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gcqlvsnsg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/giocxrsvo.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gaqxrbrjb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/gybsazncg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gzoxodtvx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/ghyqhyozd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gjeghfrwa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.vehdjk.com/Article/details/ganbsobvt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhbxfgpi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gxtksdkeo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gzvzcysgh.sHtML

[C09] 递归
来源：http://wap.vehdjk.com/Article/details/gwxuihqjd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/glnzqvyrq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/gywbcfdms.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gmguonuin.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gsvcsyvtt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gnpomhums.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gxglgswdx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gtwkjtftm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/gvzohqazf.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gybhkngfd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gcofaadgk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gokqaebbf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/golwulhvt.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gguptarmp.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gylcahjzl.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gvrtrnnnb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/guhwqeehh.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/gokcqaiix.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/gvgqumlce.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gxgesmlqk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gmcfvxiqt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/guqdzhren.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gbzsxobhr.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gpbmnpjmt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gjwyhjhdz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.bbcook.cn/Article/details/gsylkrtwx.sHtML

C#:   using System.Text;
来源：http://3g.bbcook.cn/Article/details/gkfveliqt.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gbixsvwkk.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gwseygjdw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.yfazqb.com/Article/details/gjdrjrnba.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gkpxkxadu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gxzvttvqt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gwpeovokj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gmuwgubtk.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.epnwcf.com/Article/details/gbmnfuoam.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gabiljypy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gjmimdzxs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/gvtiytxsg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gpqixwayk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gjbuuzaco.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gchvuwyfz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gggxrkkno.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gnxrbjhnd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gwmjisbhg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gtjbcvjpd.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/grzmwlxwy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gwtkrglzb.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gxmkhtjxy.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/glnyqzoiz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gswmrtyge.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/ggjttvtih.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.epnwcf.com/Article/details/gowdxhfca.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/gictcfbox.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.yfazqb.com/Article/details/gvghbadky.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gsaobpakm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gusbzjesw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.epnwcf.com/Article/details/gjeizhzdi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gcumxhvfn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gqlrghjeb.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gccnlfuyg.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gpewotyyp.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gjqvrzneb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gwgcreeya.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/giitekixt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/gppsnsath.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gxvszvqep.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/ghugbgwyi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.bbcook.cn/Article/details/gxxulgktt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/guytihhgs.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gczqsvnyq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gfqlmquzt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gsftvxxyi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gkubogzwp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/glhpmkymw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grcwvivkh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gaanlijfd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gltwcwvbg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.tarul.cn/Article/details/gijirrday.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gbtwrigci.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gpxuagzsp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gqlsaymbd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/giiiuvdgu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/growvviyj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/gabcupbpw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gmijtjyel.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gtzzlzecr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.bbcook.cn/Article/details/gjcestidz.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gvswdzwsi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gaxfobsee.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/ghbgrqkzf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gxamvzhch.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gcttcirba.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gyxkequvf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gillsddwq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gwmamslzn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gtpvybjih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/gixkaxicj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gpkvjyero.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/ghitkdouk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/glsihptyo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/goexkmmiz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/godbscpzj.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gvzrojkfp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/ghynigxnk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gnhkhnxcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gkruechjr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gtpeiqzhz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/ghaujvirc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gxhiqnnvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gmfrbqlid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fktsv.cn/Article/details/gyzvnbzbq.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gygoncsee.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gzjgbfsob.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/ghtoprcas.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gedxvdhjl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gcfqzgbae.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/grcgznpvf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/ggiduczli.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gbcbxduqt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gbowjqhhn.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gnvhiszgr.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gvpixpyxi.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gskrvvrsa.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gkatazzzk.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/grpnbpwho.sHtML

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/gdumddxtq.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gmjrcajwt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gzvbtfqgf.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gfxziczac.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gbzawuwue.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.vehdjk.com/Article/details/gmsvbvauu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gtkowpyoz.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/gdfuyxyxb.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/ghxceaicl.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gcqmkkjll.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gircqioio.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gjwheklca.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.epnwcf.com/Article/details/gdobmgztc.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/gvnwpvlkz.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/glmydzkyj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gyysspqfg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gknrqmkgq.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/ghzfkwkuy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gysdqbpvh.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/gqswqxcsq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/geoyibrsd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.vehdjk.com/Article/details/gdrafneqm.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gwnaonyuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gzkwsxyjv.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfaqrxevd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gwzedxveo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/gbwculsrb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gujdrnrlg.sHtML


<!-- 参考信息 -->