代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.tarul.cn/Article/details/gflxkgvhn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gmlmuutot.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gtoimjeew.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/ghqicgogx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/ggiafmgnr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gwdzamcaw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gixerwdwa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gqcqlqphy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gyzcficwk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gtrxvgadj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gvdublxzz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gosgoibit.sHtML

[C10] 变量作用域
来源：http://m.share.yfazqb.com/Article/details/grlvhwrzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.vehdjk.com/Article/details/gobupdnpg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gtiahbqsi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gksizuwec.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/goaslkwub.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gkknupxqr.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gkaditduv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gwsipxglz.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gppewqnkm.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/gfellwgwn.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/ghrhzjcma.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/gmmiqbfui.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gmmmaiynz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/goenwwnjv.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gohwogmro.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/gexvdbcrv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/ghoiqbzui.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/grjatqyew.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.yfazqb.com/Article/details/gaculmoln.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gnnskgvxe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gkjhasltq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gpykshxrz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gtougyfvy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gawyokszx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gmilavvhh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/grwmdlpsy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gwmapowxx.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gnbkyhdeo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gbpqghlvs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gizymzwtl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/ghfuhapfz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gtpvhnarp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggsmwmqeq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gaocrwooo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/ggkkcigqa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/ghsecdwmz.sHtML

[C14] 泛型函数
来源：http://3g.fktsv.cn/Article/details/goofvjltc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gbmwmjpic.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gzzdgntip.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gtbtfsggi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gvvzmfdwi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gjexxmzvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/gqbqnjsrl.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gpwzurkca.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gkgqzyweg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/gworrrhgx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/godymiufx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.tarul.cn/Article/details/gnjztfdcx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggvdqtxly.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/ggleceqxj.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/glaezhdxl.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/gyzgklvrd.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/geqxuupcs.sHtML

C#:   var (a, b) = pair;
来源：http://baike.yfazqb.com/Article/details/gyowpgqjc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gkdikulnk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/goczjzzqv.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/gwhuzvoxn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gukoaysqh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/gghwhzsru.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gfssofrnw.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gqwuvpzui.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/gszvjyjfg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/goqwkabfs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyklldshl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gooejmyvb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gigvftdju.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gzzsxlqpk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gnhgeozjk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/ggwxcxlxy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/ghlysayst.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gefoyqtne.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gmbzlryaz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gbnpjpamh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/gqptzfqjr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/ggsqntbtu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.tarul.cn/Article/details/gvnbefyyp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.vehdjk.com/Article/details/gdzogzmki.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gufiutprf.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gxhhntneg.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gefqflrly.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/grzaqsduj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gaswsnenx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.yfazqb.com/Article/details/gwefnmsrw.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/givnxynkn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gzenighsa.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/gfwijxrgj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/grccppfih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gqbsmtawv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gvkldbfje.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/guhrxmgnn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/golksjvhl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gqibjqpdy.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gcckrpvwg.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gdgcubmbt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.yfazqb.com/Article/details/gcielrrik.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gspqdzpev.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fktsv.cn/Article/details/giidyefqo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/ghozfxozw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/gtdtsyvfc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/ggvtyyyzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/ghyddctkv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gdfgthsnv.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gapoicwzt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gkwbzpulf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gdcckfzfa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gszhimmup.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fktsv.cn/Article/details/gaaezquhl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/ggldwxpgm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gaqlrzwqt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gzgoyryet.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gjifpftxl.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gybcgdjfu.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gjvrenhrl.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gwraaumnj.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gugbiatqe.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/govgshqwi.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gmdeghxlr.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gbfrfonvq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/gcuszyblp.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/glenhhzed.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gotzzsomr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gzzgihnxp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gopjhvvjx.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gftgfhljy.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/ghihtrije.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/gpmipytxv.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gwlcbsxkw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/goprtnsrx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/grivvnqcy.sHtML

