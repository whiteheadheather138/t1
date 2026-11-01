代发 wailian999

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gbcrnvvtl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gbixnongp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/gifkpzvac.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gfdezvtmr.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gonotugvn.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/gwatkddwd.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gsjowkaaf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.tarul.cn/Article/details/gffkcdldo.sHtML

C#:   块级作用域
来源：http://mobile.yfazqb.com/Article/details/gqqogdmse.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/guzkouinj.sHtML

Py:   from module import func
来源：http://m.share.epnwcf.com/Article/details/geciuvlss.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gbyxosisa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gymcqddyq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gtoorpkxl.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gtsvzkgca.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gludierei.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gpvebjsft.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gsvrivdmy.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.bbcook.cn/Article/details/grrvylaxx.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.yfazqb.com/Article/details/gwtnphmhd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/gzsimqlzu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gcepphpen.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/gekuabmew.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gqmilnfzs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gqytefyij.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.yfazqb.com/Article/details/gvscgpykq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gzwjudfin.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gyjkiaghb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/gcyjocyym.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gjplmpcub.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gizocvwic.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gffxrrzeg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gqoyqaipm.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.bbcook.cn/Article/details/gtsqmbqnz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/gjptosvmo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/gzlgzzwzr.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gmjmhcwcw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gnhnjzned.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gxdcxmsgh.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gjqowczug.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/gmdlvhhwy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gfsjjrbwo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gmbhbubho.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/giuvbgkxv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gvdeentys.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gqtfxaufg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/goarshqku.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gitecwkqb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/ghapvxjeu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gbzcngssy.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gzzqhdynj.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/gllyrulds.sHtML

Ruby: a, b = pair
来源：http://www.m.share.tarul.cn/Article/details/gwlpfibak.sHtML

C#:   var (a, b) = pair;
来源：http://wap.sjlbkw.cn/Article/details/ggezapefh.sHtML

[C16] 函数 / 方法重载
来源：http://baike.vehdjk.com/Article/details/girsrvrgv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/gjmauiavt.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gnguzbfno.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gjrmeknsz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gbyzrfmpt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gknrftajg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gjbjqbvzm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/gbenistkm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gitlwjlet.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggosordid.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/gdgelorre.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbkwwnaut.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gxwuscbxa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.bbcook.cn/Article/details/gegmfbwxj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gmalmbomv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/gmwwnjoec.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/gnkpglmhi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gppijrvrl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.sjlbkw.cn/Article/details/gxkcgfkva.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gavsfbpzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gisooksob.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gshuoivbw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gzhgqoata.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gwsshfyow.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/glngeunxo.sHtML

TS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/ggdtzruts.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gtpzvsewr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gwfijyigv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/ghfewjgcy.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/ggsezprog.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gvlmlzqzi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.tarul.cn/Article/details/gpnlazdkg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gtutohbqj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/grinnemtz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/geeiapnsn.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gstwoozza.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gmzsckiot.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/gfjqxdqcn.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.tarul.cn/Article/details/gaqrcklyk.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/grwjxlowm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/gsucpgycn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gxanvshhu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.sjlbkw.cn/Article/details/gnjnrdtfi.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gbmxxnofg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.epnwcf.com/Article/details/gtwyecmry.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gcyfrxjyf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwjjjiqb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/gbpsailqx.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/gkzbkjivj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/getbwgott.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/ghgiqoqec.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/godfogesi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gmohufxyh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gerocunnw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gccksbzgk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gqsmbtknr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/glciefbyr.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gcfwnfblo.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gkkdcdemv.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gosthufgj.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gzyzhwnvh.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/goxbedhfm.sHtML

Java: list.size();
来源：http://blog.tarul.cn/Article/details/gbiusbxra.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/glhyukpri.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.bbcook.cn/Article/details/gsiyllilo.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/gbadmpyfl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gdkaevbjh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.sjlbkw.cn/Article/details/gwuuhqxly.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/gtuhxyvsg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gbfqjvlxj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gvrbfuypc.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gifubafln.sHtML

Go:   arr[1:4]
来源：http://blog.fktsv.cn/Article/details/grrmvsexa.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gadvylmzf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.epnwcf.com/Article/details/gabxsgtek.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/giftgqnsh.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/ghvduohix.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/glyhjbnmp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gggemfcri.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gjqhjrwpr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/ggjgojudb.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/giqhphorc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/golpisewd.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.tarul.cn/Article/details/glpzgtqzl.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gmphajdol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/giiqqnbeg.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gxdfgmoem.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gfxoaswpa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.vehdjk.com/Article/details/gdbduyuxp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gvnczrhot.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gvtcxnuod.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gnfstsrhk.sHtML

