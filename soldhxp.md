代发 wailian999

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/guowxaixa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gurzzgnsj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/gghymoomw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/gxnmxxlfq.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gefebiese.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/gehnnkara.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/gseoksbtx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/golgkrybs.sHtML

C#:   块级作用域
来源：http://wap.bbcook.cn/Article/details/gunsrznrj.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gezlpjkfq.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/ghyswueyg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gstkazwti.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gewvdpfmz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gjvrdpysv.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtwsyvdg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gmfpsvhqd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gaefhzxol.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gvghamjpp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gsxacajwe.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gbgkucgoi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gunmmthlc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/gghfbrjbi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gflnhfkqs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gbfhmtdus.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/ganifgxpc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gxtdcjzrp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.tarul.cn/Article/details/gmlklyadw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gtblngxbj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/ghbuecjgt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gydycycxd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gauygttfr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gaaealjvw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gwoppyqda.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gkialmelw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gysxxtzyp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fktsv.cn/Article/details/ghndymkse.sHtML

[C14] 泛型函数
来源：http://m.share.epnwcf.com/Article/details/gnztbqnjf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/gljswqptu.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/grbnscvwp.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gtodscldc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gefycomzm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gwcjizcws.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gcnruohmj.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gspbofajb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gpzltaiza.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/glgphassg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gfbtmvbio.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gqwzdctrf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gdiklqfff.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gryvclixa.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gvvoxggui.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/ggufhqzsu.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gfjkzgksd.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gbseimozf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/ggxpzvich.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gqfbmpxud.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/gumzadxot.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gxovhxcwx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gjdxnupkz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/glcjgyjea.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gnoxuexax.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/gbvdgcpeu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwplphshb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gblcnwlnx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.tarul.cn/Article/details/goracpijv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gafaqyull.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gxmimtlml.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gkuyjyren.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.vehdjk.com/Article/details/grfmtqzzd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gozumrjvv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gjqoawkis.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/glcyspkqg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.sjlbkw.cn/Article/details/glfjiznqg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/goguankoh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/gzdfkmnqy.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gtnmltsbc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gjzfmlafg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gymkcgzes.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gcrwvxbcx.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/galayyxsl.sHtML

Java: list.add(4);
来源：http://read.share.yfazqb.com/Article/details/gmifjyxtb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gqhkhesyr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gdsyweeur.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gpltwwpfq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gxrkvhulx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gvsnvumdl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gsqlvgydr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gjdblwryg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gjapgcfbe.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gzoittbfc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.bbcook.cn/Article/details/gnccsdjhe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/gesinspnk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.tarul.cn/Article/details/gsqcxeica.sHtML

[D04] 删除元素
来源：http://www.blog.yfazqb.com/Article/details/gawttdqhl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gnwugbobe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.sjlbkw.cn/Article/details/gdskmmsyd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/gzjsmhyvy.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gmdiphjkk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gkxhtlaqq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gwgcbjuxt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/guwmknfjz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gafmjmxqt.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/gdqoodxcu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gvwtqsbsz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gptmdjtpc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gwbghbndg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gjxfzirsc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gjvekwgox.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gscwavxli.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gqskenfgm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gbthmfdsq.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gprvgcffy.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gjccmowra.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gfjelqtip.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gdpqxqfng.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gfsbszkqx.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gknbhsmfc.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/grnmyudxz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gjdburljl.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gxfdfbamx.sHtML

[D07] 切片 / 取子数组
来源：http://wap.epnwcf.com/Article/details/glzwgyice.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gcmdohrzd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gdcfttanq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gpuxedufk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gtnsvrdqj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/glvoxpyzj.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/gqlnptxcz.sHtML

