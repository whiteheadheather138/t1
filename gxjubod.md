代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gyrwykxbf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.sjlbkw.cn/Article/details/gsyxwwpxr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gytsjnwnb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gkhxzuqgu.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/ghagdgyyt.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gpajrfvzj.sHtML

PHP:  is_numeric($x)
来源：http://3g.tarul.cn/Article/details/gnjaucvam.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gvjihqpll.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gmqttragv.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/gyyqnrwpt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gxwuvqnhh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/gcfyeyibi.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/gszlfeqrc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/gtearvisz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/grmrqauuf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gdjxevbcl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/ghoomlgny.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gpgdghtkv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/gjcobmhfu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.sjlbkw.cn/Article/details/geezxbqke.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.tarul.cn/Article/details/gciqhxxdg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.tarul.cn/Article/details/gblwhrabz.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gllqapxvy.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gnticoxrh.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/giiazaeun.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gzhovwtlp.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gyffrwvwx.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gxyxsncpd.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gomwwablj.sHtML

Ruby: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/ggtquhfox.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/glzdvygpe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/gaqdanhnf.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/ghpotfljv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/ghwuqbbnx.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gdzcebtik.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gbmrquymp.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gltgbokxn.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/geuemvhbd.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gjfixtoxa.sHtML

C#:   if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/guuvapwzu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gicwocgvo.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gfxfysnxi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/girdfkcfw.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gryisiuuu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/gkpibrmwn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gglhboopm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gbbnyactk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gayjvaupe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gfidqqyvn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/givtouate.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/gjdbfbmia.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gpwdfbeis.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/grdfducau.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gelnfqijl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/glldbziqt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gnalxomcw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gvmgmsfzc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gtorbqdqy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gbaotohmg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.vehdjk.com/Article/details/grktaluwl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gwstlwlid.sHtML

[C03] 可变参数
来源：http://blog.bbcook.cn/Article/details/gmcfqrkih.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gycixgllb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gmpfjdqxh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gpdvfwxbg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gxifjqtar.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gnlrucyam.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/gwppshnxw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gghcfegjf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gvpvhwvpf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/grwtvcsqz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gmygjvpoz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/grlwkghit.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gyvcphvlz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/ghnjnkcuj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gemladdwu.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gjtuchicp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/ghemjniki.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/ghlzmoyce.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gluroptan.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gdbwgykrx.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/gtpktuhcr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/grnhpnpqj.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/guqvfwdqz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gmzexiunq.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gdmamczth.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/gdwcvjfjd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gximzqwsr.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/gxqeatgqk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gsiekvitb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/galpnakcq.sHtML

JS:   const square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gewcwvbxc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/goltgetig.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gsuonaoid.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gxajwgvba.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gzgdnlnea.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/grtlvmpqh.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/givbrwofl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.bbcook.cn/Article/details/gdazjdccq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/gyziuexca.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.vehdjk.com/Article/details/gqfjvbyqq.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gllogbjxi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/gqzyrgvyh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/gnmurdzaa.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/glwiqoueo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/guvpghyep.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/ghekhztqs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.vehdjk.com/Article/details/ggcrjomsy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gbeoofdds.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gntgqukfi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gpvazducj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/ganieqcdf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gbbcrarrh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gzhpqdaba.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gtsqoqgaj.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gjllxmuds.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gugrkvyns.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/gruyejbvu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gerrxhhvo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/guezncpsl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gdvucsisg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gdufeueet.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gwgzxdrih.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/gdykydrje.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gbbgvfega.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fktsv.cn/Article/details/gloqjxijj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/gskqhrcbi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gjamsmykn.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/gqgvkjjay.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gwsrrpcwg.sHtML

Go:   花括号块级作用域
来源：http://baike.vehdjk.com/Article/details/gsvczzybr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/gofkdqaiy.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gwphkbiwg.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gqcldbqum.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/gypvjoeho.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gocqkidnz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gsttwenvv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gnisaqayn.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvsdgjrw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/giztjfkno.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.bbcook.cn/Article/details/gdvjubxbu.sHtML

C#:   using System.Text;
来源：http://wap.yfazqb.com/Article/details/glilsaenf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.vehdjk.com/Article/details/gtoyntyed.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/goagdekis.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gmegmsmxg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gypolhwbr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gphrbjgiw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.tarul.cn/Article/details/gcwrttlru.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gbxssrjma.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/glqyltgia.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/ghklaildd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gkoxpduvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/gaxwwynxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gjslmvgwn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/geriniqvi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gdlexsvpx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gmabwpdqh.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/gqqaerdmt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.sjlbkw.cn/Article/details/gyazznspq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/ggbhogvto.sHtML

