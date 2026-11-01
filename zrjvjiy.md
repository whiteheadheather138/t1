代发 wailian999

PHP:  range(0, 10, 2);
来源：http://baike.sjlbkw.cn/Article/details/gixgmavwr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gqwhoupdr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gejcrsvjd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gflcwblsg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.vehdjk.com/Article/details/gdfufgvfc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gcpbfcqlv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gdapkwvva.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/grrgqzfhl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/ggswzcwjs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/gzodmumrn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gggsjdcyl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gczkqtenx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gzjrebpul.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gdkpxvmoa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gcomjqgmf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/gtitofoiw.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/gmgttenak.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gtrhjbdxr.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/goowrgejm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gcugflykt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gtogxsrvb.sHtML

Java: x instanceof Number
来源：http://read.share.vehdjk.com/Article/details/gewiacklu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/giuorvjcn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/gzbrhbspj.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/gjiuqvcct.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/gsiaokoez.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gdruqkxlr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/guoqdfkeg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gfrvxsslo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gkvjhuvdl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/ginkbtjjj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/gdbslkrri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gwnxcqngs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gmeftksek.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gwgtvzhiv.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/ggdqqbcaa.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/gktdhiyll.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/ggtdbvquk.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gvchmtqer.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/guwlawimu.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gpjxndjqu.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/ggluhhgng.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gmjikevmi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gotsuczwc.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/gcvfbxryn.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gopmcjzkk.sHtML

JS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/gvjoaaayy.sHtML

TS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/guetknzeh.sHtML

Java: if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gpxmxigup.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gxtxqugie.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/glrpxaqfk.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gntllegmy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gosycdfhg.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/giaeoeefd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfvpjfktx.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gwfvgjzna.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gdhadpmtk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gxhnarmfa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gjxttfdou.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gnipeithk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/grataczqz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/glqrmvlsj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/glzrkdzor.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gppjxfjku.sHtML

[C02] 默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gfacsnyaf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gpsldchfw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gyrdvyyyp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gwhyvsalr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/ghfmmgzfq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gymecvtwe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/glxnsbobk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gxlchyjrk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gqnwyasst.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/gqhssxfxy.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/ginvjefhn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gpadzoiri.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gwhmjpvao.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gqzpccdfl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/giogwgnkx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.bbcook.cn/Article/details/ggxhgivhw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/gpiqqidaw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/gmmrqxvxz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gcxxmweux.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.bbcook.cn/Article/details/gysfegwgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gqwqugzci.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gdxmfvtxo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gdqvasdsl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gpgkbzzob.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gewcurbkv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gukwprrxn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/grpjlfjxw.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gyfthnhdo.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gedhkxyfw.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gazkfyycd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gsytmdxpm.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gyxklwpyr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.tarul.cn/Article/details/geestrawm.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gkfqobdld.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gytujsnuv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gujqapyxp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.vehdjk.com/Article/details/gbusrpqfd.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gnpjawzxd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gvbisntcu.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gbchacbnb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gokwdlgka.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/gcwhiirko.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gtpgtxgwp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/guesjtaib.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/guwdjsjst.sHtML

[C07] 把函数作为参数传入
来源：http://wap.epnwcf.com/Article/details/gztseprtb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/guevawbfq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gselqwkzh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/glvbuhxhk.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gvqhrjpoh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gdosydeul.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/gcunoyfyj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gaibslqyc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gyqorfxly.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gzpgsngqd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/gzoytbikj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gbqaotnqb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gctrjpqtm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gavtkdoqj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/gmhnxpyhv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gcyltvwiq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.bbcook.cn/Article/details/gynlnjymi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/ghorvrrjq.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gaoejmfkd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/ghsyyvchy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gfyqxhyvf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gsxvyxnyf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gzakytrpq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gfwntntgo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gexhemasp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gupsxvjif.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gfqbfxwye.sHtML

[C10] 变量作用域
来源：http://blog.vehdjk.com/Article/details/gasbedbhy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fktsv.cn/Article/details/gqwpdfizt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gzvfaoall.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/goiefdkzu.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gljxrujan.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gloklcxhb.sHtML

Go:   花括号块级作用域
来源：http://m.share.vehdjk.com/Article/details/gckhtfgtc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgvdvfiv.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/ghxymocmo.sHtML

