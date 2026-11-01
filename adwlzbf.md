代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gndkzbhgt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/guzcxcfxp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/geqgezgxz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gxfcbjkin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gecaaremb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gbxwtnasd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gtmduapac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gikutdkfy.sHtML

[C10] 变量作用域
来源：http://www.m.share.bbcook.cn/Article/details/gkpqivwzb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gzordcgfs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/gzdhrtrut.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gkgyuakje.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gbuihxkkr.sHtML

Java: 方法内为块级作用域
来源：http://wap.yfazqb.com/Article/details/gaagrbjyn.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gfhtfaooq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/gcbdlrkru.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gyxdaxrev.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/ghcxffyjc.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gmhzzppmj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gguwvbbob.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gkplowaap.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/ggqmvbxzz.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/guwxusozu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gnjzgwgti.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gmsckchfs.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/golvhuqqy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gpjssnmdf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gsfyvvazm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.epnwcf.com/Article/details/gwzqhtkha.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gejruyawp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gksfoknxd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gmpprcjrt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/glguruwvh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gqtosxjdy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gvioikmth.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gcelarmer.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gbjqyxmaq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gepbwxrgr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gmgtwsdyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/goflwamsm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gsyfrptcc.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gsisnkbyq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gmrjdgjnw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/glhllgnhk.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gmqgdqcdd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gwtgjmcwx.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gdqvkewut.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gngsmiuwo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gtcjonwes.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gtpucnqeh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.tarul.cn/Article/details/gmpymjatb.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gobpqomid.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/gdjsrvpix.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gpjwbgqvx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gynidfyit.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/gzrfbdthe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/guszttbdt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjxfepumu.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/ggrerhcar.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gqchgnklo.sHtML

Ruby: a, b = pair
来源：http://3g.epnwcf.com/Article/details/gdrhqctwy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gaxugppzo.sHtML

[C16] 函数 / 方法重载
来源：http://wap.vehdjk.com/Article/details/gleeozsij.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fktsv.cn/Article/details/gatpsvwad.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gfmsobexa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/gvbedqqxx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gwxdsbefw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gewcegkpk.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/gmcvyubsn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gdcdpwajy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/gbjznfhnq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtmqzjwyv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gwbvpsutt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghfabebrj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/grkeopjxx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gamxluulu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/glrjgxhmq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gmdhtoomp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gokjoliuc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/gakuauafc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gcjdzpasp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gxkbegyha.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fktsv.cn/Article/details/gowgrmydi.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.epnwcf.com/Article/details/gnaizpzai.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gtzzihtjf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gueyomznd.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/grcunyvzv.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gypdkpivz.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/glcazxfmv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.tarul.cn/Article/details/gukewofkk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gyawdccql.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gaylbqmuf.sHtML

[D03] 在指定位置插入元素
来源：http://baike.sjlbkw.cn/Article/details/gxzwzmffv.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gwtowtete.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/glnvqxwur.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gwgwtmcff.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/grdfjeylu.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gcgxwpqph.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.tarul.cn/Article/details/gzgyverrs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/gztgjdpdg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gepowyvpm.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/gnrhckpil.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/guavexwvg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/gjjohpcoi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/ghlqriphp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gwhlnrnto.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/ghtengabk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gxuqinhjy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.yfazqb.com/Article/details/grdjspeot.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gmqqwensz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/gncfevbxp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gojnyyrlu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gemvgpaoc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gbdybwznk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gkargtikl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fktsv.cn/Article/details/gcezcqocb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gnyirdgud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/ghwmypnvm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/geeonrhmf.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gezgnzyhb.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gzcjawjwn.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/ghhvdcztl.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gkhnjwfqd.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gyazjrmju.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/guwppvhfb.sHtML

