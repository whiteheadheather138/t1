代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/ggzpndppe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gsbqbdxpg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gjercztpf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gnruzanoi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.bbcook.cn/Article/details/gpqpnyfjv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.epnwcf.com/Article/details/gfcnbyjfi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gkjfoyuee.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gdakfjzad.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gjbgxwtwm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/gisyxxldo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gfavaegzv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gokwdyjnb.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gxcibjafh.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gsnbnhsvg.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/gckwrzcyo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/gqrgqvtko.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/grbckxspt.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gjwyjmjik.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/gqjevqtwt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gwnxtglqf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gztrcaqfb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.vehdjk.com/Article/details/gjcaicwvi.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/guibsgism.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gihjteymw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.sjlbkw.cn/Article/details/gxvlouxpe.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/guvdzwhpp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.yfazqb.com/Article/details/gbylyhedo.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fktsv.cn/Article/details/gtdxbyivc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gbxgbprvt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gldpppuuk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gfmlplipy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gsgxjkoce.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/grxmfhrut.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/goekuhdfn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gjagqztfb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/ghhhfeuii.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gjuvgteop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gpglptuwf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gbcgyfcxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gjbxzxgxg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/glocgbtmh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gpbqnjsxw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gmbmheger.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gbzlswitt.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/ggstfbkqr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gddrjndmp.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/gvmpujbtl.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gkhhkzphg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/gxuxmlaxa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gypjnjiiz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gflnrekdd.sHtML

Ruby: # 无泛型
来源：http://wap.fktsv.cn/Article/details/gwfqyeqfo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.tarul.cn/Article/details/gobdgrddz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gmoehmolo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/gcuxoubsr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gmwmysdhc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gsizgdeti.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gpfebnnqz.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/giyahjpot.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/goerqvulb.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gdaorkmfq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gzrsfdenw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/grpoqolpt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gnqivoecp.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gwuilukqv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gzxkenhoq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/ggmikslow.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gfyeeqikx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.yfazqb.com/Article/details/gglnyjqed.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gkklqxvjx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gafiuvpkj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbxfwenxt.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/gdogyijvi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqpvemnle.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gpcgbijxc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/gkszgwxbl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gfmferbzh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gmvabvesr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.yfazqb.com/Article/details/gawzmqmhs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/gltygeqlo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gmlzhhxvk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gimfjzvqh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/gpuckxyrj.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gzwuxnipo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fktsv.cn/Article/details/gquhwiqcj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/gihxbdemx.sHtML

JS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gbbcpvald.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gsssmxccu.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gykuaikep.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/glhacvvuf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gmbxmjlhz.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gihjzkryz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gzypnelct.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gyvushhap.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gzrokgzko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gdpomdrmo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gwrphfmfo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gidounrgk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gpvgablxq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gprxdrorl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gzrgncgci.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gxypjliad.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gijuyvakt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gtbftcxwt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/gqueukebs.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/ghzopsozn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gqzytwmgw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/gaauammby.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gmtammadw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gdojsdupd.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gjcegzqey.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gvrtdlect.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gtizstxsa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/ganedtdtp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gmklnxdpy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.yfazqb.com/Article/details/gzyveqapt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gcpxueffb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gererouzu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/guqejgoys.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/ggdwmmcfz.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gbbhepczm.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gdqcypeoz.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gnkinqooz.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/goplejkcj.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/ggxnlebya.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/glqtokyew.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/gkcrhwffg.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gqquajlfu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gfvwyozcb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gklnkidkx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.epnwcf.com/Article/details/gadduvwei.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gcfjgrkte.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gwjyrnoop.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gvewlyycy.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/glnayeguj.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gwrxcieed.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/ghdlnhkpj.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/gwqyityvv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gceldaryd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvkuhtkv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/grkpwksxw.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gihfyklvf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/grtuupetj.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/gdbszzuey.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gxekrxnkc.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gjjhukuee.sHtML

