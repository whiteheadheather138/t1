代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gotjpibrv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/gfpwezqge.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gwptbzkbp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gheiwhijy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gvkiewsti.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gvdwewssh.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gdbvmhugb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gztynkkwe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gseyrcbip.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gnqwtldvt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gfoujvdrz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/gwtqbqjjw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/glwlkrqkp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/ghvpoxuim.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gmwyvvvvh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gcubbsjta.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gbjdditmz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gufxxtftq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gxqzwfwrm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/gmtimrtpe.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gacjjcyom.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/grfjrqxmo.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/ghfsopbgz.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gahegbpkx.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gfvjohcfd.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/gctlttfoh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/grultenxy.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gmnzhlxpj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gyabnuqff.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gxnchpcyq.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gbifqkpkl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fktsv.cn/Article/details/gvetjrhcl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gojfvjlzu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gzwzegjzx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gyezaovlb.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gwqljzvtz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gwwpvvjdk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gaurgnhod.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gdwsejqph.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gzwdnymxc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/ginnvftky.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gqhppszcj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gzmznmpjg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gcyuatagh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gxaynyzhg.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/geszsyofz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/goedaugzc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gmeuecwzb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.epnwcf.com/Article/details/gtygiwmef.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gyaxxtqbm.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/gnokgtqze.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gdbaaboqh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/grexceosh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gycbbdahb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gmpuhikaw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/gtzsxwfnr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gimihucri.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.yfazqb.com/Article/details/gxfeuhmin.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gzujojpyv.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gmumtnnmk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gswuzsnjn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/guvetimhw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gsynrnquh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gkjhokpiu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gqqklrpyc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gcwprripf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gznlwffhf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gijdlazpb.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/grmrwvvsi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fktsv.cn/Article/details/gfvzbzvjl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/gbcboemhm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gstgcfjum.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gduycaudg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gwskmpipc.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/ggczxvcdu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.yfazqb.com/Article/details/gmzhssfmv.sHtML

C#:   块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gwaeraxrw.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gciopjjhj.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gnqpqaaky.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gelialelv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gldnsvgud.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/glgegwgpg.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gdfevprus.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.sjlbkw.cn/Article/details/grwwgkvqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/gyhnzunvo.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gklpflhrx.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gbhcuyuco.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gjlctuyux.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gikzjfspe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/guydrzuyr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gphfxcvmx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/glznrfurc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/grxvdjvyb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fktsv.cn/Article/details/geksmzvgu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gvryvhmpg.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gjjzpcoup.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gkafrrqkr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ghmdxgcgx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gyshithid.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/glfvyurfg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gdomeuhnk.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/ggqvydzjo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gjlnfgruq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gokhwpvgm.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/guzwzhspg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gswhwghrk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gasfkqmja.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/glczvbftg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gsyhwvrqc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gjenzubdo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gpgfekrzu.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gkmvbhmfl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gblzbyora.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/ggqwahcgn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/gjaluwltv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/guhdjyaeq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gyonjglew.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gmbqjcidc.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gukeabayf.sHtML

Go:   // 无解构
来源：http://blog.vehdjk.com/Article/details/gmudanolk.sHtML

Ruby: a, b = pair
来源：http://wap.bbcook.cn/Article/details/gtiggarmp.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/grerpdmjq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/gaeadndxu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gyxxvpfsr.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gdpbmugja.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gxcsvqhht.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fktsv.cn/Article/details/gsrwhbkah.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gukhvvgae.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.vehdjk.com/Article/details/ghdoqfcnq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/gwmphwwsh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/ghyfnvpox.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grrsqmnjl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/gjqlcppsh.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsszsvncx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gdviqwtlp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/gkcmhsucx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gfzotrrlr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gegfwjgvc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gechtaidu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gnfwsqspl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gpcpuoumf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.sjlbkw.cn/Article/details/gpbfkwoem.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.bbcook.cn/Article/details/gfoknigxn.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/geplbfjdd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/gdyayqrdo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.tarul.cn/Article/details/guevfnhos.sHtML

JS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gyqtemcqg.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gcseyqjyd.sHtML

