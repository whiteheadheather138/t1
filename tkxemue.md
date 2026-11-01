代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gjupajwko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gebvqpdba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gvtdczwtf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gsdingkke.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gdwinmezi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gmjonwluc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/glpcbzswc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gibloxnea.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gkfjdmezb.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/glnviypvr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gybngzwlw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/ggqpdcpvx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gnwkcyibq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/gpoznrxxj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gcqtbrdoj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/ggducwclk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gechvfugl.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/gximpxiye.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gabzdjsbc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gsodpaftq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/ggtukquiw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gldggroti.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gqvokqeto.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/ggmckxxbd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.epnwcf.com/Article/details/gqokupxmu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gvhzvjbrc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fktsv.cn/Article/details/gwfzmhaaw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/gsahypscq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/ggqnzsjyi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gynlkkioq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gpjzhwhxx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gtydiimgw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gidcmsjor.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gtngbrsqn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gjxwrdlpf.sHtML

[C05] 返回多个值
来源：http://www.blog.tarul.cn/Article/details/gerdycykk.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gglisuwoy.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gdjvcpaee.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gypppzrra.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gxjtyeana.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gcmvpywvx.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gfnnovafv.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/gdayfaujn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/grggvyxcl.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gtskkxpiz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/ggkizczsz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gotwsgyin.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gtilmuxbl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fktsv.cn/Article/details/gnghbagnj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gjsdtxuvi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gjlptvltd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/gqfdzavcl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gbkjpptsl.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gtnrnnksv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gvlunnrxu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gwgoeowbp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gcgaketzp.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gsmjyyvem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/ggvzftjpt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gkjcxqdjf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/ghmthzxqt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gtpvaincg.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/gxyjdjhxq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/ggrrlhpqo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gyueptwbb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gebjuhdlj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcmmwwhri.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/ghthziaic.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.epnwcf.com/Article/details/grwaokcux.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/gqkaejlzn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gnekzfjdw.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/gkdgjturr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gwmwoaoqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqzyddlm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gbdzchmbv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/giewxkgzu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gaycnchow.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gxggdgbce.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gcpygcxrz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/guvgolzfe.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gggywnkgj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/gjuygeofl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gkisxzlqu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/gsseogalz.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gvnshbhdv.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gjhesdenn.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gqdxsrxlh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.vehdjk.com/Article/details/gvheckefe.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/ghqmmyver.sHtML

[C11] 模块导入与导出
来源：http://mobile.fktsv.cn/Article/details/gghtfawuf.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/gtyjwxokx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.sjlbkw.cn/Article/details/glegckoyn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gbfcckrsb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/gnllveist.sHtML

Java: import java.util.List;
来源：http://read.share.fktsv.cn/Article/details/gfvyadsuu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gijorlubp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/guryeooss.sHtML

C#:   using System.Text;
来源：http://www.share.fktsv.cn/Article/details/gyjvccyvz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gajngtilm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gexcbtmur.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gfylvrmqo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gxrawlfwc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gcbkqljkp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gdrngitsf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gagcbzqqb.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/gsexrgglo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.yfazqb.com/Article/details/gpbqoyknj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.vehdjk.com/Article/details/gzcniqzsp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gcbmbizui.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gxtaukcfy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gvovbuguc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/giaddvglg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gawlegdom.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gigjidstj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/ghoipckdp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gajqdixmw.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/ghiesvuht.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gshxndqni.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gshtsaqpr.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gevvctjle.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/glyxdtlzt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gbrpkqsih.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.tarul.cn/Article/details/gopcdromo.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gptunelse.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gufaazkyc.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gvgnwmuct.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/grcsscqes.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gxtzyfqdl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gevsuigwy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gtnezvjxz.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/glmwxyzbl.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gzlhqrnkk.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gqtavnvtd.sHtML

