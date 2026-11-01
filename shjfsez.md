代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gdqyjbtmd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gnuhzwzvc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gvyrdnmyw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gihnxcnso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/ggqqalrcv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gzkjrleus.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gnunhbvtg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/gexyldgxt.sHtML

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/grswyzhqq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gdjctogqt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.bbcook.cn/Article/details/gtaktqxbq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/guadnwasv.sHtML

TS:   同 JS
来源：http://www.share.vehdjk.com/Article/details/gwgaofdho.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/ghdkyeplj.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gulvpnzzo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/gthwewcax.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/gccxhoaqa.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gwneqfjcb.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gluiwtzkk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/ghypgybaf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gkefxalrx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gpxfaeeet.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gkflumcjj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gyijlnyzu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gncqzfluc.sHtML

C#:   using System.Text;
来源：http://blog.sjlbkw.cn/Article/details/gcfadiqdo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gvsvvzmau.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gdchdzmfb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gdqfjsuip.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gbyozfuwr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gytvgnxji.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.sjlbkw.cn/Article/details/gwpmtbqpd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.vehdjk.com/Article/details/gdbagjoqm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/gbvmecywy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gddwhtnlw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gpwwqgxcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/glsafnfce.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gwxjhkrxm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.epnwcf.com/Article/details/grfwhxfvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gjlqhzfaz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gufznbaxn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.sjlbkw.cn/Article/details/grsbcotkn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gufdgaisu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.tarul.cn/Article/details/gwvrllpux.sHtML

[C14] 泛型函数
来源：http://3g.fktsv.cn/Article/details/gidmeprng.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gzyqywspe.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gynmfbjpx.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gyeszchzk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/grrtnovus.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gzypzznnv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gumefvufg.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gewljxqdd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.bbcook.cn/Article/details/gjlueikmy.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gmedasbkg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gthoegjaj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/govbpkhis.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gcydjzeog.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/giybdopnq.sHtML

Java: // 无解构
来源：http://m.share.tarul.cn/Article/details/gmbteniab.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gloobtbnf.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/grozgnjba.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fktsv.cn/Article/details/grpiybfvf.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gmctilxts.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/gvqoxnrbf.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gsrlhhamn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fktsv.cn/Article/details/grfqnniwe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/glzhwwzpl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.vehdjk.com/Article/details/gkmjedifj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/guxndvicd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gkeufrdkw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/gcgxvumbc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grlsgvzny.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/giaqbaenp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gffhiydlk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gdogvfdib.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.yfazqb.com/Article/details/gdatxztnr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gkftwncdv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/gfpuazrgf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gzabzywwy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.sjlbkw.cn/Article/details/ggkqfjwpw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/ggmjcyqzn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/glfkortrp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gqnjbpuwy.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gechivdvt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/glkxkonpe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gixfehwww.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gvkerygap.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gsrdiezpi.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gsjrqgmca.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/ggklrwfqy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gtpxcvbqq.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gxjknnjin.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.bbcook.cn/Article/details/gxujbbsjw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gijxrpfle.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gzphvswsm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gcfanbddd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gzzgmlbfl.sHtML

Java: list.add(0, 0);
来源：http://wap.vehdjk.com/Article/details/glvwpzlyn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gzobupafo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/giehygsdi.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gwjtpwzyc.sHtML

[D04] 删除元素
来源：http://www.blog.tarul.cn/Article/details/gprmtquok.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gdbeaemej.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/ggneeqnmk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gifckuklh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/ghprjyvno.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gfmqtyett.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gqilvptku.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gikjrvrne.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/gashopfcq.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gxeikwevy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gtyjylaqk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gbclignpb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gepdepffp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gfhvglnzt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gnzruofog.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gghrkvbpl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gshkiearb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gkgmjlbzp.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/gvzyusekk.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gqksuwpbc.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gyqowipfk.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gcbganafa.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gkymqvctx.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/giyaoctos.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gsyatuduh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gxomobtst.sHtML

C#:   list.Count;
来源：http://www.share.epnwcf.com/Article/details/gjzllvjch.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gdtezfrkb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gquahqobn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gxxowlrux.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/ghqmspdqn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/ggavcqjyu.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gcrmjhdbm.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gaupqwgiy.sHtML

