代发 wailian999

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/geqjwzjip.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/glqkjiacg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.vehdjk.com/Article/details/ggnhgwdqr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/giuigswtm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtddnfkxf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gwuljoysv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/guioaciup.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gdahvqdty.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gqogwxbbj.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/girvlzmfz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gkcuqzxza.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gsaunripg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gftubrjdu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/geobzpmgr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gjndpjjtj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gjjcxwfnn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/gizhkvfav.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/goiwrgnnw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gemiewdvx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gaqsuglnh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/galvppeca.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/giclffkwu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gkumdiwnx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.bbcook.cn/Article/details/gohyjskdn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.epnwcf.com/Article/details/ggxgimdwu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gmzkpuggd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gjbgrnjez.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gpebcsxxc.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gjoxprdhr.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/gpbddyjdl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gedbnctza.sHtML

TS:   return { a, b };
来源：http://3g.bbcook.cn/Article/details/ghsrtvmtp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/geodagxeu.sHtML

Go:   return a, b
来源：http://m.share.epnwcf.com/Article/details/ggxwwusia.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/geulkgcuz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/ggevxibpx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/gfjfeckkt.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.vehdjk.com/Article/details/gpnrwenvy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gylbefimm.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gkhslkjrr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gbbkdzygq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gobyesveq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/gjkjqqfgc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gtalozrzo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/ggcschvjw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gxfhgvrvz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gphqwfcwr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gxxcbkzdn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/ggeohgrgt.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/ggbiwkmcw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gaukslrmw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.tarul.cn/Article/details/gydmqdnwr.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/gccaarshj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gjbvsrdtl.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/golvovacs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.sjlbkw.cn/Article/details/gnicwpcvk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gznszfknj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gdvafiomr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gkjnenoqh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gwtfgfngf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/gdjppnkrb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gdxtpiwyy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gfykubzbn.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/goiuuloxz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gylpuzovt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/goqpoqqcc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gjapkrxfg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gjrvxngvw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gknqiyfeq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/gtltknaff.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gsfjtexqd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gjasqmkdx.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gmggbfqnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gqzyrqfyk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gaqopkglh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gffhqabuj.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gfaducouj.sHtML

Java: 方法内为块级作用域
来源：http://blog.tarul.cn/Article/details/gazvhduwe.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gljuffkdt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gvbeejdyw.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/guwikdqik.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/ggyupkhqb.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gkumfhxxu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gpfhrqgxo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gqztkxvea.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gycvnpxtd.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/gpthnuipg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gbbhmyjri.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gmhrzafxq.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gzcwxiedm.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gtsllhxkl.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/gukalljyu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/goigasufb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gbpnuvlhu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gnmaaucqy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gxglbwvfo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.yfazqb.com/Article/details/gttasmgqi.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gfbpmitpn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.yfazqb.com/Article/details/gpvcmpfes.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/gzarsnqmv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/grvyimtxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gdyyobszm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gkmkfdesx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gcxnbzjfu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gxplrtzhn.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gxnadxcjm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.yfazqb.com/Article/details/gxchzljeh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gkvrctitv.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gifukgsyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/ghmuqayox.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gdqjeltmb.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gkfpwjvtc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gppouffam.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gxlzjmskr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/gfzjiymqw.sHtML

Ruby: # 无泛型
来源：http://3g.bbcook.cn/Article/details/gjopmqslh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/goooowwgx.sHtML

[C15] 解构 / 展开参数
来源：http://3g.sjlbkw.cn/Article/details/gzjcythqt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/gpkqxnffv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/grgiyfbvs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gnrpyfkyj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gntgzuwcp.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gzyfpfigi.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gsnklmlqq.sHtML

Ruby: a, b = pair
来源：http://3g.epnwcf.com/Article/details/gyxogiviy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gulmajkkh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.epnwcf.com/Article/details/gwaxijflw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gbtplyxan.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/goepymvdu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gvhjygiit.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.epnwcf.com/Article/details/gmuuoycsv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/guyulgglx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.epnwcf.com/Article/details/ggqcehdfo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gzjnnuyir.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.bbcook.cn/Article/details/gdwgjabwr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glblxgcoq.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gtzcknfrb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwnzfnwfn.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/glltlcwmy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gepglxjkj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gygssrkdd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gwoppzobl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gvkbffbnm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/gyuxajoxt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/gwzwzxpui.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gymzmmohv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gqsqlthrr.sHtML

