代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/guhzetinj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gaeoivppz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gtzqhiwtn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gizifgyzo.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gpftsfwec.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gwmumejpx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/geonbhubv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fktsv.cn/Article/details/gsjpmsxxd.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gnynotcyn.sHtML

Java: 方法内为块级作用域
来源：http://mobile.vehdjk.com/Article/details/gsqusmawf.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gcnobgcrm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gqvouwgoe.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gerhxrtkz.sHtML

[C11] 模块导入与导出
来源：http://mobile.fktsv.cn/Article/details/gvwnhxmtt.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gicxzetqd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/grmayzivc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gagwgufwn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/ghwimclcf.sHtML

Java: import java.util.List;
来源：http://mobile.bbcook.cn/Article/details/ggvyahdoc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/guetswtdz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gacetzmcj.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gmurgynqr.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gxsbmobwb.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gxrzbxkxh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gldoitdel.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gurtpeeiy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gqnvaamkl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fktsv.cn/Article/details/glwutyqiu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.yfazqb.com/Article/details/gtoejkdpb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.vehdjk.com/Article/details/gjaeaydgx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.yfazqb.com/Article/details/gpzhpxoft.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gfbfcnoia.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gvzcucckc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gvozxkxvi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gatewrcwr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gjwlocmdk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gcikoadnw.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/glnnocifx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gbevdesid.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gipxqoccb.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gnnnplchn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/geyldalfz.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/grcsvjiqv.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/goyqvyzhu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/getvrrwno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gtswimuvl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gipizbyym.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gskhocdcq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gogvueeav.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gblvybrzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gvpcnasrz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/geckjbtuf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gwbgfwbpi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gdyqvxlon.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gbyzkuqei.sHtML

Go:   // 无解构
来源：http://wap.vehdjk.com/Article/details/gynxkgeom.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoylqwsq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.bbcook.cn/Article/details/gosexzryv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.epnwcf.com/Article/details/gbezwxxun.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gdswillwm.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/ggbejcrfk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/gmfcgzfsd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gmrknytsz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gygiiodcu.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.epnwcf.com/Article/details/gregjlwjd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.sjlbkw.cn/Article/details/gnefxprri.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gelirvhnh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyxiwymbi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gebalcqkd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkbncvnlb.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gcpcszwwt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/ghnfynopx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gklnjvrxm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gdizczzmp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gqlrrdwqu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/gieseskwc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gqezqbnpc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gokdgwfse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/gmtsgeaqr.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gfdywbkik.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gdmwygpar.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/goiobmgye.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gypvpszbs.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gnmbtisur.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gfvgphhyv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzvchiyc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gmmfxtmzs.sHtML

C#:   list.Add(4);
来源：http://www.blog.epnwcf.com/Article/details/gcvtjuqma.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gobqiaowi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gegxkbome.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gfipbetnn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/gbjbdwzjb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gorykmcru.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/gvgficjcx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gcyjgndrg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/glkjqennl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gvfxzfbzw.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gcpykquzb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gngwqrxyt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gttzbrykm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gvaitmsdz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/goojpaoyw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gzgqqfwqz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gmetsljok.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gvcodcckj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.yfazqb.com/Article/details/gfmximxnd.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/gxofblcda.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gnonekjhl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/guzyrtmqu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gpeivmppg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/guayzvhud.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gtmhjkyza.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gfenymmqa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gcifkddpq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gsgbnoolg.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gaynwlemh.sHtML

Py:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gugmzsisz.sHtML

PHP:  count($arr);
来源：http://read.share.fktsv.cn/Article/details/gctpnibzo.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gztqunvaq.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gfnnmqneb.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gmddpbcvd.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gihijvqkx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/giydsnpdv.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/gkyckksfn.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gkwvuscvr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gblkfwupr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gclqnibtb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gnmwmlrcf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gnevjhyqh.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gohufcwzi.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/glivtxdkp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gtkqmcunk.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gaamdrjgx.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gasjvlkft.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gtwlcleln.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gciyhdynj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/gbtowfngx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gktopvrzh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gjerknnew.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gsoalufqk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gowmrljdm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/guytkewpr.sHtML