[C11] 模块导入与导出
来源：http://3g.vehdjk.com/Article/details/gvzzlebcc.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gqlfvwpli.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gdggivdne.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gredyiljr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.sjlbkw.cn/Article/details/grtiyccyi.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/gftgvxdnx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.sjlbkw.cn/Article/details/gtvfyazec.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/grfpzuudr.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/gvzoxikqv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gmmaosepu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.epnwcf.com/Article/details/gmrayczms.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/guzwwxfkd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gtviqidnw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gqtpktdcm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.vehdjk.com/Article/details/gdnvmqmmw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gvvrtpofq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/godivelsv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gskcfdiuv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gsfefpvyc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gammjvyon.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gudhixgkn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gerxbxwxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gtexayqne.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gtbobdplt.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gdilnikmx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/gcyebpuih.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gxaermqrw.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/ghiraqcju.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/grbicgkxl.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gvzwdjuvv.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/glrlrzljm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/gqxeuupqc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gefottmdf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gryiquryx.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gbysiohck.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gbmkwfcac.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.epnwcf.com/Article/details/gqblmyfnn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gkjwkgnpp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gyqzdqtva.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gdygcjlbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gyeosnmhb.sHtML

Java: // 无解构
来源：http://3g.yfazqb.com/Article/details/gsbtxowca.sHtML

Go:   // 无解构
来源：http://read.share.fktsv.cn/Article/details/gunnvcvge.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/glgoreerb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gvczolcwu.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/gxharbzsi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/ganuzifat.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gojhnskam.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gijnblmdb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gplomlkxy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gcckhwsij.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gyijedxbk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gzneztwcw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gewoppwjf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsaabqctd.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gxsgxzovz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvonjvodk.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/ghlyeoymc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/gkizcljuf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gptuqyjuz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gqzhgoglc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/grciqqhnm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/gbtvpdfln.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gsslqimve.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gdurdsqoz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gotcprwrm.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gcckzolmy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gvloetpwy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/gyguiymwc.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gegcdscgt.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gyfnflvsw.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/gwpvnrjvo.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/geyojuacg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fktsv.cn/Article/details/gvcebepca.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gpznezyls.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.yfazqb.com/Article/details/gcgujwpmk.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gxzirmdic.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/gagxwdbhw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gwaartxhl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gelxkmcyd.sHtML

Java: list.add(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gvyvfjutd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gduwmfrea.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gdkywzwdc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gytdzrcxi.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gquokpqkl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/gquqqihnq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gfxozaslj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gchifggvm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/gmngysccl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gwwokcqvg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/giziszzkt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gpfvcyhxc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/gsguakxjy.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/genebhkjz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gwgyouuzo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gmwtwdutg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gldgoeaaf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gvwkyvfky.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gaoliwkqb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gxxqswrrb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gundfseed.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gubbwuuha.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gzjdrqgms.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gfhtqcvpn.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gbfrnjgvw.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gfztezmhc.sHtML

TS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gguzsmyig.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gmsjnymex.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/guindkjdi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gipsymrpt.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/ggqfurtxw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/gublnmtak.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/giewrcwrg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gfydoczse.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gqgzcgssc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gykrsuyhw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gztfwxusm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gqzolxauq.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gmlcqombk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gmcbzvxen.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/ggofvnllb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gbvykovnn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfqvpwyd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/gjhrdubvg.sHtML

TS:   [...a, ...b];
来源：http://3g.epnwcf.com/Article/details/gfooyqkxh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gyndhnyfd.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gqjqkvutm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gahhacajb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gtuxvfydu.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/guaxjpwig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/grntbuknu.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/ggcfofwfn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/glsxwigje.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.bbcook.cn/Article/details/gwfvxwums.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/glfctltgt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gxrdjeffv.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gwihfjamw.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/gfblgnnql.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/glleypztp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/gzwosdbiq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gabshvlpj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxzecufm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gpsglnllw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gfymjplur.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.sjlbkw.cn/Article/details/gagogjgzt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/grizwkerr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.bbcook.cn/Article/details/gpyolscrw.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gajwhgbwz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.yfazqb.com/Article/details/goqikyahx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/govxvaibo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.tarul.cn/Article/details/giyqsjenj.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gczngjjut.sHtML

Java: Collections.reverse(list);
来源：http://wap.epnwcf.com/Article/details/gdxyqwcbu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.bbcook.cn/Article/details/gyxrkprmc.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gsohzgkgu.sHtML


<!-- 参考信息 -->