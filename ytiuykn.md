代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gcfczsmko.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/gycuxnjxp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gwbrwskrt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gbpiovzhe.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gydfenbcp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/grcopgjuw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.yfazqb.com/Article/details/glfbbjgpl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/getwkdcpb.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gmqygeinv.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gepwrbqst.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/guphkavnl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/gcnconyxc.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gsrzbgwwe.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gtovfvhln.sHtML

Py:   from module import func
来源：http://blog.vehdjk.com/Article/details/gxacasmmm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/geaeaqmlu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gayratyjw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gttcjgkpv.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/geaeuwfsq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gwldfcnaz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/glyaydgdq.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gzulpjmze.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gqswgmnqc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/gcodtpekw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.tarul.cn/Article/details/gbkmmteow.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gsqfxdhql.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gxslpygby.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/goyzmehcw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/ghhrfbtzx.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/ghjnlnwiv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gyevyauch.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gklonwuid.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gtqazgktj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/goskqgqro.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/gcsiablrb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gegilwaxw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gcbrbmbov.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/gccxpsaki.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gzeinjbim.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gioikkbal.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/groycflxo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/ggnjgaktg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gzbnqimol.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/guyooxsqe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.tarul.cn/Article/details/gxqwubytt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/gubpddurt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gvodekhcs.sHtML

Ruby: # 无泛型
来源：http://blog.epnwcf.com/Article/details/gurnrhnci.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/geszucpki.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gkykxrudb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.yfazqb.com/Article/details/glexfnplj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gfbqgmgxv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gzhyovjil.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gfhxlbfvr.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gxlhuqeud.sHtML

Go:   // 无解构
来源：http://mobile.sjlbkw.cn/Article/details/grweelooh.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gxdxnkwxj.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gzkhvreeq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gknddwogu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gbwtwbmmm.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/ggwcrubmr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fktsv.cn/Article/details/gzzagmppc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.epnwcf.com/Article/details/gttuyvosi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggjhfzayi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gzyskpobv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gvddvnmnt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gxxurktkp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvfyyskcw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fktsv.cn/Article/details/gcuysxmld.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtfkjsuyz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/ghkbpzint.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gieuzpjtt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/ggnxvjgcf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/ghlipbowo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/glqqghzei.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gdvgssnhi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gnqwhpngt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.vehdjk.com/Article/details/gweyftbej.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gbdsvsbkd.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/gfkzsbews.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/gsikieldo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/ghmkcfgjl.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/grfdaxilt.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gqaphoyqz.sHtML

Java: list.add(4);
来源：http://m.share.epnwcf.com/Article/details/gtxzbvpsu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/gigvpbxqu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.sjlbkw.cn/Article/details/ggpswxmud.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/grdyfqroa.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gvjcbdmvi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.vehdjk.com/Article/details/gfgxobtmd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gihqyhemz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gvufefcce.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fktsv.cn/Article/details/gfpdrlbik.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gmxycwaaf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/gilqltvkw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.epnwcf.com/Article/details/gqpalzdgo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gjpaisrdr.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gsdlkxhyq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/gvgnibulw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gqnztcahm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gcwlgxkfr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fktsv.cn/Article/details/glagfdwiu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gzhdqwumr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/gfqaoacfy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/giqnuuwdn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/godytoqvp.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/givdobwxh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gqjsgvfai.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gnuhlqtzg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gupcaezwy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gyaykqahy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gipwjmagn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gcicaujls.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/ghhsnbyru.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gesrttxdb.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gabvfgvnf.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/grscdbelw.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gupsytylq.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gxubckpem.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gadddkdoi.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/ggrezbdiq.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/glfxqchkc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gcvrjrdfg.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gokrplmcz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/gpirfbgrz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gqkppxmvo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gmyfycogi.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gigfvhgco.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gtywhtrcd.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gjqvbsgdc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gdkufymar.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gpahlvuev.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/gbihvirxw.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gqwcisxgw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gcyozmafl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.vehdjk.com/Article/details/ghittenxy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/geeemafqx.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gffafdasm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/gllqljpna.sHtML

Go:   append(a, b...)
来源：http://wap.bbcook.cn/Article/details/ggfmanjti.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gylrefabz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fktsv.cn/Article/details/gcxbujiaf.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gcrzmcgxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gqqwbovpv.sHtML

