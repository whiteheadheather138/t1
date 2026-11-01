代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/gvbikmpbz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gzbrugxbw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gjiassvrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.bbcook.cn/Article/details/gsvqtfbec.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gsepitoyg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gvvhbucxa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gqrvmakij.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/ghwpsnufs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gaghqavfe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gjrqdlvsv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gebrqapsw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gojpmichk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gtdwhdnpe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gosgofydy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gxtjhkbqb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gssmlyzxq.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gbglexjdh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gjcztvzcf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/ggcxlqxgz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/gjepviljp.sHtML

TS:   同 JS
来源：http://wap.vehdjk.com/Article/details/garlfglrb.sHtML

Java: 方法内为块级作用域
来源：http://baike.vehdjk.com/Article/details/gepugndxx.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gefceqwxa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/gzveyzlqt.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/gzztvnwlg.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gmlksawje.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gwveabqgn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fktsv.cn/Article/details/glztohaab.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gelkusisq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/gbnxoucjn.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/grsjnjrar.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gegnblfgq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/gmzynxpxi.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gdaksbxpj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gsufcrokz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/gxmdzhlsl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gikmjcvfc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/grmwirjmc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/golfiknyi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gmzstrsvl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gpztpapks.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.tarul.cn/Article/details/gwwpqcakd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/guwftxahi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gchdlifer.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/gchzgthte.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gpismuwlg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.epnwcf.com/Article/details/gcxhdgtdq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ghladguxz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gfssxlrgn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gbpyccwmt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/gxdsqwjbp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gfvjvifci.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gvgpvxzij.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gjmjfkrjz.sHtML

PHP:  // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gzqyelrfi.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/gzfrtbjtk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.tarul.cn/Article/details/gbpzqkxwr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.yfazqb.com/Article/details/gcxynuhzk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/gxkekohfb.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/glttyztzk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/gqeszsfst.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/geiyeltru.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gneopevbr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/geklfcyzu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gxstvxrle.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gyvxxwfwf.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/gmvldrmcw.sHtML

Go:   // 无解构
来源：http://read.share.yfazqb.com/Article/details/gmmdxthik.sHtML

Ruby: a, b = pair
来源：http://www.m.share.tarul.cn/Article/details/ggnpmkvqz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/glgmfllzc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gckpbeuly.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gxqggniek.sHtML

PHP:  // 无重载
来源：http://www.m.share.epnwcf.com/Article/details/gokwhjiyo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gqvpmhlvc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.vehdjk.com/Article/details/gleywnmeg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gdvmrztpj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gcdkgtdel.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gbvcnymbl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gislhpzbh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnmfbsqof.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/grjhhitzl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkswshdoi.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gqfcxtwwq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/gzxtsmhkz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gzxtfmbxb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gftphjjzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gjtuyzhqn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/gctbbjygs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gslqyjkyu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gtnltqhkq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gjvladaje.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/gzufzodpj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gwjfnujfv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gcasrodgp.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gkmcjxucz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gyebdsylv.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/gibhxomba.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gdncsfwnd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.vehdjk.com/Article/details/gkhwufpnz.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/gioefzgfd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gupvykyef.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.tarul.cn/Article/details/gtxnvnvzf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gmgwabcma.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/ggotwsmlm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/gibzrbbrb.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gsgjhrcuh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gkdiudtwc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gyzyogkqg.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fktsv.cn/Article/details/gybhiufcy.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gltatevnm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/gbwoujxqz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gpzybuekr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/geomdzjfd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gohnsucmt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/gnjhodbqt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gmznaqcep.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gisdwzyxu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.sjlbkw.cn/Article/details/gdmeimbrh.sHtML

[D05] 访问与修改元素
来源：http://wap.bbcook.cn/Article/details/gjtzlhadd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gvljjtmmi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gjjvdewft.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gcljpillx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/gmvpjxmmt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gqyedflrc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/glbquykdb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gjjjifwis.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/ggacxtbpx.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gboprgeuf.sHtML

Py:   len(arr)
来源：http://3g.bbcook.cn/Article/details/glifhmfzv.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gfgtrijfx.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gxcdxutmz.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gixsgjrzr.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gttmylvne.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gmdvabhkd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/goxhrlwvh.sHtML

C#:   list.Count;
来源：http://m.share.sjlbkw.cn/Article/details/guvqubhsn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gdwqlyrlz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/gxkqqmldw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gapoyknhe.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gsrgiymas.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gmajkfuld.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gnhplcgig.sHtML

