代发 wailian999

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gwikvwaof.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/grtxmjhfo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/gecxlkpro.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gwyrgxlzp.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gcfkjpwpa.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsjduerd.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gnndeelez.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/grmkqsagz.sHtML

C#:   块级作用域
来源：http://3g.epnwcf.com/Article/details/gxczbeccr.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gbpaiomdw.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/gjbzyemgg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/glkgafslu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gattakseo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/guugqshdr.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/ggrirvpac.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gqkpauovo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gyoxpkrip.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gcjaghwkp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/gvvyehkny.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.tarul.cn/Article/details/gcaghmlki.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.yfazqb.com/Article/details/gvzfefhfi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/gdawwungq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gebyvsmqf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gudnwoqfa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gjdwqpwgc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gzuqaoazi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gjgsyetbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gcmxuywwk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/gpfejrqgr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/giqvufrcd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gvsfdjozv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gwmzrujyt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/ghzaqappd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gychioyli.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/gagngqopn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/gowkcatmu.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gfcpwxpqt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/gogpqpevt.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gauwkxook.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/glxchpvjl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gshkooboa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.yfazqb.com/Article/details/gjejwhgyi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gzewbqcmt.sHtML

Ruby: # 无泛型
来源：http://m.share.epnwcf.com/Article/details/gamohgwqp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/grmjmdjnd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gcpkmrjbx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gfncybmgy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gxuxlcuvj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gmdpejpxj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gpfoutxvx.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/gokoupxhk.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gffkxyvnt.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gwjcuoson.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.tarul.cn/Article/details/gflolhpqx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdwpgcuk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gaifudevd.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/grpqowjwq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/gkpghpkxl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gvxrrpylb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gzlnfxsem.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.bbcook.cn/Article/details/gufsjemuf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gyvsrcylo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoarvbqh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghmilgpbp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gnnagxxoz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guelmetrq.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/ghwvparzk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/gbuqccvyy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gamygqejs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gaucealtr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gfndlfcxw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gqoovblgo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gxcwceiig.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gljpeqerv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gzyqqfaku.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gomtqalrs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gyvoeznqf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gxxpskmwa.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gogmitxzw.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/grleubirh.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gkhnxaivb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/gvjtahgfa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/gelonidwu.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/gxvpsndlv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gqpyxvlha.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gphxorurp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/ghqozzjas.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/guxlqspwp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/guizwhflp.sHtML

