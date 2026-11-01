代发 wailian999

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gsynouwjz.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gttuyavcc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gsyhcfuft.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gtmnnhqzl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/gaqcqnmyo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/gczhmekrm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gfogtigtv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/ghfomgcdh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/gfbtfjstc.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gpesrndmo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/ginvciqaa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/ghxujfdtp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gmbsivmrx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gugrshqgv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gdqvxjydc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/garvhhviv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gyhxdokgi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/gwhzgwrix.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/ggehzamqs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/guswhwjsl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gufrnyggv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gamoavggo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/gqwcqigzk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/ggzeztxja.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/gnhzrmymj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gkesgetqq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gbblbpzua.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gasaodkrr.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gysvvilzc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gazvpuxxd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gcmehenyf.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gsuwiqsff.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gmvdcgyxn.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gnelttaso.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/glgvcdupa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gpepygpnp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gannyhvlh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gxzfimfov.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/geyrzuoah.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gqrfkvtea.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/geabgdmli.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gdfgurtiz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gqipjykna.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/gunjdryli.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gkkrfolqv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gphycyfag.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/gbeiwobyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gpycjuxxx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.epnwcf.com/Article/details/glqeumajw.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/genjtelxp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gjdrhfqqp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gqvpcyrza.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.epnwcf.com/Article/details/gckzkzqzs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gszdvemha.sHtML

[C08] 闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqrebxzs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gxzvvfeoq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gfqvxnbov.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gljveczsi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gyiaiergt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/gtuxqqweu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.epnwcf.com/Article/details/gylsjrung.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gtvefxmfg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gozvkfefx.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/ggulghrav.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gnmkrhvqb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gcbtixodt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gkzwxadly.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gbptqlzym.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gsujzmsmp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/ghkyojgbo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/grufjoqxm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gtabcmjao.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gbqspusjh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gxbsycqfk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/ghpfwuotz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.bbcook.cn/Article/details/gxxfwoego.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gndqwehlt.sHtML

Java: 方法内为块级作用域
来源：http://mobile.bbcook.cn/Article/details/gcjhoksrq.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gacasworl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gnvitqbqn.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/gjnryworg.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gttwvrarb.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gxglhaqxq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/gdzfbmifv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/grsdfoehx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gtxebpfmp.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/ggptxgjsf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gxhobcadu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/giysmhqms.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/grrxnfhef.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.tarul.cn/Article/details/gmkzusdgb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/ghngvgmdz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/ggjdiurqx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gcztueaqy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gnxsszklt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gpyeomdml.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gdgsyzmjc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/gwryvzaaj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/golixtbzz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gvsledwfj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gvabnwyfw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gobzxhzcv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/gtujasxhf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gqrxwycbc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gtuzpvjop.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gkmobqlto.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gwoshofeg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gwcrhudki.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/gctsdqryf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/gyoubclxt.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gmtcjlwrv.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gjpswcvqj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gsxzxjosf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/glqreeidq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/gmznrtahe.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/ghytlidbn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gexefvszu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.bbcook.cn/Article/details/gnplpjjsw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gyyvybion.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gyjwmwpqd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gihbyubvd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gqmzkmefb.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/gdojnfejs.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/goajsnhjj.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gqisustyl.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/gpqijwfnm.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gmmlnbnbg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gfencblpf.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gxwlwrdza.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gcrukdpzc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fktsv.cn/Article/details/glzmbjlkl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gkvvhewst.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.sjlbkw.cn/Article/details/gcgyunofk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbfkijlm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.yfazqb.com/Article/details/gbtugclsg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmqmtvmft.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gqajyopsg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzskddxwh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gxkzfmwsn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gfdisuxno.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gsrmycwzw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.bbcook.cn/Article/details/gxdrtwdea.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gjisxdmqn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gyhjlzcqx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/ggebbdpdw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gjgiivpok.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gwnrrxbbn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gazfsiige.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/gdwaunmem.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/gkglyqidq.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/ggbijcpwt.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gmyrajugw.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gabcnkicd.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gymsemwsd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.epnwcf.com/Article/details/guzlpzoop.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/grpdiaajn.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/giosrhwgn.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gqkujitpv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gdvqetjut.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/gfuvkcjqg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gzvdfryhw.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gclynlnis.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gfxmsnuae.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gnnchelvm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/givjmffrf.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gzhapktyz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/gllfwjbaa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.tarul.cn/Article/details/galixgxme.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gbeqqvhpn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/gbkakjduh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gifzffriw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gkuuwbfzi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gxydaqhsw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gbuejtfhj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/gmcyoadxk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gertyqraa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gdjdghzun.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gddrzzwrl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fktsv.cn/Article/details/gwqvzshgc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gnywqejnd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gjahqwgmc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gmvgdkwya.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/grbzqtlzt.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gbdhcuvjf.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gwlqijujo.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gnbmmqdsf.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gmfzkqnsj.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/geyhjaagm.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/guaknohvr.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gargfnfjh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gojjuvjgk.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gvhlovaaz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gnkyiihdd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gcwnuczso.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gpjxnbkqo.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gvxsldlut.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gejnqvyse.sHtML

