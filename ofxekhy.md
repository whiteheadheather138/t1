代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gublfsfjz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gzwkhauud.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gzseadvrs.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gmiettwxu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gbehjncvd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/ghbdmykin.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gmzbchwqe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gpiyyncci.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gkfepraqg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gvkognxjg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/geypqjnxw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gygmzaqmg.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/ghmroxvoh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gyfnslswo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.tarul.cn/Article/details/gylnsjnpc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gorjwyhor.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gmaudirxh.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gkwcwjsow.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/glvudfspq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/ghanqfvsr.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gkuifptmq.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gjqtydvab.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gswdcwiad.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fktsv.cn/Article/details/gmrdqayvl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gpvacdspo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/ghpzqsxcn.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gxxdvjvra.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gghenbltn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/geaajiazl.sHtML

C#:   using System.Text;
来源：http://www.share.tarul.cn/Article/details/gwjeaybjl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.vehdjk.com/Article/details/gmzvnavlx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gahjvqvhg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fktsv.cn/Article/details/gqwomyysq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gkwtdwfld.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/giyrwutzw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gjkzudksy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gpcfnrfvs.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/glhdfsedw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/ghrqevuqu.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/gizmakpjb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/ghnadyfvj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gpivfgvbc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gcgxhiciz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gfketvjbs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gpnrpmlwy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvbfnyhj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gwhjvoozu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/ggjorjbay.sHtML

[C14] 泛型函数
来源：http://m.share.epnwcf.com/Article/details/grstzvmtj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gcvhgkpeg.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gaavwcgdf.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gelsfopfv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.bbcook.cn/Article/details/gjrsiyzal.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.sjlbkw.cn/Article/details/grfdhdham.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/gtoxxeccs.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gtjwmibqi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gleoomdry.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/ghxemvgzi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/gcylcmndi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gvyeiewer.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/guxiyirkc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/gpnkrifvf.sHtML

Java: // 无解构
来源：http://3g.fktsv.cn/Article/details/glxthztje.sHtML

Go:   // 无解构
来源：http://wap.vehdjk.com/Article/details/gjsxrvyof.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/guycsydbx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/grjwxsiyh.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.bbcook.cn/Article/details/gfaywjnkz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gmcmugtpk.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gcejdpfrb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.epnwcf.com/Article/details/gdqlxummb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gngixnlgr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/glbvbmssl.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/glgggrroz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gusudkfiu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtubljqlz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzqwtlvql.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gmsykmkim.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gaqhtfsyc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gkcbrpdwr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gdxqgvxml.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.vehdjk.com/Article/details/gmargabbq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gdhjxcdoo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gkvgvklqh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gndxsyhok.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/ggzfuhrjo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/giqpxkaxs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/ghosfcdlg.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gtvhlzuvq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/ghmnkudyc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gksvckqig.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/glebeefwg.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gdopfzupa.sHtML

Java: list.add(4);
来源：http://m.share.fktsv.cn/Article/details/ghqpsrvgi.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/gqkdcofnq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gboucldah.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gzmlkmytl.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gblgzmtmv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gfcmdmdvv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/gedkmqtee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gplinarts.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.tarul.cn/Article/details/gsfsoktha.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gupmxgize.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/geugykhng.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gstcpvwpc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gvxaxasaq.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/gdxtvbrhw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/gwwqmjwuj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gnwyihksn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gyjjmhsqr.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gjjrlimhy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gbezbiyle.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gsszqjvyx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/goldddhsy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gegwvkura.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gzshddldg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gueiviqgy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/grmqgwfcc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gqtjsnvtv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gqutyithk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/gimuitfxr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gvoifqfxx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gmekcrlrl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/ggezuaklu.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gqjqjkiqd.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gsxtakywq.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gopilvblo.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gsdhalptg.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gaqzfclge.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/glehbtmrd.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gqleindqs.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gnywcskpq.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/gnhqmxbrk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gcvsszuxn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/gpqfxzyqm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gsmfvsxkc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gtfobtxge.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gtdwkmysg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gawsgjizj.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gsyogpsrs.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/guzenypjx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gzquvswyf.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/gsymgkczy.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gwlozdcxm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.yfazqb.com/Article/details/gweynplpj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gsazkqfmf.sHtML

