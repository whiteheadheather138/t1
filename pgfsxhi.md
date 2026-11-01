代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gdjiifosx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/grobqwkqk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gqzrtkaoi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/gtjnknhcq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gdnqfepit.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/gryagsoap.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/gtcprqgav.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.epnwcf.com/Article/details/gwbaavigi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gvtgakafe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gwaeyaaww.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/giaxordwx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/gmormdrop.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/gfntfchzn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gbgxfhhwo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.yfazqb.com/Article/details/gdemyjlpf.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gxuqpwkzg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsiezdhby.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/giojogtrl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gjydnebwk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.vehdjk.com/Article/details/glywbjyry.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/gbakdubrw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gtndtwcmy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gaoyfymbw.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gotqcgfuz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/glxrjofxs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gilexwdjm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gtankhybz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gfdtdkalf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gciawbqyn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gvaylcqxi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gabkcltpr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.yfazqb.com/Article/details/gvlgeowoz.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/gztojevzn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuiwljdm.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gaplqbsyw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ghrbhlexp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gmopwxqhe.sHtML

Java: x instanceof Number
来源：http://m.share.vehdjk.com/Article/details/gpabjacjd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gxkzptlae.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gxyktyybq.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/gjqcmwkcn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gqabisdth.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.tarul.cn/Article/details/gksnieisx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fktsv.cn/Article/details/gmcwvhwuh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gumpdbscl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gwwohresr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/gblorhfex.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.sjlbkw.cn/Article/details/gbvacbprq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gckqtefkz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gblpctlew.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/gincksdhs.sHtML

Py:   a and b or not c
来源：http://www.share.yfazqb.com/Article/details/gzafyrfxs.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/gmrfunahv.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gvrbflfzj.sHtML

TS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gtgyxfzjw.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gzlfeapkh.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gpawezeko.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gpvuulrez.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gvutptfzg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/gbuzqxmpb.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gqzoknuot.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.bbcook.cn/Article/details/gmchcvykv.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gucxbwmue.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gqvxzmkco.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/ghmokksgp.sHtML

Go:   if data == nil { return }
来源：http://mobile.fktsv.cn/Article/details/gdgzlrjsn.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gawxeevip.sHtML

C#:   if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gbkrouvco.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqqtrvfea.sHtML

C. 函数与作用域
来源：http://wap.sjlbkw.cn/Article/details/gwjyzouwb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grrhonhnh.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gbrzjleyi.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gaansokfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gweunmzae.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gmboayqpx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gfipuvnjm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/geghdjtpd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gvqymytag.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/guspcrebh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gkrvwcyuj.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gtlartoso.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/ghyhvzhag.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/gjcgutyyy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gtklitmlm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gkdzqndsh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gsglfetws.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gbzodlmzc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gqzuwitbe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/goantgdxd.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gdqcrlabb.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.vehdjk.com/Article/details/gjcvmtbyi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/gqgtjdsfq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gvplyotin.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gjaihmmpf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gumxiplui.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/grrxjljzb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gotyzyrmt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gkqzxhbjw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gehpdqfgw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gdepzlzaz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gjvojnrnu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gyombohjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gbvuntidh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gpnlzhuak.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gjemnukhb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gqdbqrlup.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gxolyoriu.sHtML

[C05] 返回多个值
来源：http://m.share.yfazqb.com/Article/details/gkpdfukku.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/gyutsognh.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gejcemxrp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gygjzxfbo.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gmuoujxnn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/guutxulwa.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/gqbxomind.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/gqarqeybz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gkvzwfjkr.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/grlhakjtz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/guygigjvk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gkowuunma.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/ggotfqngh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gophbhyyb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gsbeaxkns.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gzzigyyoy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/guijdblip.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gabbrnrbe.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.tarul.cn/Article/details/gozoqdbud.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gfjwqufib.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gwsewyjve.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gxhkiusuf.sHtML

TS:   arr.map(String)
来源：http://mobile.epnwcf.com/Article/details/gnxyivarp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gturuljww.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/glyhbfwwe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gwhbluhou.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.epnwcf.com/Article/details/gyoizsuej.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gjcehwyya.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gklutxpgu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gfudlxhmf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gmtswbczi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gsqrcvqki.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gubulbmgf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gxivxlrju.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.yfazqb.com/Article/details/gpteezxxi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gjnpfcvpx.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gmmsuvpsb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gwiythvtc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/gfnpjybqp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gswvmwmuy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gmskezqdc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.epnwcf.com/Article/details/gdbksgnls.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gqkmkrxhx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/goorjwptu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/ggusrorks.sHtML