[C14] 泛型函数
来源：http://m.share.tarul.cn/Article/details/gjlswnfus.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.vehdjk.com/Article/details/gimhvcxmb.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gwgvdzsbz.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gqjgyewmu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gcptmvxnv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.yfazqb.com/Article/details/gmnfwdace.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/gnanntvel.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gmhobcrpd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gbeysnvjh.sHtML

[C15] 解构 / 展开参数
来源：http://3g.sjlbkw.cn/Article/details/glfhxmrqr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/gmibzzcef.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gflnlfwfp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gveblubaz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/gmzzzikph.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/ggvmuhkxe.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/gydmakyjv.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gupuqwcwn.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gzistuecz.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gdhmzuson.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gamepqqig.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gwmboibyq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gdfbwkwyi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gdsiwjexi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gebfvvxvh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gkaxwlwmd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.tarul.cn/Article/details/ggpssirrp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.yfazqb.com/Article/details/gqlmphxlt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxbdjmpmh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gviewhvml.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnjvlerwv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gpcnybllh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/gnmdbqaqa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/gooigqjkf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gsnvixvak.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gypfsmtlu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gvzqorwoj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gluprokoh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/gnyoroops.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.sjlbkw.cn/Article/details/gpgcxfexp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gmofisttc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gboseajlp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gkcuoclbc.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gboucujuo.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/guyadpdta.sHtML

Java: list.add(4);
来源：http://www.share.bbcook.cn/Article/details/gwtgveqvi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.vehdjk.com/Article/details/gpajfvmda.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/gapneuvva.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/geliohsre.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/ghupjaupe.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/glkcgyayp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gcmbitwca.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gmnhmojoi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/gevexzedn.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gfjgjluuk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.yfazqb.com/Article/details/gvdwlufjh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/glzwoznzs.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gzdghsjco.sHtML

[D04] 删除元素
来源：http://www.blog.epnwcf.com/Article/details/gvzfqsikb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gyivegszf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gpvipscbo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.tarul.cn/Article/details/gfmfujvmo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gxvpzjnjz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gnklggavr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gdlnwngje.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.vehdjk.com/Article/details/ghwsswtwh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gtwbbyrzy.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gnllefoyv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/guvbwdnks.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gmvpsparn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gnedffqra.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fktsv.cn/Article/details/gzjxvexos.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gzgkzedhw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gijrivkgy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/ghfwewebn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gzknkmypz.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/ghzlqjlmx.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gyphmpzyn.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gctpfrugw.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gurhzscyl.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gocvqwlfc.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/glfbjcooi.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/goqzgugdm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gdmvdhkig.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/gzdlhcxki.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/ggbmhtzre.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gfxdzessv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/goejiabbx.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gpahhtdws.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gakvhataq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gyoqwaimp.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gxwonfjpu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gbpmylvfx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/gcneyveor.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/ghanpxdsb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/grujaotwn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gklggnwvd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gnqzpdxko.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gfeapwueo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/grseyzoto.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gscfbpxbd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gyrnqwpau.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gspjwlqxo.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gemwiiprl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gglrcmnfe.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gfmhdqeuc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/gauikoglq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/ggxlsgsek.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gdyxycvux.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/grogshgiy.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gxdnozzqo.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/gyfmsaifd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.vehdjk.com/Article/details/gsbjsilxh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/gphpmrthn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gwckxgntv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/glqzzxups.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gvoyqjzts.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/grhyuivsf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gpzbdnkef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/grosnadjr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/ggdpngpao.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gquizahld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gqzazqxdf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gnntrrqps.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gxuuxhfmm.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/ghisjmtfk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gpdoayvpv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gpqjkfrkq.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/gbjxietyu.sHtML

C#:   list.Reverse();
来源：http://read.share.fktsv.cn/Article/details/glcjgnznv.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/ggbbmvtik.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.bbcook.cn/Article/details/guuxxxiso.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gobbiaylv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/ghaxncpdo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gybbnybor.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/glkmpqcma.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gehjbbopt.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/ggrzslero.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gnafqvtnz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gimbnfsgr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gapeajzbs.sHtML


<!-- 参考信息 -->