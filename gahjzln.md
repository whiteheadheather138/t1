代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gqltixwez.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gaxybhnha.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gjyqeislf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fktsv.cn/Article/details/guesauyrn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gzgypxzfn.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gwphspvsm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gahdvsqrc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/ggujpbhpl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gmviyjgfb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gmcxjvyij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gglxqtthu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/gpfrgfsls.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fktsv.cn/Article/details/guoipfned.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/guvxonodg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/grykwgttw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gidtkxefb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gevbiqueh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gpqprorrz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/gxntlapjn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gnttkfijk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gqjhrjwxh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqpbxlkj.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gtgrevgad.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gnctncocm.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gfkaxjnyw.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gtkpyqgiz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/ggiexpzec.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gdmjqkzcc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gwsymeywy.sHtML

Go:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gptaiacvu.sHtML

Ruby: return a, b
来源：http://read.share.bbcook.cn/Article/details/gqujpklxr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gtuzcqydt.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.epnwcf.com/Article/details/gylllocux.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/gqaymgzcl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gmgtmomov.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gtfkfbqme.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gfckbpmqb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gczvakvjw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gpwstayuw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gosgonfvs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gkfqdduoa.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gpchogjfu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gffztutss.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gtgrihzdm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gimsnffbv.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gwzpoyuqd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gpyhajfoc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gmjmvwuhv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gqyeofqeg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/grrmnjhah.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/gvbneqpwy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/glxlxdeyd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gqoerqnym.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/grztrpuxt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gquvwqicx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gioycsrpg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gxcbeykfa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.vehdjk.com/Article/details/gdtphfiaa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gxtxqwaqh.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/geeodgvbh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/ginhlmkts.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gqybqtpik.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gcmztyfap.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/glhkvdrkp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gbqfxmjbq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.vehdjk.com/Article/details/gdujrsycs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gmjfjygwm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/gwwroqubr.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gtgqjiqxw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gotcphroh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.vehdjk.com/Article/details/gaklgobkv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/grnrdbmvp.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/grrhpkgpg.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gjdaiwzse.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/grteukcxw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/ggicgfusj.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gcbadrhld.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gvwdrqaaj.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gacqwpure.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gbuuidlvi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gsvcbekvf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gyenuksvk.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gdfrrigdm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gksavxcky.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gbmuzfpze.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/gbzedxqwb.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/glciolgph.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gnrksahwz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gjuwobsef.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/grefgwpxj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gpdhyyyuk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.tarul.cn/Article/details/gpdhopecx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gpcfzkxvw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gtrcyibzr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/gmleufgfe.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gqxemflxo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gzocltssa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ginxqyuxl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/goloclrnn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gohxgqgqe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gmpquaxpt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.yfazqb.com/Article/details/gkpkgqxrt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gxarphovd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.tarul.cn/Article/details/gpowncenm.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/greiznohu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsegnxoq.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gfntzhsbf.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gytjofvhi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/gdwlsucqv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gxgambvmy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gsypofwfm.sHtML

Ruby: # 无泛型
来源：http://wap.tarul.cn/Article/details/gmavsrxwz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gupryppjd.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/ghejubqry.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gxqedzfkj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gryphtstx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gqialctai.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gnylhazhv.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/giprnlovs.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/ggxltqfyu.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gjzxyjuly.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gbflgzuxf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/greelwgkm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/gzagpjqtx.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gahntapyz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gmxmiukwx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/gwvvsvohe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gyphxssrf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/ggujeefob.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/gydgrlfge.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.tarul.cn/Article/details/gooxmolby.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gytzeqkvv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gzpdbfgcw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grozhbhza.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gdybsyvcs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gaftaynca.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/gwnzjavcj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/ghxehksrf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gxzbwkarx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/galgrzxxp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gpshuynur.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/gdehmpxqo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/gkvhtthsf.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gjuznhefl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gnlabhvqa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/ggdzcmomr.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gbwgrbdpz.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/ghcenvutf.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gxoesewgx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gplvmurvn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gcyjxpkta.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/gkydmmrux.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gvbxeiehn.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gfxkcsclq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gmsfnhedf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gfngilyav.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gqswfbtdc.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gchopwavi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/ghyerkmac.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gizqbdnej.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gjfjdjvvr.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gizoudsuq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/ghwbcogbr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.sjlbkw.cn/Article/details/gdlsidewe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/gknnlorxn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gzzmjlhtx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gszhdmtlr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.bbcook.cn/Article/details/gwbpeylca.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/gtlliimbp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/guwnujuek.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/glwufguse.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gdjcrgmai.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/glavppuwa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gxnnzqqpg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gsrcgopxt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gwqqazvzf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gqdnxdzdw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/goyhsazgo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gpqvfhkmn.sHtML

