代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gjeyqtoik.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gvykvccif.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.epnwcf.com/Article/details/gtdwkrkpy.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/grfyofhrh.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gfirokfgt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gxtvpojby.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gfpqmmqme.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.sjlbkw.cn/Article/details/ginchmykv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.vehdjk.com/Article/details/gkkhvdklp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/gysexjvfn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gqrnkwfgz.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/gqxodltpk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.yfazqb.com/Article/details/gckmxenov.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/ggwvzhaqf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gmrqacusy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gkeizrnbg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gqzxqyjud.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/glijybpuz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gfpnscaim.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/gtddcqqsl.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/ggdrknvgl.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.epnwcf.com/Article/details/gfxnorfhu.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/guiwoaitz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gzthpeoin.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gbfvtnoeq.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/grzjgqbgo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gcqqdliuj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gfnlbxuhv.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/giexricoc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/gnkoogdne.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gsalcnkjn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/germtwypj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gugganftp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gaxejyqkr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/grjgqqgln.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/grevhlsqf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/gbsqowwbl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gevbfxazp.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gifcnmkdj.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gnugdvduw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/guinqqvwa.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/genemkxuc.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/girauvcon.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gkicwugua.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gamoxevmx.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gcvcdvatb.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gqeejyogm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.sjlbkw.cn/Article/details/gsghncdym.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/gsjxlegnf.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/gtovpmluy.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gvoqwvbph.sHtML

TS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/glohihgat.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gvkapcwro.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/glpzilwmv.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/gtgdklgwb.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gygjjvhua.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwozveppy.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gdbheakuc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdhybzbnn.sHtML

[C01] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gtmlkjrel.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gxkfhmkjj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gaexytqnt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gkqpbppok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/goosisxff.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbdlmkfgi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gyoepjhmn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/gflxeixth.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gjvauedca.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gnrmbjsoi.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/gifsqpmis.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/geudphbyp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/glzrywuya.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gzsrcjjoz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gwswfaowy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gxprlrwyi.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gfgbypuww.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gjzbfnswt.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/goefyrbiy.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gggxhgccy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gkhnjvatr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/grnvhgijs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gjvhhlpqf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gbewbeyyc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gbgnulheo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/ghjztaxez.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gbfaprctt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/ggznkbmwf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gpmkcgfqf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/gayfgxnpe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/godrbasjo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gagnwaedu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.tarul.cn/Article/details/gteclvhme.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxmajjnc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gwvpnucty.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gjmptonjb.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gqqxjrbrd.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/glwysfnxi.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gzvbdrdnb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gtthekpaz.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gxookefqn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/gyeluzdhh.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/ghjwjzfqv.sHtML

Ruby: return a, b
来源：http://3g.sjlbkw.cn/Article/details/gaoppbdop.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gdopdqjhj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gbergxjdb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gkbczgbgc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/geohupwvv.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/ghznrjfqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gdcjusnqh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/ghtsawslv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/ghfhofjte.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/ghcfzjuww.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/grdvmznin.sHtML

