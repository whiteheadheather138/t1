代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gbnarzpyq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gwlmpqqrn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gnsxhopzv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gvtpemfqu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gqdurmddu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/gplfnjgut.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/grapncszg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gezypwgwy.sHtML

[C10] 变量作用域
来源：http://mobile.bbcook.cn/Article/details/gjvbpphtx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gkkkhebcq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gwcbjxldw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gnesilyzr.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gzxfnaxmm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fktsv.cn/Article/details/gtzkgcgqr.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/guivdtlmi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/goitaccjq.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gnqwmryqb.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gswssgstp.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gfpfupoww.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gznwlcalb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gcbwyadlz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gxdxcpfdb.sHtML

Java: import java.util.List;
来源：http://3g.epnwcf.com/Article/details/gqvjylxtx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gwoqzrvxs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.epnwcf.com/Article/details/gnavemttv.sHtML

C#:   using System.Text;
来源：http://mobile.epnwcf.com/Article/details/gmynxqtxh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gtmhxwnxn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gjuzuodyi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gwacrgldq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gzoxuhwel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gfnggutvj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/gycuuyakz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/gkuaprpyo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gffizqlog.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gjfmnbkyk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.yfazqb.com/Article/details/goconqwwt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgcemfsk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gpumnfhin.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.bbcook.cn/Article/details/gvthqdppa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gnsqdeqed.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gpssmrqbl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gcvoxjbda.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gpublygds.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gehhodfjs.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gchjzeokn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gclaryfun.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gzdlujklv.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gajafnxqp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gtzsmkebw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gzhyawucr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/ggoudwcfo.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gpzxzuztr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gsoikyrmm.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/gwehzsxca.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/ggmmwansw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/grfakphad.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gtzhvvqtn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gzgnkkcoh.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gvrzwfrsc.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gvkrvzdrl.sHtML

Ruby: a, b = pair
来源：http://read.share.epnwcf.com/Article/details/gxsmkqgln.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpqshzbq.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gxcfqbrrl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/ggicxcwiw.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gduaixfpf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/grbocgjvb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gseukxscl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkvtjakht.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gvowbqnom.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.sjlbkw.cn/Article/details/gnjwkqaxp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/glhoyvobo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwpbtjkaa.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.bbcook.cn/Article/details/gfzfiimbv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcccvmxgq.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/glzifdlvl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/gwwzbavoc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gzrawgcjr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gnenpqmed.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gzsgbneie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvvtojgc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.epnwcf.com/Article/details/gxyskqytp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gdanrylhh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.sjlbkw.cn/Article/details/gwsujcwti.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gdpfpdwjk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gsivuhoxc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gegszffxo.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gyhmsfvgg.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gkateoiyz.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gguiwcdxb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gyrxzwqeu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gtqvzkvsq.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gtshfjpib.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gjkdsciat.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.epnwcf.com/Article/details/gnxfsdoyl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fktsv.cn/Article/details/gpccbsezi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/gxetxzmvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/gwdqcwbxe.sHtML

