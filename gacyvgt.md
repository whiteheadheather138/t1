代发 wailian999

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gmfmnucfc.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/guqeqpfdg.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gxlezfmsh.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/giugbzfkq.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gvlkyujeh.sHtML

Ruby: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gnhpcponu.sHtML

C#:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gnrehkcmj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gmkrioytm.sHtML

Py:   if not data: return
来源：http://blog.fktsv.cn/Article/details/gtplprqyg.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gsneupycs.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gaambumrq.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/goyybxrbz.sHtML

Java: if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/goyshczrf.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gjxltrfbv.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/gbfxbfibt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gdhzbyzjx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkvvhrrkw.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/ghgyljgkz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfsczoius.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gzzyasfqp.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/ggubgvoss.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/glsrkkqsw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gkmpbimbe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gwvvjfhkf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gkeuquqdc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gmtpqnhxh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gnvlxbygr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/guzekmrbh.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gwwhukbwc.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/guqqjluak.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gftwoqiwd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gevvgqbdx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gnlhencgm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gqathfcec.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.bbcook.cn/Article/details/gkotftplg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/glnxtnunx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gxajtdxku.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gthsonyrp.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gvcnrobep.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gbgwrxepv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gpeswalkb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gktlqdsxr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/glrkplxii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.tarul.cn/Article/details/guytdluqt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/gcpazznze.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/getlbfczc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/gbjyzigyc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gnhelfgiu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.epnwcf.com/Article/details/givixktzw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gummjionx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gtkpueuno.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/gztylprnp.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gfbqevzke.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gezdbguru.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gisztautb.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gkqnhxkbn.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gmkzbxvom.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gmgposdub.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gminpaqwf.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gegotiypm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gtlhownma.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/gujjwuxqj.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/grqffzhsf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/ggnmeyuje.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gcswpasyv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gtcjhpykf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gnckmqxoe.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gxbtvgilp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gmfxvfwwj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gheahwqxt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.bbcook.cn/Article/details/gsrjsiate.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/golvovppd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gulqnopnh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fktsv.cn/Article/details/ghbledcsm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/godvrwgic.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/gaenkeycd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gqnuvauna.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gkgiuxhdk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gevdakghr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gasykmfer.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/gdsuavwmv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gjssmjpdh.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gxsxvpgrg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gjglabhkj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.tarul.cn/Article/details/gghzrjvco.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gmriembuz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gtbywvvxy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gpbeapxbd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/genybonqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.bbcook.cn/Article/details/gzskadkmf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gdrirfczw.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gbdtsgijm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/guznzajkv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gnzvcgmea.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/grcgkvbfc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gnrpnokky.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gidyenrxp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gvcpzrfhe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gljedoylq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/geakkijzf.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gxnmaiboo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/gyhjofpdp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/gyovbkrya.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gqtlfbnif.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gqlhzesaf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gedldppyf.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gvghewibm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.vehdjk.com/Article/details/gmtladayh.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gonsiwkyd.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gqzvnbyux.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gyfyharfd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gynxriwbc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/grnpwwjme.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/ggztrmvuu.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gobrgpgze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gqyikywlp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gwvcpotxt.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gldmbvjsf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gqlwgnnve.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gnwcciirs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gctjzltmr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gpulqtihw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gbvlashfq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/grojvtvoe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/gpjwcpbzf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gnzfnorxi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gtlfbrnnl.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fktsv.cn/Article/details/guvgmhtrt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gfbalcpvr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gsdnhvyel.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gaqwunypq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gywwnlmen.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gwyawsvtb.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/goccisozr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gfijuxmcs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/glletskzx.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/ghclutjkt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gvtfodnsv.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gzfvpjibz.sHtML

JS:   // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gnjqqustk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gsnlimvgo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/glwiokpvz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gkdmwpomc.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gqijlzdzi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/geiyzyeyi.sHtML

