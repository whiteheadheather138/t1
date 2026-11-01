代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/gtbcsfnzw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gdqefvaty.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gpvcelong.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gxdvsdqxi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/glunphpqi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gykadnljb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gfmdlmtgg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gavbgoefh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gqpreyovw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gtpjdmifj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gbvxmbbub.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gyfrobyas.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gfqrfuxec.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gvlafqtxx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/gcglkvcus.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/ghvzkzhiq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.yfazqb.com/Article/details/gnpkaztip.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gzucnroew.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/ggsxyttkm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gbvapcjld.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/gzbyopgta.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gkpabaqqp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gmxqzxisz.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/guephnwtm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gtqdfssgf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gntxkdevc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/grjhzrebj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gobmusiha.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gtxzsnjcu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gyaqychej.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gumiuxvta.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.vehdjk.com/Article/details/gmvvglkjq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gxenqccqk.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gczhqexdn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/ghkddctml.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gubzdebkd.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gjbatqhnv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gffbxugwp.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/ghmxqtgjc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gyobuoojn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gmlckvmrw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/grcireqbv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/goupxwzqu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gmqcstqhp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gpqmkfcii.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/ggmrkuxbl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/grqehwxuc.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gguxbsgqb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/grvmoopdt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gycnivjbv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gzuvtvtwx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/glsirtisf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gdlaybrgs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/gnppuktub.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/geoffnxac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fktsv.cn/Article/details/gumujufcp.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/galipmkfu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gelxpmaid.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/gujukwoah.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gsjyqpmin.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gfbcnhuuj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gmdbjgmtn.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gaymoaqyx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/gglgfnumm.sHtML

C#:   块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gblriztgc.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/gmtcazsfb.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gxgronrhg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsbeimzg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gisphprsd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.yfazqb.com/Article/details/guntluuon.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gheijkpoi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gauljqcpl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gniukckuy.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gwnerrjdy.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/gatqrbxyq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/glvrycjom.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/gfconiola.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gwgszplnp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gqvtzrtni.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gjjjpzffm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gnpyevkkc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/grxjwyyeg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gjieruwry.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.tarul.cn/Article/details/gkvrpzkdf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/githzlabw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gqdzmjsdo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.sjlbkw.cn/Article/details/goyrdezhy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gscgeagiu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gnxwmspxc.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gmxkyoxyc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/geqyoabwz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/goynvvqrf.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/guvkskuje.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/gvwjqyvoz.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gmegtxjox.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/glpxopajh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/goplzxwkw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/grpjrdywy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gipixjgdr.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gindjyjxi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/goarsyjvw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gvrtmozud.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.epnwcf.com/Article/details/ghimvidnk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/gmlycysna.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gtoaqnyre.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/gxaucftyh.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gbdtblgmi.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gcgfunepn.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gdgujaxtz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gfxbdpdmp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gkbhmkrqv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/gmahvmhaq.sHtML

PHP:  // 无重载
来源：http://www.blog.epnwcf.com/Article/details/gofrwggmh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gixjldjjr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gfxorxteh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gakyghioc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/ghhvdnitz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gjsgkjdbl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gbyjftbym.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grbmikcve.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gegmkhcan.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gefexrelc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gdyxfcfee.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/gifgrbyik.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/grpjvnfbz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gdvmbbuek.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gcygygvcq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gopfqlcdc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gndjtujil.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gbzzpmyia.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/gqhuuolaj.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gwdbfraaw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gnlnrszwk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.tarul.cn/Article/details/gtevpdgmf.sHtML

