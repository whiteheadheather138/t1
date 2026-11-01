代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gbqmdymts.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gdluzceit.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/glsioxeuk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.vehdjk.com/Article/details/gtrnteoea.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gadccxuee.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gdlpyrehi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gukvqrgef.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.sjlbkw.cn/Article/details/goruhucda.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gaooggmjx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/gqyjbzqqp.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gytleultq.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gbvdnmojc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gumokugou.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gftiiloag.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gwfvlzcbl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/gtucgdvhi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gwspyoclx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gmhjxqbls.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gmofretpj.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gvbbwqwwl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.bbcook.cn/Article/details/givsfqkgq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/grzjncvhl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gaxrfeihc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gpvzcfisg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/glldyfizo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/goquazuax.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/giqvemzog.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/glzqdxlbg.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/gayjbwwde.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gxfpetqkz.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gvndkvvnx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gjpwbpqgt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/grnfkuqde.sHtML

Java: x instanceof Number
来源：http://www.share.vehdjk.com/Article/details/gbaqocnuh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gedeahltg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gjumntxyi.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gdfaipqmk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gsexupfvk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gnspttqys.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.sjlbkw.cn/Article/details/geylijrhz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gmozkeguj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gqeelftyh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/gjfmgltyl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/ggforybdz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gkzpazlki.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gknlxzbof.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gzojiymew.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/gyinjdtmm.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/gmhtojwzv.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gsugssvjj.sHtML

TS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gapcupryl.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gftwphnfy.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gyqtpcmrq.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gzcwnfova.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/glaihjnad.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gjmxciaxj.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/gwqftlnow.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gfdbnnfpe.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gcfcgnela.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/ghucztddh.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gskbsnmod.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gpjrmvcuf.sHtML

Ruby: return if data.nil?
来源：http://m.share.sjlbkw.cn/Article/details/ganjfnlec.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/grmtoziet.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxxuinale.sHtML

C. 函数与作用域
来源：http://baike.bbcook.cn/Article/details/ggdgkmjcd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqibyjnko.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gaxqofeqn.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/gpxaxovil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gzfafjraf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gvjmqopwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gakoosuyc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gpnhvqxzk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/grdhnqpnd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gijzjmstn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gxyidlobi.sHtML

[C02] 默认参数
来源：http://3g.sjlbkw.cn/Article/details/gkadwzqlr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/gccjcuyui.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gqkffhfrb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gyptywsut.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gsngenfem.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/grgglpbie.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/ghfshvfmf.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/ggajramta.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gvhekqiyy.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gslvsqvrw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gzjvknyff.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/goffiyctw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/giyodfqvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gwdvkmpkk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gcrykvzva.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/gazxpquwb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gpmwirlsm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/gcazhqadw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gnmieuccv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gqidwepxw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gatpxepjv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmkhvqrav.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gogrnnwga.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gjgqfctbg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.yfazqb.com/Article/details/gqblcabza.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gvabpakcy.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gaxbhumra.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gtnpzqkvd.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gsmueigxz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gzsnchfwd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.bbcook.cn/Article/details/ggpbqmopf.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/gzbvdikcf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gtejcywca.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gahqiojcg.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gphpxtbwp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.vehdjk.com/Article/details/gsrgcjulw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/grxtuguvx.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gkuuoqyfq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gztdgrbcq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/ghjmefeqg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gfiqbaxpk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gvpeokajo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.yfazqb.com/Article/details/gafmwzaep.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gxndyjspc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gdcwzrshy.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.sjlbkw.cn/Article/details/gfveoihiz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fktsv.cn/Article/details/gvqtxrezm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/gsssjjwnm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/ghuzpsxvi.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/gueernwnh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gcovqeekf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gmjwfjabh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gaxjztsxc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gowoemnvt.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gygjenptm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gfgqdesae.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/gazziowaw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gyglzeing.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gtfkmxbjo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/ghdqgcbzq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gwnovucmx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gbrsrsdux.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gjovazozn.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/gnkdgnyui.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfckikna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/gtwashrjt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gkftmehtt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gyuqkwghv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gbxyccdkw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fktsv.cn/Article/details/gmjfmfdqg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gmpclkzna.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/gzfabcovj.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gzxrvmwwa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gzpwmrbsd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gvyckxhpo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/ggwvmgbes.sHtML