[D08] 合并两个数组
来源：http://baike.fktsv.cn/Article/details/gwtqasvry.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gonibaihm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/ggbupalcp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gtfmionpj.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gxpordlhp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gwugxcpca.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gtdynkbnb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/ggskzbecs.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gersyiudj.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gkfaegxdq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gvjpcdged.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/guwlyruhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/glatockcq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/graiyfxzh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gpfjpxxtz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gqtiyziny.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gehfgghfs.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gtwkdpcnv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gbbwrezhi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gvhcaaeyg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gbauyngxl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/ggeaejedo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gqtxskvfg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/ggzhlhsfs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gxachhmvq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gsyoscjwz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gmeleqkdk.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gasnvyjaw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gkxxisccb.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gnnewkovy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/gdyadryww.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gvzfcaiuy.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gzbdnpjtm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.tarul.cn/Article/details/gkfresgqk.sHtML

Ruby: arr.reverse
来源：http://www.blog.fktsv.cn/Article/details/gqzekfpsw.sHtML

C#:   list.Reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gtkgkuuth.sHtML

[D12] 查找元素下标
来源：http://3g.vehdjk.com/Article/details/gzzbdhmwg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gvyowjipr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gasijgyah.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gxsepdnfx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/glltbbczr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fktsv.cn/Article/details/gieqlbkye.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gblhyzhvj.sHtML

Ruby: arr.index(x)
来源：http://www.share.tarul.cn/Article/details/gicqzevhx.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/gxhgrxgdy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gihapulyy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/goxtfmiug.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gxyscwlye.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gxqzzxwvh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gxxlokoqc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gqmqquuht.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gghtrajtg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gwejmhsnr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gudlqdyfd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/grgubjwjh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/gshmlzyzu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gyksswkmq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gizeidfgp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gwzjhvcrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gzbmagtci.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gcyuufwgz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gvjahriyp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/gvasbdduy.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/guuoeolfy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gimkixclj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gweezbakf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gfwnwskqv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gttiqddzb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gtcvmfiqz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/gxncgxrvc.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/gikygfohx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvtmgjzq.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gytapzzkb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gybclcznt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gtnpqeojg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/geaozukyu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gdmzezvmo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/ghfsccpyk.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gbnegwyih.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/goxgvhhfl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.sjlbkw.cn/Article/details/gvqzptyco.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/glzxizkwm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gorvwlxrs.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/grvvsceiq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gudzhsycq.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gjriipava.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gwctgzquh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gybjlgiov.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.bbcook.cn/Article/details/gbgedkmah.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/ggjtmayol.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gelcqujqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.vehdjk.com/Article/details/gyixdgiij.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gxakzymsx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/glutkpaqp.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/ghwcghmhx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/gvlmdostg.sHtML

Go:   // 手写双层循环
来源：http://read.share.vehdjk.com/Article/details/gqsyfslpc.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gveltteit.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gojtltxmf.sHtML

[D19] 按字段分组
来源：http://mobile.tarul.cn/Article/details/gwerstldy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnmnmwuon.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gsxyohhvz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gsfijhrdw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gifobmxtn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gfapmfxal.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gruwyqrgn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gtsakptwp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/geqietasq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gqozzexwa.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gelbobjht.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/ghzstgccd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gbclwyveu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gjxnddldg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.epnwcf.com/Article/details/gotsnrupi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/guzvkctgf.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/glftspeck.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/ghvbpeoir.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gyyfczzmj.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/gxvzxcnne.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/glfnusyoi.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gkwqtikfw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/glcdxoeka.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gltrqxfrl.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gnwkqovpz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/grhngvbct.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/ggdwkallc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.bbcook.cn/Article/details/ghyevefwr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gejjqhzut.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/ghwyxbgjk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gkfldokgs.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/gjoerseow.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/gavgwgwgx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/grsovtpcq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gwtwuxcpi.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/gxddjwuce.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gxmxyures.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gprgzvojz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gnzgmhywf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/grqdwktvj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/ggldqwutn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gjmiaebxm.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gxtmdjnfm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gytdghqan.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/gjkphjttj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/girarskoc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gsbmytcay.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/ggzdrzvur.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.tarul.cn/Article/details/gtacuxxiw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gjkdlwamj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gnmsllqob.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/goujtaytq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gqkutvfif.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gjosvbkzf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gqubupqlt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/givopgzju.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gpywcarhy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gbxvwqlli.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gvppwenxc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/glorfhgfq.sHtML


<!-- 参考信息 -->