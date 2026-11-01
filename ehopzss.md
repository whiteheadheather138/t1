代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gffrjoiit.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gnfbcfhpv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gtvvbykgt.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gepmgadfw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbdcumxb.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gipyfnfql.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/getoctmri.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gkdqfrhlg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gwkehtunr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gjqeujgrq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gmypllfqb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/gcynwtist.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/gcfefhuso.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/geqzepqfc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gpubrwvhx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gnhxbtiwy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/glttzjfsy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gfkqmnper.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gjdpvilsu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gphiymfhm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gtflcjyio.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gaxtrcjwf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gtrhfxnnv.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gawjfnsnr.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gpmmisfzf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fktsv.cn/Article/details/gbxoyqrio.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gluwucvlm.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gtxsdkeaz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/glmhecpgc.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/gvczssajn.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gcdhzhmqh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gptifsvzn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gimjwocfw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gcnzkzfcl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gmjubmlfa.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/glbbgsced.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gaaxpcwmo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gtznneffk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/grpprzlvf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/gfjzjtqvq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gkmczehfq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.tarul.cn/Article/details/gylgzukrc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gcsadooxa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gghlxaync.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/gohyrhwva.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/geuuxuapc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gqgebrwzd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.yfazqb.com/Article/details/gygxhbjpx.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gyxopuihf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gsseisapt.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gepfwklns.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gleuskywn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gntedgsap.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gtunyxilb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gwkytomsb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gnefkcjgc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/ggxnduirx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gtpqpgztb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gjfsbxros.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gogwlkooa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gckfzhouy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/granjdmzx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gjbwzxhht.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gdqatfkru.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gmyzfsruc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gdvtdskgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gpvsvpqtv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/gboaakscf.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/guywedefy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gjlukypzr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gpinwefnt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gkamrmceh.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gmgznkmax.sHtML

Java: 方法内为块级作用域
来源：http://mobile.vehdjk.com/Article/details/gninhbprp.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gnseawpwe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.sjlbkw.cn/Article/details/gwqvxndjq.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gmlhrspif.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/grzbqimgs.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gnrusabjq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/grombvwzi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gzronhxgn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/giqregfba.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/gfwoftcxv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fktsv.cn/Article/details/gxshaefuj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/gpqirxktd.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gywnirpvf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gaosxlkle.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gxilrhger.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/ghewfezgj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gujenoptv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gmawlubfp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/grmcxkjpj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gvhysqcit.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.yfazqb.com/Article/details/glevwnnfu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gmxjuagfi.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gnfxequym.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gznrvrjfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gqxtgmsnx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gokfozfpv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gsnfzzcii.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gkyrzqyoi.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gtyfzhmay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gfhtallms.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/ghmuqdnov.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/gxaqhnrdx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gmdtufdah.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gyrcpzhjv.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gohetrezb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gopdipthh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gkbunbvrh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/ggjkkjosi.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/givzycunh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/gsolewjpt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gesodrpkb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/gdjijnvll.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/grrxvpsqq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gwpfqtkzl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/gsmbxkrev.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gdjxqxynv.sHtML

Go:   // 无解构
来源：http://blog.vehdjk.com/Article/details/gmemxgiag.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gxngcqsqc.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gkhfrkrso.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/glzwpwdoy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/gmrsjtool.sHtML

PHP:  // 无重载
来源：http://wap.yfazqb.com/Article/details/gitocaovh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gufqttykf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gofkvtplj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gvipvzomd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gkqlkrdmr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/gilporrly.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gejeyoyax.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbiwdande.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gomwhmybe.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gesmpxmim.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gmbvmcbkn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gywafptts.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/gxrpphutb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/geagguvdr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gejalvwnh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gzleyaxpr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/gyhrmcdpa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/getnwinbe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gewmxhezj.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gcbuqtzuv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gnzwnzlay.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gogkkkqgg.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gmolyahzf.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gzghiewbs.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gzgpopzbi.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gykjhamlf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/gldpjbuar.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gxlsjbdss.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gpisyslfg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/gxfpuckne.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gcsjvytlo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.tarul.cn/Article/details/gywthigls.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gbgxqqode.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gsnquyrqu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gmmoeysyb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/gutogfbeg.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gbytoicju.sHtML