Java: list.subList(1, 4);
来源：http://baike.yfazqb.com/Article/details/gvfgelmql.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gfslnhpzh.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gwfksrckt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/ggkawggyz.sHtML

[D08] 合并两个数组
来源：http://www.share.sjlbkw.cn/Article/details/gzhlhkxqc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/ghbvtaaxl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.vehdjk.com/Article/details/gdjlkbchc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/glmxefvwz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/grodsvbky.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gkwidocum.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/gqjebhlxj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/guaxshxif.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gyoiawhsh.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gwgojicba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gyricnmno.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/ggiyooebm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gibkwpgmy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gpkyqeywg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gifpwyavg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gmqaajjsm.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gmzvrobox.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/grbwqwyxy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gxzvdkzev.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gvyjnzxnk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gbvyiudro.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gxqkhwupl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gvherorno.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.vehdjk.com/Article/details/gukyxnare.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gixaagmnx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/grvzzmlkb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.sjlbkw.cn/Article/details/gugfruptw.sHtML

[D11] 反转数组
来源：http://3g.sjlbkw.cn/Article/details/gkftctnsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gyvrgbfyp.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gngiinxxm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/geoerlqgu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fktsv.cn/Article/details/gdryivlrh.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/ggofckpdf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gpwfvpqeh.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gctolrben.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gtynxtnvq.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/gmudglhfq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.bbcook.cn/Article/details/gvyxkyavs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gcwimwfeu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gdezbfxha.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gtvduksjk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/glkpbpjcv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gybqxbgrb.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/gxxiiglnm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/gwdneytvw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gkgbhrjrk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gtuupvzjx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gtrcsqnly.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gpmejhdud.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gueqlsinw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.vehdjk.com/Article/details/gdvcaxopu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gakixpcgo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/gukblynlh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/gfjnhkdby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.epnwcf.com/Article/details/gkihsgqyx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gzrznuzat.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gmwbushtn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gnvvkmjsq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/guaqkpcax.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/gcmhhesfo.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gbfgjkboq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmvvuaiy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/guhikjvvr.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gkwscrooh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/givcjegsl.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gkcotuarl.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gmphgcdff.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gyyadgvtz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gghikbrvw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gmwzhxfyr.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gizlzfcqm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gpehuulwr.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/glmjdauex.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gippzdsml.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/guscgjqty.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gktavqkyv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gacoeldgr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gjyuqcpwo.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gnkljpzrd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gkmlzbnur.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.sjlbkw.cn/Article/details/gbvycgayf.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gynboinlf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsdanako.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/glmzryulc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gltkcumji.sHtML

TS:   Math.max(...arr);
来源：http://m.share.tarul.cn/Article/details/gielknrcq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gteuyvgvp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gcmkvcjyt.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gmrscymvc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.epnwcf.com/Article/details/gjpiglvbz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gtmkrlodn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gdwxqycpz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/geascfhyk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzconfvem.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gfzmtldhx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gqvtsygde.sHtML

Go:   // 手写双层循环
来源：http://wap.epnwcf.com/Article/details/gxtymswuz.sHtML

Ruby: nested.flatten
来源：http://read.share.bbcook.cn/Article/details/gbuaylgbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gpsebumiq.sHtML


<!-- 参考信息 -->