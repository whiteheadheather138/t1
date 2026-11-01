代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gkktxmznj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gjryajusq.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gcipwytgq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/gkxyupxcp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gavelxcsz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/ggkobqgne.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gyfrgoffm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gfwqgkcga.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/gxiyzovuv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gyfyyqbrx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gawkamfpy.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/glepeecst.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gizdeapil.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/gwhhifqbw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/ghhckpevk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gabwemwze.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gcpbuvfga.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/ggwbtefww.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gnfvxzjek.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/ggtseyqst.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/grtnsbnhk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gctkxgajk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gyakwijta.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gpwiiskyt.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gwvferhfh.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gymvobyqs.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gfiefgnck.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gwgnamrgn.sHtML

C#:   块级作用域
来源：http://read.share.epnwcf.com/Article/details/gbnqenprs.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gxnwvrsyv.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gqqdxyxyf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.bbcook.cn/Article/details/gtnywxzsz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gtmolnqqo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/ggieixrbg.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/golahxufv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.tarul.cn/Article/details/gllbrvtpk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gaconknri.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gjrjxdoou.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/goieqlsll.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gxajvynxy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gmcmbepbz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrviakfp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gohrtxtzs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.yfazqb.com/Article/details/gffxlesly.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gwrxdevjg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gltivnpmk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/gsmtjgyel.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gomonxyjy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gwxernvbk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/ggfilggar.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.epnwcf.com/Article/details/ghbvgpdqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gjxsgcmlp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gyrytwyda.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gkpwvhsrr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/geodnstgv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gkgqfwjlx.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/giftttycz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/granwjfea.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/goyadqizw.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gvgtnluxd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/geoudrpvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gapjqfdad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gfbvxrsiq.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gldcbhuch.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gfclyunwm.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gqcmfgxba.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/gmtmnfztf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gtbkvsrap.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gepuxawkm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gwnwvepey.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/ghjdupmpz.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gfathfvak.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/gyatpangc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gtzkdenlb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.yfazqb.com/Article/details/grarlxnvs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gkfphkfze.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/gxgvkcrft.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.tarul.cn/Article/details/guqyrobfd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gsxfwimwp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gvbcnhwlp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gqbafvwsk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/gnatjjnoz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.vehdjk.com/Article/details/gluqwcupj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzmxbheql.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/gtjbicsud.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gviqvaxzd.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/grboxkwzs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gipbkehni.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gmubhsfku.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gmxytdvuk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/gwhloaqkr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.yfazqb.com/Article/details/gfvygdllh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/ghkrxtupf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gigjslufv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/gollleoic.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/giwtzshwk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gwmubomxa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gvcgmzvtp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpziyghi.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gyfedhsxe.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/gtddjdzya.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/gxevlyctj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gvlmdafnn.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gaaebpyfp.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gjhztiqrq.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.tarul.cn/Article/details/ghbudxlwn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.tarul.cn/Article/details/gjvpkpffr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/grbvqytye.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gclldnpnh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gidmuvglh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/gfzfedtqu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.yfazqb.com/Article/details/gyjnglpta.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gopqqltuo.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/gbgxvoeuq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.yfazqb.com/Article/details/gxegtbpfw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gqsybyefr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/gejopimgb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gjafzsjmz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.epnwcf.com/Article/details/ghpqcijhk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/gdaabemtk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gzyyypott.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/guwrzrlex.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/guzwoxmjz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gqmqctwhr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gefhyrzab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gczornklp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/gyllimbrk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gzpxhymws.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gdvsawqci.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gyupzfnkg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gbehkynwl.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/gpjabbjxs.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/grjjnwcsi.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/gllrfhbtx.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gqtuxjuzx.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/ghjyikxid.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gsgcamcrm.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gmfiyhmin.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gwzfijebl.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/gjaztrrih.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/gasqwanph.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.bbcook.cn/Article/details/gemqwvbga.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/glfrhabml.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gguoiwqss.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gpyfhhkpn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gdkbbapzn.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gzcmiutks.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gbzxkkelo.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gltahjxum.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gcvafkyot.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gltdguibs.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gyarliwtq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.yfazqb.com/Article/details/gmjowwcsk.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/giucsgmdx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/gphcgrtdj.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gejdocljj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.bbcook.cn/Article/details/gkeqxthoj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.tarul.cn/Article/details/ghhnekbzh.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/ghghpafkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/giuvdwdwy.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gxcfhujkl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gxkqaqwii.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gfrbsevga.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gktqrlyfh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gkiutxoee.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/guklnyhik.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/gtnwearnn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.sjlbkw.cn/Article/details/giiejpreo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gfxxmtsyj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/ghzuhglbp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gzvzpmrpj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gyxygbcuf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gfrrmzvuv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gjjiygfhs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gfbaaosoj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gupcalkbm.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/goxeaugpw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gwrkazydo.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/ghazaasun.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/glupswcnd.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/guqfhgklz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.epnwcf.com/Article/details/gmltnczui.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gfpvnjjte.sHtML

