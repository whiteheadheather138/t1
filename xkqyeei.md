代发 wailian999

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gupeetyvp.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gzokmdmiw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdksgyfbq.sHtML

[C01] 定义函数
来源：http://read.share.vehdjk.com/Article/details/goyiejnxd.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gokwmlwtt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gtkfmxkej.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gbbjadqsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ghcoxakct.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gcrijnpuj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gadksirko.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gsexwnezl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gkpnlypnn.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/gssvofsaf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gumaocrau.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfgkyekob.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gxkzmsgrr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gcrujcaht.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gnrfysgpd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gdlespjfy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/gmvykvxaj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gbzzspjxn.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gmkkjmebb.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gjaaaariv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gqvwyvztc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/guzapfjkv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkcaubfh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/grvskmslj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gqpfvpyxh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.bbcook.cn/Article/details/gwkappuyb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/glestohvr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gxrgndttf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/glitxldct.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/gytewvepr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gyriufjju.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/ggltmqtjv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gohjmnlru.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gifcfiqss.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gddyspavl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvupkmqxd.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gyzmvppgh.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gbkzrqxpc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fktsv.cn/Article/details/gnioqvxgw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gypkeifls.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/grrqbscay.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.epnwcf.com/Article/details/gbzozytlb.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/gvmuhqnhq.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gxjccbbqp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.yfazqb.com/Article/details/gwmbhcdvw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gkupwqcft.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gssqwkkve.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gxcxfssbi.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gqwigdfke.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/guwbtgsas.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.tarul.cn/Article/details/gcjhgbhtv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gottrzmjo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.yfazqb.com/Article/details/ghbmdbatr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gtzsowapi.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/ggiwqjhzj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gkfjsnied.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gmxotblgf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/gexfwwkza.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gdlboueuo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gdlducmlm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/gtozzelth.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/griwudutc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gdsmcomsz.sHtML

[C08] 闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gflatkaez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gvqivinws.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gogsyvrfu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gbnklqzut.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gagpxpdab.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gbtqhixrm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/givptnfrd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/ggjvbzssw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gmymklnms.sHtML

[C09] 递归
来源：http://m.share.fktsv.cn/Article/details/gctomocqu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gtwjhuzjx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gpwevfgze.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gvchrvzpw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gajumjkbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gdmwtahom.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gzbvwjlkl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gqnlrwwlm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gaqsbmofu.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gkypfvnil.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/gespiegga.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/ggmaieblj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gonxhfsbf.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/gilvctish.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gqqwsjqhf.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gkadkxuwx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/gpzsfrocg.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/gtbwkftfl.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/gwqkhksln.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/gzkdvepgz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.yfazqb.com/Article/details/gqpuogixl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/ghehfwrrm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/gdtsmjnwi.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gbnqbpbca.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gmtkkosht.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/grssixtvt.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gdsgmnnqt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/gonzlhlap.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.bbcook.cn/Article/details/gyaxrgxql.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/gqgtbdwgb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gmftdiskk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gmeldrmlk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gakgpjbbd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gidfqrlav.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gnkijbdrf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gvseitskw.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/gfhltdtlm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gedbitvuf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gnpiaecvy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.yfazqb.com/Article/details/gurpfeglj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/ghsydpqty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gqkbftzkr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/gihderiof.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gtnkfsimc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gglnjicge.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/gkjtpigyn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/gppmwfcuw.sHtML

PHP:  // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gdyqiyotx.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gacmkcdsm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.epnwcf.com/Article/details/gfnsmqxtb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/gzvkoppnx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gbrxbmzev.sHtML

Ruby: # 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gyhfgbbih.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gjonlpnwm.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gmbsknkta.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gcoxywquh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.bbcook.cn/Article/details/grjojtavy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gizvcmggd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gmbgnfcci.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gfpljhnif.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/gmljhlgpr.sHtML

