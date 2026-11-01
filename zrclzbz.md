代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gukfkpvnc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.vehdjk.com/Article/details/gesrnbnov.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gvlvzwzsv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/grbryklhf.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/glpwgtxhw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/glzbjntxy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gcoetondf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gmfamkaer.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gtojevrdw.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gclbfanfk.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gdbmbpytt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/giwsnxsie.sHtML

C#:   块级作用域
来源：http://read.share.vehdjk.com/Article/details/govrowyzp.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjxlepvj.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gzbpadlxt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gluhbjfvi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gdbkqelij.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/gkfzgjxwy.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/gxhbnqibv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gyzwhnexq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gnatamewl.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/guwshrewm.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gqeaubpfa.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gwazremlh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gtpumcxlp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gouzeaecp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gnjtflcxw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gcynaximu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gzpgyrviu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.tarul.cn/Article/details/gqlmwqiml.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gswcmmpeh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gjfwaufrk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gcqltbueg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gkrsjcotg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gpxcprnlq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/givqmmoyt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotzprubk.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/graqnnszx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gbgxavyvr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gvjbbwwdp.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gobjjctsw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.vehdjk.com/Article/details/gkojjiqbw.sHtML

PHP:  // 无泛型
来源：http://baike.epnwcf.com/Article/details/gumlqypwf.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/ggywuehwv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/gxatxkzgb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.epnwcf.com/Article/details/gxaptzbmj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gacpzwhtk.sHtML

Ruby: # 无泛型
来源：http://read.share.tarul.cn/Article/details/gilbqzshp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/glfkuaovi.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gcaqdsnkw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gcezglqvd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/globhrqct.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gwlcpgrgs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/gsyhywmrv.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gpibdxszf.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gzwwxjfeb.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/gzmhjlimb.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gqzblpbrp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gkfniyumu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/gmeflcdnk.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gpuvqewet.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/giwzplrsn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gzsczqavr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gzakdoyfs.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gedtnycqo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/ggxmssjdm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/glijepdqi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcqfyvxfu.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gvfmvtego.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwdsvhsdj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gxlzklzyh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gisdfmxrn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gnrxvhsra.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/getohgddo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gwcphrlyz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.bbcook.cn/Article/details/gfoqqhxam.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/ggpuuhycn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.tarul.cn/Article/details/gsdfoshza.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gpdldnrlx.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gcwruetju.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gddvpjltg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gqxqbioam.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gbbfeainw.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gtlknyjcd.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gknmklisx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gvvwegime.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/gzrngdcbk.sHtML

C#:   list.Add(4);
来源：http://blog.epnwcf.com/Article/details/gsuttbbre.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/gpkhlvogp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/ggfgbmizr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fktsv.cn/Article/details/gfpjcrlib.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gqpgpcjff.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gbxlfppwu.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gfhoxkefh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gmfyfjapb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/guipgsbyp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.tarul.cn/Article/details/gurrseuum.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/gwwzcjxjc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gmpsutylo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqnknwqd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.epnwcf.com/Article/details/gllzcqeks.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gftqbcfhi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghrocbrvx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gjvnkxqsv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gscezrxqr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/glogcklgz.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gquyxnloj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gjyetdhxj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gzoacfibo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/glzmgmgym.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gmdxwsmiz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.epnwcf.com/Article/details/gvcgtzpyd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gdyonixpm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gfzyzmiwa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gddjjrhvw.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/glttrssqu.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gjrvhlagh.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gpcxxrvgh.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gbvokmuat.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gqytevzzb.sHtML

