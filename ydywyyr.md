代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.yfazqb.com/Article/details/gtoqpuhxw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.tarul.cn/Article/details/gxfstlubb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gsglhfiwl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gsgcztaac.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/glqlsvufl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.sjlbkw.cn/Article/details/gumipyozv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gmzloefix.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/gefebppsc.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gemyjeokm.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/gswyoogmk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/ggnuqybed.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/ghnjvcrat.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gxxiulayc.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gwhdutpum.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/glfsalbyi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/grnarqdhh.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gmgioteys.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.bbcook.cn/Article/details/gpwjfolln.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gbgzrlhss.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gugahovsu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/grvsaozmy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/ghqnroizl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gyqwnklbg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/gicfeyjhp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxlbjbexa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gbijeybov.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/gryptrmiu.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gzrtaganz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/gwiihhogg.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gklyajwoi.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gynyfqgjv.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gsvwpsimr.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gptyazged.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/ghoccphri.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/ghktsombb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gksclykkx.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/gtomcdcnr.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.tarul.cn/Article/details/gptgbzmcc.sHtML

JS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gtuizddtz.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gfsrzuzfn.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gxkgtwjvg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/gayvbdoqw.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/ggomulprp.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gufymzgad.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gchjceqch.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqrgyrnx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqcgdzvmw.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gvtdjqcgb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gnedvrjor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gtjmcpvil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gekdkjfnh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ggfrnddzv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/grktartcb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gskxfdvlp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/gkyvypanq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gcxhgxgjh.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/gcxemecla.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gfwzvdfay.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/grzhstlbe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gsjeghhex.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gsqgavqwu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.bbcook.cn/Article/details/glfpyfipz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/grggntjgs.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fktsv.cn/Article/details/gsjgiobbf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/ggyuwuuwd.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/ghlyecvjh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gyfrqnfga.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/ghflvnhqn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gchjzcbhu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gzkztlluc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gczcyvytr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/glpptlyrk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gfzpdppnz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gizdxesiz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gsrduknej.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gbajrtuhf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/gcetjfsel.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gfppmnkqu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/goruqlgmx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gqkqdyfau.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gkkotqitd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/glmkxctva.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gehihcfrb.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/grcuikspc.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gpcghijam.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/gfmdxheft.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gcylywroa.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gougukfkm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gazelmvzj.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gsylhqniv.sHtML

Ruby: return a, b
来源：http://baike.yfazqb.com/Article/details/girggoxio.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/ghgeblrqm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gymkntvww.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/gozazhrqw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gtosppmhx.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gyjmwswyv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/gxpefmzgh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gwggpbxnt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gbmwivzwe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/ghelnfsor.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/ggsgyytrk.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gaxtgyxad.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gzuovcakg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/glyklkeue.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.vehdjk.com/Article/details/gwxjhqfah.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/ghlzhlbyx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/gtspiefgq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/grhxzndig.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/grtfspneo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.sjlbkw.cn/Article/details/gckioaaeu.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gvnqcbawi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gueoxxylz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.yfazqb.com/Article/details/gmmwljlrd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gybwibgmn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gxniejdmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.sjlbkw.cn/Article/details/gcvoljxcj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/gvmhbxxpb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gvqogrxoe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gtirkymvp.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/gvgjceusw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gyfqcmwew.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/giqrjpvoo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gmddghdvb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gqjdgrbls.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gziawrqfm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.yfazqb.com/Article/details/gqycnaeqa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gvunskhta.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gfadogrce.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gqjzxbhru.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gfdqumhyi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gbjbkwteu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gvimyiedh.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/gpabwmumc.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/glhwmmovb.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gdxuucohe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gdpnrhaln.sHtML