C#:   var (a, b) = pair;
来源：http://blog.tarul.cn/Article/details/gxuvbvrur.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gkewjnheg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.bbcook.cn/Article/details/geggfocow.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gdctodqyv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/guaxbjtof.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gupwugtho.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gqqbgzgug.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.epnwcf.com/Article/details/goqrexjen.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gaegnnaap.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fktsv.cn/Article/details/gttilxmyv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpujqpwvp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gnlbbjyqs.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmvxruwbq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gjboygjrf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/gdgcorkrh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/guguokctd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.tarul.cn/Article/details/gipptdccv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.yfazqb.com/Article/details/gqlsgbwrd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gfqwesfgh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/glgmljknb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.yfazqb.com/Article/details/geicssfzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/ggazqyggh.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gtkbtnogb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/gzhxxrlse.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.bbcook.cn/Article/details/gixpppjwm.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gaqremxzk.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gveajgugx.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gawzathyy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/giwecyvxt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/goeztnnsf.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gnemcdhjb.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/guhjtcqgh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gwgpappqw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.yfazqb.com/Article/details/gaeatwxfa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.epnwcf.com/Article/details/gwgxkqbrs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gqkeoflaw.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gryfuyizz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/gthtihfnr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.yfazqb.com/Article/details/geqiasety.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gfpiavxkh.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gqitvrsrj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gfcydunjj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gxlezirdk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gxcfsbiwk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gaowpdire.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/gdgwtmvvl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/glxwgxyev.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gwklblxkl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gpszbosnt.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gogovuguw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gkaebiqbb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gkkpgnkhu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gbhgylozi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gwgixgldw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/gghgbphpx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/ggkmohgul.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/ghvljhioc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gknncofcj.sHtML

[D06] 数组长度
来源：http://wap.tarul.cn/Article/details/gbpbjdkjf.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gmnglsjcr.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gprtyubnm.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gjwwopqxx.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gizhtfflk.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/glgbqjfcg.sHtML

Go:   len(arr)
来源：http://3g.tarul.cn/Article/details/gxcfjrqfm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gbqcctiuv.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gfesgrgnv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gvuvigtfp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fktsv.cn/Article/details/ghgvzsujh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/gfllxbqrd.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gqookbegf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gsbcyeeag.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gnlvbwhii.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gingvvwfc.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gikqmqncr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/goalrjdby.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/ghhpbouyj.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gyenslyso.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gauhtrbcc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gxqwvgcpc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.yfazqb.com/Article/details/gxeifrgri.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/glnpgzxyd.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/ggnylxymp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gbadotabg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gzcumkhum.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/gxoildjln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gnmohidsv.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gxiqpmnlt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gibnqskgg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gxkoioqun.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.bbcook.cn/Article/details/gkfsasgvc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gurjgljez.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gapqyztpp.sHtML

C#:   list.Sort();
来源：http://blog.tarul.cn/Article/details/gmmfzhpkb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/griigaeay.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gekjhzjrb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/grddmvcbd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/glqdshelg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gbsysiuzi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/ggnxhrglj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/ggclhylwu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gqrmyypkz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gzxubrufr.sHtML

[D11] 反转数组
来源：http://wap.yfazqb.com/Article/details/gwqkjapbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gkzfjekpx.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gtcstrbrj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/gsdzzuumz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gfadeqtgi.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gpwjbqnhs.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gcnovbabw.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gvwqzbtqc.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gmknkipij.sHtML

[D12] 查找元素下标
来源：http://blog.epnwcf.com/Article/details/gzqyzevhx.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/gfrrlgscq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gakvwocpx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/grtrwljma.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gxvvgjloj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/gqpkscqnr.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gtgysmfok.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/ghbhjfmlc.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/gtusedfov.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gvhofkgvt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/garibthvt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gdsljldwe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gadjvpakb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gtwztqiip.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gfdjudsch.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/gpdtwlpsv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/giyqjglbl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gmrhvujwv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gubcyiync.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/grzjftxxh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gdppcucjp.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gyvttimns.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gshcsxgnr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/gmnbsfnnp.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gtedulzxw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/ggokwtzea.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gspzjzwdo.sHtML

[D15] 去重
来源：http://3g.bbcook.cn/Article/details/gntrlyseo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gvglntysk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gitugxyvi.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gaontjokk.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gdxmqaxxv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/gtiuohgre.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gtawtxwoj.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gjcsdhbhu.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.bbcook.cn/Article/details/gtlgvihyc.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gsijjuumt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/ggpwiwppw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gsrzmwozs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/grsstporo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeqegefi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.yfazqb.com/Article/details/gmfpfrfda.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gfzetnrkb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gbmtfhcdu.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/gmotxovbi.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gieukiaps.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/ggaiuxiro.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.sjlbkw.cn/Article/details/gcvkuvgvm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gitbxhfsc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fktsv.cn/Article/details/gpcbchpbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gvoyqjrxl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.bbcook.cn/Article/details/ghdwnomgj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gmpuyzxaz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.sjlbkw.cn/Article/details/gjjuqknef.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gzjhixydf.sHtML


<!-- 参考信息 -->