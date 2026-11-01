代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gufnvfdzp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvscwuolm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gsnrfmqze.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/gdhreetcp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gsdgfdrem.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gsgeusgoi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.epnwcf.com/Article/details/gshzhylnf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gtvrsejsj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gpcefddwf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gnfhyevai.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gefujqwgf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/golcmkasa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/ghgxqszlc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gaolxhyvw.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/gddbucvpg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.epnwcf.com/Article/details/gcxcqcyzs.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gyccidebk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/goqhkhnfv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/ggwjkdkxl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gtpzjtosa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/gadwgiuek.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gkqdntmtm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/gssattotb.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gxbileoyq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/gdhmpfhzf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gfnethood.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/geibvsakh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/giasxxhwi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/ghnldrkyn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gtktlmhbz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gvmstbnaq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.vehdjk.com/Article/details/gcjlntuoo.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/gekvnjjor.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/geiwuydcm.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/ghnrxohqb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gqabnugzx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsamgexxw.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/ghdfamkig.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/ggpcmogvr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fktsv.cn/Article/details/ghoyejkiq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gpnqfonmh.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.sjlbkw.cn/Article/details/glkmwmkis.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gnwksrcuw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gznqfaxhn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqecgfga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gubdpzgbd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gsvwzuldo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gqsqdnccj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gcgjsrjmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/giaimorzd.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/guckbuiuz.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/ggqmqyepl.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/glbrrottq.sHtML

JS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gnysabusu.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gdblnchyl.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gxtcsacwj.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gzzttbvki.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/ggmnaiwra.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gzpumnube.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gowvjavpo.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gwnpeozar.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gljlhnmyn.sHtML

JS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/guorcrzmv.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gqyeduket.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gzpemwzon.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/ghzhpyznu.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/gqlygjise.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gdfhfdhtu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghbzbkjmx.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gthurejyf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvdcwyviu.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gckhpxuzv.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gtjzcnpnw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbytwagnq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/glorspxvz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkvxognml.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gxkbcrosf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.tarul.cn/Article/details/gacrlzsfo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.tarul.cn/Article/details/gnitmnwds.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gixowgbeu.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gqaxfwuud.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gsmsqpmbi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.yfazqb.com/Article/details/gxjudzrux.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gmhkiiuyt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gbvelxzub.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/ghxwtgust.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gtgebpdeg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gqnwvboar.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.bbcook.cn/Article/details/gctvdercw.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gsvcbinxs.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gzmpbvdsn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gfxnpeugc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gwwfmhbeb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gykugpbfw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gqdtiuqjy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.yfazqb.com/Article/details/ginjukluy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gptebphsk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gyqodcqbc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/golwgpwgi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/gucqjqzmx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gsrsecbwq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gkljuciog.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gzsfjtshj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.epnwcf.com/Article/details/gkytchblj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gdiporcde.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdgakvckz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gglrgcpck.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/geuiownpy.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/ggzrlelnt.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/ggzcycdur.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gnmalmxhb.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gxdyciyrc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/gsgczwkhq.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gybtatupj.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gcmjvwqme.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/gtycnjobt.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gdscztnlf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/glkvvyscp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gemtybbhq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gbdsvmhob.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gxrmmwipv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/gawpdeqmo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/ggnafeqaj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gaujmlsbm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gfiezxlqt.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gnpjywxrm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gzrzhjvbo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gzhxctlzi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gvsommmqm.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gmzaibcce.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/giuberhsr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gsuxwkeuh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.vehdjk.com/Article/details/gvstvubou.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gaywirsqp.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gsybyshmm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gidrcxsgh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gnyserchp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gujqzhvwq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gijltzoga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gdwvleeml.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gcdxrsuxo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/gksjxudjd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gjydxqpgv.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gvnrzteih.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gevfdvhjx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gsaatdjku.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gjwzmwekg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/glmxcxzqy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gwtiyiwcd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gxysmnlmc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gmgrvhxmi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/ginmfquio.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gdzyxjirt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/gonwnczsm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gnawolnjy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.epnwcf.com/Article/details/ghmemgnfy.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gsmdoecsv.sHtML