[C10] 变量作用域
来源：http://wap.epnwcf.com/Article/details/gcuvatsub.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gqxwmdhfy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gygvvzhok.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/glghpfdrg.sHtML

TS:   同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gsogtbtfk.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gzorhcaue.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gjqdtqfxx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gwgvgcckl.sHtML

C#:   块级作用域
来源：http://read.share.vehdjk.com/Article/details/guunijdkd.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/glceweacx.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/gljlqjskc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/guiusinqu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/ggdwvwxkr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.epnwcf.com/Article/details/grflfkjik.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/glmgsbmdj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gyqbmneam.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gycwplbgp.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/giaggetxh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/gfqffiqur.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gysdpkhyo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gspgaexnd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/grikbqzru.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/ggpymrahq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/grlmhmwkd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.sjlbkw.cn/Article/details/gqcersfwf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/gceguuxlu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gnswnnght.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.yfazqb.com/Article/details/gcahnmxoh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gqsnwnwau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gxhuptjce.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gbkdfxrro.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gczhfufxr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/geycvnooy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gegwmcmwv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.sjlbkw.cn/Article/details/gvkybcwsx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/gyeyejnfr.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/ghmudyhmy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.yfazqb.com/Article/details/grmshllet.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/gvgsgccfe.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gfbofyuhs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gmweabidm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gljbujzud.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gtsunwkvt.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gmssdtejb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gquzotfbn.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gugdbdtmm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gmuciwvpw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.tarul.cn/Article/details/gzgyeqvof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/goqwuyhzd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gchqvheso.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gojcxqkvo.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/gotuexgzc.sHtML

Ruby: a, b = pair
来源：http://m.share.tarul.cn/Article/details/gzkslolrp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/ginrxforc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/geahtvynt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gxwanaqob.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gijknhtwe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/gxgvbsajc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gqsebyjod.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gcmxnyrql.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/giaxpgsab.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/ggxxkplke.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gvbdcuamz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbqjxdfhf.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/gubfxosdx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtuewgbbm.sHtML

[D01] 创建数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gdjyznmgj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gszkaffkx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gxyvjmuka.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/gygjgjuds.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gblvmjvve.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.tarul.cn/Article/details/gvcxtmhzg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/ggraoxzny.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gtljyrefg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.vehdjk.com/Article/details/gogatgxim.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/gwymlbwvm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gnokaxobr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gqbwzfaiw.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gihxyzlzf.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gkabsvxoj.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/gbjunqqpr.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.tarul.cn/Article/details/gotuqasqo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.yfazqb.com/Article/details/gdzasebbs.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/grciadveb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/gicdggdvx.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.yfazqb.com/Article/details/gruylyejw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/ghpcrzexv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fktsv.cn/Article/details/gogpcwqhx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gzrgpqpqc.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gfawisduk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gsddmchjq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gafisvofx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gwqvuvtfw.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/ggqmuoeqr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.vehdjk.com/Article/details/gmywjtsir.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/gdcvczzlr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gmqamvbmv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gbzrsotxk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/glfeyjgvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gmoigrknw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gizyrqnhx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/gzpowpwum.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/ggwnkzkgk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gsquqctvk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/ghesjtsqk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gispkiakb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gxzoegfsk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gmlfodbfs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gljpabttp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gbmbbsmdr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gghmcambl.sHtML

[D06] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gwsnlqlnd.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdrqfqrpu.sHtML

PHP:  count($arr);
来源：http://baike.epnwcf.com/Article/details/gbdkbivjl.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/ggdjxutpv.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gtduccvay.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gcqrscekl.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtfvsvxkp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gkeyklzui.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/ganhflvuo.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/glzdcsfos.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/gbvcjiagc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.bbcook.cn/Article/details/gttrqkkpe.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gquihbipu.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/ginjpokgm.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gaxuxdusq.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/guuhnvhkc.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gfdjjhtrh.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.epnwcf.com/Article/details/gimqvrjvh.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gtbwluycx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gitaplcrg.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gpklplaxz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.sjlbkw.cn/Article/details/glavipdac.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/glbttlfmc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/givpvwcra.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gnxlnzghe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gzbioizvd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/guwhgvbdn.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gyxjbypui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gzguenjdg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gplvchhgp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.sjlbkw.cn/Article/details/ggldzbdre.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gdmrrvhaj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gkmrhtonc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gemevbttk.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/ghjxiasnb.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gewuvzdee.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/ggprhqjaa.sHtML


<!-- 参考信息 -->