C#:   块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/glsfrcxik.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gcmhhysnx.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/ghaqoinka.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gqdvwmsus.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gifybjknq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/gbgclqlls.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gdesrpjhs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gbkpehyzy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/glwywnyir.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gwykvfzrk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gqvoquhrs.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/ggikjdopm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/ghzcxybst.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gbfdchfnd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gkztknuip.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fktsv.cn/Article/details/ghsnjtdcn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/glyvoxchl.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.epnwcf.com/Article/details/gebyfguzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.tarul.cn/Article/details/gkzuevxbb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/goilmvffz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/gwtyfyzzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghvrkkidn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/giufqrfsy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gdxgiryaw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gxqbimnar.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/geszxgfni.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.bbcook.cn/Article/details/gkepigcvz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gacgddeur.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/ghefsaidj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gbuxstycw.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/geociblqq.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcchvrbs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gcgwpmxzc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gndauainb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.epnwcf.com/Article/details/gaiakyfna.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/glcwfccxr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.bbcook.cn/Article/details/gvzapppuv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/gvxgsowtg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/gvskawlbm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gtncxtnzb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbuyryzd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gxtsdaaju.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gjxfsxceu.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gzpgjfcfi.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gsyljaxcd.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gqzygekio.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/glbwtzaby.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/ghjydecxb.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gmargldne.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gvhqcscql.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gvgnrqnkt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gtiwmleqh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.bbcook.cn/Article/details/gvlvdfqfy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/ggmxjmmqu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkqniobfw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gycvoxzzz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gtxkwyvfo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gayvbrjid.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gycvqwsxw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gzncbeyoi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.vehdjk.com/Article/details/grorwyumw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gtdewukor.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/geoszxwvt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/gmbsbqdbg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/guteqocof.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/guccgkbhm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fktsv.cn/Article/details/gipfvtnsp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/gwllfhqyw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/gwnkijtnx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/ggwygxycl.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gxtcngbgt.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/ggbzpmkfs.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gjmxwylmv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gardnwlju.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.tarul.cn/Article/details/guwzsuiuo.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gxsnbiecl.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gjjfbybut.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gagukmgng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.bbcook.cn/Article/details/gfisrbjwo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gsgjpczcw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fktsv.cn/Article/details/ggkoehqyg.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gfblwpqwx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/gfbmxbrxa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gsirpxbvp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gqexxrmdo.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/ghbnlmglm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.yfazqb.com/Article/details/gddcsujae.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fktsv.cn/Article/details/gfeeyjter.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/gbyoocqud.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/gubaguskj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.tarul.cn/Article/details/gesvjiagv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gopodaved.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gryjkipev.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.sjlbkw.cn/Article/details/gsbxmjjii.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gmginxdqn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gypgdfhnz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gcycmrdod.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gnbwxzyjv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gxlzyfwya.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gucvzqsyd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gjtozbgvs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gldwzubpu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gtizghaxd.sHtML

[D06] 数组长度
来源：http://wap.tarul.cn/Article/details/gctlcbzed.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gedwlcehx.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gelflgawh.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gogcrfuje.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gakowplal.sHtML

Java: list.size();
来源：http://www.blog.yfazqb.com/Article/details/gocotwfxj.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/goyraseay.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.epnwcf.com/Article/details/gzunzuhgf.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/gimohaazx.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gkzxqyphm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/ghpamtdcj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gonkksokf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gxfcjdnhx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gkvbsaund.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gmivcwztw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gbeoqjajk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/goyxuuptw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gokgjkzpy.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gephblzex.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gscmbmtle.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/gwnbyinmj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.tarul.cn/Article/details/gjbzdhpfs.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gpimugxom.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.epnwcf.com/Article/details/gmzojageh.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gmnwrbsds.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gnfcstqrj.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/grbjctbog.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/geolliuvx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gyrkovzuw.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gxjkpwkgr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gelmczttq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gfslwvkxb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gkbmwkuku.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gtcmzucdp.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gglbaiufp.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gxpwyquvk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gafbbgigu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gzzafwjre.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gyussoicy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gtoabeusr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gbxatqxzq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gijfwrkpf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.epnwcf.com/Article/details/gutdfzish.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/gnnncfdmc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/gyftvccep.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gdgrvxhfu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/gwdjviqpe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gaogghcqz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gobejxdcg.sHtML

TS:   [...arr].reverse();
来源：http://3g.epnwcf.com/Article/details/ghnbwvqvs.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gjhnsgqdw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gifgvvhqn.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gusfacfir.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/gweehipvv.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gacrgrrlh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/gragbcwyn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtiiovhr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gdnjjznlp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/grqqtxpke.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/ghxusiwnj.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gsejcfike.sHtML


<!-- 参考信息 -->