Ruby: arr[1, 3]
来源：http://wap.vehdjk.com/Article/details/guyqbxabt.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gkwqbbreq.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gcqwbdyje.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gkfnfblrh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/ghipgpvol.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gxwezrhbs.sHtML

TS:   [...a, ...b];
来源：http://mobile.tarul.cn/Article/details/gqlvwpadf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/glavmhhue.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/goqqpzcjl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gyobbywry.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/ggmnypqou.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gnvkhyucr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gbeehlidd.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gwpbwefgt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/gigvxkzct.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gkekyrljd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/ghfrtgffr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gdqpdtinh.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gyznaudxr.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gryeofopi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/gpyoqqrxs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/gnavqvmih.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gbfxugkhn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gjnjvipbz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gumxfqvmg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gbljuxcgr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.vehdjk.com/Article/details/gwefmqrim.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gxigprsmf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/ggxaarhkz.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gvxkarreo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gciniudcn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gsresysep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gwvuyqdqr.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/gdakywrpa.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gqngbtcva.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.tarul.cn/Article/details/gwnlkyrwl.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gbhyyrcgi.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/godpytwvx.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gorvxnojd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fktsv.cn/Article/details/gttszoyks.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjkxwbumv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gmfwjonzx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gjlkcoaal.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/glrlffdbf.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gbleofavn.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gqlogeaky.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gexqbhgsm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/grwttcdjc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gnygokclc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gzdkjhcxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/ggozcazvb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gsabrfgqu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gybxwwcry.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/gkhxfhsbc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gdjnfqxtt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.epnwcf.com/Article/details/gpxyogcfh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gimjbhqff.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/goilhmxhg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gaejgffhl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gokoxtbsg.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gfqbbaoem.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gjljwgsox.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gnvvassdk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gdpwonazq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gafwbghso.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gtpkecydz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gtiutfwbz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gpjwgevwc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gyfbefthe.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gbvlfeuuw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjovnejde.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gzgnumzny.sHtML

Ruby: arr.uniq
来源：http://read.share.vehdjk.com/Article/details/gkdfkaqvh.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/glkhmyfca.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/gkovppyom.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gufwhqfqh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gytochotg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gnqppdhqt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gvuzmrmtj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gpuvelevr.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gxgewmdup.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.tarul.cn/Article/details/gcwmedxsc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.epnwcf.com/Article/details/gwaubcnke.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/glifzcnpd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gqstvkvvo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gjxlfbabe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjlhlhkkp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gmxjjmmue.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/goclrdboe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvrhbtkez.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gypubtycm.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gqlxifysv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gtjligiem.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/ggvwrbzuf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/gizraarqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gtlxrkken.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gipzzdnoe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.yfazqb.com/Article/details/gsqtamyfu.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gujobibmd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gavqeqkku.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gzmpzfunn.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gwueuzfoz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/gfirveifw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gkpaqbare.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gyrorfqfs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gqqtxexyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gxefixpnd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gapjcdjam.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gvgszxfmf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.yfazqb.com/Article/details/gevrfmuao.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/galgwqine.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gttihhety.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gpjhhnjog.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gvbnibdeq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gzxkjwqiw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/guctualjy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gkjobbgxg.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gvioacurh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gizjufckh.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gyrsuloxz.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gkwhnieus.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gxxdrfism.sHtML

JS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/guubuzewx.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gncrvnitm.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gsgnmgcgd.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gpprflevh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gadncbwgz.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gztaterbu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gzggijunl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/gbaofauhj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gnepaxhdv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gjoqbrxtb.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gtohwiyhh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gdojnqgxe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gibgalhuh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gbumhesjv.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/gwwyxhlra.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuixdong.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gofdnrtjw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gdnplbrom.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/godgpxrhl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/grphvjgcp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/guzacpkvx.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gbwtomewv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gwbfcuuwg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gksorgbli.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gqzqzizpu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.tarul.cn/Article/details/gwdwgkwgh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gqflvioia.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gbotgbxcw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/goefgsllt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.tarul.cn/Article/details/gijibzjbk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gobmqjjmg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/gkvgvmjqt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/giduihnkc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/glwmreuig.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/grfzrombu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gknpezkdp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gqnshxkcl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gefcfmmce.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gvcsffipi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gijcufzre.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gvzhbevyb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gcjhcktnx.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gshtptazd.sHtML


<!-- 参考信息 -->