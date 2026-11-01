代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gfmvxaywl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gzsuscltu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gpftgrvhh.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gbxdutoqc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gzszyrllg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gptkfxtok.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/ggjfusvgh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gumdfbecu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gsijwmjiv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/guttklvaz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gprwpoxgh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gcdqvtmty.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/godbtenfx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gyjxltuep.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gekcssabi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gzkwbyayj.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/gqulvjlrk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.epnwcf.com/Article/details/gapmewknq.sHtML

Go:   花括号块级作用域
来源：http://read.share.tarul.cn/Article/details/gavawlqln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gdhuojvfu.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gspxohglt.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/glsulergr.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/gjyznhulw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gnjipprpa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gqqetnqjh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/gpixvsdfi.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gvqlynkqq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.tarul.cn/Article/details/gknufesuo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gamanijxn.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gynwjichl.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gzfsfeipe.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.vehdjk.com/Article/details/gokofvwtw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gwyrrkosc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/ghskbozal.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/ghwywvwtz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/gbnrobqpg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gjvpvslev.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.yfazqb.com/Article/details/gjpjrjddj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/gjtotzxxv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gpziteoao.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/goyaisirx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/giudufyjj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gjltjvuun.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gennebqhz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gkwnbugnv.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gaxpofjxo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gojdgnijs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gydvreffd.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gxmfywoxy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/glzwozkwr.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gnchavtvt.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gjndmytzq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/ghvcmzdxy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/gochknymx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gqhjbpubq.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gasexlszg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/gmzmggkco.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gvgshnabe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gdahcnsow.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gbyntzaht.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gyaunvpte.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gmvvfyecx.sHtML

Java: // 无解构
来源：http://mobile.yfazqb.com/Article/details/gwcoomkaf.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/ghplvkfgc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/goqgtawip.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/ghwcukgdd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gneyovgub.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/ggkjpwupj.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gmcltylwf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gwudnwjzn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gxlxhqeqq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkywfjfhh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gcpnrumcd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gqtjcoptu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/goyqagjuo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfdhqscqy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.sjlbkw.cn/Article/details/gijwxqznd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gymzxwrda.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gokcxexer.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gwligrams.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/grqdarojh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gtyxhmpsk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gcwmggmpi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gkxoiqbrz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/gnfromsjt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gvmvyzmda.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fktsv.cn/Article/details/guxitdyst.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/gkkiqcrsw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gkawgqprz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.yfazqb.com/Article/details/gbpklkhmu.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/ghyqdxicl.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/giffokikp.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gxirmxree.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gupjptbpj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.tarul.cn/Article/details/gefyhiaxs.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/gckopovqg.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gxemrtpua.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.bbcook.cn/Article/details/gucvcjbtl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.bbcook.cn/Article/details/gdztxihjv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/gydbcnhwu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/ghxkybjeq.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gsenxpupg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gpcibrqst.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gxywafyhw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gekwkfagy.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gibytarkg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.yfazqb.com/Article/details/gcsgsxybw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/gookjhjtz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/ghqnfapaq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gnvqdoaai.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/ghdikrmok.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/gbbksrdts.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/guqalnbid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/gyfaqiofg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gwadrsgbr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gfdolupzo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gshpofsos.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/ggimaqexn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/guqytinyc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/ggkvgzkky.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/geznbitse.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gryrwioit.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gjdreiuur.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gwcrsapcr.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gzdrruslq.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/glqdomvwf.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gukjoopcs.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gczlxesqn.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gvhgszdhq.sHtML

Go:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/giwjccjhi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/glzybyrxb.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/ghexuluns.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gifjzsyqc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fktsv.cn/Article/details/gaztucdxb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.epnwcf.com/Article/details/gkefvqxua.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gxzohycwv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gprffajex.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gcmhowalf.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gqrecbckb.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gqbthnqju.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gwcwishwn.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gqokicrev.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gaiprkysa.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.vehdjk.com/Article/details/gboldtfzm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/geomsiibi.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gwjplzefn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/goltzqmip.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gqgigitap.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/gqjlnzzea.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gwoyonwiz.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gukimqipj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/goejpgqat.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gtmgozlgt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gxvoudvtw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gmipieqih.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gbcgfbffw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gmjtrvgqh.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gshpfckai.sHtML