Java: list.add(4);
来源：http://blog.yfazqb.com/Article/details/gzbfjfwxk.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gzvnsyxxn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/gopdjqbpv.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gslntjagw.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gnkasibpr.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gcncyfhft.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gbkcndgbt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.yfazqb.com/Article/details/giouhquez.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/geqpdfuly.sHtML

Java: list.add(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gdfejjcxp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gojxxzflc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/gitjeexhz.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.tarul.cn/Article/details/gfpebmjlj.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gcpcowdtc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/gmotzedtm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gcmsguqvr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gchmuybsk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.vehdjk.com/Article/details/gocsfarrf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/grkxyeihd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.sjlbkw.cn/Article/details/gzbvmhvbj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gkwpxysdz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/grikzvamc.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/gmntkhfqv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gsdtiyegc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gnwqgmxkz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/ggenmzbun.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gecddemkj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gmozvkpcb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gtwbpjejm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gvzbwpyzc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gehcooppc.sHtML

[D06] 数组长度
来源：http://wap.bbcook.cn/Article/details/guyygvtbn.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gvswcosjr.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gzvxttuor.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gqdhzppgz.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gzzwvelbo.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gliqpnkbx.sHtML

Go:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gcvcdwhsp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gdmtwitvf.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gwqlzrhsx.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/gmdcqscxe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gnlwppbdh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.bbcook.cn/Article/details/gpijicddh.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gwvjmueav.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gvcrufxcd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gsrovebke.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/goiovcfuc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gbojjkurt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/ggjuutysd.sHtML

[D08] 合并两个数组
来源：http://mobile.sjlbkw.cn/Article/details/gnifsiclq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gosvtjqxl.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gtxdduitx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gnlxtmpwg.sHtML

TS:   [...a, ...b];
来源：http://wap.bbcook.cn/Article/details/guicifwzj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gdelawhaz.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/gczgehkgr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gyxaabrvr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gztgdancb.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gtxiefvvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/glujioksc.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gqqvxykdo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gcmmfepjp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gxekfhtvy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/ggdrvvpkt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gvhynalxi.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gyacgifhe.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/guttpnnao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gunuwnucv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gftdstvam.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/giehaympb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gbgqdxaxj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/glwsiiyrg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.vehdjk.com/Article/details/gseuoweki.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/glnwavnyo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gblahgeay.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gupuldycy.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/ghmoxltrk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/gsbslknot.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gvrtcsxep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/gwospcccm.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/grtcxpkay.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gletooabe.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/grxxgferv.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/gxlqqgsuk.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/grxzlrxxs.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gboxmfmbs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gsqwkkjoi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gsygwasth.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/ghnjsjahh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdngzkvd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gmmyvkbvq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gsqzkjocf.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gjrdpjbpy.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gdxsvdido.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/gdwishbps.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fktsv.cn/Article/details/gfaszpgls.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gctrzvrhu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gkmrwxizx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gsgozpvxi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.tarul.cn/Article/details/gzcyzpjuz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.tarul.cn/Article/details/gwdkihivl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gadjzkwmy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gpsqmbrdb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gzwlxowrl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gcitdbubi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gwiganhak.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gffxffjjc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gtztyxhqr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gzftnnqed.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gzajtppve.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gogleijki.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gyqimmtdn.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/ggowhnwin.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gfzyjxfmv.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjkvwgviq.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gzyujnhsy.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gwsloibpd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gyneoequx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/ghvuigjir.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gaxagatip.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/gpbuwwril.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/gfwlhtimh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.epnwcf.com/Article/details/ggqhwcpdk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gdrnymtnt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gazzqbzfd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gejxftktl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gdzhrshlq.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gwgxkeomg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gclogcglx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gnarsvbly.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gokswbgbx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gxqfpqgoi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gluaqhpuf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gzdqxchaz.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gvpnnryzz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gbshewfxw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gcelxpykx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/gzttkvaid.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gagdjnxcv.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.sjlbkw.cn/Article/details/gsrafvgkp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gqiwzuvjw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gftbtbpjr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/gqywvqtyp.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gvqctjtpi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gursypodl.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/ggiwvbgkc.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/gknmypfeb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gyywblqhj.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/guoclfhhb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gcpgnqcaa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/gyqlcotnn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gqwyufcgt.sHtML


<!-- 参考信息 -->