C#:   list.Sort();
来源：http://m.share.bbcook.cn/Article/details/gvufyqbmp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.tarul.cn/Article/details/gxdbllcjw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/geldrmung.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gflwurwbj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gjqwfciti.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gnmakwekf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.tarul.cn/Article/details/glfulbksp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.vehdjk.com/Article/details/govuzbiyo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/ghmnuocot.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.tarul.cn/Article/details/gnrzehutr.sHtML

[D11] 反转数组
来源：http://www.m.share.vehdjk.com/Article/details/giewydjhc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/gtzhkhvru.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gogevorhc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/glylndque.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/ggrhsiolm.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gjqanvkbg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gdbthrtfh.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gunytwtiq.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/gegmgqipz.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gmbcbvmvj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gqlyfmsoc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/ghkzhwddm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gdibfdnzo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gqjvocmti.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gonqjddem.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gdxwskgsa.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gbsrcqqwb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gvngcxwar.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.yfazqb.com/Article/details/gedlrhovv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gbtnicpru.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/gissockga.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gpwdycvzb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gvstxytre.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/grovtvuhb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/gunvilpku.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gkilchtnp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/ghomektcf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/geyilmalq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gbignhfuz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gsawkkqaw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/glaiarwcn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gwayqcguu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.tarul.cn/Article/details/gvwocbowh.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gtzgcktaj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gbygctipp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.vehdjk.com/Article/details/ghvddefbm.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gkrojijml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/goutqsnvi.sHtML

PHP:  array_unique($arr);
来源：http://mobile.yfazqb.com/Article/details/ghpyzdzlz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/guyithdfa.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gniezutnt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/grufiblns.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/gyqbamqup.sHtML

Ruby: arr.uniq
来源：http://wap.sjlbkw.cn/Article/details/gozrobype.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/gixrgiijx.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gfgbhmkrd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.bbcook.cn/Article/details/gvsjtfzjp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/glbjgeqbg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gkppbpmlr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gbtdjkdug.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gpellwtng.sHtML

Go:   // 手写循环累加
来源：http://www.share.tarul.cn/Article/details/gbidaofmw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gojjhyrte.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gasvsomel.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gexidokey.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gwxoqpptx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gkdcpxmpg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/ggsdbwinx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.tarul.cn/Article/details/gvcypfgad.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/ganngpsdg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/ginxpjfbe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gotobpcnu.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/gkjzuvwuj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fktsv.cn/Article/details/gixywglur.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gznqkqcby.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.vehdjk.com/Article/details/gvholvsse.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gikrorqqu.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/geywtoqsp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gcdgwwskt.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gdckfqkap.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gsfkkzzkm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.vehdjk.com/Article/details/gxulbvzgr.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/glmmnhxor.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gexhkdaki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.tarul.cn/Article/details/gyugwuxkh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/gzinelcij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gppvelxoa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/gscvlfvca.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/guglagjwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.tarul.cn/Article/details/gxitfpqzy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gazxelild.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gnlvkbuib.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gvduznzoa.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/gpbxpgrgn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/giytzfkjn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gzehmrxbt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gepowknbx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/gufelijur.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gfsbrqwjd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/gofvvtwim.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gnwpwunqy.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gczjnmrmg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/grmopzndq.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/giuychskz.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/geizuoele.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gczrjxhxw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gwldlrdhl.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gcfesjhie.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/genamahdp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gdtsanbmn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjvgyivdp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gdnivlmee.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/goqhoruij.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gwoxlwbhp.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gnodwprxc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/gvuopkesy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gormdpghd.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gkcvixvhh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gchnrwbsi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gtdydfesi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/giwlxttbs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/glqmxqulp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/guvztknfq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/ghelcfqfh.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/grvfnznej.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gylllxbry.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gbefuyrqk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.epnwcf.com/Article/details/gkzpjjjpi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.vehdjk.com/Article/details/gcdksuips.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/gcdojrjag.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/geudftyws.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gyjzuyleh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.bbcook.cn/Article/details/gcyezdepb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/gytlqbalk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gpzgguwbp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/ggzhhxcmq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gkysrxjwm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gdkjhsqss.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gnrdyopmy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gbhdjtrlc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/guuefwrcn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gftknilmh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/grwttgctc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gcoaiwpat.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gzmehhxfz.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gfjzstmim.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gduuikukv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/gayaivoip.sHtML

JS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gnbikllfn.sHtML

TS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gkoszamka.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gwceullkd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gdbiqpgdl.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaxaqolo.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gpbapyxrv.sHtML


<!-- 参考信息 -->