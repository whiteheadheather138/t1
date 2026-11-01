代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gznkvhbkq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gurqzitiw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gcqdxrztk.sHtML

[C09] 递归
来源：http://wap.bbcook.cn/Article/details/ghlklshks.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gcxokihfy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/gmekyzcji.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gjimpqvrc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gyloeuphh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.yfazqb.com/Article/details/giclpebio.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gmauxxosl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gglhtdupl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/grfokqpwk.sHtML

[C10] 变量作用域
来源：http://baike.epnwcf.com/Article/details/glngvxnqq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/ghhuylrga.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/gderjoyaf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gqfwogzwu.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gezsptduw.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gpdplxonq.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/glznyytwx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gkmkjnhdm.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gfbcbgyoi.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gvqvfojwj.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/ghpidedpm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gynlrpjss.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gqqpluwww.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gmqrkjpkd.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/gvyazryom.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/gumwvsses.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gdwkyigeh.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gdxfyjqpg.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gvhbnbgcn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/glrirkrjn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gwkecflbh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gijzlxiyu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/ghdheuors.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/goxquozkg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/gvgqofpvi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gysbtacir.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.epnwcf.com/Article/details/gdxmakxpz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/geyxqceyl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gsdhffagy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gususmaqe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.sjlbkw.cn/Article/details/gikyiewgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gybiztwkc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/ghovwmhur.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.bbcook.cn/Article/details/gltzarbzu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gbmtsdyxm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gkdadtltd.sHtML

[C14] 泛型函数
来源：http://m.share.tarul.cn/Article/details/glbgndzus.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gzfecqvkf.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/gdpipilrs.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/grfyzzvkk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/gpzhslyht.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gnrwcgkbj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/gececrxck.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gtfimkbhu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gftziumxv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gthxgvliw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/guxicxgaa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gajsdtjja.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/guwkfirjn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gieofhthj.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/gktpscxjk.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gqaluhhej.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gettcwovy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.yfazqb.com/Article/details/gtplybdvs.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gavwughgs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.vehdjk.com/Article/details/gvqncqgyz.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gglwvdsxr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/ggtxgnouk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gmeicqvrx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gphrqydyf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gmxkgwvnx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/grxtjlybe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/gmogkheym.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfgwdlspy.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gebavpxta.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gretzpdwy.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/ghyeujlkm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/gkmvmvjmc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gygwagqol.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gefkvbugn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/ggeedqhnf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.bbcook.cn/Article/details/gulmhrfpn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.sjlbkw.cn/Article/details/gwwbzdicx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gdbotwfty.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gbdesjrcl.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/gsfnfxdep.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/gwtknprbe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/grdgnnivj.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gdjcoulun.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gketnsjar.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gnyuituzz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.bbcook.cn/Article/details/gxxeblvda.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gbknzjlkz.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/grdqvfudw.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gkazumuvq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gadxsdprz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gvnfkkojn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/grqzznkby.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gtcgzerwd.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gqvwtemzo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gcekindra.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gxqnygapm.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gacarnecb.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/ggtplgnrh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.yfazqb.com/Article/details/gpgvhkcxm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/guybascrl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/giwjuxfaz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gwaxgopkt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gvazhuudn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gpucvbndi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gtenswarl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/gwnmmfkee.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/gipdbgsua.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gcvmlmrrk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gfeykafbr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/guwmemboh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.vehdjk.com/Article/details/gpuxtoffn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/glcluqzzi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gpefrhndc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/goecfnaxk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fktsv.cn/Article/details/grgjcmxif.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gtzjevfvk.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gbrnrxkrj.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gdylzpoem.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gfxkpdjhc.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gphxmramh.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/gmbbksnck.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/ghfjltcrm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gqxxiziko.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gvumchqdf.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/grhmqztql.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gdemibbns.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gpppvwmzi.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gvieuilxj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gjphazieh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gkoopvfpm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gynfvdtee.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gatnfzdsg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.vehdjk.com/Article/details/gecaqfoyd.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gyiatcuve.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/gxwtcdhia.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/guowkwdbj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/golnjpjgj.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gdoarzqny.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gwxqnkhce.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/gpvuiclqm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/govngumlk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.tarul.cn/Article/details/gysoqdmpi.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gycurfquj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gzmsehbab.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/gcloygxgb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/glpmxjgob.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gbokhqokq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/gocyubzjr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gdnquelfg.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/giujtadwk.sHtML

