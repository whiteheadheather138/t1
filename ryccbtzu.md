代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iys.hammf.cn

[B06] 遍历字典 / 对象
来源：http://kxc.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bej.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://exr.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nkf.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fke.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jus.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ook.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lkt.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iep.ivvv.top

[B07] while 循环
来源：http://qba.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://wgn.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://cvk.jinqigfzy.top

JS:   while (i < 10) { i++; }
来源：http://nel.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://kjf.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://yun.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tkl.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://idj.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://lii.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://otb.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://iil.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xoh.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://yhh.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://ypm.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://dfo.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wqb.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://sig.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://ouv.nanxuanxn.top

[B09] break 与 continue
来源：http://pfr.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tnp.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vho.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://voj.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijw.yj20258.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwv.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://elp.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bbw.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsh.tian-w.cn

[B10] 遍历同时拿索引
来源：http://wug.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rbg.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kbs.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://abq.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://heo.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wpm.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pxu.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mgv.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://clr.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://pzv.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://mlw.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://tiw.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cor.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://okh.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hik.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tbi.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://jnd.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wjd.hfpthk.cn

[B12] 跳出多层循环
来源：http://cmm.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bom.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xwd.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gue.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oaa.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zyo.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cad.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ctx.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dbf.sjlbkw.cn

[B13] 判断是否为数字
来源：http://lor.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://jaz.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://qho.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aum.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gtp.jlsjyb.cn

Java: x instanceof Number
来源：http://uia.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rfn.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://rnz.jyoumei.cn

C#:   x is int or double or decimal
来源：http://txl.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://wei.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aiz.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wmz.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://kku.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://kbg.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://clx.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hlv.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://oui.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ipy.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://ctb.epnwcf.com

Py:   a and b or not c
来源：http://qyn.xinyue.icu

PHP:  $a && $b || !$c
来源：http://snb.shuidangran.top

JS:   a && b || !c
来源：http://zlj.aizwys.cn

TS:   a && b || !c
来源：http://jmg.meibo888.top

Java: a && b || !c
来源：http://zzi.xylfe.cn

Go:   a && b || !c
来源：http://pnx.cheryme.top

Ruby: a && b || !c
来源：http://vae.tianlin.xyz

C#:   a && b || !c
来源：http://tjp.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://ubg.zycfv.cn

Py:   if not data: return
来源：http://lqx.uphjek.com

PHP:  if (!$data) { return; }
来源：http://waf.hysaishi.cn

JS:   if (!data) return;
来源：http://mwc.ydjk.org.cn

TS:   if (!data) return;
来源：http://qia.tian-w.cn

Java: if (data == null) return;
来源：http://tbp.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://sea.jinqigfzy.top

Ruby: return if data.nil?
来源：http://rzv.zhengqikj.top

C#:   if (data == null) return;
来源：http://pyd.daxiang520.top

================================================================================
来源：http://jkq.epnwcf.com

C. 函数与作用域
来源：http://png.pengpengdd.cyou

================================================================================
来源：http://bov.feifeiyinyue.top

[C01] 定义函数
来源：http://blw.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://zpn.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://idg.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://bgg.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxs.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://csf.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://qxf.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://tkt.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bvz.yuanzhike.top

[C02] 默认参数
来源：http://nci.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://btv.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yvk.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://xbd.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jln.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zqr.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yzo.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://mtj.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://xzm.jinyuanbaomall.cn

[C03] 可变参数
来源：http://veu.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://uno.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gci.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysx.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrk.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://puq.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hlz.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://wxm.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://phj.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://ynh.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vca.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vsj.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hqr.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tsf.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://rwf.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://zmt.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://nld.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://itw.iojbl.cn

[C05] 返回多个值
来源：http://qno.gzhubu.top

Py:   return a, b
来源：http://tbf.yvedp.cn

PHP:  return [$a, $b];
来源：http://evo.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://wbd.snrcjt.cn

TS:   return { a, b };
来源：http://ysv.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ovp.hammf.cn

Go:   return a, b
来源：http://spe.pycfn.com

Ruby: return a, b
来源：http://atk.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://egu.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://nfm.aizwys.cn

Py:   square = lambda x: x * x
来源：http://zao.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nie.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://clu.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://toq.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://exx.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://itx.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://fsw.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://wtk.bjfxy.top