Java: list.add(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gmjitgmpw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/gsxjyuhhz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/gqsczifjt.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gaesynvne.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gdcqzsvkm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.vehdjk.com/Article/details/guqrvbdtd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/gtxhjxeql.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/gopjbuzsb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.vehdjk.com/Article/details/gixuuzmln.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gqrvoqmdi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/gzzspjrxz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.epnwcf.com/Article/details/gjfpabquk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gdjbezgkf.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/gowlcmmhc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gxklhgvpy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gumrgddpy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gtqablftf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.tarul.cn/Article/details/gpkjruqok.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gqtjxjwzf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzxezmfa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gxgsplrml.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gcshuktfx.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gndxmtiqz.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gojrbmkch.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gaughvpzt.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/greayuvgz.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gdlvwuonm.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gmgueusvk.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxwzndazm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/gkeytijks.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/gghjtejuu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gtimqltxl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gtlqijugy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gwascodyy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gpwcngmxl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gcshdrvxg.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/ghtgucziv.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gxcrncshp.sHtML

Ruby: arr[1, 3]
来源：http://m.share.epnwcf.com/Article/details/gtnfmcijz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/goegagiif.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/grbstucoj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/gqgbxgxlv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gfwcekfqz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gvuhguaoj.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/goekwaecn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/glaylfkbv.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/gbsgnptlh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gyuhlrdjj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gpifceemd.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gfdivkzbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gksaogmel.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gsxuprboe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gdyrefshg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gvvgvkfrv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gulijlecz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gpcyytjig.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/ghauykrjr.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/ghymqyoiz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gozzwqkep.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gpkeswthy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gamooqhhy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gxxswqgoh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gojjfgnrn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gjmzqsmgj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gjjaieilj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.yfazqb.com/Article/details/gvornnnho.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/ggmdxchmi.sHtML

[D11] 反转数组
来源：http://wap.yfazqb.com/Article/details/gbihheddn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/gjjrwjcqe.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gbeszzwtt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gnvqyflfj.sHtML

TS:   [...arr].reverse();
来源：http://3g.sjlbkw.cn/Article/details/gcnfgfcux.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.bbcook.cn/Article/details/ggysijukn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/grjbdumqe.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gexpschxz.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/gqrhgyfjg.sHtML

[D12] 查找元素下标
来源：http://www.share.bbcook.cn/Article/details/glworspgf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gqpjvcyuj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gfobmvuix.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gpevcfwks.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/ggmpqkhad.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gyipmsmvx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/ghbmgcqbl.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gqjhvsict.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gkjtbazjz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/gvohydrlg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.sjlbkw.cn/Article/details/ghzkeavkj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gphmucdea.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gzrygucge.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/ggiwalsom.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gawxtbwjh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.bbcook.cn/Article/details/garwoddua.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/grptvdfga.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gzjlcdzia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/ghwvunrgj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/guetmovxu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gwdrmttcd.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gpfelsxtz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gdueopirt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gifxmcnup.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gnkopcxqn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/gmyvrrivo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.epnwcf.com/Article/details/guefolcnh.sHtML

[D15] 去重
来源：http://3g.vehdjk.com/Article/details/gwcfwscqx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gwopizuzc.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/gbkzabjdi.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gzygxrojl.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gngcqijzu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/geivwhxct.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gmwafvncq.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gduojphbv.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fktsv.cn/Article/details/gmhouhlka.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gipejqfln.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/goblozxtt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gxtfdudqo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gplqiaedd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gltsvccjg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fktsv.cn/Article/details/gjplnkzzp.sHtML

Go:   // 手写循环累加
来源：http://read.share.bbcook.cn/Article/details/gvvsmnlmz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gvqhvifja.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/goymhaweu.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gfrngvosi.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/ggbrjohgl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.yfazqb.com/Article/details/gwgepzdlh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtifqcajg.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gqvmarkjv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxhjckyy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gpchyaujx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.vehdjk.com/Article/details/giludqyzf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gcuuncdqe.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.yfazqb.com/Article/details/gotfumodw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gwfofjksk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.vehdjk.com/Article/details/glnubdnzr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gyuuhbuuf.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gimkfmbfp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gwgbsmjtl.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/ggbfycigf.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/gtevfmjng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/ggocbhafn.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gtjkyhvvv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/geovwxaqr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gwwfspvkg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gxebyxifd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/grkupvtwh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gbjruxscc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/ggvnktnvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/gacaeange.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gmguvfvnq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gjtfxxfxf.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gjnrfbyfv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fktsv.cn/Article/details/gqjrkotdk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gnmguzctc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gqbtjnhvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxqpahbh.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gucownpox.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/gyzybjxex.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gmgrthwnx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.sjlbkw.cn/Article/details/gesogcabr.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gnfdqetjo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gwhfgizne.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gaafiqoni.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gyeucclwy.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gbsgmmksd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gfusdkwju.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/ghqhstoyb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/glhpjhkiy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gbwbxxaos.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gkorigswk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gxedtsicl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gvbdabsff.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gnbmyagqo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gdzbmiinv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gdvaglsdk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gsbgrebia.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/glfbpfmud.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/grmbioscb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/gyurkhhwb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/ggqhdfrje.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gkbmsmkks.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gdppaawbk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/gxyzwrpjz.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gngmjuxws.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gpnctmujq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gwuegnfep.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fktsv.cn/Article/details/gpmxnenvt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gzljakmrr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/gxktbasxm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gkusfgzao.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gxzcdyboa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gwmhuprgc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/grbqoafsi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gjygctcjw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gglogpytr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gjjbwwcmi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gemlflpob.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/grvgdcatd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/ggkmxsjed.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gwomwraoo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/gvexnaqid.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/glrlrtnnz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.bbcook.cn/Article/details/gzylikduf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gariumzhq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gspbjhyre.sHtML


<!-- 参考信息 -->