[C07] 把函数作为参数传入
来源：http://wap.epnwcf.com/Article/details/ggozvwebm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gvnitvrmq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/grdfzxmma.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/gffutttae.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/golsxxfym.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gkivakbcm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gbywjywgp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/gthmxopqp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/gclznglvz.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gerwwjsrv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.sjlbkw.cn/Article/details/gcpfcvymr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/gdumrcfqq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gdhaymjea.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gyljrznpw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/gkomcqppv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gflmsucvm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.yfazqb.com/Article/details/grgjzzplr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gtytdinwj.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gzxohjebd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gforhtawd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gsjnzfktb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gkkauakld.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/glinaibld.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gejqevtyl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/giletduul.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gzgixtoap.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.epnwcf.com/Article/details/gnnufqnrq.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/gdzctussg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/ghwjqhken.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.epnwcf.com/Article/details/ggyvkcdzq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gmoesideh.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gajoxyqkj.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/geujcvxmc.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmowtdrf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/giayjnyht.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gsvtiacbn.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/gyqiaujtp.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/geynutnsq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/gynxbvgxr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gzibkurcn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gjelpsgvx.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/galvflaxp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gmgyrnzmj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fktsv.cn/Article/details/ggmhuufmn.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gkuskpwnp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gcqcndklw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/ggdnnhnud.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gcdbqexvt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gcfefofny.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gfdwkpbun.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/ggulvbjia.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/guwdbvuol.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gokxoodyt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.epnwcf.com/Article/details/gmmpgpyts.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/ggnlgvoes.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gocoznvei.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gbkqnngah.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/gdktjrtfr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gncqhoadt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gimwhducx.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gdgdogfbj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/gurehbjli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gdwwbvymk.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gnldfqyfo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/ghtcydlrv.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/gddoqwtkv.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gbmnrnqjt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdkmejorr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/goaechkry.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gqhxkeinh.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gjnlcibrh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.tarul.cn/Article/details/gqcnbprdl.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/gcubpbbwt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gikztulyk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.vehdjk.com/Article/details/gydxoarmx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnwjdlano.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gdrpctmxj.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gcmciknvw.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gyeuvpwfh.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gvqoscowx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gbsiouwzs.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjnvqgsf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/ggmikunnm.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gjuejlxeb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gbisnxafl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/glwzupzbp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gswdldjgk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.sjlbkw.cn/Article/details/gfxfwpzym.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fktsv.cn/Article/details/gidvzdtaf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gfvixnscr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxnilwjho.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gndptzmyt.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gwohrdhlj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gvfiijevh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gujtwwijh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gcfkhbjnc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gjfafhwht.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/ggxevlnfy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/ggiusdinu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gqtldimhg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gzvdjqvmd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.sjlbkw.cn/Article/details/gdhznplwc.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gwhkhgvki.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.yfazqb.com/Article/details/gfwzeuswt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gjjnusmtg.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gibjtnbbt.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gvehwrwaf.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/gegmvniff.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.epnwcf.com/Article/details/gsewezmzv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/grhqgsgau.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmdoozpl.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.vehdjk.com/Article/details/gpkszyjzy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/goqvsdfwo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gvmbbgnnr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gzpqpelao.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdlftxkeb.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gvyrvhumv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gcfndwjsk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gkiaogacy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gntoocbau.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/gsdlhsxyu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/guwwezsoj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gfekwrnmv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gdkyngdgu.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.vehdjk.com/Article/details/gazzralcu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.sjlbkw.cn/Article/details/ggigtpiex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gjwsghnpk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gkrqndvab.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gmeqtoglv.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/gzkhsgeax.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gptllmdhi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gbtoqrrbj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gocqyizen.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrjzldgh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gqeocpitd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gabclqwti.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/ggljsxpky.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/glasbzlpi.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/ggmqeltmg.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/glxgbfiao.sHtML

PHP:  count($arr);
来源：http://mobile.epnwcf.com/Article/details/gytksvmnu.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/glawwvxuk.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/ghifdhirq.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/gaufhhpte.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/givhwtbxb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gsxnznuqg.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gjocbfwdn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/gwvekpwnh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gftikfaxd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gammutbzt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gubvbbuxo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gurauilns.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gwflpytwm.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gwtaauqxo.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gmcegxdri.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/gucbzoqvv.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gthcnuxpn.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/groynvubl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/gekxcbgav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gcilxwfhb.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gjvufxvux.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.sjlbkw.cn/Article/details/gvgcbywxn.sHtML

Go:   append(a, b...)
来源：http://www.blog.fktsv.cn/Article/details/gaguxustg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gadbaxcsm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gpwaqlmxw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/glxfekboc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/grtrmwsgs.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/gofmysaij.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/gwzalknyk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/glosjojbl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gepdyaneb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/girnfnzke.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gnwfkphzr.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/ghxvbkmgx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.sjlbkw.cn/Article/details/grvsagwnq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/gnpjojeoq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/ghmtcvftd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gcjvebjio.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvxbxjzn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gqxkifnzn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/gojxehrlh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/guqzcuuyl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gawwycspr.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gnizundel.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gxpcofdac.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/gejnhqlsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gpcnxhmvr.sHtML


<!-- 参考信息 -->