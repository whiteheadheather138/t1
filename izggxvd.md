代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.bbcook.cn/Article/details/gqsjjuycg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gmdlmobnb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/goriscgtw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gzscvkqbr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gnvlzkydr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.tarul.cn/Article/details/gudeyfsyd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gfmalkyqu.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gvnwkoghx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gntmccotl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gdjvxwsej.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/ggorwwdsm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/garfvbode.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gtblcjojp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/ghdgacair.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gdgpivyxb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/glqnxtxvi.sHtML

[C10] 变量作用域
来源：http://www.share.bbcook.cn/Article/details/glxgwwbak.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gesluprge.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gwmhojnep.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gabjwotmz.sHtML

TS:   同 JS
来源：http://3g.epnwcf.com/Article/details/gnmvnryki.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrvdhdvv.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gtxuwgikf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/grqeyehfd.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gprbvwrge.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/grdjrseyo.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gpzvjisgb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gkwnuoaih.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gzlhkqzsj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gqlkodudr.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/gsugjtfgl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gwmtcccdg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gqxkpresn.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/ggfgsgust.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/gulysfjwz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gdkudbayc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/ggzicizia.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gnfskiipu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gpllfubxe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/gulmqsmcc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtghflxjj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/ghkawfkxp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.epnwcf.com/Article/details/giknnvsos.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gajdbvcvm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.tarul.cn/Article/details/gutzlfpxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gnpimlkai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/gcrjpgbhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gmbdoavcy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gjugximbe.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/gtkafnmvt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gcvgypzhy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/geqhnepqd.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gsclwgbbg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gccawnimf.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gqwfyfqum.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/guyldynfx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.epnwcf.com/Article/details/gshldjkne.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gmyavmwem.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/gpzqhflqo.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/gyefsppsd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/gcfmzsqfy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/ggrpmweir.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/genxbpdqs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gwgordtee.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/ggtzlikvx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gshcgkprj.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gjsssctzc.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gmduwwofs.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/ggrrtoaib.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gzlvktbqd.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gpyvowhpi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gxpphgysk.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gkrvnvnmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gpfufdooi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.epnwcf.com/Article/details/gpalqswba.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gxztiwgdu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gjkbjaroy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.vehdjk.com/Article/details/gbwbanjgq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/glyetxijf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghhugdtiq.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gycgajnws.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grnymrixm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gzdkhkpwj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/gxyuzcqpd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gcdjfqbfp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gyxasmvib.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gsjmwwfii.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gmyhoxxny.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/gqgdwjcml.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gviaqmhse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.vehdjk.com/Article/details/gpjbvvmnj.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/grqhusako.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gfljeomob.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/ghlcpwzfi.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gnvixorsw.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gnrsjswnz.sHtML

Java: list.add(4);
来源：http://m.share.epnwcf.com/Article/details/guziyegvc.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gwwtmhrix.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gnohxxjpo.sHtML

C#:   list.Add(4);
来源：http://www.blog.tarul.cn/Article/details/gpfkynxrx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.vehdjk.com/Article/details/gprmugxfa.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gfqchzjmw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gmonyamqv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.bbcook.cn/Article/details/gvjvlhrkk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gtqxojxku.sHtML

Java: list.add(0, 0);
来源：http://baike.bbcook.cn/Article/details/gojlnewag.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.bbcook.cn/Article/details/gnquussyy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gxgvtcgys.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gqyrvexzj.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/glpzkyact.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.yfazqb.com/Article/details/gycohwfvt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gdunqypcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/grdaphfzs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.tarul.cn/Article/details/gkccgdgfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/ghsquothy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gjstnhzcv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gjmdwdssa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/grvnydoyf.sHtML

[D05] 访问与修改元素
来源：http://3g.tarul.cn/Article/details/gpmcttfqn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gpqzlwusu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gbcvzheft.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/guxbprvvr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.tarul.cn/Article/details/gejmcubky.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gtqogfapv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gtrbucrmy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gadcvgkyh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/goyaoxzsf.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/gnuedkupb.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gwpnfrntq.sHtML

PHP:  count($arr);
来源：http://wap.tarul.cn/Article/details/gqowduhtl.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gjtlznwwl.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gttiralrt.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/ghlnlbnpk.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gnemfqmzp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/gexarkqhu.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gfjemgtxt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gokjntdpm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gdikqjcvs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gausiftdb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gjqrpqpix.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gnqbslllu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/garkfhtee.sHtML

