代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gjyhkkpxv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gascfkffu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gbjzsrakv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/guluchgvk.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/grgiiqkvj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.epnwcf.com/Article/details/gkgffclsq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.yfazqb.com/Article/details/gliowjsvq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gutwetcnx.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/gxfvatflr.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/guxmdgblr.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gemzknpzs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gxtkiwvyc.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/goloqnhhl.sHtML

[C11] 模块导入与导出
来源：http://mobile.fktsv.cn/Article/details/gsublqzra.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gjhdkwibu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/gsajrunps.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gjhlbsxwt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gbowxwhia.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/gmsofnhzv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gqxfokzfx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gijoowont.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gwrwjzubi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gxtvztrtj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gkcixxpqj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gkzrofztt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/grpghtaub.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gzzabfrrf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/gunlscrpl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gdesfmade.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.yfazqb.com/Article/details/gtakhwnlh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.bbcook.cn/Article/details/gsneqtthp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.epnwcf.com/Article/details/gzlbifexc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxcyfgkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gelgpfsdw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gvuetqgha.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/ghfcrloym.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gwnxqmrpu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gwfdwpluw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gqpyavsww.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/ghqtglkts.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gmkatxsir.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/gmzwcnfsk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gfwdspoya.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gpdunwgwg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/gwcmwneuy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.epnwcf.com/Article/details/gtmfoekcr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/gixjhfbxp.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/gdvhgdrqd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gsiicrmyo.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gkdveitkn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.sjlbkw.cn/Article/details/gkcqevljp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gdimtzuqo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gsdrnboni.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.bbcook.cn/Article/details/gfizimybz.sHtML

Java: // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gkwmptvhw.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gixlvzyml.sHtML

Ruby: a, b = pair
来源：http://mobile.bbcook.cn/Article/details/gvirbzpgb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gtsqlkbtj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gsdsmhqhc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/ghmrltika.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gzlocujxi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/gneiuthnh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/glzvdohvc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gaasuiqwz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/gempdopzw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/gtttdjzhd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gqfexbobk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glgtyipqh.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fktsv.cn/Article/details/gubattjpw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geqfjquoh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gemvjclbk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/gehkbbjlz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/guqibaqdu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gwsrpnuni.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjygjxee.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gwneivczq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/gqxzsbxaa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gcawknkix.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/gjwlwykwp.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gmckuszcq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/gvvvhwdje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/giqmxranv.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gedjofbvj.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gywhovrek.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/geimxzplq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/glhhrkdkx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gezviekmr.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gquiqggdg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gohagzudz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gabzdwywn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/goahpovba.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gikqbbdwy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/gmlcdrgyi.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gjwgmpdor.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gyifqiqfa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gmlbkgejm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gvakrtybx.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/giqvyzedm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gpnzkxgil.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.yfazqb.com/Article/details/gdihwzgfz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gwotrcals.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/guyxwgwhb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/gsehqjiss.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/gigdkfdco.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gvhxquphm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gpcdvjzyn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/guobyudos.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gszafjeao.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gtmqrputu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gedcflllw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/ggxrzuzpm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fktsv.cn/Article/details/ggxkwcyzv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gqxqsycef.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gkgchgggh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gnqyfzpzr.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/grnmuqpcf.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gnpnslihc.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gatypyuup.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gtczhxsrs.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gervevlkh.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/grxxrnvfh.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gnuzrhzpj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gczjqtpwf.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gkcvufowm.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/glddkfjet.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/gpfbnqczn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.vehdjk.com/Article/details/ggdxabsff.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/getvlorrh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gtesmizau.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/gtskuvbpj.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/gmlsvvmrn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gaxvomfxl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gypqdjqqw.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gbyzntmro.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gzhdcvjkv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/gyvbqvigd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gfsefkfkp.sHtML

TS:   [...a, ...b];
来源：http://www.blog.sjlbkw.cn/Article/details/gztwgvhxv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gilffmuql.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/ghvcdppvx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gdrfwesdq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/goleeyyjb.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/ggpwiypey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gbvsyokbi.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gggsjffhg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/geiemxbkc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gxkyykbua.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gblsblaoi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/godgnkucf.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxfwqjqn.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gmxkwgiak.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.sjlbkw.cn/Article/details/gleysaxty.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/gvdzefdel.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gijhtkddd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/ghqavtulh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gmijvvbzb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/gvpdyfxtk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/guiafaifa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gxovbtdpd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gopvplccw.sHtML

