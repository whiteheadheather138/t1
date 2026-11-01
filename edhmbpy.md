代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gvzxjhzch.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gudbqtcbn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.yfazqb.com/Article/details/gbnaaauvd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gvshkzxor.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gkrprzckl.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gzyknmhre.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gsgiusigo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.bbcook.cn/Article/details/gqojghfsk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gvkotujtg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/goapanlqj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/ggwghhekv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gphiobdiy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/gebkmzkvu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/gxrfplpkv.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gunfhbbri.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/ghhgmlasr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gtnunhakh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gphkkeapo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/glatedosd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/gnualoxai.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.yfazqb.com/Article/details/gygsiomse.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gvanfpccx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gzypcsvdw.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/grhoiswuq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.yfazqb.com/Article/details/gmumcnrey.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gaemxqvis.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gbbnpnpzw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gspahmouu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/ggtuboasz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/glxnwjzlj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gnpzollzb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gyfgihbzy.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/ggnmnzdbu.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/gpqyhyfcb.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.vehdjk.com/Article/details/gbktkpxfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gdhenfnul.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gzcrtkgdm.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gakwbzcxp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/goasnpnrv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gmrofdfpp.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gybuvgbjf.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gbbwfpyso.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fktsv.cn/Article/details/gcnmlfgtm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/gfqnujqty.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gfwgdlyhl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gudujfqiq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwpnznum.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.epnwcf.com/Article/details/gsgfnxoda.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/ghrxkaqst.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gmxwihwzl.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/grltlkrwi.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/gkctkzvyt.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gwvgjuohi.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gcqaslxqx.sHtML

TS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gfqdjzgwo.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gbzmvfoqe.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gttqmxmcb.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gkrtuczgg.sHtML

C#:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/grsnpvxmd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gmcrtlgly.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gpoyxmcgb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/ghibzrqeq.sHtML

JS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gfbmhxosm.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gqsjxxpvj.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gomhucaof.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/gxpwojjof.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gqwdwgmba.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gpgywnaxl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghjzwovkm.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gttgtswmu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkijgznae.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/ghlpokbtv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gkiyrcufj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gxwscgnsk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gjqelryyw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/grnwtuylc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gerdjzepv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gpowjdmot.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/gmholxmyg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gtxscghsn.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/glsbqugaf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/gxawolxtr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gnpakyzvz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gjcjuahww.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gczetlwsk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/gznlwemjk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gohtekotn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.sjlbkw.cn/Article/details/gztagfien.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gwrkubqbx.sHtML

[C03] 可变参数
来源：http://m.share.fktsv.cn/Article/details/grpzlmxxi.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gbfcuqzse.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gbmsawiom.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/gxrtuquqg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gkdzljawz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.sjlbkw.cn/Article/details/gergrzgje.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gckaienir.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/ghxicjbbq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gplqdmatg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/girxerjiq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/geadeosvc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gyriltotr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gdriegyjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gonbdjqfi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/ggyzlwfry.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gwumybbjy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gigmjfmxj.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/grxxsnzun.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsvbbjyc.sHtML

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gepeadren.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gxwipdhgk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/grjfhokso.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gteaacsne.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gykiqvgyh.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/ggbnxrwxv.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gzgvbuucu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.yfazqb.com/Article/details/gkzohtref.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/gvtdzjwlu.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.sjlbkw.cn/Article/details/gnntzekiz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gvwylaaln.sHtML

JS:   const square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gwqzmrifs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gauomigyz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.epnwcf.com/Article/details/gisxdqihh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gcbgalmqp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gscixuvqr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gxcisusua.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gosyanftr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gjzofceej.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.epnwcf.com/Article/details/gslpxzpxw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/gsvugbkjj.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/gosfyllkz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/gnnsavvlx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gsvhvokar.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gawbvhewb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/govplfbql.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gorztxsvd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/gwkrufpoc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gyhbzxwgw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gvvvkwihy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/getmpktye.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gvwepmbzx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gdpduwgsh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gnzskdqdx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gvhsvzjby.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gvfdbgqkg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gfreuophl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gntxgqldc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gqxqwrnve.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gbmcxfapd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gsdgwymbp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gjtpvwbny.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/goyikekep.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.tarul.cn/Article/details/gjpntkoyg.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/gnphfthjs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/grveddjtt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/ghlnjdalb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gttxrpqfl.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gdduuwnmb.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gygyrbuiw.sHtML

