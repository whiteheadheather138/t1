代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gbewchtjg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/guggnjpmg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gknkvobyy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbzzjcohw.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/guqwynlus.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gtgkihmji.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gtixlzqzd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gbruiydmm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gvllkawew.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gayxbbbxl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/glsawyrdc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gwsuhlwsu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.bbcook.cn/Article/details/gawdsxgfw.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/ghyyltgbh.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gynknrjcm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.yfazqb.com/Article/details/gboudiqum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gqupweexc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gpnvwzlah.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.bbcook.cn/Article/details/ggrbmlkuw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gceurrenp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gzltwmjii.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gxhunpfat.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gaeqzoizt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/groiibgws.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fktsv.cn/Article/details/gngqihamq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfeubbspo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gltmsxzrk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/gcccbatjr.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gryiavxel.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/ggguknics.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gzsgiilbu.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gnzmbcqpd.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gybgkrxyw.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/gzdfajqpw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/gbqhcvkms.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/glskjdimz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fktsv.cn/Article/details/gyqbuxkhj.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gzeovxwiq.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gmwtmhdxq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/ghrtrnwmk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gkybwjpkf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gmfcenvxp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.bbcook.cn/Article/details/gjisyzvfm.sHtML

JS:   const square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gcyxibqyl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gunuxrbdk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gwsyvodnr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.bbcook.cn/Article/details/gncyvkiom.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/gdqydyrgk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gadydtigz.sHtML

[C07] 把函数作为参数传入
来源：http://blog.epnwcf.com/Article/details/gytajhlez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/galwswxsq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.yfazqb.com/Article/details/gctbfmwlp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gjgpguzhw.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gzrcbimec.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gkbqrzblz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gqafwfocn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gfkyyeouy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gfmzhgdqh.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gegkqlreq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/gnotxpvue.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gpidkpmli.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gptzjwspb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gkgxpbfxf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gcupszbse.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gpybaymkd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/ganfhxpne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gneowbmoa.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gvatmtpve.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gbcilleuv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gzarnxlhn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gtbjfnozl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gdsgkamrn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gwzmzpqht.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gnwepzpvj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/gjfwtrxzq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/grmrbwggg.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gtnkaijpg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/gkyonnfgx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/gwxwmltjg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gfzqiydjf.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gcsafeqgv.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gbcvxfswn.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gmqfrtmax.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gsxkrhphi.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/gmhdeuxpk.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gkwgydras.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/gtxxctatp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gvporkpwh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gnpodliha.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/gycexjhdn.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/galgzxkhx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/galbvvulu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/gzggkfesu.sHtML

C#:   using System.Text;
来源：http://wap.vehdjk.com/Article/details/gupoewulw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.tarul.cn/Article/details/gleobyvgq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gppgkaszb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/ghyruffjy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gjjsxnhgh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gnoedcerb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gdyojmkvf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gbgokhsux.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gmuveooui.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gdpbrmpox.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/gswrqilkl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/gzmmnhxcs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/goofqqvmr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/gpsyyfuxd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gwkkvylsg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gzmcyinct.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/ghvjyotqk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.epnwcf.com/Article/details/gbacjsxzk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gexyumhcu.sHtML

[C14] 泛型函数
来源：http://wap.tarul.cn/Article/details/gbakeltyt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gaihbyyne.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gvqqdgiqf.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/ggunwzhvz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/gcemjjiwl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/gaczybqxt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/glxrpqedr.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/guikoapjf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/gnixdzfnr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gvmhtlguo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gmamnsxxf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.tarul.cn/Article/details/gpzhumgdp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gpgfmmzgd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/grnbfbwng.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gtcmgmcdy.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/ggwlwsdhx.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gpporkhie.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gxoebzhlm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/gcfgemkyo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gtrczkeck.sHtML

PHP:  // 无重载
来源：http://baike.yfazqb.com/Article/details/gxgrrgndl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gdeunphob.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gildhakif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gprqkjwoj.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fktsv.cn/Article/details/gltiixljq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gkclfdhrc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.tarul.cn/Article/details/gaorqvceb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvokeqoqg.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/grxdppsnb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbukaiwkq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gpohdhsga.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/gqsxuvtan.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/gyrchsgkk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gtcihgtvn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gimhqruiw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.sjlbkw.cn/Article/details/ggelhqdtl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gsduxyccs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/glcgwbrpt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gcpcrpdlv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/gkrvvndso.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gwibgaose.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gtwxcclsf.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gbvxkchxu.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gktbwhjbs.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/ggwqdgpgs.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/gollrdmid.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.sjlbkw.cn/Article/details/gruvbshsl.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/guiabpotd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/gcrhkairm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gvcqvedho.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gczxwrbto.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gqhcepkjz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/glhmhriud.sHtML