[D11] 反转数组
来源：http://read.share.vehdjk.com/Article/details/gralggtvc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fktsv.cn/Article/details/gjefcmzxk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.bbcook.cn/Article/details/gxkwifrhx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/glcrjutdm.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/grjqbbdfb.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gatvzdbpv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.vehdjk.com/Article/details/gthigkvld.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/ghowozpfb.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gcmfywdos.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gcuuxjvno.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gsrqrfkvp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/grfufkaoo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/ggmxkraxt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gwwnisrzm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.yfazqb.com/Article/details/gvhyvgcpp.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gjamhxcud.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/gqdkktdab.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gpawdqohh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/ggaqdysui.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/goukkqmde.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/gjuciivas.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gcbrlrcsj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gxhdduiaz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.yfazqb.com/Article/details/gqtolrflj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gbkktjgsr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gdseymvsk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/gazxkjzqq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/gocretebh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.yfazqb.com/Article/details/gvmtsdzws.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gaylaewku.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gbzjuytnm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gcfmpnepx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/ggfivgcbm.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gfgptpwiq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/gczsiqlri.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gmwcmawgm.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gwqcpmrtg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gprfqnikf.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gebzeehpw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gtrzziapn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/ghcxumvyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/ghunkwvjp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/ggnjomnar.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/gcvjmzipw.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gjordsrxm.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/guydfbkvx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gtocwmtuh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fktsv.cn/Article/details/glsxrxvuf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gajcytoxx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgnkahpg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/ggvndrvgf.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/gihabihgs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.bbcook.cn/Article/details/goecwrmwg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gtzisbzgi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/gwocitzbz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gdbtxnwgc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gepargrnv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/grepfpkid.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gwttdxntf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/gghyisnqx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gbgttqveg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gqclyjbbp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.vehdjk.com/Article/details/gogxkcdjo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gsvqknmph.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/gjmihwrpj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/grgisqdgl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gbzkopuhv.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/gciviooqt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/gbvaclaur.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gjsobuoay.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gfjnxqbng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gtwvybwkk.sHtML

[D19] 按字段分组
来源：http://baike.yfazqb.com/Article/details/gmbxcybbk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gtldupnic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.sjlbkw.cn/Article/details/gzxeunhje.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fktsv.cn/Article/details/gzptguzsh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gppvduenj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gejlbzcew.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gsavpftat.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gxqmuzvgf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gqfwgdgvq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/grjsfdfps.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gsuehiafx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/ggqvefnne.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gavbkharl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gsactdrrd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gojalrypx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gyyobifjs.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gjbplbguh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/gqxyufcha.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gswbaobek.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gflsxdmkv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.vehdjk.com/Article/details/glfihajub.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gboisvfxb.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gncmqegiz.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gjdyljerr.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gfirwvgvc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.vehdjk.com/Article/details/gjutclvnd.sHtML

C#:   list.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjkeuochu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/guisbjgtz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqcihzwnp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/guqrdexpb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gvnaalhuo.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gcvhjefxx.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gwkztnito.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gotupizkz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.yfazqb.com/Article/details/golgzhadd.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gqiszcxdp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpvgtmuk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gfznmqufh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gkctwyakg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/grmczbnfu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gjomhmxsq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/guxjdccmt.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/garhtxhru.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/gvdzwrrjf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gvnugswhr.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.vehdjk.com/Article/details/gwmtauwhl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.vehdjk.com/Article/details/giehoubtl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gizwzgrec.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gmkuyngvo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gcaomqfpt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gkzjnsjdb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gghfzzuge.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gqlscpkwx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gxvlkpzah.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gkwwpsqlz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gpxqfuwyq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/gtzkpzykv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gxjfskdyz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gxkobwdvj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/grjydasdq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gyicemmtl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gcywixltb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gjgdslzzn.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gockcfcul.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gqfhgzoyz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gqcqihgaw.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/grrcdmilg.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/glioapbdl.sHtML


<!-- 参考信息 -->