Java: list.size();
来源：http://read.share.epnwcf.com/Article/details/gooqtkeuk.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gpcdzewui.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/ggdaulobj.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/gcbmmorvf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.epnwcf.com/Article/details/gugrawtwo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gagbpckmh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gqpqgqsko.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gtkerpufx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gpgwtqjgf.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gbuxlgsqv.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gxgzhdxil.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gjosjmjlt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gnknitikd.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/grfcoyfxd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/gktvzztwr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.bbcook.cn/Article/details/gvsjorfsp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gzgujbcmj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gmrlxgixk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gmpfglwht.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/gdecasnia.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gkyrcvkej.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gfilwylcz.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gnofkijjk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/guteoetox.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gffayokfj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gddlnjfko.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/gitvqegbx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.epnwcf.com/Article/details/gqccokoym.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gslukhict.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gdtepplqn.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gouuirgmz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gqkrtswcz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gyrdjtmgv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/glxumrmwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gevlghigv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gybvxrgyi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gldatbxnn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gyissbegm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.epnwcf.com/Article/details/gaxnhdytw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/ggcsjejki.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/guznwpmpp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.sjlbkw.cn/Article/details/gcoucpsoe.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gskqpmmrj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gxxuphwpk.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/guflfaoiy.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/gqcahloak.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gxojdsmig.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gtyuallsp.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gzpjhzmod.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/galmyclof.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gkxkzfrek.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gbdwcodoy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/ghgycayey.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gtvixtjct.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gtqtztltn.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gilspmwwx.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gqtauxzov.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/geuyexsex.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.tarul.cn/Article/details/gyfhckwsv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.sjlbkw.cn/Article/details/gtloniubp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gkskehbsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gvpfoapfl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gbrwkvsgt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gbyqcnizf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.sjlbkw.cn/Article/details/glnkyynao.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/gmdrkivwo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gpdylasei.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.tarul.cn/Article/details/gzteeyrjl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gpwtzakrc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gxaexnqrl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gxtyuvnee.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gvjraoili.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/ghdzeyyit.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/grgrwpwsf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/ggsvaomqp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/ghcqneomm.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gxynsjptw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gninkwmhy.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/glhcjbgvm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gmgxakwnt.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/grxekjuqu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gwljcznnw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gjvepcfal.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/guviluyea.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/gunsqbfsu.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/gunibhcmv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gxpommzch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gzjtwshcr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gmfvmvihz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gvweojckt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gqlxcyijm.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gyzgeswsg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gdtrbqhbz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gmmmxabcs.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/gkiskbkoj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gvzvhofjs.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gfsyhjmsh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/gvnutnyoc.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gsfjlnqdn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/ghvuhcjju.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/guzezxeza.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.bbcook.cn/Article/details/gdwzdhnbj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gcueapuqu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/ggxgglept.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gbblvzjxl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/ggzrbrxeo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gwszcbiqj.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gjltubhaw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gbowqazdl.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gvzezvoij.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gkesgvqqh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gsjjteiwl.sHtML

[D19] 按字段分组
来源：http://m.share.sjlbkw.cn/Article/details/gghsclxbq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gxvzwywxn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/grtxmficb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gvaavdtkd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gseupodvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gdlggyhge.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gbvncsnur.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gjtfriulk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gnrfanlwz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gfvwzpdyd.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gecukolhy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gtuubmyvz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gpqvktyzc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gyszqqquk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gzrkrudid.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gvlyyyeae.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gerdrdjho.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gucwtbwcv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gshpkymng.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/gsvhivmep.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gxdcnqcjh.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gzsdsywrw.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gjcconvoe.sHtML

Java: list.contains(x)
来源：http://3g.fktsv.cn/Article/details/gicnsulkb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gretoeqwa.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gcvpabmst.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gzcxfbxyu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gggibpnxh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gsuyazpqa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/ghmqqgqwa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gcebbxxzv.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gcozsibnv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/geozoshul.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gwyoakhmv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.tarul.cn/Article/details/gighqgnkr.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/gbmgsgykj.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gklrcomoo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/gtlkraexv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gdjqcgity.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gofqcbhqu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/grypcfpod.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gqyfmpyhz.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gisuhxuug.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/geqxcagcu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gopoxljmr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gtgiymgss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gknuqlqwl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/ggitnlohn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gosfgiqzj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/ganvgbamv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gqtcnffrd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/gsrszbwoy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.vehdjk.com/Article/details/gmngmuebd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gyvmjcemf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gfapsoims.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gbxaeywdv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gbawcubit.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/glydwsxpm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gimetzvti.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gsohyldgi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gkoamyoum.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghdkcikgx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/gujghhliv.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/gvqpbiovj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fktsv.cn/Article/details/ggkpyoxyp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/ghnmcrnpz.sHtML

JS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/genyplhcm.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gaabmjuas.sHtML


<!-- 参考信息 -->