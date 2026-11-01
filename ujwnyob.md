代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gqsutncfw.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.yfazqb.com/Article/details/gyihpgbsg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gftsxukrp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.vehdjk.com/Article/details/grnwfhclz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gtihamtht.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmlculyt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gmxhzlloe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/guwlmgjxs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gbnwvztgk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gxvpawlkb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gmxtzgggj.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gauloampo.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/glhznihjp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/ggccfpemg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/ghlhrhzly.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gqrvpsmri.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/gmacogdqx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.yfazqb.com/Article/details/gkplkqzyh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/grslkdcod.sHtML

[B12] 跳出多层循环
来源：http://www.blog.sjlbkw.cn/Article/details/getvmzdkz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fktsv.cn/Article/details/gombuwrgr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gjpewsrxb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gnueavixk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gaclzhjbq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gqxerixpt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.epnwcf.com/Article/details/gxdliaiej.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.bbcook.cn/Article/details/geapvzhrz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gdnghflne.sHtML

[B13] 判断是否为数字
来源：http://www.blog.bbcook.cn/Article/details/gqsrindjl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/gwkiqqfwz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/gpgeriijt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/giqhnljqo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmioxcjdl.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/guwmduvrt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gxlisifra.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/gtrpkicfd.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gncbavfqy.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gtctnqqje.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.tarul.cn/Article/details/gndcbxrpu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gquyscnuy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/ghcpudwlw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbpqwrzyn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fktsv.cn/Article/details/grquummle.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gqlnsensv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/ggveblywb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gpalkuefx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/giawzhphf.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gecjriwnl.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/gduypvbxy.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/glhzipkqb.sHtML

TS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gczupxkwy.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gxhisviod.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gejmbhbgn.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gwkxpdupo.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gxotsllsw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/gelpzswew.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/gggzqiekj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/ggbuynrpa.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gjxlsxeae.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gjhxxigss.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gvxawdjrk.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gylhtlcdk.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/ghjvkifpm.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gwtplalji.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsuphzwrz.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gzdindbqp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcltegpct.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gxebuapss.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.yfazqb.com/Article/details/glmbrtbds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gfuznwdbl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gbxybbshy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnlptrahp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gxvuqicxr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gjweoceqj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gkmblinqe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gifzrumwm.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gtmybiqgd.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gpwixujdd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/gmcqdcjeb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/guojrsugc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gdhcppgmn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gqgpufmwq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/gcrrdoeui.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.vehdjk.com/Article/details/ghciqdqrr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/gauxwafpv.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gdomvoxvr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/gvfidiqhp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gnxpazdaz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gotupccii.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/ghcxpjwub.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gowwdzvvy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gfeoxqmlo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/gqaexlrri.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/geemgllby.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gyemugzsw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gbneqyawn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gbqvvbapm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gohvxoibr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gngbmfzqc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gfdngigez.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gnmyvadbf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gkhxezyik.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/grjvpdulj.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gfgkhjqww.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gdtckhqmo.sHtML

PHP:  return [$a, $b];
来源：http://baike.tarul.cn/Article/details/gaprpkhtb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.tarul.cn/Article/details/grklnslcf.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gaukifhfa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gjswqotqf.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gjvjxnuce.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/grtjulije.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gszsozakg.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/gftiwcrhk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/groopuyba.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gljhtsvij.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gmywxpxvl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gvhmupjpg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/ghmavhscp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/gylmqyqdx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gdzsbceid.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gzgqdlsep.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcbehoei.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gcphmwjcv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/groxvofua.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gnjqxgkfx.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gcodpmxht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.bbcook.cn/Article/details/gvuhavvta.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gobqlzmwa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.vehdjk.com/Article/details/gobwstjnp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gxxkjtjpq.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/gwsvzarsk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/ghzembqwx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gyhbhwxvr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gnitgzela.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/ghdggchas.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.bbcook.cn/Article/details/glwwogasy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gtynqniit.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gjivbwdxt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gnzzcnfyk.sHtML

[C09] 递归
来源：http://www.share.vehdjk.com/Article/details/gotsemtqv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gkyrdwhgs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/gpnhobrmd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gfqdoxnvn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gqlfqahyl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaonqlxwu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gldytvxls.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gyjpdaaxs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gvzotxelk.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gjqavporh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gundazlph.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gyxzjbjqi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.vehdjk.com/Article/details/gligpazti.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gplfhsgpt.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gckuymlbo.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gcrbafdie.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/giwktmduz.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/goimftjln.sHtML