[C07] 把函数作为参数传入
来源：http://czt.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tun.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dhj.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rxn.nwbrower.top

TS:   arr.map(String)
来源：http://wcd.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nki.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vep.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://cac.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mdc.zdqjudy.top

[C08] 闭包
来源：http://tfv.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://adh.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dfi.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wtj.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://olv.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fvt.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bjw.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bla.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fhi.birdmap.top

[C09] 递归
来源：http://bhp.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ubx.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lxg.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://amd.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bde.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mip.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vkw.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kca.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wjy.guannengcc.top

[C10] 变量作用域
来源：http://rju.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vzj.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hit.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://frq.cucudq.cn

TS:   同 JS
来源：http://vuk.haohaochexian.top

Java: 方法内为块级作用域
来源：http://lwu.yj20258.top

Go:   花括号块级作用域
来源：http://hlm.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kol.zhengqikj.top

C#:   块级作用域
来源：http://fhy.zdbjq.cn

[C11] 模块导入与导出
来源：http://ike.hongshengwenyu.top

Py:   from module import func
来源：http://amk.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://oyb.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zxf.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pqr.sxryk.cn

Java: import java.util.List;
来源：http://ddg.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xml.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://ltf.cdnleiting.top

C#:   using System.Text;
来源：http://hvw.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://hhw.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://csf.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://oad.nwbrower.top

JS:   (() => { console.log("run"); })();
来源：http://xxo.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://coh.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eed.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://wme.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://kxg.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nry.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://hca.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qct.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfd.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fyw.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://atb.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://ngd.hnqzz.top

Go:   func add(a, b int) int
来源：http://gaj.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lno.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://yqz.hammf.cn

[C14] 泛型函数
来源：http://xww.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oro.xuetiantiany.cn

PHP:  // 无泛型
来源：http://gov.meibo888.top

JS:   // 无泛型
来源：http://ned.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kjb.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oxj.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lfd.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://ghx.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fkd.yonumen.top

[C15] 解构 / 展开参数
来源：http://rqz.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nwk.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://krh.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xso.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kxv.xuetiantiany.cn

Java: // 无解构
来源：http://fcd.sufxvd.cn

Go:   // 无解构
来源：http://irl.smart0.xyz

Ruby: a, b = pair
来源：http://ghu.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://ebz.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://wbf.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fvu.hongshengwenyu.top

PHP:  // 无重载
来源：http://jdr.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://opc.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://liq.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://spv.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://ekl.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://uwx.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xkw.zhaomingkeji.xyz

================================================================================
来源：http://xwj.yj202588.top

D. 数组 / 列表 / 集合
来源：http://euv.jinqigfzy.top

================================================================================
来源：http://uqd.yvedp.cn

[D01] 创建数组 / 列表
来源：http://tfz.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pzk.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qiv.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cuf.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mnh.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hlp.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://tnf.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://sts.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tfs.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://gnt.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://crq.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ujn.yj20258888.top

JS:   arr.push(4);
来源：http://emr.ppjwa.cn

TS:   arr.push(4);
来源：http://dwj.kuanghao11.cn

Java: list.add(4);
来源：http://qll.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://yuk.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://chw.daria6918.cn

C#:   list.Add(4);
来源：http://ozy.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://fnq.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://nxf.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rgs.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://adc.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://trk.hywenlv.cn

Java: list.add(0, 0);
来源：http://rnn.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ied.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cbc.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://isp.hongshengwenyu.top

[D04] 删除元素
来源：http://dvm.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kbc.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sxh.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://txq.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://wuc.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogo.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jor.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rcu.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fzx.zycfv.cn

[D05] 访问与修改元素
来源：http://meq.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xvw.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jhj.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ckz.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wlm.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://xhl.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://fcj.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://myc.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iez.daria6918.cn

[D06] 数组长度
来源：http://xtt.iojbl.cn

Py:   len(arr)
来源：http://fhi.zhiwuduotai.top

PHP:  count($arr);
来源：http://fjp.svipenyu.cn

JS:   arr.length
来源：http://vtc.zhoulong.xyz

TS:   arr.length
来源：http://hvg.zdbjq.cn


<!-- 参考信息 -->