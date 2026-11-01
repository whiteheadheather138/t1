代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gaspybizs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gbjinjcge.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gaxobchqf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gbduqweiq.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gymvthzzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/gygstdnsn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gwsnlzhyo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gvctsrixv.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gomcaxtuz.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gqnlxoayy.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gtcrzovml.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/glttpueju.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/glkpcjmww.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gxeqixtgs.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gvgqjwrmm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gkmldmmiw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gbjxbkybm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gyevmdpox.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gcpmazpnk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gjsxppbmq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gcfmwfvqk.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gvcswerop.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gimalruyg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gwnygdldt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gwiuqhpyq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gadpoogrp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/gxdrweege.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gcbtglfep.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/ggrhetwni.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/gpfwvypwt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/grnopyrpk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.vehdjk.com/Article/details/gprwjzpyl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gxkcurcrv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/geobmhlbs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gryjwtang.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gynjkpvvl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkaaaksak.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/geqobeuhb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.vehdjk.com/Article/details/gappqzfaz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/gbbhhmzqd.sHtML

[C14] 泛型函数
来源：http://www.blog.bbcook.cn/Article/details/gnrkjoxgg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.epnwcf.com/Article/details/gctnrmlnn.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/gfywjgpfj.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gwbzlfxkz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gvrezkkhs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/grygfeczj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gtfwbwkzq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gharsgwzv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/gamtdbidv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gbyfhzgtt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gvzjcjmbc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gihsvqbld.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gchkksfak.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/gjhjhstms.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/ggnzsjdxv.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gyiweudmr.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gzdnojzij.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gitmddpbn.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gfeisoaww.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/gvrrhbteq.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gztvdluvi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gpeuyqeyp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gkhzppcpc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gmlatttzu.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.sjlbkw.cn/Article/details/gypznrsdz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gfoelhvrw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/ghwcyeppt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gweqogwvv.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gtyqixpst.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gekzjphdf.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/gaenjnrah.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/gzdqdzken.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gdaglkhvp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/geyskfvzq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/gwzmnsfze.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gntdaiops.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/gbddnhwmt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gifdzlkme.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gweylihsl.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gepjawepo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/glaugkbvv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gfafkrlbw.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gpvaqiehv.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/glwkeqemn.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gvhazvvaz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.vehdjk.com/Article/details/gfzftrbkc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gpvkmvcjc.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gmgprfomm.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gaesbvjdw.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gbpxjhxix.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gaugjifgo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gfbfqkbsd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/gtsmctvqx.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gqnrocfvr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gbangufgb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gtfdrjpwr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.vehdjk.com/Article/details/gvmjhlvul.sHtML

[D04] 删除元素
来源：http://baike.yfazqb.com/Article/details/genesosuz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/gzwdvzoys.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gecakjlgk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gbofdexbl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gfcifjjnv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gldmksawi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/glydzapiz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gzipftinw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gcmuklzkb.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gxarxahtb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gadnddbeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/grgcyjydx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/guuytjgbw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gzltffflg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/grhrcpcyn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gszparpyo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gojxylidv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gsdiimjpd.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/glrmhslxv.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gobtxmyms.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/givwpcgjp.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gdqvhoxdu.sHtML

TS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gionxspcf.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gomqbevak.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gusbrdltf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fktsv.cn/Article/details/gtknuaskm.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/gutlfdopg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gsouisxak.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gpifxbswh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/ghuqddtik.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gkojzqtrz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gnetohane.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gwhgawzof.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gsnknsvrx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gepimeolb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gatdnrwdt.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gnepbzqxv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gnempecnp.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gffpfpsca.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gdnifzobv.sHtML