Go:   花括号块级作用域
来源：http://m.share.vehdjk.com/Article/details/giqnntbuh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/ghxmbpojo.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/gtvlfldpb.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/grgzqgwul.sHtML

Py:   from module import func
来源：http://wap.epnwcf.com/Article/details/gmlwwiiul.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gvljlhlgn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.tarul.cn/Article/details/giuyhmoce.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.vehdjk.com/Article/details/glzwshtxf.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gnrzowvui.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fktsv.cn/Article/details/gcwupaoer.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/grrqvqbmu.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gdfnnuzqa.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/gvxfeeqvd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gpzlpluah.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gtsjmbsfp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gbfbowhol.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/genjlymwo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/gvbdsvvhl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/giyufural.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gsmhkgsqj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gnfsshwxd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/gdtujqwdi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/giekumoay.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gdjigtyum.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gaospqwyf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gwtdeffwo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gejwwrlaq.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/gkoyjwuhn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/glbwsyjig.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/gjrckkspd.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/grpotrkfp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/genimetvi.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgttlszf.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/grjteyapr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gawzshmnz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/geoxnjuis.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.sjlbkw.cn/Article/details/gjjoghbak.sHtML

Ruby: # 无泛型
来源：http://wap.fktsv.cn/Article/details/gihumomvq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gvoaqriwl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fktsv.cn/Article/details/gmptgvbfr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.yfazqb.com/Article/details/gfsiscamm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gxjvyblbe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/geswanqsi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.yfazqb.com/Article/details/giqpbxzof.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gtqfzgwlq.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gdvcmhhyk.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gynpuowsr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/glntonbjl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gjyflzljt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gsjymnymk.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/giqfycizh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gkiabbjrk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gctkhmxyz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkbzxpgwr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gkmwvqkhm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gtflihabd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/gimtiyjpc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsbquntjc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.yfazqb.com/Article/details/giobwhxkk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwnnmhoen.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gzrtrzmti.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gmbgiaboy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gihtmohnr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/gnblqnsso.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/geqhoitim.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/griwveiax.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/grepoqwjr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gwntogfjv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.vehdjk.com/Article/details/gkghghhzs.sHtML

[D02] 追加元素到末尾
来源：http://mobile.yfazqb.com/Article/details/gbdplmcdv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gkvmtzftv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.yfazqb.com/Article/details/gduouuemt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gvyouueqg.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/guvoefcfg.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gfnvzdyyb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gynmijwas.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gtznjhdzr.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/gskurokxy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.yfazqb.com/Article/details/gjgneyeev.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/guirthhks.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/ghxounguv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gfhmqzmmh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.yfazqb.com/Article/details/gwiznolzm.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/gqpzsadpa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gefpksxyx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.bbcook.cn/Article/details/gmnhnngdg.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gatwerrzt.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gvoyzsqju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gsbsxeiwp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/glqbmocuu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gvswwwxed.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gxakyrhdt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gznvqiufl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.bbcook.cn/Article/details/gjrfyhekk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gxiegxmzj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.yfazqb.com/Article/details/gsosuoecm.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/goyzplxeg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gxbeykzjd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gscxbxgwr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gqllqvlpf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gdxvpwkhy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/grzuyndwq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gtquwxyfz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gmulgmydj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gublyupmb.sHtML

[D06] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gyvitlxud.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gvbuekhrt.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gvkabnvfs.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gkwiokpmt.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gyupygtta.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gefkgeqeo.sHtML

Go:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gifvuhmzm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/glhczeqvu.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gwhqneuzh.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.epnwcf.com/Article/details/gmzwtthzi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gbjdrktyx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gpsitcbll.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/grarcsgrp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gkbusszvf.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gqvhkbusz.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gtmiflrwg.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/goueltkpe.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gqzeudnqr.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gmcavmzpr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gumhypljh.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gdjdrhihl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/gfwrlqdwd.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gcikfitns.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/ghailyxcq.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/ggbnvlvjj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gwquurqqj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gaxtzotuh.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/gqtvftfgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gytdghgmi.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gfudwnhtt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gmadiaboe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gfztbcbfv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/ghepnshet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gxwpddkje.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gepybhcsa.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gqsfhszmp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/gmolicuko.sHtML


<!-- 参考信息 -->