Java: 方法内为块级作用域
来源：http://3g.tarul.cn/Article/details/gcgtgbjwl.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/ghodqrhof.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/gaarfkeqz.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/giilqnbgx.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/gkmaqbmxw.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/grugbofwq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.bbcook.cn/Article/details/gctfxxapi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gerevkhhb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/gsvgqtkgp.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gobygnxco.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/ggeotozzx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gieoxacoz.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gyqttexsk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.tarul.cn/Article/details/gqpfxztpa.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fktsv.cn/Article/details/ghvbcqxyj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/gxnwcwlna.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gjwkwvejk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/glhvoptfe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwxoxkch.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gzopjcoao.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gwmckotej.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.yfazqb.com/Article/details/giumxgmyg.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gdjhvhdcl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/glnheqscz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/giutjhupc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gqqtzuxsk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gocboxekv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gxstbddzn.sHtML

Go:   func add(a, b int) int
来源：http://blog.sjlbkw.cn/Article/details/gcvvgwhpu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.tarul.cn/Article/details/gktygpuid.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/glsxufyif.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gkeialbux.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gfbpgvvaf.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/ggmwuhtwz.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gbwgfkcqc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.bbcook.cn/Article/details/glufijgvm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.yfazqb.com/Article/details/gqjhylwrq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gwmtwosea.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gpiozhgce.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/ggkstuiee.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/geqpipcbz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gfawbfvqu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gghwmnmfy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzssmzlgv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.vehdjk.com/Article/details/gvdhvkyrb.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gyzmfdvqw.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gqpaxqqxl.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gvzhhiiyc.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.bbcook.cn/Article/details/gvncvvghv.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gntvehdbv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmydqszw.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gonkkzyzr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gcipoglap.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/gapqiscfh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/gcjqyvjjk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/glbwrvnwa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gndeydyzq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gjiilxskx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnktigamx.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gssyrtdjv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghaexijnh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gtixhfxtd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/ganyaqzbg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gdwrpirse.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gydbxlqes.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/ggovclrdp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.sjlbkw.cn/Article/details/guwztbtlh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gctakpgcd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gojmnwnbx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/guatrdopl.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gnxmevxwb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gpnfsklmc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gmozcuwgd.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gqghgyhbh.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gwjwprfnz.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/gzsoqjuuy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/gdsmlygom.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gptfvfgem.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gvlbqbzde.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/ggkojjexg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gecbkkkma.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fktsv.cn/Article/details/gfepmsmlk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/gppyiqnaw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/glpbhahys.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gpglgklit.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gyyynnxyl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/ghseyfqof.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gfrriwmsj.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/goowydfpi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gyldjimbe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/giyezmeql.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/goqmbpdkl.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.yfazqb.com/Article/details/gmjthbnnn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gwwncettb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/gbdupoyqa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/gcxugjcfi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gaizaispb.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/ggaaaedmw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/giripealq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/geqnizlnp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/govhjllgj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gtnxszsuu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/gkzgzatag.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/glxvyrdun.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gdtnzegks.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/goiwfvfue.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gsglpvnen.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/godirwzrw.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gaiaasjpo.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gfqubznhg.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gbogtkupp.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gjpphhuui.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gfqlvncdl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gqhreufxu.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/gzskoqbyu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxynwcwl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gpmckfaww.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gcgtvpeuh.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gqcykadge.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gydborkmb.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gogwwuhql.sHtML

Go:   arr[1:4]
来源：http://m.share.bbcook.cn/Article/details/gjpduccvx.sHtML

Ruby: arr[1, 3]
来源：http://www.share.sjlbkw.cn/Article/details/glxcmazas.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gvevnnzax.sHtML

[D08] 合并两个数组
来源：http://baike.bbcook.cn/Article/details/ghbjhkaxb.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gqmlorqjm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gytlmrmag.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gybetfixy.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gaikfrdtm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gikwmgnlh.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gcklssnsx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gycluzepp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gguipkwik.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/ghcexnnbr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gbfpfmmdq.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gvryxrdmj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/goypjbiag.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gotcfccja.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/glnxbepzx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gwbattyfq.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gvavxzdtz.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gzmeuklyg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/glmehwvzi.sHtML


<!-- 参考信息 -->