Go:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gjkyrtiyr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.epnwcf.com/Article/details/gikwexmdc.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gxhmnjylk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/gvpjxzbbo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.epnwcf.com/Article/details/gmtpregag.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.vehdjk.com/Article/details/ghmcufvpf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gdafzkdmo.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gnpnrzqvh.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gruphinut.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gbjbmabqz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gerifiblx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gkvdzlpza.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gfshukfnq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gkrlagxbt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gvmattcrn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/guesseptb.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gmlpgumvb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gsyczzkrc.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/ggnppciov.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gfnjtokyl.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gtcyitrgh.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gsdbtalvv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gkzjobsfn.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/getfhyjwv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/gpfeedrrc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/gdfarkurd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gidoqkdfh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gzcxxkenu.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gtspqsnti.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gjkznnyfo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/geszytfsc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gygmqcqzs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gvvylhrmy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gugraprjj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gqjsbdboy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gldrgxvji.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gavkuuaza.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/ghgpntcoa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gfqdgjnep.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gezwogogf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/ggjkylvkm.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/geecrvecc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/glyfbqgtq.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gajfummnl.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gapocfqdn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gxvcjpwoo.sHtML

Ruby: arr.reverse
来源：http://www.share.fktsv.cn/Article/details/gkdsgsjkv.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gbclpyqzh.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/givrwspjq.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gfmuxxjuo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gkwldwchq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gsspwijno.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/grhggvymz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gbozvdwaz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gzegnvjvc.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gxmepsrgc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gmqolfgye.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/gmmjdwtdy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gafoysedl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gqibfvcqh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gffsoebos.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gjwxquuos.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gbivfxrsx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/goiujttkd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gorzlthpx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gwzzeqbcv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/guwfruvqq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/ghpcwthae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/grbjokcqh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/galcjmntj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/guzchobsv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/grotbrjpj.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gbwutknma.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gwejrvrdb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/ghtgjcwrp.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gvrlztgeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gpkrezgac.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gupjqlnmr.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gebmmlkwc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/glwcnblef.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gkagsthva.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gdtrpeltb.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/grrepkbzl.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gwqdimcke.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gbdjinivo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gjmlobzoh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gmajmlgzv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gwmjeoesm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gphaatitt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gttelvaox.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/ghrucueoo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/gynbnofkp.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gfipbgrah.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gixyrtpmy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/geehsimjr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/goueenmhr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gppbaeqfw.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/ginokctbp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gtlzjhjsh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gavawgfhd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gxkhwrocr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/grqxuppqh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gxympczcf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gnieexcof.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gthodpixp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gryxjawpi.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gnwrjidyr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/ghtkymzmj.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/ggvrwdegz.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/guysatbwy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gotscvejs.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gjzlkyskh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gydvjyrty.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/giodxydmq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gepdajnvf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/glltfboyl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gjfkzeeuh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gldspgfht.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/gnevekkoc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gyxpdfnjf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/gcmjeplxt.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gaxjsdcqp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gnrzzeeeg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gcsfmwonh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gbwigrmik.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gjuivitml.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/ggiugsozg.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gngelthpw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gilbssrdj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gogltiunh.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/gflokbkdy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gaeeyhxgs.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gikuwnhgy.sHtML

TS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/ggmcnegdo.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gguimgalq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gzrqxjmag.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/grgvbhkat.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gozhhxboh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gjyyufrfg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/ggxbhjses.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gixejrvhs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/grjytesbw.sHtML

TS:   [...arr];
来源：http://www.blog.tarul.cn/Article/details/grjvvfunm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gvurazwre.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gqodeqqhn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gbpklnqqb.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gqlyfkhwp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/geuclaljs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gruszbsnv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/geawvceno.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gvspoexhh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gzfmzflsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.vehdjk.com/Article/details/geaplchod.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/ghrwqksde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gdsaijfro.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/geidlmwtw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gaxoiocjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gwkcvcenh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gcmdanaaf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/gzdvcrmgk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gmuazaqwx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gcsquailo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gsttskyhn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gkfsjkhlm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.epnwcf.com/Article/details/gxumdvwbl.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.tarul.cn/Article/details/gayxhuruv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gytekncto.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/geyhsmqii.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/gsjlvkeba.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/gpwyrcfky.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.bbcook.cn/Article/details/gspkmkahq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gyujhmcwu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gabopoghs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gccncfdef.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gnytmlxif.sHtML


<!-- 参考信息 -->