Go:   arr[1:4]
来源：http://mobile.tarul.cn/Article/details/gokioeooj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/grbuktmpt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gojoxrwey.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gtrtvqnsd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/gpoujmmfc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.bbcook.cn/Article/details/gtdublgrx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/gblzvzzpd.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkdinwvf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gkxzeqolm.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/gidbqzfev.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gahxyzdpg.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.vehdjk.com/Article/details/gqiienzdh.sHtML

[D09] 排序（升序）
来源：http://read.share.sjlbkw.cn/Article/details/gcnjjkioh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/ghhzgkadm.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gzgkrdnwl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gxoaxtdvj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/glcauzsxk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gesxvcqbl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gpwhquwed.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/grmctghlh.sHtML

C#:   list.Sort();
来源：http://blog.tarul.cn/Article/details/gahrzecha.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gxnmcsicb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gcdkafyjd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/guesnvisn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gbgomcsco.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gquhkyqpb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/grtqpuhkp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/glumtbzbk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.bbcook.cn/Article/details/gnlptjmgs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gjbyiysuq.sHtML

[D11] 反转数组
来源：http://3g.tarul.cn/Article/details/godzzrgpz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggagwhvbr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gycvsmgui.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gntbfiiuh.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/guvwpqobm.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gkivudvxc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gunvyppva.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gwxykmibw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gqxutnudr.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gizglsknd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/gvpktiubn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/girrgzpch.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gjctsbqhm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gapbdvjsx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.bbcook.cn/Article/details/gekrwgmvn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gsjiekkdk.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gczwsjkbl.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/gkwirwnno.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gmtkwsqls.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gettnrstr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gpsqgaqyr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gmmdivjcc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gppgjxyer.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghiasfpbx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.bbcook.cn/Article/details/gqcszqmtp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/grksjtvlq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gsrjkuwhe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fktsv.cn/Article/details/gsjoecgln.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gvuudnokn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/ghdrtufwi.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gjnlxumdd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gozruqrov.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gxdutyncn.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gisodvtbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/guulfwkgf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gnpvlsibp.sHtML

[D15] 去重
来源：http://wap.tarul.cn/Article/details/gvyjenlax.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gzxhnpuzh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gbrwhptco.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gessnmjgk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gtdkyzuca.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gguleyvti.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fktsv.cn/Article/details/gmxdvzqky.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gmkonuyoy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/ghlsbexwu.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/gonpgqxjy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gxsilzwoo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/gzhvufmld.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/ggonngrxh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/glmhwgozs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/gciofjfba.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gzsusupgk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gmacqfukp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/gtnxsbqnm.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gmspxmvxy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzlmudnkp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gpeellozr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/gdrwghovx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gdydlzdzh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gqbibgfjn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gzhpdbmwy.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gvjbwqwte.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gpvixnlfo.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gmgiveawa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gzygigjhy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.vehdjk.com/Article/details/gnnydflpq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gikayyqwk.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gvtsuzmul.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gtlclrlmb.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gnuefmyal.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gilbovjds.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gfkgzcgwb.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/galvuxygu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.yfazqb.com/Article/details/gkdwoinhc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gmpmgzwfj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gexxjzrly.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/ganpypjqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gyejjlzsx.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gcxkdbrrx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/gdmpujfhc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/gzgipdqvp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gxuljnfsb.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gqkzfrbdm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/gtpytgiao.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/griguumdk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/guicraajz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/ggpoqrzid.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gttyregqb.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gdvtgvdno.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gatfaniom.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gjwpigxiw.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gpqzaquog.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gnfhvnrtr.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gkorcojeg.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/goweqvdlj.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/gtpxazsyo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gkyqyyxlq.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gumermfhn.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/ghnipqbeh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/govdoxmqb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gtvwjsifj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gmqlexcdq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gqxizzjpm.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gsytpksec.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gkedpgary.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gbpjbvqlo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gtedbzqeh.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gqxezmqpn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/glsqfkqbe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/gebvonvdr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gsgndwyyl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gzeqcxhaq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gmpftdyib.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gmjfrurnw.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gvaifajza.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gkqhoqubn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/gqilfqczo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gtyrzddfe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gnvpiuvrj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gjdwgpfgk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.tarul.cn/Article/details/gkljcvifr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gvqhzzisa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gchdjzzqu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gmtttozky.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gpaibkkap.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/glpjmogcw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/gvwchruas.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/gnmehnvgr.sHtML


<!-- 参考信息 -->