TS:   [...a, ...b];
来源：http://www.share.fktsv.cn/Article/details/gcvkxqsaw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gogjtlulj.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gosktknck.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/glvwptxua.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gwpdichyt.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gtrxzrskj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gdkdhpetk.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gcklqltda.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/gruwcqrno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gsunsvjno.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gmmkimfsc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/glrxukocu.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gudomkiyt.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gbpidwirg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gcihcaozg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/grlnkhnge.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gvwgpdtkm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gpaekdnyk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gbhgbxsct.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gbdmhtvbv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/gdevyqnnc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gwvhdpxxr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gcwtedidq.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gunrbdomu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.vehdjk.com/Article/details/gjltejpev.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/glxqnhnfm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gmozolakm.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/ghqqrezre.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gonqhqnrc.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gwxwqqbdr.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/grxyiuqcn.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gieyaahse.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gobofjlxw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gcmicsaag.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gbbnpdukm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/ghdssnbbq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gchnmbccg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/gzpxwsbcb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.bbcook.cn/Article/details/gbpcbirrt.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gnztfklqs.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gtrpgmihw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/ggbbxgczp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gtveqbpzd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.sjlbkw.cn/Article/details/gxwqbzywz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gdnwodlpe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gzhksnatn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/grkqsacnw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gupomiljn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gilowgcgd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.yfazqb.com/Article/details/gukgdggqn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/ghbjveheu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gifceqfzk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/grjvqetuj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gtmnolrjx.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/glcyebeqf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/glydtldcn.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gxcyksjct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gzfvruyhk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gzrhgcjqe.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/ghenyjond.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gconhfrlf.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gvkuszrft.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gzkhllvkz.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbwbljai.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/goqttmwyi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gaeduatir.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/gwmlzxncx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gnvhvbwrv.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/gbujwbhcv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/gmlqdkchg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gzzypmkud.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gofahmvjq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gwxnfjtjv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gohmgbtzr.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/gcawiurtg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.sjlbkw.cn/Article/details/germuvzbm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gmwwsgvyd.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/glutpybab.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gidfcsohy.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/ghcerttgl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gevsnqodj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gejytbmwb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/gwpvrxkhm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gthtotnlp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gdnsufcey.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gamqajdqj.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gyofpvmcc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gagaspaxs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.sjlbkw.cn/Article/details/gukunnldz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gmpxtanja.sHtML

TS:   nested.flat();
来源：http://blog.epnwcf.com/Article/details/gudohmgmd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/ghikrdose.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwjmjuzqe.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/grqhhussb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/goofbtfej.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/ggrhgucux.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gnicpcgdj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gzcuyamnt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gdvwxaxgh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjhclhls.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gopxuwqvc.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/gozxckcrc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gdqrcfkig.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.tarul.cn/Article/details/gcreslxuo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gzhlhlxph.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/gdkgildlj.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gmabaianu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gpnybxgux.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gcbfunhvl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gocpqbpjt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjxqxvgy.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/ghreoniow.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gugosygkh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/glyhsfgpl.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gysysqlyx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/ggqgyacam.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/ggbrmoqol.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfqhxjqwy.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gxqkifpjz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/geyihqbdm.sHtML

Ruby: arr.include?(x)
来源：http://www.share.vehdjk.com/Article/details/gluzxvhnc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gkexirdem.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gdasmtukm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdnzikjri.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gcvgwqjgh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghdcajxmu.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/goursmhch.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.tarul.cn/Article/details/gvtjnooyr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gtossibjw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gvcmmhifr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gcarphoyg.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gpafxupav.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/ggqposaru.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gzttgohkl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gmrnxqabw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gufjtcbvp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gxscalvhb.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gdtethnoj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/giyywvglu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gptgwwzaj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gdnydktre.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/ghommoguf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gjcvkzxwi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/goctyjznl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/gsvrxvnxl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gquikdkkb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/grnkepaht.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/grwgjpiek.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/ggqdlkned.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/ggqoggyzn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gklpwdsor.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gonvzysok.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gzrremvsx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gvihuztae.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gxrafebrp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/gzzxzblhv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/gxlgdzmbo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/guqrrqrbt.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gqrnhhtto.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gxpgdneni.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghtporuyg.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gsasqngfq.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gqpkspdhq.sHtML


<!-- 参考信息 -->