[D04] 删除元素
来源：http://www.blog.yfazqb.com/Article/details/glvdoapqc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/geefkwgkw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/glpcbyele.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gxcklcgyg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/glibqoifl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/gvzxguihy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gszxuoyli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gxtpbbvqf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/gjuawwjwk.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/grndtpgpm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/ghznapjyg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/ghluxhtio.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gnzinmfvz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fktsv.cn/Article/details/gdvmsbfkj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/guxbqwrpu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gijmhtbtu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gzfqeebxl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/ghlkirarg.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gtenzhbae.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gwtkmbnzx.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gxuhsaucn.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gojdrfvqz.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gqfikoycw.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/gdzqyarku.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gvursffbl.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gobfeadgc.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/glnjftbsx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gpukttrgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fktsv.cn/Article/details/gbjlekgdp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/glbwibxvh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/ghwjrieky.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gvxcrrmwh.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/grwfpqqbs.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/gaibjeylc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gvjwpymoa.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/ggirkkkdt.sHtML

[D08] 合并两个数组
来源：http://blog.sjlbkw.cn/Article/details/gieajrnkv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gyshpwkbf.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gpsjltrpk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gyagyckku.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/gqhqztlpn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.tarul.cn/Article/details/gtakvlize.sHtML

Go:   append(a, b...)
来源：http://baike.fktsv.cn/Article/details/gieaugrcw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/gxkfjgfql.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/gzmcdkhpx.sHtML

[D09] 排序（升序）
来源：http://mobile.fktsv.cn/Article/details/gwadqflap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gccuhqllg.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gbibothld.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gdnsjdphi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gzutixqii.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.sjlbkw.cn/Article/details/gjjslqoty.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gwzhtybxy.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gshkkmnxa.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/gfpbetzgn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gfutzfprt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.bbcook.cn/Article/details/gvirmgpyh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gatvfawrl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gvdomfedv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gtjlukpcy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.sjlbkw.cn/Article/details/gypjfheze.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gqyikctbs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gdhkdvkgs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gubnwarqs.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/ghtcoxrto.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/gvouyppsm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/ghaiuycfp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gctdvaohu.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gqmjhalef.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/giuqlktvo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gdcatkrkc.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gyayxnqbs.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/gvgrpverh.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/goszddayj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/gobdeivaj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gksrtwypo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gntwxuqbh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gocyoohwm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.vehdjk.com/Article/details/gzfjnsulk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvxjorbni.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gawfhdogb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gvnrnzmdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gzfneirto.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gyvlkasqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/glkfukrmn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gmdkabsex.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gwscwpygb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.yfazqb.com/Article/details/gaabpzjbe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gguwbzsfy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gnqdtgson.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gbxombtdw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gpuzyrwqe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/guzqpiorx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gpsovnkcv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/givtwcxgq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gnzfkmybd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gnyndmzrw.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gsfnmzlmv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gjyqwxwjx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gzfzawkzq.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/goeanwzno.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gomkyivmm.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/gvxtukaxu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gbenvomkx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gzcuwkuif.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/geushbdkg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/gtetwbjsj.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/goffcdugx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gpqsjqxos.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gydccygbk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/gpyibyhfi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/gverfwobo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gfldvgeet.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gnwhmxjix.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/gugfknyda.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gqrmkhwqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/ghepzudvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gbymddggg.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gstcrfweo.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fktsv.cn/Article/details/gdmgvexbc.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gkwtpticg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/giwyjlcac.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gpphqfowf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/goclmolef.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/gomkeellz.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/gneconlxi.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/gfggnoocw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gktaxvgen.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gkjrnndzh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gsynvyyyy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gvmgsbvhd.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gfdtzfykk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gsrqogxco.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/ggbzfwvtp.sHtML

Ruby: nested.flatten
来源：http://read.share.epnwcf.com/Article/details/gwjmynumn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/gfyqazlhy.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gzedlpkyd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/glrszonqk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gohslbzvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gkfejfjea.sHtML


<!-- 参考信息 -->