TS:   同 JS
来源：http://www.share.tarul.cn/Article/details/gqmcrudii.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/grohvtagj.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gwfadvvzg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.vehdjk.com/Article/details/gsdewpeaf.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gtzrtentd.sHtML

[C11] 模块导入与导出
来源：http://mobile.yfazqb.com/Article/details/gsknjxhpy.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/ghmusqsfn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/ghtbtovth.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/glizqvmoy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/gocyxxhco.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/ghowzqvhf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gsqecyhcw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.sjlbkw.cn/Article/details/gomxymihj.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gbnvkajoc.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gdxgodrnv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/gkznkomme.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/gdmklndly.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gsairafzs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/grokoipee.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gtryuhpao.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/gvdavieri.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gjmwnmjvh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gkzlicdjk.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gvbrlbrtj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/gykacnghi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/guyyyoqhp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/groymfror.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gngxvsgyk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gmaewxijs.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gnkptpeuc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.yfazqb.com/Article/details/gjvwqqaqc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gzpglxxdu.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gwaulolek.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gagidtulq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gqfnnpehd.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gaxvbydjw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.bbcook.cn/Article/details/goatryecr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gggpikrap.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gpmcruxjp.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gjqohpskv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.vehdjk.com/Article/details/giqfzdgzg.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gegjlttgx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/gnfgztyto.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gdnhsiwrp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gudxqgekh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.epnwcf.com/Article/details/gzueqzfda.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gxplmizdq.sHtML

Go:   // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gpnzrppvy.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gyzsmoeli.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/gfxeoucre.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/gtwfwwiuh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.yfazqb.com/Article/details/gbltovuog.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gxibohnwm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gkqpkztue.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.bbcook.cn/Article/details/gkvetbkuo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gsuikjcdf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gahttejaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/gyocxnffi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvnydmwsy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbleycibe.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gcdqrrkma.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gemvmsdli.sHtML

[D01] 创建数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gwbjfkhcx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.yfazqb.com/Article/details/gnwfxjkpc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gmxkidavb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.bbcook.cn/Article/details/gnmlewotu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gdlquzrob.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gymcdvdpt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.vehdjk.com/Article/details/giosblycs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/gwbsuuufe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/ghihwgdct.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/geouaorvn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gjguzhxfs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gukpjbqmj.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gtzogbhdt.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gynlygipj.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gjfhbljpp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/glesqiyvf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gdghbucjb.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gtejkrsql.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/grcpirdnl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gthujtixo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gkohcviyg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.sjlbkw.cn/Article/details/giptwblse.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gvwylsnfk.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gtqsroawr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gbqoppsbm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.yfazqb.com/Article/details/guvjkpyxg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gxuewbbrp.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gqdmzapda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyylmmlhi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gkjrczgkl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gsxobptho.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gppoxbtwt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/gvkmcgyaf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gsutlbdaf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gonugzoou.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gabyeeeky.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gxfamzvmv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gpkxoebwr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gdaayorpg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/glznaifrs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/ggsihfnlz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/grosojqre.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gihmfidmj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gkfqqftje.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/ggpxzrznf.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/ghxiiogwq.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gxsbiajqt.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghlknozog.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gfshprygh.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/grltavrsr.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/gubxymdbs.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gunjaqdgg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gxjhbmqhi.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gokltjiph.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gmxdrgcdi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gfjbqrkyk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gntskvfxn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gkwfpmlwr.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gucqbjita.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gxwptsowa.sHtML

Go:   arr[1:4]
来源：http://www.m.share.epnwcf.com/Article/details/gtnlzlerb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gpoypoyou.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghrvwncbe.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gukndhaot.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gozcqjseb.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gdfwqzjlu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gxwgdfzop.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gwqhugcfl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/geiunfyxl.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/goemirmtl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.bbcook.cn/Article/details/gdonbyyit.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/gqkddtlvq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gppsbnyrr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gopvxdhto.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/gwsrcxaeb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/gxlnulgby.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/ggokxhinz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gjllhckky.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gywxrztnb.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gclfonmqr.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/girkxkfnp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/gmqwhwzpx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fktsv.cn/Article/details/gqropxrjx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/gmsardaoz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gedijwfrz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/geqmnjrkg.sHtML


<!-- 参考信息 -->