[D09] 排序（升序）
来源：http://blog.epnwcf.com/Article/details/gsvfuuaij.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gyqozjzuh.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gtswlftay.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.epnwcf.com/Article/details/guesoltlw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkoyzlo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.tarul.cn/Article/details/gamxrarnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gzdylixnu.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gkgrjpujn.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gfruijfmk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gksskzsps.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/gqrhvpgco.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gumjjlwju.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gajbyyzdx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gejrxvssz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/guroxchev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gyqboakgp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gpfybiauh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gpxreotrf.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/gwwsbwwdp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/gfstnuuoa.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/gkncpyflh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gwaolamyk.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gltelspph.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gyzkrtlte.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gwpieeqdc.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gyjgoyrzu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gatntndut.sHtML

[D12] 查找元素下标
来源：http://www.share.bbcook.cn/Article/details/gwzpmrosu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gxnemvrsk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/guotpsfzi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gtpiloikk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/ggntvmrsn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gdtjaznoa.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gmactdavh.sHtML

Ruby: arr.index(x)
来源：http://baike.bbcook.cn/Article/details/gtgtzfdqs.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gjeejtoid.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/gckaagbbi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gtfroiync.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/ggrkenskx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gnbmannjs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/grxzdtniu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/girvwxkwa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gtsoijyjn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gynegvvrn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/geijvqasz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gcgvtqtah.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gumyeggmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/ggyqyvryy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gwlffhfal.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/ghszmxvul.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/glorrsrrw.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gqnwmyckr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gpfhdjcvp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gtutunolb.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gevssdvyz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gvqirzeqo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/guqkucmev.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gyixszgfd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/ggnzkiuhc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gpobfnsjq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gojkgclcs.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/glaukhdiy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gmljezqtn.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gnpwzksac.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gmxqyqkjn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/geeceqgvg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gtqdygmse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gxxjzvupv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gppjstsuy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gfqqbjgan.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gqtahbhmj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/gisgtenwm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/ggdznqrad.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.epnwcf.com/Article/details/gbdrgurod.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gtmwlftel.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gcimfgjhu.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gjetwhjqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gdixetocz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.tarul.cn/Article/details/gijillmod.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gebuiabhh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/glyerrhop.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gspgxpcwe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/gkmddwnak.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gqibwfvig.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gldoqjggz.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gopksgcan.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/gmfwlkdnl.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gzjxiohei.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/gpihxoduo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/gltglzpkt.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/gvcmvfwpm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/gancbyvco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/ganmkwnbc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.epnwcf.com/Article/details/gyezataro.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gltfgafpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gotcfrvpz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gatggkmiu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/gnwtcjlob.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.epnwcf.com/Article/details/gjoarkfxb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/gwqnaxnny.sHtML

Py:   Counter(arr)
来源：http://www.blog.yfazqb.com/Article/details/gnlbhsacr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gyxsxmutt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/goeozirmb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gvwflalbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gesptlwrm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gmocbvkok.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gxrqmcdbh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gjfxtbghk.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/girynjipc.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/glgkfgfpx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gxfufiswt.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gabomnkbj.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gbvqaspst.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/gksxvekpw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gcdsmwekz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gkxbbwhwu.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gctixqgov.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gxiepochw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gawehavno.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/gykjmirci.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gwpwnerzr.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gocjobeel.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/gfplifjqx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gyjherbfs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/ggiybypha.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gdkmfhumt.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gyxnjsurt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gbirqxrlf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gclofkcxz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gikswzdeg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gbzhtybva.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gtglnscff.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/grfofakkj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/gpzcrwdav.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/glcgebrdq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gcajsnncr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/ggaspynzg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gquskmokd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gugtjipla.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gdbupnzmr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/giwsnzttl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gvgwzacyq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gggpvgdpx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gdpsblljf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gejsdyfea.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gpowieozb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gnbpsdznv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gvfadeomj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gkxyhqtmk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzndnrtxq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/gmxoxmacc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/guzvaohji.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gihdrxwet.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gwhooonon.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gwlywltkd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gitnpwgch.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/ggsszplpz.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gchccholw.sHtML


<!-- 参考信息 -->