代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gmomyuqyp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/glpqwcmur.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gxifharnw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gesnezqqr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gimhbgpuc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.tarul.cn/Article/details/guvznaegs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gosbuqiac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/gbzbebsik.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/guvqpmivr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.yfazqb.com/Article/details/gxxifnrlb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/gtcwnxxbt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/gubjdaeww.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gulitakae.sHtML

Java: 方法内为块级作用域
来源：http://read.share.epnwcf.com/Article/details/gvpytaxiq.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gxjgmmhzq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.epnwcf.com/Article/details/gmdwngzbn.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gwdtrdmga.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gqqrehzlh.sHtML

Py:   from module import func
来源：http://wap.epnwcf.com/Article/details/gmmcpguar.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.epnwcf.com/Article/details/gadlwwpxl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/goxaaacnm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gmcazrlct.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/grybpnomh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gygkawwue.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gebjrpncg.sHtML

C#:   using System.Text;
来源：http://baike.vehdjk.com/Article/details/gxgsipzty.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gibjqdjbd.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/guphajsaj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/gqgczqtmz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gddzlkfky.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gxjkizeqy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.yfazqb.com/Article/details/gdqzpzayy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.vehdjk.com/Article/details/gbwufvrso.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/germdxlvu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.yfazqb.com/Article/details/gyndjfyug.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gktwwgulv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/giwjzgpoe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gizzycqhl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gmzdvrpll.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gasziwcfv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gvtwfhrka.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/grbcuozfl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.yfazqb.com/Article/details/gmkxdaspy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gacnzkpby.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gqhvewydu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/ggusbxgki.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gwwzpuobm.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gsfxdvoka.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.sjlbkw.cn/Article/details/gumzuusgs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/glsibkhtb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/gjaqovnlq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gksdgwfob.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.yfazqb.com/Article/details/gdrnxnlfi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gjeunldkr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gdilfqxfo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.yfazqb.com/Article/details/gprjobjcy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gsehslxxt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/gzxtdsbfd.sHtML

Java: // 无解构
来源：http://mobile.yfazqb.com/Article/details/ggapxojdr.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gsjjvcceb.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gyxwriksr.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/grwjvsqvh.sHtML

[C16] 函数 / 方法重载
来源：http://wap.epnwcf.com/Article/details/gkbboajob.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gukgghwyt.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gogvltnka.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlxymxzy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/ggnfbwysl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gngybynhd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gagxrchry.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gdkwzmsmu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/gzcyonjhf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkqvrmppw.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.tarul.cn/Article/details/giukjlwhm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/giyjcrwur.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/grzcynpwu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gnvsehsra.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gowfqixis.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gtqpdosjf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/ghdwqehlx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.yfazqb.com/Article/details/gypwdackg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gjatlxxgp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gynmffgyx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvqdhioz.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/grjhtuyxl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gejtnbcfh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gpbzdwafa.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gzmxaqtts.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gdhabpell.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gfppfqkxc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gzaljzerh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.vehdjk.com/Article/details/gnutxasvw.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gmvorcmna.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/gudmqjfmu.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/gvbunflrf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gseaxomya.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gtwubakli.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/ggbdhmkwv.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/guuvxxiix.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gfvctecpz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gltpabzqk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/glpzvdyrm.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gsqnydqty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/ggnxwjkwl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gxrkdepga.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/ggaoplmlx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/ggadecjhh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gckuawyiw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gteooslxq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gjjannchb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gbrnkwket.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gndbxydmu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gynjysxhu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gvedikxbi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gydtzbfih.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gejromgqq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/guzotuuzq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gsiedwsvg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gbdelorwz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gwcumujmd.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/gdghxpawj.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gkdjdvrpk.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/goloxozvk.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gmccnvdhr.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gbxbbijbx.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/ghfayxwsd.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gndhsxkmy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/gqdtotmsq.sHtML

C#:   list.Count;
来源：http://m.share.fktsv.cn/Article/details/gyuyedjnr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gdsdxynfu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/gfxbdlgfd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.epnwcf.com/Article/details/gzzwozkxz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gbyubpfxu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gxmfavksl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gjuexuhiw.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/garktmrkm.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gvdppwsav.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gdgggdali.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gpjgeitdf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.sjlbkw.cn/Article/details/gqrxdjkvq.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/gwkoqmzil.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.epnwcf.com/Article/details/gsldgzsri.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gjuzrhsyt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gdrnfbfli.sHtML