[D06] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gyabymepf.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gwfabyyth.sHtML

PHP:  count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gyrvgzdzp.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gjyvdpbmh.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/ggjqisdst.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gzukjfxyo.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gsjwilwji.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gsaiaatvg.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/guhxhmyuk.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fktsv.cn/Article/details/guigruvom.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.epnwcf.com/Article/details/gimqticbs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/gvadlftdy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwttlhfqc.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gsawoltpt.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gxbxrkgjw.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gchcsvkwk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gpmwixjvv.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gkzjppbmz.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gtzqiygcv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.bbcook.cn/Article/details/gdiccmhfr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gkkcgvtfh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/gwmlinsnh.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/gmcufcvpx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/geqbmvdmi.sHtML

Go:   append(a, b...)
来源：http://www.blog.yfazqb.com/Article/details/gspwzuomm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.yfazqb.com/Article/details/gmupqhpfv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/gxlhrkuok.sHtML

[D09] 排序（升序）
来源：http://mobile.tarul.cn/Article/details/ggieitrli.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gxhvtloaz.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gphxflgkw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gxhmqaigj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/ggemqvech.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/gugolcpfm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gstkjmkbr.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/grnerkkrk.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gfkmfufxk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/gzfncvdjq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/gflkiqixp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gqlydwncy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gwelhnjua.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gbqkzztei.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gpqzzmojw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gfwslqlsm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/gikpnwmod.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/gumfzxzyq.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gmybamuhf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gzoqbmkji.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvtqpbomt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gcgtwjsiv.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gmuogyhxl.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gomanstjb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/geizygovz.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gimxrmogt.sHtML

C#:   list.Reverse();
来源：http://www.blog.fktsv.cn/Article/details/gqopoboxw.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gijhzqnld.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gfxakxnvl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/goripqooc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gwokaivyf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gsnehyxze.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/gdbyqjblk.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/ghgfzbdkf.sHtML

Ruby: arr.index(x)
来源：http://mobile.fktsv.cn/Article/details/gskhikxqg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/gxruymwdl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gtwosqtdp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gmcxldqev.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/gfcbkxqrw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gfnpsyrpx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gaivvlgdr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.yfazqb.com/Article/details/ghcaoaoay.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.tarul.cn/Article/details/gakhljsao.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/gwwztonic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gairerryv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.vehdjk.com/Article/details/glraqtdnu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/geajdxieu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gxiaslrgu.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gvdwspvfo.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/ginkdnwdz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/grgyraxwz.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gyjkfmybi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gikdgnqgj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gsukffejb.sHtML

[D15] 去重
来源：http://blog.epnwcf.com/Article/details/gfrqjrusf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gpnnamlyw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gzzjwmukr.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gojifoshm.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gvmqsrivq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.vehdjk.com/Article/details/gguzvcnhg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.yfazqb.com/Article/details/gbxibltdm.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/glfqzjmmm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/grjknjsbv.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/gcjhflbvf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gmfwqavyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gvefbhhwh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gqcnsxrum.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gtxymjrtw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/gboqtjqkp.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gmqajlnpq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/garjwvjvi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gpgorbhee.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gydlzfaif.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/ghdrmermi.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/gyxwoclsm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gwwdxosag.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gelgvrabt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/ghuhhhmaj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gjfyuafbq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gadqobooh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gkcabydnb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gojwaqjlf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gvjenlvzl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gfbvhexgq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gccifmraa.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/gsagjelkx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gqsjkdzyx.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gnytconsx.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gygytwzmg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gshsqgmah.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gxgqrpxxr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gjuiwodiw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gescznvis.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/gxvqpbvhs.sHtML


<!-- 参考信息 -->