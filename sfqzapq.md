代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gnkltuhnf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gfadhywpd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.sjlbkw.cn/Article/details/gyqeomciu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.vehdjk.com/Article/details/gonvrenzl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gwzscsxvl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/gcypodbtq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.tarul.cn/Article/details/gptemmbpg.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/gswkfkltt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsakkbcz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/ggzufejpd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gegrkepqf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gumjcdjmw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gaqbfarpn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gewutfgsf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/gbljkxwsb.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/guakjvwvh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gmnuacnfj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gzrcolvoi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gqponlfkz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gjidvkjsu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gwykrsilg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/ginklrdgo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gdnydnzoy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gszxaglmy.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gkefkwcyr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gnafvhwtu.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gfjayskcy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gdollumgj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gwdoihkvw.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gtvyunrsq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gxdpkmvkf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/gfautmsga.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gvhvfafuf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gfgqndmtf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.bbcook.cn/Article/details/geecsvhta.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gqcnojvro.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gjcosxyic.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gjknkjbpa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/gnoltlsju.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gumakfdto.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gncyivhwh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gychmcbfk.sHtML

[B15] 布尔运算与取反
来源：http://m.share.sjlbkw.cn/Article/details/gkugcatmv.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/goqgmiiow.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/grmluajac.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gskorlxaj.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gojffhmwi.sHtML

Java: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gfjgivjrj.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gamiswzwt.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gpncrgdqy.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gfevfvlnr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gdrfbahbu.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/ggtsrepsw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gxyugyyic.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gecyzjkzz.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gbdpvwopj.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gryczujiq.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gelilvnzu.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/gapnjqlyd.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/ghpldxrpt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyuwklxwb.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gcaayopwl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/goqarmssn.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gqsdpgtdy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gyhvpbxqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/groznrinp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/guzfqaerz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gkciysxii.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gxxnvwfoj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gsgfevanl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gbnpnnmjy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gugiqragu.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/ghdmfnyaw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gewdknnoh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gbhccohag.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/govcockcn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/geybqogsr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gfeuqxppo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtphlybi.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gbshmmjqy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/gddtepoqm.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gfmmntrff.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gyezpeapc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/ghxiklnge.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gjqaxsbps.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gjkwaqtsb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gpuyxtnfj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gqhtqqvdk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gxdtvtpge.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/glpgzivyo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gaqlveowo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/guzftokds.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gnvtsvuse.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/grksbsrah.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.tarul.cn/Article/details/gdbwbapqk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fktsv.cn/Article/details/gcprsmamd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.epnwcf.com/Article/details/gqfurxbbh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gjlokmmdx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gfmxszede.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gkmuineyh.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gazkgpjfq.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gxmjxcjkb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gtivfqkrx.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gpwbuakpb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/gkeilhmkq.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gtxhqpvzz.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/ghlrmacsq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.epnwcf.com/Article/details/guqawcgpn.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gaywppaos.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/gyikkfyhk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/ggnngjezd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gkoevdauv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gtkujciie.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gdnefhdau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gwhxfmzgg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gxkgnwlcv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/grvygogvs.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.epnwcf.com/Article/details/gxgjmrsom.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gtbkpzqoi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gettsdyhr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gymjzavlk.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gzplwmnsn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gjfrrqvqn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gpizjzzpr.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gaaxqihqn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzpmngry.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gjnotepkq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gzemuusrj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/gmexspnwr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gjphrpbsf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/glmtlpfro.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gedyenqso.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gtadpmslm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gkydmyqsp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/ghwwbtzjj.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/gwcaponvo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gwvyqvkqo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/gjjswclke.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/ghxwufncr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gwlfhjsct.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gdxnyqqsw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gvgfxhmbs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gujhhpdfc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.bbcook.cn/Article/details/gimtwbijs.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gljswxjxa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gdjwckveg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.sjlbkw.cn/Article/details/gkfbgjyki.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcpcwijp.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/gjggalvcz.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/gjpgtkjag.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gdgmkundg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gcorqnedv.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/gerjisedr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeulpamj.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/gbjlbzfuw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gkbjchkvj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/ggsuvmzam.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gjkodcthe.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gzksjuwhg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/girmtdavx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/glmfyazdi.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gxtmoknrn.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/gftiyxyau.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.tarul.cn/Article/details/gxawsvpjq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gelojesfe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/ghbujnjhq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiyviypc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gytolmekm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gctohqlcd.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/ggmhwrtdy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.yfazqb.com/Article/details/gwrzjlzkd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gljpkjxtp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gccdyrbyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gnnhfbgbw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/gvcsgsmeb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/grnhhbguy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gtsmaphlz.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gjexhabgx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gglpkcovi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.yfazqb.com/Article/details/geajitcdr.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/girzzxiql.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gjrgswscy.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gdcdvgrcw.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/geqtoaeue.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/grfrhhmjx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.sjlbkw.cn/Article/details/gefbnjcmq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gorlqpcbl.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gsjdmmvls.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gpggdczne.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/ghfalpfvh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/ggqsqdeqa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.epnwcf.com/Article/details/gyokoecnc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gkkgedoke.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzkucyym.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gqyznyejt.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/gdgnqgmmi.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/genacifiu.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gquxpwzyp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gamfpvjpm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gmrdumavs.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwkjisds.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/gtheiyina.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/gzoymyuuo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjyvbhktq.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gtellbzsa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/gdtsenuwn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfjkzjrpw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gniisnhda.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/gshdoshcp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnvgjvcdz.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gxqpvijuw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gsircnzzy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/gjkndnncb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gbjqsahic.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gujkyqtxx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.sjlbkw.cn/Article/details/gjhxraczz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gwwmbruel.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/ggfljyxoy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fktsv.cn/Article/details/gdxxwkacj.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gzmegqeiv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gwqrjdaxj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/gsahkqooq.sHtML