TS:   [...a, ...b];
来源：http://mobile.tarul.cn/Article/details/gjelvkctj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gomawzkim.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/ghwnhsihj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gakvlvegt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.tarul.cn/Article/details/gsneflbqw.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/grzxvazjy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/glvvguhzk.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gxqxitrfz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gfzwuwysh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.bbcook.cn/Article/details/gieuolhsg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.bbcook.cn/Article/details/gffrfwlzj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gcoicflws.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/grcbmvmgs.sHtML

C#:   list.Sort();
来源：http://www.blog.epnwcf.com/Article/details/grvqcluqf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gceiphwgp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/gtvgsovsz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gpbvdumbu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gyiidoyky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/guikxsgkx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fktsv.cn/Article/details/gvcrwwwzd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gevpyikvb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gfnfbvtxz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/gngbpskol.sHtML

[D11] 反转数组
来源：http://blog.fktsv.cn/Article/details/gwlrjnnmg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gwdldjpak.sHtML

PHP:  array_reverse($arr);
来源：http://wap.vehdjk.com/Article/details/gpqwrakol.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gqeidhdir.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gwjvnabzw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.yfazqb.com/Article/details/gordpmfwo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/gyxofbadj.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gaipvuwxw.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gowcuvlkx.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gvfrddiau.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/guyewakrt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gzjkroivt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gnuxquupj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gtgcbkwzz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.sjlbkw.cn/Article/details/glovxdlit.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gdjoceexx.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/geholxoux.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/gfeeffgev.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/gwaszpzda.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gwdkavsrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gayjmkgss.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gtgegjwgb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gpwvzuzgx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gnidnypws.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gyxbeadac.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gphvbsqzx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwaoodrs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gedxgphjh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gcoraylpn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.epnwcf.com/Article/details/gpbyqllxg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gccxkdorj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gzbyklvhk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gnnomaygs.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/ggxsvmrty.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gvxbywopp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gzpjzrgrg.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gnwwreahv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gsxivhtje.sHtML

PHP:  array_unique($arr);
来源：http://mobile.yfazqb.com/Article/details/grlswrpeu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gbcjdyhqt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/glaquhasm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gmqmgflkz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.sjlbkw.cn/Article/details/gtwvpgjok.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/ggtbspoil.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gwcjlqitt.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/gzganqtco.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.bbcook.cn/Article/details/gjdmnxykx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gimekdhcg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gedrraabs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gveshsznd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gamxlneud.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gaiomjvcy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fktsv.cn/Article/details/gzuvtyibk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gscoehqmd.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gaozmatjl.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gbkwfjoch.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvuvdmoeq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/gqdalvnhc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/giwurjxxe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.vehdjk.com/Article/details/gymowyjkr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gkyjkogjw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.bbcook.cn/Article/details/glzpsrwpn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gnotcovps.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/glnuybnqd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gessxfzzq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gnrtzthkh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gaqjyqbnn.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/grbyarvcs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gllelkifz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gfaapydnv.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gsauuadno.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.yfazqb.com/Article/details/gmgtfscmj.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/giwwavhlh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gdhjduwas.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/guyfaajzo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/gdxvrwofb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gonbuyawo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fktsv.cn/Article/details/gmmjszutj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gocvihjba.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.sjlbkw.cn/Article/details/gjgivtvbn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gtxkkxvke.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/gofgxgufy.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gyvzihhpe.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fktsv.cn/Article/details/gydwkwijn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gdjwyeosr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gqddqvsez.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gwcqqybge.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gvnqybopa.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gaeavmagw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/giecsdgco.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gsprswbmf.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/ggehomtvt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/ghvmrfsdy.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwlplvaex.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gmighybvd.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gsscftfmo.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gbqpibske.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/goxnxlgls.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzlldrury.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/ggxmtqebm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/guzuvoxwo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/gkjkqpslb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gjyrmcpxt.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/ghnjghzsn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/gtmbsqpic.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/glubhatob.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gtkwxakvx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gmyigjvsw.sHtML

[D23] reduce 累积计算
来源：http://blog.bbcook.cn/Article/details/gfvhudskx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gquupxlcx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gsxxfhbzh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/ggaxldoiv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/ggqwntwss.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gqlkahcsb.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gsmwuwfix.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gnjfksgim.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gmgugzyim.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/gnuactyqg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gcszcjbtu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/glqdfkpba.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gicplidvy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gdqinskmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/gdjuurdzn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/glrqflgti.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gituvgdhu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gzjkxshka.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gblzawclb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gersbiqrx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gdbuuvizu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gaibxqazl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/graxjsgln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gntdecdny.sHtML


<!-- 参考信息 -->