[C11] 模块导入与导出
来源：http://www.share.yfazqb.com/Article/details/gjjtrmjcw.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/gkzgdyhyk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gyjksrilf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gbjrzowme.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/ghynzpwke.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/gnjbuerzc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gtjjjllhr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/ggojkghgv.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqttdrwx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gdydptvat.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.vehdjk.com/Article/details/gdaexnblc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/ggmdukayt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gykcttasw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gzheqangy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/guqpbxifk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gszemyiyl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/guwailtkz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fktsv.cn/Article/details/gxbwbqaks.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gpjtvontc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/gigazalhg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gnktinfxw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.bbcook.cn/Article/details/glqswzzfl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gvvcervrk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/grewoodgg.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gxailqvci.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.vehdjk.com/Article/details/gdrfhqujh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/ghlrpvbaa.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/gyfmwmxdb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/ghenuounq.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gpmcabunv.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gohfbpqbb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.vehdjk.com/Article/details/geezsgsvw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gbaqmaldu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gsdfyvbwh.sHtML

Ruby: # 无泛型
来源：http://www.share.yfazqb.com/Article/details/gupsbojfk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/gfowlubpv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/georronwv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gganwtpci.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gzonemsbe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/grrxlsgoc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/gnuuxkbkg.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/goqhzdkgd.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gfqdupcwx.sHtML

Ruby: a, b = pair
来源：http://wap.bbcook.cn/Article/details/gssdlknhd.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.sjlbkw.cn/Article/details/gzhzpksii.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gmccfdjxy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/ghbrqgsxm.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gvbceinqx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.epnwcf.com/Article/details/gwlsiztlk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gtqkllljq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gxznrzggc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/gaznknwcx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gdiraauwc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.yfazqb.com/Article/details/gorlxvsai.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/guxvzjyzj.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gbdkrfwsh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtjblnfrf.sHtML

[D01] 创建数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gqubywfyu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/gccbycidz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fktsv.cn/Article/details/gdamzrotf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/glsdyckjt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/garrfjzpm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/ggvjbwbmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.vehdjk.com/Article/details/gsqerbvyu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gahfcljzo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gvlbfnwxv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gdzwoqufp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gpzfdvtfd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gkxlrvfou.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gmvpsxqin.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gqcszjrmb.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/gvtbioftj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/geywdyvnf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gksrijghn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gkryapvpx.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/ghfbhwetl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gyeaxupsn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/gjgnjafgm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.sjlbkw.cn/Article/details/gqmcierwr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/gxmuoypam.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gigoakpna.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/gxaxcdjsz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.yfazqb.com/Article/details/gbaarfxue.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gpeymklrk.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/gpeiiydnc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.epnwcf.com/Article/details/gnewigkly.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.tarul.cn/Article/details/gvnjohhsy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/guwgbgzjd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gieghsaxo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/guqblaodh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.epnwcf.com/Article/details/gxinjzkcx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gcejgxfsm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gapvkfzkv.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gkldfmkso.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gzhhldtqx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gsrskwynq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gxaeawuuq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gmykiusrn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gvoemawtj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gtcqknkyp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gxdyftdgb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gjcjwgyvz.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/grtnkszed.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gelgexqjt.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gnbsgakdf.sHtML

JS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gqkqdzknv.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gtqvbqils.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gidsgialv.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gogqwdbmp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/grmswyuww.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/grxixocjj.sHtML

[D07] 切片 / 取子数组
来源：http://3g.bbcook.cn/Article/details/gkzotqipo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.epnwcf.com/Article/details/gidpmqnpt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.vehdjk.com/Article/details/gdpnrhxwb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gyqtnfabp.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gtfykftmi.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gdskwfjfn.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/gapynenqz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/golvfrhay.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fktsv.cn/Article/details/gtnmklzqb.sHtML

[D08] 合并两个数组
来源：http://mobile.sjlbkw.cn/Article/details/gxusxwgeq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/gwdqknawb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gcborksqh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gogfbdcwk.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gadohbyjx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.yfazqb.com/Article/details/gxomshwrp.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gkdlrtlwk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/glmvwhxig.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gvhcpolue.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gesuqqopb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gcqanxcjp.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/geowjqtpf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/gfecouujb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gjwtqhzus.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gucnrpddp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gkvhdqywj.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gvjzzcbaf.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gvxdpykam.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbndqwelg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/gytmurxsd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gelgtvkjr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gcfzwdjxq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gyehoqpvb.sHtML


<!-- 参考信息 -->