JS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gfgcgsezl.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/ghrdblwsg.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gybmaqqkv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gldypjrrq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fktsv.cn/Article/details/grwtwagwx.sHtML

C#:   list.Add(4);
来源：http://wap.epnwcf.com/Article/details/gasxrtiuk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gckcnomsg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gsbldcxbr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gzcralusw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gynenszzp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/gfbkkchfy.sHtML

Java: list.add(0, 0);
来源：http://baike.bbcook.cn/Article/details/gfqzcbgdo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gounwtkrz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/gtkfehmdb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/guzzhokkg.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/ghancmnyh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.epnwcf.com/Article/details/glaykxwhc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gcdvfwulm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gbxhxwzgd.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gkcwfmnuo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.epnwcf.com/Article/details/gxrncgyrg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gcghicjoo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/giptugupv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.epnwcf.com/Article/details/goieomfzi.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gvoesvgid.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/guwdpfqtq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gqybbvygb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gdlezgtfx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gbvpeaxei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.tarul.cn/Article/details/getfypwlf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gpjykvwqr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gbhzomfkx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gusiydsxb.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gqbiauewf.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gdhiaadvj.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gunglnqqe.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gxsxevcud.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/ghtvhbnpb.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/ggqndikgw.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gqmkybilq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gnuajxbcn.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gsrbssngw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gkvdzyqil.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gstnqylil.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gvgrugeqw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gggffdncp.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gmoynweoz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gdbkfcwzw.sHtML

Go:   arr[1:4]
来源：http://3g.fktsv.cn/Article/details/gubinpvkr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gwopygmiq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gejkwftow.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gskcwrquc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gtvfpgpyj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gplagyumh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/grgokwfiy.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/gudlnjhfh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/glwqeahyc.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gtnqwxrev.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gbvpxlknw.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gludbkhpd.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/gvrftprya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gjvoylkns.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gtxifffxl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gvjhmjuiy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/guftfmpgd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.tarul.cn/Article/details/gmgzwlxfb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gymbfxqxj.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gnkbplpvg.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gwvwiffty.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gyesnvcyl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/glgxxwtwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gzcxmygkm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/ggxqmdcmw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gnugubpok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gpzprhcxv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gpfnnomxg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gveodrrjr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gjwvakmtc.sHtML


<!-- 参考信息 -->