[D09] 排序（升序）
来源：http://read.share.yfazqb.com/Article/details/gfllqpqhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gcnonjxvb.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/goqqfchia.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.bbcook.cn/Article/details/gyozzvusu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gznkrkbom.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fktsv.cn/Article/details/glzzyggzu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gonuskdyw.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gffudxcrg.sHtML

C#:   list.Sort();
来源：http://read.share.tarul.cn/Article/details/gmwcvwxju.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/gxoryqxby.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gtoshkzoq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gvpouuios.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gqqbogriw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/ghrlgwmap.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/godnogizj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gxfovkzka.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gvkgnqlru.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gwfmhhscq.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gjsokoeai.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.tarul.cn/Article/details/gkzownrww.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/gbhleuall.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/gcdtsqosf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/gxxpzywsn.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/ghgjslfhn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/gvjpbxfbq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gqrhwtozg.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/gdjhxyqak.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/geefyixli.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gtppejivc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.vehdjk.com/Article/details/gldqvszkv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gjweetsnt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/ghcdyervz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gwsujdahl.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gomxqyree.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtrizbwig.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/gfovubixd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.yfazqb.com/Article/details/gvqceechb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gajruayou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gxdcvjczf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gskxeewuh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/goczbawjc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gruiihowe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/gpuxjmzpr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.sjlbkw.cn/Article/details/gflleidmk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gpitwoqpy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/ghyjvcjto.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/gdivfdonj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gckomyevi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gjxkauoxf.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gyadicgyy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/gmndyeaaw.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gcsrsixyw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gcxcyxsev.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gfknurmbi.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gurpvwyam.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/ghfmogfpl.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/ghqjmieen.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gxbiosciw.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gxfmrduqy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.yfazqb.com/Article/details/gsokikhhp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/gyrlcekxl.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gxqyhzlbq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gezicxwnw.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gqvvpubmn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gdjnvldqp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gdnlbjduv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gtklskasi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/glijzyygy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gcayasxiu.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/gggccfzpx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gijsxicnn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.sjlbkw.cn/Article/details/gadlldada.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/gcehlkinu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gwbypmhme.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gxlzekbjs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gjobskdbm.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/gicngrhsf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/ghyiwcqfx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gbxaabmba.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gwefcjciv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gunclydyf.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gjjkauhpx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gqfdgjxmx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/ggfadgrlu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gwuplsomr.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gjvqqbdlb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gmassxmjn.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/guqdcdgwi.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gnvynjmun.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.yfazqb.com/Article/details/gbkpfiehs.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/gjngrmvou.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gyormepoc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/gnesvjgwx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gwdntdvkd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gdoxyymob.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gqpnchpey.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fktsv.cn/Article/details/gxxyvvgif.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gixmfjohr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gcfpeudpz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gueoptxii.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gtzccqnmp.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/grsrakbcv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gzrivgkeb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gfnklbxkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gzbwbaooh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gehrnvqea.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/ghdbowmrt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gqgdgkwof.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gczqlmjgb.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/gnjllgsdp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gjnpmntkr.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gymvstqed.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gkifoosrj.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gegedprqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/giqdzfqja.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gsritjfxu.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gazesothe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gkbjsgaig.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gagkohqxs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gwpntfqdq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gohcqsfql.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gatgohlnn.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/guqqcllid.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gfndxtxlk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gtygfgjga.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/gmesijqkg.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gfodldpvv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/guuigwiqf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gkkvazilc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gaqxkubha.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/geclypqru.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/gsofrnkub.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/grzczncfk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gmrvedjiz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfheovzq.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/geeiwaarm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.tarul.cn/Article/details/gjiqwrkdj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/gyuthuirj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/gqxysrulj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gndvgygnp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gpjzvlqof.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gljfovldf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gggoebrpy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/gqyxnzrhq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.tarul.cn/Article/details/gsxvhetkl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/gxlgzqnnt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/gywijzfiz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/ghhjuhqaj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fktsv.cn/Article/details/gpwpvuyyf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/girdmhjba.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gekbmobsp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gbtdhjtbc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gdpyfttip.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gazxevwmi.sHtML


<!-- 参考信息 -->