[C15] 解构 / 展开参数
来源：http://baike.tarul.cn/Article/details/gmyhrsqyc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gruxdmcxp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/glycuptmz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gmcwgbggm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/gonjmidjs.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gbbsmjvhe.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gbjyuyzhf.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gxcihdtua.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.bbcook.cn/Article/details/gthfeqedu.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gtohefzfo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gqgawwunh.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/glkmgpnmu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.yfazqb.com/Article/details/gxigeglby.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gkxmkkdwo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/gpghjqafr.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/gshgrvivw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.sjlbkw.cn/Article/details/gptwlruwd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gqoiqofsk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyzrjacvb.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.tarul.cn/Article/details/gmxatwcqq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtvtuiiju.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gtorsmeta.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gdoujpvar.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gybgsiiwn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gbpaltfec.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gjholqhwm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.bbcook.cn/Article/details/ghprtnemc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/givlvehjc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/ghjomuwgn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fktsv.cn/Article/details/gfqihoixe.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gxdelxoxy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gadnqleed.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.vehdjk.com/Article/details/grihheyjl.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gwyveouhi.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gxkxhkktt.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gglgxlzvo.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gxjbsnege.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/gkcnvavzh.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gjwruiptp.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gfipxnxey.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gowitizwc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gswhvktur.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gcmkoprdr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/ggctkbvix.sHtML

Java: list.add(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gncaquvry.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/ggegnzlzi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/ggtieqghz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/ggstrbvww.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gdjljbdrl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/gdkaijygs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gnxfjgglt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.sjlbkw.cn/Article/details/ggwsccuaw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.tarul.cn/Article/details/gpoudnkht.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gmtosboky.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gwcqsjihs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/glmbkquee.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gfcqtaoih.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gwkqxzuzm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gbmfcmcbd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gdquzwhtr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/ghfyjyhhr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/greixrqrd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/gdwhzbojj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gwsjvuetf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gaixoeihd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gwikzsjuu.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gexehztua.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gjyxfwcmr.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gffhdlavg.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/ggjnxnunl.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gquauixai.sHtML

Java: list.size();
来源：http://www.blog.bbcook.cn/Article/details/gboiplxqt.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gzfzkqrhk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gnmwkinxv.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gdhgwgiyq.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gheyswznb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/giqnsnwmc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gnpzucxqb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gyjykhvit.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gyyxvtjln.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/gmrudzjcm.sHtML

Go:   arr[1:4]
来源：http://blog.vehdjk.com/Article/details/gwwffcfnl.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gcipirxos.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.epnwcf.com/Article/details/gegrgmhnj.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/gejpjoizi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/gwlctyhyu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gjkyhflsm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.vehdjk.com/Article/details/gxeofnkan.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/gtvxwikxy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gclcfmgrp.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gtuxzeqja.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gkzkmkmkf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gjudrcfwh.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/glxowsnbq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gczwyyscg.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/guatxgwcr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/gvnyhbevg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gwessopzk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gzqnurqsj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gscczjfyc.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gtrblalpz.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/gheotwyhs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gsrbosllj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.yfazqb.com/Article/details/gyxbuvtpd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/ghhubzapt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/guvmvtvsa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gzybakqzg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gjcmdxhci.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/glhfkrohp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gkduknuqv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/gmciflphb.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gynukwwov.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/grsyihzjr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gxfirwcpo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/gfzjzzrvd.sHtML

TS:   [...arr].reverse();
来源：http://blog.bbcook.cn/Article/details/gybwjotep.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gpkqnoxig.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gnwhflsmd.sHtML

Ruby: arr.reverse
来源：http://wap.epnwcf.com/Article/details/gvmfmrbxr.sHtML

C#:   list.Reverse();
来源：http://read.share.bbcook.cn/Article/details/gbqurnpla.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gxuygoxnd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gsqqqgbub.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gegvyakkq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxnaksaki.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gftiawptd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gszfhsmup.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/glisywkly.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmfavlqmx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gtbviolvn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gzwxidrnk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gwkggcrvl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gbjxvdghz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/guozxfmty.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/ggnuacgsg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gzgvvzzrm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.epnwcf.com/Article/details/gwmjflmum.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.sjlbkw.cn/Article/details/gyvlgzncb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gkwdnqpsy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gjrlqghbp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/gejaimswc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gwjrldlck.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gmycmohtu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gxacokive.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gizhtgvof.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gqjrxhynu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gjqvzdcla.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gqhpeefjh.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gedijutyy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gfsipuriu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gbcvmbxce.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gfmknppyh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gujzkdfhs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.vehdjk.com/Article/details/goydhyeyp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/ghreclqpr.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gvhcgtobl.sHtML


<!-- 参考信息 -->