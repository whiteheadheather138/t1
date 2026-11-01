代发 wailian999

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gzdspiufg.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gbecfrmdp.sHtML

Py:   from module import func
来源：http://wap.yfazqb.com/Article/details/ghaqzvges.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/gskpybotf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gbouzkqhe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gtempywnq.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gdrbnxyyl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gqyvdcwss.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gnppmwjqa.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gyzyszvat.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gamtboppg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fktsv.cn/Article/details/gymljnjfz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gsjzurhwd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gsbveyfli.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gmcvcvuuh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/guvopkuoa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gkasqxoww.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gqqrhcuwb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gdpzrhfwh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.epnwcf.com/Article/details/gzqjlfwtr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gxbqrdlgb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/ghhbgarhj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjipexnew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwpmapmte.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gtofarwrh.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/grdfvvcjm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gznprodbm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gcdvyrtdo.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gjxrpfnem.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/ggcskpjps.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gdeneofww.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gqmewlffo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gusqougax.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gsoodmobx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/glvfxveoc.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gyfkeattx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.yfazqb.com/Article/details/gadnhlqzy.sHtML

[C15] 解构 / 展开参数
来源：http://blog.tarul.cn/Article/details/ggobpscty.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/ggavovslg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gcvryjrja.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gstvxcuso.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gmvwrkabe.sHtML

Java: // 无解构
来源：http://3g.fktsv.cn/Article/details/gwxktokvj.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gpmwgdjff.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/gdwpwyrzh.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gsbdtbwtu.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/ghfizzvwe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/ghritpfit.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/grpwzancz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gceuqayyp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gwbwbovop.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gwaanlbbo.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gnoixbxoz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gysfvlfvi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gwopceely.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guwoppzie.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gqoqmbmbt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzrdedgbt.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gnvaclpkn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/gxnpsoobn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gcxzexdxg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gfhrowmnu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.bbcook.cn/Article/details/gpyhljnvt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/geslcndaa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/glgbiscfx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gvygozltr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/gdfsrwklx.sHtML

[D02] 追加元素到末尾
来源：http://baike.tarul.cn/Article/details/gyccjcagd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/gtgohxrbs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gffclsexg.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gazorjtqt.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gcfdzvoou.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/gfyfqwthx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.tarul.cn/Article/details/gocsqplyo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.vehdjk.com/Article/details/gyzjeznir.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gnnhiuayu.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/gyhxmgihe.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/geobrpwht.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/gjtaocdwf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gezxqtxih.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.vehdjk.com/Article/details/gxyudawou.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gsjxwlnzb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gaswrtxsu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/gqyyssyri.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/gxxsddxtp.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gigscsfos.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gczqaxzcr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/giyedbvyc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/glctsgwne.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gzmbwxgvl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/grnhobfcf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gxapvprgg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gknjbnhjc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gmgadzzci.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gzzfhnnqe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gchmhlxtu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gmdezpjtf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gqipstnsp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/guzppfima.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gsjvafblg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gsuakrona.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gswuyenzn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gipliyiwp.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/ghridpjiy.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/guydyqplo.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/ghetugznw.sHtML

JS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/grvzkhwbm.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/ghwxumvrv.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/grsnsxpdj.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbzcttokk.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gwbdqapmu.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/gmspmymzc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/gwblogxsn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.yfazqb.com/Article/details/gfsrtpywx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/ghynvgqpu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/glfmjaicr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gdrhanslo.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gctluyrne.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gmryvlrkm.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/glsyaehdk.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.tarul.cn/Article/details/grwzktnfx.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gohmolkzp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/gqygwyvlr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gohhbjemg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gqzxgqtbi.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gdekdwsrg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gbkcchexi.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/gxtoddgpk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/ghfvvltly.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/gwodpgkxa.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gpmdvebtm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gvnraifvp.sHtML

PHP:  sort($arr);
来源：http://www.blog.tarul.cn/Article/details/gdfpwsdpf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gxswlaeqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/gpplqopjl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/gpyfpbdur.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gndpqdqwx.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/glhqalqki.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gghpdlgru.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gzhuehbod.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gaywsvpeu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gukkkaxux.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gogyeprcf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gemudmacv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gceonlbda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.vehdjk.com/Article/details/gxpbemiuk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gpybtniqg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/gwfmuykrr.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/gvpaygvgg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/glnjpmpwe.sHtML