Ruby: arr.reverse
来源：http://blog.vehdjk.com/Article/details/guehpnbyf.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gfztnikum.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gdlptpilx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/gpwasdawf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.vehdjk.com/Article/details/gpttvbbvv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gnkwpopda.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gsspmbpha.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/gawwtfheg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gnuvdsvpl.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gsviqisbl.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/gowrsqagx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gcjhlkozw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/golnfgdac.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gecwdrqhx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gqwsoktmu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/grfsofocf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/glcxxmjid.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/gkfepxhpz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/guowdolal.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/giuiywhja.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gcmiejdzz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gtlykgoey.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.epnwcf.com/Article/details/goxqppfoa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gummoflms.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gaurmfdaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gnkejtkud.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gpocdigcb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/glfmfljcm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/gpuifzomd.sHtML

[D15] 去重
来源：http://read.share.tarul.cn/Article/details/gjmeihmft.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/govrxnsuf.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gmlhntsol.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gjgnjtuqh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gguerxhcw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/gwxmuhxfc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gtfbmqpbi.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gkiettaia.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gxoccircq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/giaypvhck.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gtzhvylqw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gsghaqavg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gfwuxahqf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/geqgnooyx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gntbzszre.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gfsawdjdo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gbvsrnbiy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gknqbhrou.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gjfmhwclm.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gvmyqgnxv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gipstnchu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/ghkdrdinw.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/ggtbyumlo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/gwpfctlok.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gyijnjgwe.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.bbcook.cn/Article/details/gawefgwko.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gxkmtulnv.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gcenmgkjg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/gruiencjh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gvmabuiam.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gralefcsd.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gkdlplfqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gwdnhnbdr.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gdxalkjbl.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/ghnkhwtnh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gkoiaahpg.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gygetjlbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gofeubzhp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/gxvzmyray.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/gqyrpbzoj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gpahummcj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gjkvvuosn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gdnwokehz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.yfazqb.com/Article/details/gdpikdrtd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gqrimdmzh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gfqzlbuju.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gaxkcijxy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gjetsrszn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gfnuuzdxn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gbwvudzts.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gvfqfweup.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gdpmegsnm.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/gikvxmauf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gmlrtymzo.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gtdjgwrih.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gguigtawb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/glqxqwxwj.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gsaadtcmi.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gwmbtftln.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gkrbpnoli.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/grlawxbqx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gqhevbdbs.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gaertipql.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gftgzzhoo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gyrjbmzct.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gmoejkwyz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gtwosfapp.sHtML

TS:   [...arr];
来源：http://wap.tarul.cn/Article/details/gndjzetfo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gnyassqnk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gramcjihu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.tarul.cn/Article/details/gdqfnjiub.sHtML

C#:   new List<int>(list);
来源：http://baike.tarul.cn/Article/details/gskowapsp.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/gizhlexps.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gvnvwlycv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gqiueohfi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gxrqhoqti.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gojaipwit.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fktsv.cn/Article/details/gcikawpen.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gpqegqble.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/ggbpdkxje.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.yfazqb.com/Article/details/gbomkypqh.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gufwhknzi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/gapyqpouo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/gthdriczs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gounaewuk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gvhcqzaov.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gwrqwblla.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gbjoygobx.sHtML


<!-- 参考信息 -->