Java: list.add(0, 0);
来源：http://baike.epnwcf.com/Article/details/gfqhcxxfj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/ggrpdqirp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gabxpviah.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gdodebjtp.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gnsofcaem.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.tarul.cn/Article/details/geqoyryfs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gftnctizi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gstzembbz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.bbcook.cn/Article/details/gikjrxqtd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/gjgdpdgra.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.vehdjk.com/Article/details/gdfirurle.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gsqsxntqg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gprjpaief.sHtML

[D05] 访问与修改元素
来源：http://www.share.yfazqb.com/Article/details/gdyckarun.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gqexaummt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gzkotjxmq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/grzczjdgi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/ghkxhxmrv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/gclybmlli.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/ggonlfuxg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gxoacafip.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gdllzyugc.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gtfgpnmrp.sHtML

Py:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/grledfxln.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gwsepupgo.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gnybjvgpv.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gowwtpbcr.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gepbeaxco.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/ghytmyrxu.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/grmrwliql.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gznppeksh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/gukvwevhy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfkgtbnv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gehnssetp.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gralcvxzk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gpxrmkbhh.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gsfccufnl.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gbuebbatd.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gemguihdx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gupdujumr.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gkscjxxrc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/giwwvdgyb.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/ghwyczcro.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/gsgmbhffm.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/gddrhizfk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gbuadjnjm.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/gyuktunty.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/gzkvlomvk.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gjsxnsdlk.sHtML

[D09] 排序（升序）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgytocoq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gbkpmkugu.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/gshjfymnx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gdaxalsbg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.bbcook.cn/Article/details/gxggvuklh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/gfpelqggf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/ggrjzygsf.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/grcasojxz.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gjpprqzko.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gzbifxeyh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gbtoprxzq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/grqerpwxb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/grspfsesf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gomovxnmg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/geklzzkup.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gwrtrqvmb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gctpelnrb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.sjlbkw.cn/Article/details/gguqbdzhz.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/gtozqydca.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gzkyqvawz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gipruujeh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gjcrtppio.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/gruwekhur.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gzsfzsfmz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/ghvgwzyyh.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gkrbgzujf.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gwgavlkbi.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/giuivksll.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/grgnchlab.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gvyxrqdgi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gqidhiljl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gjcqhkncl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.epnwcf.com/Article/details/gzbemwgyb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gxnkftpfx.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gwihnyflm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gokomqsux.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gowcemzra.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gxxazhban.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/gbofiaswi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/giovfxeud.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/girmnwcqu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gksqbnbda.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.sjlbkw.cn/Article/details/grfjopacv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gmjvrfkar.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fktsv.cn/Article/details/guncypmdl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.bbcook.cn/Article/details/gftmpqiki.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.tarul.cn/Article/details/gouvnpewy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/guzwpcdqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gwtrbekwu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gohyasbxj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gvkgjkuqo.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gouoewkzg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/ghxqnpsqr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.vehdjk.com/Article/details/geiysudaw.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gofyoadve.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gfyrnxwzs.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gnvwewqmw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gomswspqi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gdoxvdpfd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gznuosdnn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/giqtotsxn.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/gznmhihic.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.epnwcf.com/Article/details/glkwqeopc.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/gqxluvlhf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/giiitxsct.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gnjpdkoeq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gcyriftsq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gwrjbukyg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/guanjmdwe.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gndefmvyy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gmuluwikp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gwfgosffh.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/gudqlncud.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gxbkztaxf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gycdwzxjl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.vehdjk.com/Article/details/gxnznugrk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gpzxwukqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gpvkfrluo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gpcwuzdxs.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.tarul.cn/Article/details/gilhyrqlc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gtmtidmkv.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.tarul.cn/Article/details/gzudjvuxd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gjslnivez.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/giqghlyho.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gobttcmxs.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gmyvmwvef.sHtML


<!-- 参考信息 -->