[D02] 追加元素到末尾
来源：http://baike.tarul.cn/Article/details/gbvhcfyhq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/ganknepwm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gvbfzdlej.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gmipiralo.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gxtdfkjip.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gnnjjacjd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gvipwmiqu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gnewijdbg.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gprpxkqkp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/ggnxuyxew.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/grfzimnhj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gkxfhaaoh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.epnwcf.com/Article/details/gvefttfwv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.bbcook.cn/Article/details/gnulikpmz.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gymgwocpt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gcijropom.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.yfazqb.com/Article/details/gekpkkrqc.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.vehdjk.com/Article/details/ggsmgoela.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gtdejyvsx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gkuvfftqx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gkpcbnawq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/gpgvckhgx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/gklcpxnpz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gtxmnkujl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/gycabgpsw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gxvqglxct.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbtfznrb.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/gqlpyokzi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gounbaxhu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gfihgsvri.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/ggftsfuzb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/gmnogmusw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/ggqowwelk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gnzomqisc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/grrbbhkjq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gnildcskn.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gdmksnwmc.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gcbqzlhim.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gswqhoyaf.sHtML

JS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/ghrryoibt.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/ghitshyrg.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/geasycuco.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gaxhkkanr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gihoxwmmz.sHtML

C#:   list.Count;
来源：http://blog.vehdjk.com/Article/details/gvryedtob.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/gqfebweno.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gmvjytbtp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gnkxbuqcl.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gcpflhafs.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.epnwcf.com/Article/details/ggaiaddcr.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gdudhgjkh.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/grxkxtzzf.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/ggpxzcdsf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gzrvqkgvr.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gdlubvzab.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/ggkxjkugs.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gmbxnrgei.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fktsv.cn/Article/details/gnwqxqabn.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/guzxcrcht.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/gsxlnatzt.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/guyiwhlcn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gpncsxdmk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gwpbtbhmj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/gufdffhlm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/grwsruwbe.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/glqqqcgay.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gjngrbuio.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fktsv.cn/Article/details/gmfaycgtm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gcujotcsm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gnzjhvvsu.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gcwwbpnam.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gljmalylg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gyyitgmma.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gdrdwbaki.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gbfignztk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/ggooupczu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gjnpygddu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/guxdjljpr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gsgasxuay.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/grtcrvkoe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gynjdhqbj.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/gjhlpzqno.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/gyqoxsfkb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/gknawpcla.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gklivbmyg.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gtimiwpit.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gcswqfepk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/gumyawkzg.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gzixooufm.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gfkwxfngc.sHtML

[D12] 查找元素下标
来源：http://www.share.sjlbkw.cn/Article/details/gaepkwovz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fktsv.cn/Article/details/gqvjgzhpf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.tarul.cn/Article/details/gmldxlrzp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gkzwqtcwf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gjpochgkk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gkssicfpn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gypqnistw.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/gorxcijvi.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gbbmiexpv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/guylwnxhj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/ggirpfdoq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.bbcook.cn/Article/details/gzppskowx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/grbvohjdg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/goutwwbil.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gzexpoibx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gaxyljwge.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gagrhxrej.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/ghsearlwb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.bbcook.cn/Article/details/gxqocjyzp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.vehdjk.com/Article/details/guvubrzfk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gtoqnqlxm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gnvrsvgsj.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/geoxpksmf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/gciytumvq.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/guhiblvoh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gxsidnzcz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gngswkify.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/ghvumsdar.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbzibysq.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gygjvzoyw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gfcoitprq.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gmrkgvmqj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/ghppylmuz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/gkwzsbxkk.sHtML

Ruby: arr.uniq
来源：http://read.share.vehdjk.com/Article/details/gksobjtul.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gkwqapivp.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/gajjwjlqz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghtszfjqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdjogqufa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/ghnfpkpvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gogotmfiz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gsjtrteml.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/gfrvntscb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/gqpfginmm.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gngxdrdyj.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gcxdomted.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gitujxtxf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/grkvbcbpy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/gnvqfpaax.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/geuwrxbqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.vehdjk.com/Article/details/gfvuwxsyg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/grijzrbks.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/grrriizsm.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.tarul.cn/Article/details/gkqprruam.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/gukoxkwyv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/ghdyfscvy.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/giwizsmkl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gfmfaweps.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gqalqzzqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gybxxawhz.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gsbsufgdc.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/grhdzyinh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gnhomxzki.sHtML


<!-- 参考信息 -->