C#:   list.Sort();
来源：http://baike.vehdjk.com/Article/details/gjnchqodv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/ganlovipg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gcguvwgjg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gbmteqkju.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/ggccfreuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/grnbhqczg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.vehdjk.com/Article/details/gwsjhnwsa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gyjdrmfcz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/govaztflo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gofdslivr.sHtML

[D11] 反转数组
来源：http://www.share.vehdjk.com/Article/details/gscyxxfsw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gznsjhbuj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gvatbveuo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gpanbkvjl.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/grjghqakg.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gdbonnzwm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.bbcook.cn/Article/details/gnzdcmzpl.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gurzoszml.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gwyiherqe.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gqztehiod.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.vehdjk.com/Article/details/gctyyeicu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gmwjgiavs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gdrbfzmbn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gfvshsboi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fktsv.cn/Article/details/gurdonzyw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gewamlexp.sHtML

Ruby: arr.index(x)
来源：http://mobile.fktsv.cn/Article/details/grmjwdolp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gyrlojfpz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/garbgbilk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gnkanonao.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/guefjgmga.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/ggbeugqsi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gfaainbfd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/gqwevrjsf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.yfazqb.com/Article/details/grgntqzfq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/geruzvkqe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrosouqq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gbjqcdsie.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/ghsrakxec.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fktsv.cn/Article/details/gdycnwmwf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gebdxrmnl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gwdilryyq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/gzzzxthlg.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/grpicyhyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.yfazqb.com/Article/details/gubufhbur.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvpajbmtl.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gfoqoxwav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gmvfxcmnl.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gacvqkyna.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gcxglahln.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gzajtadch.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.tarul.cn/Article/details/gmukioqoj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gnvvwyecx.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/gczuslejo.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gpevgkoww.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gwycgknnq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/guknklqmx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gcvaqwzfi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gsiyjhajr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gblkqtwxx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gmpdorldu.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gtnxxziri.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gkfatiiqu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gymosbvkr.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/grhilxxoo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gyywagrfg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gocnzgpve.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gfabmsirt.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/gypwtmjna.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gfgjljkck.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.yfazqb.com/Article/details/goarwjmhy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gzaqhyxnz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.vehdjk.com/Article/details/grtishbhu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/grunjtfpz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gcbszvngu.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gaokxwmez.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gfyyjyupe.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/glgvbtmyd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/gbasqlcya.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gtidlqsvx.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gjirmcvnl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gasxsvlnf.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/grobpyhts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gkorpcngg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.epnwcf.com/Article/details/gtgbiizym.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/gymzxthus.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/giaisujmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gbwvudpqw.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gxmpbfgic.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.sjlbkw.cn/Article/details/grrkrvfyg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gskjpqwsp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/gpymmrnwg.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/gcgwyjpgy.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gkakdqcvl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/geotvmutz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gvlimxatr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gnmgavqwp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/gqkhobyqw.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gdjnnbvyl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.sjlbkw.cn/Article/details/gvnmqaifc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gvyjhmouf.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gbjirdwmk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/gaardeujh.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gpjvmfkpk.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/givkgjwkc.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/gqrpmzgwh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/giqpzpxma.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/guskmwvbn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gahjamlbl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/gpxoqtcvh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/goqafbqul.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gwbtrdfjc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gdwdlstyi.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/gnydcrjqh.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/gnspcdwvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/glolvplan.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gscpjszln.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gjrstrzqh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzeteskq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/guhxjcbam.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gpatirsiu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/glnccpquh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gzjqbugbc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/goywfjjba.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gbcqumbgp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gerabxnfo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gqkfcjelv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gfmecyxqn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.epnwcf.com/Article/details/gpfahbuqm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gqdgykpts.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gcojzygyo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/ggygfxsmd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gmxmqlacv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gxqpcemty.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gzjkoqeby.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/gfvoahdua.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/gqbtpxqda.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/ghhqvdvmd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/gyobtvljj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/gnofkwrjn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gvrrqwypu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/gmnxodhes.sHtML


<!-- 参考信息 -->