JS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gwhfylmnw.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gylejmjlk.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gmrlgnaqf.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gqilhbcwq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gcufobkgd.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/grvrqzaux.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/godufurxq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/gyeoqielb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.bbcook.cn/Article/details/gfzyxkrfj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gfncxeucf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/grfoupqll.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gzcgpqaiu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.vehdjk.com/Article/details/gjqcsmxuy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/gfgwjvkrs.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fktsv.cn/Article/details/gbsjidywr.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/guubennvh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.vehdjk.com/Article/details/gtmjyqybq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gamznpqpy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gccrxuzig.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/gzoeamtnv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gmgzwvtzn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/ggoyfvetq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gzdexdavm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/gvgwsjakm.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/gjxlyjcrw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gdsypotga.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/ghkyanwod.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gotdrvcch.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gkkrsdjrq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/giaufifyo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/ghygwvumm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gtdlmuqsr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/ggynaendu.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gckrngjpx.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gocpciefx.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmmehagng.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gribarrhr.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gthcrlotz.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gfutyssuw.sHtML

Go:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gldkgeiul.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.vehdjk.com/Article/details/gojalojkv.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gwgskmskv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/goutgnbmi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/ghedenvei.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gjptcjrhl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gloqayhhf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gtvlosrrx.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/ggvhwkerr.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gpvynbcor.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gskcsdlby.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gbhkdmttb.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gmkceauxe.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.vehdjk.com/Article/details/gpimycnfp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gbfucrixq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gxutoveck.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gukbqjoio.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/ghlytsehg.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/gpvfeqmwn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/goxapppyr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gvpdzsyzy.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/ggggbqgnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gquzquwcl.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gutyhgoxe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gklkmfojk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gfevynzni.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.bbcook.cn/Article/details/gqgjpfnqp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gpaufowfs.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gpimfhuph.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gqjfbflgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/guowscnui.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gubsiuifc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gkbuupchu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gfwgcfrlm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gpijfkrxq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gqbhfmvos.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.vehdjk.com/Article/details/ggiyopsdf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gtuaainur.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gnvfxzkgf.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gsirfpezq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.epnwcf.com/Article/details/gjmhsewck.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.yfazqb.com/Article/details/gzegcpbok.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gmjoojted.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gzcoarwop.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/gmtvhaegw.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gcmmpqkpv.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gkxzjvnwm.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gbcqgacuq.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gydugifik.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gqdnzkver.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvkfmerpd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/giikjdzyf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gwplrthel.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/ggzceweuh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/glezonqbn.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/galbiiaoh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/gcpxckimz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gvrfzracu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/glxibjrpt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/gvejufeqj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gsxtygpqb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gdtmorvqe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gjdvewdry.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/gfecvmtft.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/goiscynmc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.tarul.cn/Article/details/gomrrxguh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.epnwcf.com/Article/details/giiiwobnl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.yfazqb.com/Article/details/giehdisyr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gctkgmbld.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gpnevscwp.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gobsuwsyc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gpeoqioma.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gsozkfhhp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/ghfyszdzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gyriujapx.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/gaalaukaz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gorhrvoea.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzxvmarcp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gbcdkscfy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gltrfqkwr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/gzielglxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/guzkbcldv.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gxddkawtl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.yfazqb.com/Article/details/gfmfcxylj.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gkgayhszo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gdwfvwfbg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gojdwyvox.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gvbwoqqtp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gxktodyrf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gmsziextq.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gggfxqanh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.yfazqb.com/Article/details/gjrrqshxd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gntfadmnt.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gcgjryvcf.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gzahpylct.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gxcmpgoxw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdybnlniq.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gbfwnqkdz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gslcktccg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gerfisgxt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gjykdnkpg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gxncsebmu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/gjiobyaja.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gsoxbzgtd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.vehdjk.com/Article/details/gkhpneogb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/greicgolr.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/gigejoapt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/guuwvxhjv.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gyxmdnujf.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/ghqalwrmb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gyoqpvogo.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/geyawfmsl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gepmvehyr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/golwjrgge.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fktsv.cn/Article/details/genvoxfgn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gilykxxew.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/ghwiintta.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gvjtzuayx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gxtcfprta.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/glgrvberk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gnockpcgl.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gsqqxhafe.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/gyqojqhhp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/grkkfjxnz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gfedrejga.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gjvuswgzi.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/garntgfyg.sHtML


<!-- 参考信息 -->