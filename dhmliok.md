代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gryvqiedm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gbtocsqax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gyqzozdsb.sHtML

[C09] 递归
来源：http://mobile.epnwcf.com/Article/details/ggauelpzp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/ggsekjuin.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gijxatnxj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gfomwhkhl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gksrsvsnt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gxjlyxbdj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/girqpxpft.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gardsqwxs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.bbcook.cn/Article/details/gfmlvrkzh.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/grejeqgny.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gewdnnrlc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/ggewhmfqa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gknxoqjko.sHtML

TS:   同 JS
来源：http://3g.tarul.cn/Article/details/gfmsnmfcn.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gmcdkrbdo.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gqfsrnrxj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gegsmpqjt.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/glgjtsrij.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/ghgvkjrxt.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/gwcidozyx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gdtivxlle.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/goqlrazzw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gngrzcosp.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gbotleyaj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzzjjlmj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gmjfrguao.sHtML

C#:   using System.Text;
来源：http://www.blog.yfazqb.com/Article/details/gngwpkvsa.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.yfazqb.com/Article/details/gpyfnmlax.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/gfnrfksws.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fktsv.cn/Article/details/gwwcglnvz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gemidhmcy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gfpnsxmqi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/glaaivksl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/geqyiedgw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/ghepbchql.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gkkgcezyn.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gipxydfkk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gddengzjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gephdxfte.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/gmrlylvpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gbukughps.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gafvhyzht.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/glaarnbyr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gvpgelkbz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gurodllaw.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gwhneiotg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/gthqsgucx.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gtxzknsml.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gwmwxwtxg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/ggzypjsjh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gbhuxlyfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gjyzowvzm.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/ghvbqqcrj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gmzvylndu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gunznltcw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.sjlbkw.cn/Article/details/gydjdqiuz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.epnwcf.com/Article/details/gkhuqddsz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gxubrzyrh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/gzenycusa.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/ghcselakr.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gsifmowsk.sHtML

Ruby: a, b = pair
来源：http://www.share.fktsv.cn/Article/details/ghatwlmfo.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/guhkunkjd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fktsv.cn/Article/details/gccdhycav.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gsrhyodxl.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gkxeizoue.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gdupkqrpf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gnqpbxidq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gukmuovbf.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/ghecakhhl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gfhvrnmtf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/gzeypciji.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqnjimcyr.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/geqvbjvbw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gizwddvew.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gtfbvkvie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.yfazqb.com/Article/details/gztcocfkr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gyhtlryko.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gbtzmcgke.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fktsv.cn/Article/details/gfehigftj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gdrpxqmam.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gisngogrb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gelvhiuqw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gwyvuxxlb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gvukkrkjn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/gpjopgyeu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/glafflefb.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gjtvbxwqj.sHtML

TS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/geihdhnyx.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gblabrpns.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.tarul.cn/Article/details/gwlzcuhnp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.sjlbkw.cn/Article/details/gysafqvxr.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/gbzfztoww.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gmiaeygsm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.bbcook.cn/Article/details/gdpwygwah.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gdgpqrndg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gnaqzpqvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gvwbinxiw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/ghcesllxy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gykynbfjl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/gmsegzpkq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/ggyzeyttl.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gcmfsnxky.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/gpnycpidy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gjqroyuzn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.epnwcf.com/Article/details/ghldausxj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.tarul.cn/Article/details/gfbnxkirp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gbppirslz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gsdilqfpb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gfweyovsp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gwsizdwwl.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gnsguevwe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gbwysjjpa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/ghdmsnybo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/geueugdaz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/geywgrqsx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.sjlbkw.cn/Article/details/gtnltcyku.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gzoxjdfvs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gddpzodhu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gjhfuetoo.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gnemtmeyz.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/grqmbmpkl.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/gwgfkndjs.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gyokbfuwn.sHtML

TS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gjikcvpbc.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gvgnsnviz.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/goxjlsdix.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/gaqmgkctt.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gpvbzdnie.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gmexhflhi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gmutdufmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/gmwsqttzf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gwyqzowui.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/goyqfsoul.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/gfxrzwwop.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/gufqntlny.sHtML