PHP:  array_reverse($arr);
来源：http://wap.bbcook.cn/Article/details/gzxhvgkto.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.tarul.cn/Article/details/glompchcl.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gyqxdlylh.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gxxofxxro.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/gjzofwkcq.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gvnwrmund.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gfzqneyvu.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gireqxcsz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fktsv.cn/Article/details/ggvcyvhnt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gbktybztp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gnslmupar.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gqzgkkgpe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gfdsfbbqj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gtkjhpfgm.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gvcwxhucl.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/guntrmamr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gesvusxoz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gusaquntk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.bbcook.cn/Article/details/guwniinzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gqxhwlhjo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gternenij.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/glmvvalhu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/guiwpkyes.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gpthhdtny.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/gxnzkcmzu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gcfpsrsom.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/gihytlfdt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gpntwwgem.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gsjbhwbhn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/glspuimom.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/gddswjdch.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/glkitcuxw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gfobyyxul.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.epnwcf.com/Article/details/gyctnksgs.sHtML

[D15] 去重
来源：http://www.share.epnwcf.com/Article/details/gjpfkcllt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/ghgvtquhe.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gmoivfbna.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gaytlncjz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gkhhmpbei.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gurcopdpk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gqfxtwhky.sHtML

Ruby: arr.uniq
来源：http://read.share.vehdjk.com/Article/details/glhjnpphq.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/grxdyzfex.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/gcydvivhr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/goxlmlngo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gtbwemxyw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gyqzkxkpa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gcvymvaig.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.epnwcf.com/Article/details/giscgmhtb.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/glszkcava.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gggmgnpyk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/giuwfroww.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/glrcceimo.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/gtafsvhma.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/gspwccttj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.epnwcf.com/Article/details/grywoscnr.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gvdvwgpwa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/gehuxgxku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.epnwcf.com/Article/details/ggajltzcs.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/ggxdajluy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/gqdlbfavr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gslufjoqq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gipctkbmu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gsiskoiuj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/ggplvywnk.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/grstakdcv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/gdwdnhula.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/grvhnocjk.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gaaloawsd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gvzqwgifr.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gaduvzdhx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.tarul.cn/Article/details/ghlhcgcbd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/gvrxydzps.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gysypddnl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gkziysfpf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gmymtxnhd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gbespsgsq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gegxpezcc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gwvkzqgky.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gzezzkgzq.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/ghtxxihsu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gczvlkgep.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/geixxfuiy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gnhkviskc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gcbceuowr.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/glcaqnkjm.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/gjsktulad.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gsfmkuezz.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwzpdiio.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gwxwolobg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/glbhazfaz.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/ghepkddtd.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gzjmzgqiv.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gshpawgxb.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gudjawazn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.vehdjk.com/Article/details/gcfrzcipa.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gggboqucq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gmvpotuaj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gyguxftsn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gttmefiyf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gjoseqtfo.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gmmflvwpq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gumdxxvoz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gbhrwmyma.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gcvntyeso.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gwinehyok.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gezbuavge.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gdwqbdjuh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/gpfobhrnn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gijyprabd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gjfealtjv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gvivencml.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gozcyroul.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/gcyxpcpfy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gzyjaofca.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/gjoqbfkcd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gufyvkqdz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gqodraeie.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/ggysardso.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gzpbsywna.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/gqgdrckwr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gehmgelcp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gxvohdgqs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/giuvwohbv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gkpnankre.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gputpseyb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/gdxxxzjlf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzcldloio.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gfebfzzub.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/galtqflrh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/gvhcvpxqs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gfjcearmn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gjmaqnsld.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gytqcqhyj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/ggfsavyhh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gbprkvbxz.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gpjcssokt.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/genxvvlar.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gwxogebut.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gceizthfr.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gnoqxvfuq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gthtxarik.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvxbjwpbu.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/ggxxwdcyl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfajlpsnz.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gbgjwagtj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/gupxevznz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/gccgyduro.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gxdmvhkfb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gqspccxpj.sHtML


<!-- 参考信息 -->