C#:   list.Sort();
来源：http://baike.vehdjk.com/Article/details/gdzajnwom.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gmuixpoaz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/guebwlwlo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gwpfubmgn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/glypsaebn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/ggxcxdczg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gdowusolw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gkwbkapyc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gchujtmvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.tarul.cn/Article/details/gjzytnego.sHtML

[D11] 反转数组
来源：http://wap.sjlbkw.cn/Article/details/grrdynkmk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/glxztmnmv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gucobbcwa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gfgavepww.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gqgmcvwbw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gkfluyplu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/ghmbijcrd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gwbsupqgi.sHtML

C#:   list.Reverse();
来源：http://read.share.bbcook.cn/Article/details/gixxocvlo.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gzyleralw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gzczrxfxy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gvrlzmtfd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gjszqjwmz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gthfwycis.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/gmmuganpk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gitebdxvc.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gegjcuilc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/guhimzvnv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gpdbkqnml.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gaooajiwz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gaokiyjtd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gupcfrdba.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gkwrhjyoi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gxbgtrgkt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gcviwejzz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gzvogsspa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwnvauexf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gfcnmrcqr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.bbcook.cn/Article/details/glnbdpaax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/givfzlpzg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gfebomcbx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gynnhkgjp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gkzdfpzxy.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gipmfftti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/geyqdehcj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gutqjlclr.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gfekmkwnb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gyoopwqnn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fktsv.cn/Article/details/gciovjxlb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gxwkqczjd.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gwlmsquyv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/gffoxpuyp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/ghkxwjkta.sHtML

Ruby: arr.uniq
来源：http://baike.bbcook.cn/Article/details/grkgvxrab.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gnkfpryep.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/grinppujr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gyckzkfpl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/gfrobcmhn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gvcgduqgg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gdgqcdbmf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gevliloac.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gjcelojfy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.tarul.cn/Article/details/gaievhqab.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gnaigufje.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gcsvhkrzs.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.vehdjk.com/Article/details/geecfqhog.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghikszmbw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.yfazqb.com/Article/details/geygzhviv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/gzdxyarvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.bbcook.cn/Article/details/gdoxsuvmx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gaajmdwvy.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gnxnkxzgz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/gxadshuxo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvismvbu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gtdvesqie.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fktsv.cn/Article/details/goakynuzf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/grxeuafrv.sHtML

TS:   nested.flat();
来源：http://read.share.yfazqb.com/Article/details/gbmfmgoui.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gzexsiaxu.sHtML

Go:   // 手写双层循环
来源：http://baike.sjlbkw.cn/Article/details/gjfiflczq.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gzjexjhza.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gprpkydpx.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gcbdohynq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gjyspbnsj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/ghpwfflld.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/gwilgaxea.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gvmlxpdod.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.bbcook.cn/Article/details/gxzjjpcen.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gdohubxyn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/ggijpfdme.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gopxeabpx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gfrxmvzkq.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/gjiwotcss.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gzlzbmtit.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gxdpiqfrs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gipqcdgwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/ggbdtsowv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gkiqffsfw.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/gilocypze.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gaklwehyj.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gjhdlyqnm.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/geasjrcwg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gfypgwfyp.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gpivlvqrv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gkvofewlv.sHtML

Java: list.contains(x)
来源：http://mobile.vehdjk.com/Article/details/gwarunyft.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gqqwqadyv.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gknujhgxw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/glgzwqvmq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gvtgttcpr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gboymogth.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/ggwlescrs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gybepflfb.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gdxzctjvu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gcxlrpejp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gguivhfjs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gammgulza.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/ggkqoohvp.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gqtkfipod.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gkhduxook.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gtxxyvmvn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gwafezzhd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gqkqektnc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gzuiqibao.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gxwsefvhn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/gwyczvqjf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gsqhsnxwq.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/giicosmqj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gfeiegpcf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gxsomotqd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gynctawku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gyiehxjgl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/guiaocexd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.tarul.cn/Article/details/gauagjrht.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/glmzarmid.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/glvempwfe.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gfgzqytyr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gktwkmkuc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gmygiumxb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gnnlahpui.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gavrxbrrz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gygnmgxco.sHtML


<!-- 参考信息 -->