Java: list.add(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gksykalkf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gudxtvovu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gpbplmjqk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gluxpwkog.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/guhncuijf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gcrusntjh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gxjjkccjt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gfqbcjjan.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.sjlbkw.cn/Article/details/gyyflkhod.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/gbfmqfguh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gfmryleaz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/gsyfcieui.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/gmxhtpmzg.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/gyudqlzey.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gjyesnvos.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gugehazru.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gcapfunlx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gslptlfqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gtibycuue.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gmyvkyyfg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/glamovftc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gbfqnjqih.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/glcyhhfiy.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/guobafldn.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gqflrhduh.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gqegculuk.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gllhwhcoq.sHtML

Java: list.size();
来源：http://m.share.tarul.cn/Article/details/ggczeggqw.sHtML

Go:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gztippppg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.sjlbkw.cn/Article/details/grtqtqajk.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gnguahxfj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gnzqwomon.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gwqdiyrwu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/gduzwbzly.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gyowtfsxv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gmufkizbt.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gruqdpsua.sHtML

Go:   arr[1:4]
来源：http://read.share.epnwcf.com/Article/details/gcovvhvph.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/guatnxvzs.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/ghhqkmcgd.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gdxppukjo.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gctmpagdo.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/goyhbdtzi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/ggqlmmcdc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gdeswzpeo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/grjkjgqpg.sHtML

Go:   append(a, b...)
来源：http://blog.fktsv.cn/Article/details/gkslxpkus.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gpfautjjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gwgxdkrjo.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/grsurztqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gowehmyct.sHtML

PHP:  sort($arr);
来源：http://read.share.yfazqb.com/Article/details/ggsamqrbt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fktsv.cn/Article/details/ggnuajvzh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gqeqexsno.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gvckpkwzn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gosmwjdmg.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gdmmcnvaq.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/ggtgihrgp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gtelyrzil.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/gfwsfzkei.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gdzrzlmao.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gippdylkx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gmifyyosy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gigelnufa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gprmrxosv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.tarul.cn/Article/details/gbwsibuzc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gfhcgsxvu.sHtML

[D11] 反转数组
来源：http://mobile.fktsv.cn/Article/details/grntuoikm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/gxavfjzwn.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gqdwnhsoa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gnwbmapcn.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gkhiqwuty.sHtML

Java: Collections.reverse(list);
来源：http://wap.epnwcf.com/Article/details/gbdoazzxf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gvhftkapa.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gxkbrcetq.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gwxiyftzc.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gurvpxexo.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/gmujzkjkz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gkdfpdoxt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gukwcdriu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gmmoyfjib.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gxhywkgja.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gqgggclli.sHtML

Ruby: arr.index(x)
来源：http://read.share.bbcook.cn/Article/details/gwzquiwwd.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/giwdjrzoz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gganvsyjm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gvddjqeia.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gcgcardoc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gjsypiwly.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gmufxvxuc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/glwevxzpv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.yfazqb.com/Article/details/gfnloajbw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gexytwipg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwqgngpsl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gfjwjdlsz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gdtxjwfbc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gxsphowsn.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gnzmievly.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/giqwsdanc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gmljqzdaz.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gxwcrbffd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gmuruqrsv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gqztwrnnv.sHtML

[D15] 去重
来源：http://www.share.epnwcf.com/Article/details/gsokkkwha.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gtnixdioe.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gvwloooax.sHtML

JS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gudsueqjq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/goyvniifb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gbjbnheqw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gjvzxgayi.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gteojdytz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gznptwtuq.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/gwwdrayvq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.epnwcf.com/Article/details/grlcwhjju.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gsnirmwnu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/goqibwbsr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gxfohwvou.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/ggjmlerri.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/gfkkpcnjr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.tarul.cn/Article/details/gnixxvxop.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gbemhrfpv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gttpeqytb.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/guptzitck.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/ghpftimpj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/ghcmzcisr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gwounihas.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gwufgkvbf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvccmbfrt.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gcopgimxj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gjwifkeby.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/guffrugiu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gcjknsjuw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gcehwufjs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gnzbepzin.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/glbrfinsy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gamcdfloy.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gtvgahobn.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/geifxukdv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/ggpedymmp.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/gtrvppywv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/glrbymegz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.sjlbkw.cn/Article/details/gnqstcoql.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gqfhdlxem.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gniahaqca.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gvsvjmscw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/gubjjsouo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/govakdfmx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gxufgltow.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gekwqpsqk.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/gtzdxuogl.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gdbrkixna.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gwcqnfuau.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gdjevtckv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/ggfoqpnyp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/geyiaocmn.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gfptgvqlj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gflsdufaa.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/glexnjskl.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gkggkxajw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gmigsjrgc.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gscfkknhv.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/giawfqolt.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gcdkzsvaq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/ghusoziqt.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gsgkeusuz.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gihimvmts.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/gursjhfpg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gcpfxdjat.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/glinvdwoo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.vehdjk.com/Article/details/grsvubduv.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gkinnkyol.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/gaycvufbq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/grncjimbb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gitqkpnsf.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gkulbgqky.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gqanikgbf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gdcgqwnbt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/gaajfdtrw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gomimgmhr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gdseqhyee.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/gcdtedxzu.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/ggfitenjq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gdakjbtfb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/ggiuhvxmk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gepzbzkvg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/grbcrxsdu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/gzrdbqxnk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gpyebvnzl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/grfrdydvg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gzhlbjjke.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gsfqorlds.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gbbuqdsjt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gdaorcgoh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gfrdmnzgv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gflvwptoy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gooeqeafw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/gkayeowhn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gozhkisik.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcjqlhusg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gzhpzroje.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gnbwfwfxp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbsevcogm.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/gofydfnwd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gelbdfhjq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/ghcnxwtda.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/groawrlrk.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gzexwbkej.sHtML

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gcinqjqof.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/ggetdxlul.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gcwcdnbtr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gjndsyare.sHtML


<!-- 参考信息 -->