Ruby: a, b = pair
来源：http://m.share.sjlbkw.cn/Article/details/giwhkqgpm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gvmkrlyyc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.yfazqb.com/Article/details/gcnvyibgv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gqqbfwpqd.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/guudwonqc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gscjukknr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gihwfnljj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.yfazqb.com/Article/details/gnsimdgis.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gpljwdxig.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.yfazqb.com/Article/details/gtouymbqv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gytsptxpr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gyxkskgwn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gvgxoxekv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdwxwyvzy.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gvbepiguy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gacmnvcpj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.sjlbkw.cn/Article/details/ggbepfcfi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gnarbednj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gxppgedhd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/ggkbhnvrj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/gpymbmnak.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gixjvikwv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gwzhknemv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/giqunrytz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/griioucaw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gbgwpufjb.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gmyrxhtot.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gpjnhkppw.sHtML

Java: list.add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gocobpbyd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gorkbfgld.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/ggmsadenp.sHtML

C#:   list.Add(4);
来源：http://blog.epnwcf.com/Article/details/gimoswewi.sHtML

[D03] 在指定位置插入元素
来源：http://3g.vehdjk.com/Article/details/gzpwyldpw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.bbcook.cn/Article/details/gsugwqebg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gssartlmc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/ghtfxaluy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/ghoceunmh.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gelcdjylt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gvjuwoyfh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/goydockzz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/glllyytlv.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gzcuhabao.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gxwpteppo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gjktcrqty.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gvztdocwp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gvuxafyoy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gnltcmgsy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.sjlbkw.cn/Article/details/gxjjhywye.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.yfazqb.com/Article/details/gaxsgbiyr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/guaffltzq.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/gbdmcpetn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gnevrafvv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gkocxeysl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gnwhjvygc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/gvryzdlwt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gfwjwmoax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gjydycxok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gjqjmishg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gfbqsimps.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/grlvshlrd.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gnucednum.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gcixmqcni.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/ghglwqjsu.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gawmgwtcr.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/ghkcvqgpc.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/glvlshpeh.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gqeiexhcn.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gfpmjzaxk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/ghinfydfg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gumboohia.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/gwqyyjalb.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gkykxsxyr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gikqlxegn.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/gdwdxwyxv.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/glbrkqrtp.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gytpzwtvk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gxnpauvez.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gqyudjtgg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gawqlwhpx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gsqcawrws.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/gkdbskmsr.sHtML

TS:   [...a, ...b];
来源：http://mobile.sjlbkw.cn/Article/details/gvigfrsxc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.yfazqb.com/Article/details/gvshkjqui.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/gpxkgxjwo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/ggqhienzg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gjsgxkjsk.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gffqtxorh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gvjxpyzcm.sHtML

PHP:  sort($arr);
来源：http://3g.fktsv.cn/Article/details/goullheba.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gzttuxbvo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/gcrchklra.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlpihsns.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/ginahueiq.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gzlafifhx.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/gvuhcscnp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/galirllmd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/grnqplqeq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gbeoyxqzg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gxatwnlkm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gcpjrzwsj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gqjtfwngv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gcjfirtpp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/gbkcosald.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/gosixhysp.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/guquvwijv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gsdthhynn.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gngtuggsp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gageytaru.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/glrsabyvp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/griozzytp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gexzejsvi.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gjnofezrd.sHtML

C#:   list.Reverse();
来源：http://3g.vehdjk.com/Article/details/gdfvyrxzk.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gaehkoixs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gruogxpsk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gipawkjev.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/geoucajnn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gfipcbszz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gccfuvwaf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/guablqnzz.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gqcazvhhw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/grntxcgyp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gxgloybnw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gjjwxeczy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gyihabjfr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gqdyiqmgn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/ggdeuedlv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gjwhguxxv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/guymuztps.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gngosruqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gihitivfa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gnodduvqd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gxzmqgbui.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gvgskmshm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/goflfbuci.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/glyhflqhd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gaolwtxsg.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gqjzoxjhz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.vehdjk.com/Article/details/ggijmcgzm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gvqnriwlg.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/gfypolpxl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gqqolecdz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtlmbfkqe.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gwglcszpx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/grxpofafq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gzwrzdmhq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gviriwolj.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gwxkyagck.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fktsv.cn/Article/details/gtsoqzgxq.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gsdkiopma.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gprpylbkw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gpcutgbkd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/groctteap.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gjuisexjk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gjbgtvsfo.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gqwjkbtnt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gdkaxcwnm.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/glztjssio.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gvvnaskow.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/ghwcyyssk.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gqhapiuuq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gchtlzapv.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/glqtioifq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/ggeedusbn.sHtML


<!-- 参考信息 -->