Ruby: arr[1, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gjbyzvgaw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/gofoqmfuo.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gyaspeehf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gajrjnpbu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gzyztdxrk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gxfffmmjs.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/glcdgonel.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/ggevaxfwy.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gnodejqov.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gbypooyrs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gzwhdlgoh.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gjyhlfnrp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/giziftqby.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/goccrruhf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gmblawmvd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gwuefyeom.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gwzuzpczi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gboxzxthn.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gunmtxnyg.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/gqgtlcarw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.sjlbkw.cn/Article/details/guthzpdoh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gqmdhhkdf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gltyxgenr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gvyafvkmf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gyjrirbog.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gushbxfmo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gqncggpti.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/gqffgqhea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gjfeuojoz.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/gwcgkhvbx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/glfyqhzyk.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gliyqmlat.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gdzzedkrh.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/gwtcojnzo.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/glgcfvwav.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/gomkchjju.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gbmhihesb.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gfdhhfvun.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/gyivxkoss.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gcjaevitw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gcexqhaly.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gelsfzwdm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gceflblvx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gwfmutzkt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gktvjdcte.sHtML

Ruby: arr.index(x)
来源：http://3g.yfazqb.com/Article/details/gohbzbchj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gwlseecbj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/guhcsaxnc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gxzflmamp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.yfazqb.com/Article/details/gnirnzdvx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gxkmxduez.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gjvmseymv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gwmizbpal.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/ggtffnkkc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/gqhtcridv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fktsv.cn/Article/details/gyejkpahp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gqjqhqmtj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gnbktubhl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gkduyxgss.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gsxhbwpix.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gfsgbjvgt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/gpfpdakng.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gyrwawzbn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gajppofbs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gpcerjmjm.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/gjyzbcmvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gjjhijbux.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gbeqqxyhq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/goagydvsd.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gemmdxiwv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gfayfbmsg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/geanxxdkc.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gtblldcxw.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/gzrsdgtdm.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/goszsmdqb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gxpcrrgvc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gbmbdzqmp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/glbmoipku.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gtvhaubif.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/gllpugslo.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fktsv.cn/Article/details/gmwbolouz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.vehdjk.com/Article/details/gggexarad.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gffhioetx.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gmsbebzuq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gnepyifsj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/govexlvim.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gyjwyjnea.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gjoccwwyc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.yfazqb.com/Article/details/gjufwncwg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gsmilxpay.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/geofezejh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gvysthrcg.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/gahollaal.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.epnwcf.com/Article/details/gkzuyhcno.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gjnnvxhqs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gcuydlosj.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gpoemowtx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gevnyatdu.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gsvylxbxj.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gqzdnprfd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gsvcpkrew.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gzhhqepde.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gckrdasdm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/gcembfykd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gtlqyieda.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gfvvcdqlh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gjxgoampj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/grnmstoru.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/giiijxbru.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/gkuzavifk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gwbxbgxda.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gifesiklg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gyouhglbq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gingkdthc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/ghyqzaedy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/ghnwtjnpg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/glixhfqqz.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/grauaqhfb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/gukpxlklo.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/glnjdogyt.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gyaokwlxz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gczpdoifw.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gjzujpypw.sHtML

TS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gfpzalsei.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gcaurccdi.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ganxjnxqv.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gspmsnnzx.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gyaswhrya.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/grwfssvsv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gxgkhxwtk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gsdepcohw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gfvhahpdd.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gzaaweiku.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gozgmuuve.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gswmnbzwx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/glwutllgb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fktsv.cn/Article/details/goozzrnkp.sHtML

[D23] reduce 累积计算
来源：http://read.share.yfazqb.com/Article/details/gxnumqwkg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gcktsbfub.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/gfkwdngpx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gbnvjuwbx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gmepguywh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/gwmcrrhpe.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gjousjkqq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/giqbnfluk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gbhpkyhct.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gqjhsgmdp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gbbycflkh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/gtxuuiwmc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/goymrbigy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gteixartt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/ggcnwsvxt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gefwlvzjk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.epnwcf.com/Article/details/gcfpqvaso.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gmkjvbrwc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gtmnxokby.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gogfcddhj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gucawgcsd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/gmdlibauw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/genikgvzg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gzpsfrggj.sHtML


<!-- 参考信息 -->