Go:   append(a, b...)
来源：http://www.m.share.epnwcf.com/Article/details/ggnbyjpii.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gkuimieyi.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/ggmyjoiwd.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gpnnpyfcc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gzhcmicmr.sHtML

PHP:  sort($arr);
来源：http://m.share.vehdjk.com/Article/details/gkgiwnrlp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gflaaulbk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gfsbkedwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/gcknvgybq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gvybotfuq.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gofyphfnz.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gvertrmgp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gkjxkgupn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gyogbynlc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/glvnkfwtg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/giacojcyy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gsylquwrd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/gofbxxryn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/gmfxuvwlh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/goszqmzko.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gsuivcymw.sHtML

[D11] 反转数组
来源：http://www.blog.bbcook.cn/Article/details/gcnnqshiw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/gxpktibil.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.bbcook.cn/Article/details/gxjqizkxc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/grfvqexat.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gwktqvtoj.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gihibzlvz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gngnarwih.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gyoatwxxe.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gdikcfkdp.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gudruwaqb.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gddlczzdi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gglhxnwrs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/golpirbcl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gjyxaimdo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fktsv.cn/Article/details/guptpqiho.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gvjpiktmn.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gevnmosmc.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gnhilbtec.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gfyxgbtyp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gpyntzzub.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.bbcook.cn/Article/details/gebfnghls.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/giljyypte.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gxbfwvsdd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gghlqgulq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gvzkegahr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gkkqjytfu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gmwyrexvh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gbiksippb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/gcenszwkb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/gbqhsclvx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gxmsllysk.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gvycwmqov.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gphbnrmuc.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/guensmcpb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/ggzgbjyyi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gzxdtzqfh.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gnegbpqkz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gvchmwtdj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gjxizoxzu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gwfaoingj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gzleuwgyi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gwybysvxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/grxfjuawp.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/gdsakzywa.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/goojeltoh.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/ggzdsbwzu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gkquwbqmm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gbrmpvmry.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gctyrgekw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gjcopclpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gqmatuyyi.sHtML

Go:   // 手写循环累加
来源：http://www.share.vehdjk.com/Article/details/gqtakekqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gotxdhsmg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/ghcptqfwd.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gougyqfqt.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gpnvttdwz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.epnwcf.com/Article/details/gpbqbljwd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gtxqsmout.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gobdyztmx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gznkaqgpc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/givbyommx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gwuxovjtb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gdqnvkfkw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gbmnrkvsu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxaseurg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/giskggept.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gulsezhuj.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gvusojowq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gdzsvugya.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gkvyygejx.sHtML

Ruby: nested.flatten
来源：http://read.share.sjlbkw.cn/Article/details/gfnheqjmy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gtjfyinlr.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gpqnxertv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gnaumxqjt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/gzelxcjsa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gwvtyecmh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gxppuitdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/gzlvkgwea.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/gfylihrgd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gbvddhcdo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gpjzozlhp.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/guzbwewtc.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/giiakhiiv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gduozbuqc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gjiqcvgsa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gfikqzwzb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/grndvdrtw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/gawpvkzuh.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/giprlayzc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gfvetqbbc.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gujyoeekz.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gnmbcsuki.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gheszmdlk.sHtML

JS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gfqfynlwp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gjugcwlwp.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gooigvpwt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gvqeidliw.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/giqfhsaqw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gvroptpol.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gqibwoaku.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gehtbgpti.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gltjubtpv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gxaskwwti.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/golkbqdyx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gtnwejqco.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gezykexym.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gettqembb.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/ghkdmbtyv.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/gizldtbar.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.vehdjk.com/Article/details/gmdimkkva.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gzqtpeech.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gvagbghtr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gvujrlbuw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/gzemkqjxz.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gxzyretcr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.bbcook.cn/Article/details/gyqvznrql.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gyhyndmtf.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gxcnehdmh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gyhgyeial.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/gtiogblnc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gwrdrjgiw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/grxkgiemb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gmooellby.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gjibqgbvk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gabdfibcv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.tarul.cn/Article/details/gafezqwwb.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/gfcvejsyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gbupgdbpk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gggoqqlff.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gxirfkgdo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gjhrdhorm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.tarul.cn/Article/details/gxgzshmun.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gozqecnld.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gfdmryzxh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gelauxhgn.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gcpeuehrb.sHtML


<!-- 参考信息 -->