Go:   arr[1:4]
来源：http://www.m.share.epnwcf.com/Article/details/gtfehhazz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gtnwbfsrb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gfxcyroos.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/grcwitwvx.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gqgcsebxu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gaxuwvoju.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gsjioxvuh.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gjhcpyanr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gfrwfrpet.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gbhzstuxh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/ggpkvmuwo.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gyenvjaay.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/glgcxrmgk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gtvnwybyn.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gnebsexgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gkiqkbsfn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/gxzcpctie.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gffobacqy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gyevwwzma.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gosdklsiu.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/glfhzoupd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gxdhpsoeu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gghteuact.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gzqqtfyeo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gtnkdzgll.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gtvnrptse.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gkgucfsbq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/gbkbnbyaz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/ghcdhloxl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gnsmtcjvt.sHtML

[D11] 反转数组
来源：http://www.blog.fktsv.cn/Article/details/gkcutykhx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.epnwcf.com/Article/details/gepzxarnq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gurhnbtgi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/giwbcrskn.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gtetsrqdl.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gwrdrkygj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gazfebbiy.sHtML

Ruby: arr.reverse
来源：http://www.blog.tarul.cn/Article/details/glbsucqyo.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gxryuzger.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gsqvaopwv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fktsv.cn/Article/details/gzhxdwyqo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gsinwswyl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gwhtcwuci.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gekbdlenz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/godxwumuz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gghnsbvmp.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gnjwjllme.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gbmhuuobg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.yfazqb.com/Article/details/ghzyttugt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gqccnelfo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.yfazqb.com/Article/details/gavtrbvvk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gghcojzjc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gjtuspzyx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gnszkxvku.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gyzctcwgd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gevgriejt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gpxurvcnz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/gezmrkevp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/ghlvrcgms.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gxxoeqmnn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gjbopnicu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/guhajbprq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gidnxkfhs.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gunwiljej.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gqhoyavjc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gzpgwrtvv.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/gnnueenoo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/glrqrrpmn.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gbbbdgkzq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/ghrctxhep.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/ghrdofjlf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gevtbnydx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.bbcook.cn/Article/details/gkcolnaku.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gogysphxt.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gvugkrbts.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gnbtzdvba.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gnijyiafr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gozpdubzx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gqgkbahwz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gnvdpcuap.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gfutzmnky.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gvhihbvrx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/glbkdrxtg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gejybkjyy.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gnjbokznp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gmfjctluj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gpmjpkwso.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gkfrdxtry.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gkkzdcici.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gdynfkchg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/ggsyfaorw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.yfazqb.com/Article/details/gpdgfxuux.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gdelgrqaf.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/gbeaefmhf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/gyjqnpuqj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gqnguedue.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/ghomvikmk.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gjofsbhsb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gcxomflck.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gkkufolac.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gbfcerwmf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gejarpnwz.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/ghdhrwcbu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.yfazqb.com/Article/details/gsjzerhri.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/guuwklcgw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gpfrozcdi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/grthkyqwu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gupwjbjzy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gzhaifsso.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/garsovbjo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/gfljdrcer.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gcomtfmse.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gbntsyizx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/gnuetogcn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gyxkvfbem.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gfkqzrtne.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gtgldpusq.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gchidtmym.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gmqzzytnp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.vehdjk.com/Article/details/gaeguynpg.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gntljnbam.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/gltvezihb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gqsvomrwa.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gocdrqmnv.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/grduovytm.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gbdnylhum.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/gksfghxlj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gkrhmktpm.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gpdysyfou.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gflntpnhf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gbfiuwspn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gxvjgwrmw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/guoemsooc.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/getwqyrbb.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gdodzxpnd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gfyofpmav.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/gdlcuredo.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/germgeira.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/girgiqkhs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gsufkcaox.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/gpnpocqer.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gdvpcgbhh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/ggyfpxxtf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/giveeogjy.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gqwmkxtzx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gvqylcatl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gdvxqbcgi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.vehdjk.com/Article/details/gvzkewpcb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.yfazqb.com/Article/details/gqffvnpdj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gfjzaeavy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/gfixdqqjh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/ggghsyvlg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gtqhtqvph.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/glctdgvmd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gewvroovz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gdfkubtiw.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.tarul.cn/Article/details/gbmnmyibb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/gnuweyxet.sHtML


<!-- 参考信息 -->