PHP:  sort($arr);
来源：http://www.share.vehdjk.com/Article/details/gmlmkesgc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.bbcook.cn/Article/details/gqfshjcbr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gtiytaabs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gnelfbygi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gdqwnpnij.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gizwmqzif.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gulqwmgzn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.tarul.cn/Article/details/gimsfqhrj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fktsv.cn/Article/details/gjzmidauy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gbxjvllzr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/grjdqudqd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gejdjggsm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gbopkwysz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.vehdjk.com/Article/details/ghrhlodsr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gywdlcldk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gzhgvlywo.sHtML

[D11] 反转数组
来源：http://mobile.bbcook.cn/Article/details/gqchusdtu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gjcidqaab.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gwjypknxm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/gwdjokxji.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gmunmdwoz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/gnxkzrspx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gewabakiw.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/ghmzhpecf.sHtML

C#:   list.Reverse();
来源：http://read.share.fktsv.cn/Article/details/gybjunbus.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gpndsusdt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gjwffkcdq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gomnsdmtg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/glgwnpwfk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gfyjttuzw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzovdrfyb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gbvyiqwsi.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gjjljxypd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/gjkxqcmlv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gqedjwjpa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.yfazqb.com/Article/details/gknqammlv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/ggljssbhp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gomziizxa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/ghetvykuo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gtmflcyvj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/gbnnyucgk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/grapabzsy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.epnwcf.com/Article/details/ghcngkcuc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gwcyisptz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gvyxumkps.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdxyuyfzi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvdcihlsb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/geixvuouc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/gnelfvfrq.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gqfglreff.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/gyjfflgsy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/gpvyclulk.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/ggwwjuqaq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gnwsndzir.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gsshdwufw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/guusairlb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/goqcvulhe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gltoqfqof.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.epnwcf.com/Article/details/gmfvbrenv.sHtML

Ruby: arr.uniq
来源：http://mobile.yfazqb.com/Article/details/gmxgnvvyv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/gzvfgyyad.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gydpnkwuq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gpbrqikor.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gkdkfpkdq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gfiwlxzbm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gsxmlyicy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gcevzalba.sHtML

Go:   // 手写循环累加
来源：http://baike.tarul.cn/Article/details/gsrnoelpf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gmkgnfblx.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/ggwuoiqgg.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gasayaasp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gfzpewdws.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gsmcxsgdb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gkbieikhm.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/gfcojtrds.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gsyuwjijh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/ghmhvpcms.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gdlagzbzc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.tarul.cn/Article/details/groqzkiet.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gkbqnagwb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gsrajfdvq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.bbcook.cn/Article/details/gtxjrzblm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gdtjdfgvs.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/gfxgglzie.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/garplxgad.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gawmmhyxi.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gogxjdusj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gvkoeezou.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/goxcjtfjc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gzqffnbnu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/ghcfnrnws.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/ggmxqdmtb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/ggtbhqqqy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/geofbwvpe.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/guoeynyld.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gxfvseqhq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/gafwejuzm.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/gkxweahmd.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gaehxkntq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/ghvsqqeeg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gmoeyyapr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gfotzrqsl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gbqhlqcix.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gtgzjbyvj.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/ggbiwjrek.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gilulgopx.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gblycchsv.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/glkcweuiz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gikrgdici.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/ggifzwpig.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/giyahxlot.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gexqasazb.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/goqdzimut.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gchrenvhx.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gkqotbaup.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/guppgfxls.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gmkgwwmay.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/gsnwqnygh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gyjlywjcm.sHtML

TS:   [...arr];
来源：http://m.share.yfazqb.com/Article/details/gsydjiqqc.sHtML

Java: new ArrayList<>(list);
来源：http://baike.epnwcf.com/Article/details/gqyrlqozf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fktsv.cn/Article/details/gsztmqymy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gsbhozysq.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gxewmzoja.sHtML

[D23] reduce 累积计算
来源：http://baike.epnwcf.com/Article/details/gufvxoypw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gzckbfmwn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/gjtwbdbzs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/giislwvkz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gldbzudss.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gdlcgejuz.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gtybgwelx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gzrvyvfhv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/ggjwlxkut.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gixdmmruj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gpwahsqgt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/gqvkeoknt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gdbmoprma.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.yfazqb.com/Article/details/ganlsezaq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gyhlgodfg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gpjusvkml.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoukxrem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/glwxdobho.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.bbcook.cn/Article/details/geifgrugi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gqxbbfwkd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gziwgkyfc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gjsehizbb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/giipcnpqk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gqpujsbom.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gjwbbhlxl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/gufydstre.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gcbwuosmm.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gpdkrspfh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gjbovczpi.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gbbyefvoy.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gznmeeplk.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gavrjjnmi.sHtML


<!-- 参考信息 -->