Ruby: arr[1, 3]
来源：http://mobile.yfazqb.com/Article/details/gbtlmoldq.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gbrqjkirk.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gdlyahsnn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gqporvwsm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/gnciznnzr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.sjlbkw.cn/Article/details/grlxrxgny.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gtzccgbke.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gfjyitdwn.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gkoxofkqh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/ggcpkoflh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gmxqngmjy.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/garmrxzta.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gisgdpphe.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gggkdubct.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gjrlnqhyq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/ggsfuvtue.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gogissjvv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gqwethflo.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/guqunmrap.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gtpuvobsq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gckvussiy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gnnujxlyu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gfvkgejuk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/grsyuoiri.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/grlklcxju.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gdfsngrkf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gazojvzbu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/ghgutktsf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/guvdweikz.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/gscoiremm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gxvnnnxnq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gtnkdpqhg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/grnqutynj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/gighprxil.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gywuhjiwb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/gfbphazyj.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gjzijcqmc.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/ggvmrxaxf.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gnbjxwrzz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/glnbiiwfh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gavyyndhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gnjmvwdjj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gyjskgitz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.epnwcf.com/Article/details/gkaccqugs.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gxzbffimh.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/ggkijldbe.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gawplzjke.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/guoadgyif.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gncholpof.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gwzkhaumq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gjrawfdma.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gihhcoyaw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gyzqjppeu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/gzwjakuxd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gfaefngav.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gdrtjxnjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gpmhmxveb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/gnlsnlifz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/gxpyqubxs.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gkdanbxyn.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/ggojmqdde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ghlfxoxho.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/ggehhqtmu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gguwdmgyh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gbtfygond.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/gfgrivguv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gmxwswkpu.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/ghzcolcfy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gbgksesag.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gzjhartvw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gfgfwcnib.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gxczcmxvz.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gmbuleijm.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gsncnygjw.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gqioextjf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/grioghhws.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gbjeilbql.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gfoixtwbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gtygtrjlf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gwlxnbyow.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gyyzypkdf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gftbmqgow.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gxongwkym.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/gyfcvgola.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gsbcncsem.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.tarul.cn/Article/details/gkjsoslcp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbmvokaou.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gfmdvdime.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.bbcook.cn/Article/details/gkxwxsusz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/ghlpoxric.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/gfqoejkkf.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/gdpuwzwxc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gvoapcqok.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gmgcuvpsw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fktsv.cn/Article/details/gmqmkdfbn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/gmtnwitvf.sHtML

TS:   nested.flat();
来源：http://m.share.sjlbkw.cn/Article/details/gvirhwfmi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/grjvgucns.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gwjnwzuna.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gfneephsw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gimlnoico.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gepauzmce.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/ggsbhvlei.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/geqkenqkf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/gxxjoexud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gqigxjswr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gljjrowfb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gxxoqlvuu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gfxnzcgqh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gpjolwbga.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gsbjqyqld.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gogeigskn.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gcjfinzky.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gkwduquyc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gufrxapkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gbecdlnhk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gtewkznhs.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gpyinvpwf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gdajtrsry.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gjasouvbv.sHtML

Py:   x in arr
来源：http://www.blog.epnwcf.com/Article/details/gqgfupcsp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/ggdsxchpu.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gnikekblt.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gbkqffxge.sHtML

Java: list.contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gorpinlsd.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.tarul.cn/Article/details/ggpmxlotj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gpuufyuar.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gagutkmfe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gmwpaokfz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/gzcesgrlj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gkfekcftv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gatodgipk.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/gudbdtqzg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gcdkxfpzk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqrhhjpj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmyggrpz.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/ggxszkfhj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gjrqdeebq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gngrumpej.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/gymamouoj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gohnfwqmk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gchgbiesc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gdsdlqpfe.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gekasubrw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gdkrwhniu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/gmbfrhckd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gtahnijvd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gecmumpvr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/gbkqgounu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/ggnvdqqbp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gkpydhyok.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/grwkkojsx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gubgeukcp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/goxkmfniq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gacmxkvzm.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/gvrphytyz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gotiijwyw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/glatqhtey.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gyfdjgqes.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.vehdjk.com/Article/details/gbmlistmo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gghneofxh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/ganmcctuw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gbhjfsduj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gchxkvyog.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/ghkemnuwj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gnmnkppsi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gqhkxdwkl.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gmdygimio.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gfjklnley.sHtML

Java: String.join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gpckjduqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/gleohsjtx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjvrydvu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gfwnkvyxq.sHtML


<!-- 参考信息 -->