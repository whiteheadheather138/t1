代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agh.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://csl.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hxf.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ybd.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ygk.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epr.jinghuilouyu.cn

[B07] while 循环
来源：http://xcg.ivvv.top

Py:   while i < 10: i += 1
来源：http://uzq.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zfe.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://klf.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://bbz.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://mbb.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://msq.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://ums.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://zzk.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://hok.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://rie.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://ndi.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://jat.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://qmt.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://qvv.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yel.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://wlp.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://rda.feifeiyinyue.top

[B09] break 与 continue
来源：http://kqr.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lte.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vuu.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnk.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmw.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lok.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cko.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mvp.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwm.yuxming.cn

[B10] 遍历同时拿索引
来源：http://tem.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sxl.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bsd.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gcw.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hib.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sem.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yin.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lfj.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hbk.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://rql.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://ots.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://qxd.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://orm.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vit.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eru.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hvc.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://cjd.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vuu.tian-w.cn

[B12] 跳出多层循环
来源：http://igh.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zrr.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nno.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cna.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jyh.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://isf.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://slo.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejz.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pwk.ppjwa.cn

[B13] 判断是否为数字
来源：http://etp.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://afg.epnwcf.com

PHP:  is_numeric($x)
来源：http://rux.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aty.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ndi.sweek.top

Java: x instanceof Number
来源：http://zoa.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://awy.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://rgp.andypj.xyz

C#:   x is int or double or decimal
来源：http://bix.smart0.xyz

[B14] 判断值是否在集合内
来源：http://ova.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qgw.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xpw.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://wqf.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://ebv.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://owu.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zms.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ywq.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cqt.shzxlz.cn

[B15] 布尔运算与取反
来源：http://ith.hysaishi.cn

Py:   a and b or not c
来源：http://lrh.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://nbm.yfazqb.com

JS:   a && b || !c
来源：http://tjw.kuanghao11.cn

TS:   a && b || !c
来源：http://qki.xuanzx.com

Java: a && b || !c
来源：http://hcn.uphjek.com

Go:   a && b || !c
来源：http://fze.zdbjq.cn

Ruby: a && b || !c
来源：http://urt.hcnkem.com

C#:   a && b || !c
来源：http://pdq.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://jnt.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://fxn.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://hgn.mhx1999.top

JS:   if (!data) return;
来源：http://kvr.316326.xyz

TS:   if (!data) return;
来源：http://crw.zhiwuduotai.top

Java: if (data == null) return;
来源：http://fal.smart0.xyz

Go:   if data == nil { return }
来源：http://kmh.zhixingplan.top

Ruby: return if data.nil?
来源：http://sga.yonumen.top

C#:   if (data == null) return;
来源：http://jnq.yanxiufei.cn

================================================================================
来源：http://ujr.sxryk.cn

C. 函数与作用域
来源：http://zmg.316326.xyz

================================================================================
来源：http://pfy.feifeiyinyue.top

[C01] 定义函数
来源：http://nog.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://gqt.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nfe.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://nto.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eqn.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cvx.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://qkk.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://btc.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jks.quarkkingdee.top

[C02] 默认参数
来源：http://eff.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://xmf.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fyz.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://rcg.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yvv.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://cae.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gft.shzxlz.cn

Ruby: def greet(name = "World") = name
来源：http://eyf.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://pjv.ywan-chungtsiang.top

[C03] 可变参数
来源：http://gff.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://lzv.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vqr.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://coi.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jfx.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://etm.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fnn.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://imn.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vmx.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://pja.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hlo.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sjd.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwu.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bvw.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://txs.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://zyv.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://jte.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://lne.gogol.net.cn

[C05] 返回多个值
来源：http://btu.redwolf501.top

Py:   return a, b
来源：http://kpv.hammf.cn

PHP:  return [$a, $b];
来源：http://krx.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wph.smart0.xyz

TS:   return { a, b };
来源：http://kmr.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hgp.aibaodan.cn

Go:   return a, b
来源：http://mqs.yangfankeji.com

Ruby: return a, b
来源：http://ekm.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://srz.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://ijt.cucudq.cn

Py:   square = lambda x: x * x
来源：http://azv.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ggc.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://gib.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://ojk.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bgy.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://kmh.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://ost.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lno.zycfv.cn

[C07] 把函数作为参数传入
来源：http://wxt.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wwb.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://sbd.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dbm.xinyue.icu

TS:   arr.map(String)
来源：http://xkt.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zlj.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wsl.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://aai.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qmp.zdqjudy.top

[C08] 闭包
来源：http://hsc.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ccu.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xeu.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://icc.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oxf.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xrc.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wsr.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jbo.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jgu.xylfe.cn

[C09] 递归
来源：http://jzv.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://skx.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fpu.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://atl.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mfn.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jyl.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kth.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hqc.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://obb.wangshuangyany.cn

[C10] 变量作用域
来源：http://dgu.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qub.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lch.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gvh.shanyushiyangkeji.top

TS:   同 JS
来源：http://poq.dianchejie.cn

Java: 方法内为块级作用域
来源：http://rul.pycfn.com

Go:   花括号块级作用域
来源：http://sqc.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://inv.sufxvd.cn

C#:   块级作用域
来源：http://gwm.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://oja.chenlongwang.top

Py:   from module import func
来源：http://dlt.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hop.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xax.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ayl.chenzaomai.com

Java: import java.util.List;
来源：http://hza.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qaz.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://iib.jqgfzy.top

C#:   using System.Text;
来源：http://vpl.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://xpb.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://gyj.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://lan.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://dhg.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://ocz.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nwu.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://qlb.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://fgx.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bce.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://wzv.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wki.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xgr.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lla.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ave.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://dci.meibo888.top

Go:   func add(a, b int) int
来源：http://ous.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://axa.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://hxo.nanxuanxn.top

[C14] 泛型函数
来源：http://etm.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lkg.fehbvm.com

PHP:  // 无泛型
来源：http://hxd.ydjk.org.cn

JS:   // 无泛型
来源：http://jxs.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hbr.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nzs.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sgm.gaohongyu789.top

Ruby: # 无泛型
来源：http://erx.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ypc.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://snd.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhm.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://qbl.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xnp.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yog.zhiwuduotai.top

Java: // 无解构
来源：http://xdm.svipenyu.cn

Go:   // 无解构
来源：http://amb.hcnkem.com

Ruby: a, b = pair
来源：http://pwl.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://kch.hesvh.cn

[C16] 函数 / 方法重载
来源：http://zmm.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://klw.uphjek.com

PHP:  // 无重载
来源：http://siq.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xig.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://gsm.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ihh.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://whw.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://sbv.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wor.zhixingplan.top

================================================================================
来源：http://uif.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://nhu.zhiwuduotai.top

================================================================================
来源：http://sdg.c1oappe.top

[D01] 创建数组 / 列表
来源：http://zor.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pjx.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://idd.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xzo.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qmt.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gsm.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://wfl.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://sgd.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zyb.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://akx.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iwx.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ntx.zdqjudy.top

JS:   arr.push(4);
来源：http://rgo.guowangkeji.top

TS:   arr.push(4);
来源：http://xrz.fanxiaobao.xyz

Java: list.add(4);
来源：http://ocf.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://igb.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://mbg.0kj1m.cn

C#:   list.Add(4);
来源：http://shx.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://cif.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://hun.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sjd.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lem.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://ojo.yj20258.top

Java: list.add(0, 0);
来源：http://mlq.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://ski.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nsc.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://cvs.andypj.xyz

[D04] 删除元素
来源：http://uoy.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fhw.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pwf.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fmt.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://opq.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eak.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rve.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dew.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mns.c1oappe.top

[D05] 访问与修改元素
来源：http://ofe.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xkh.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rrp.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lfq.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://ggl.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://dqq.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://kwa.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hwk.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tew.jinqigfzy.top

[D06] 数组长度
来源：http://adk.jinghuilouyu.cn

Py:   len(arr)
来源：http://syi.gotoacloud.top

PHP:  count($arr);
来源：http://cyc.hcnkem.com

JS:   arr.length
来源：http://boa.epnwcf.com

TS:   arr.length
来源：http://dxe.hnqzz.top

Java: list.size();
来源：http://wcg.bjfxy.top

Go:   len(arr)
来源：http://rnf.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://wdt.sysykeji.top

C#:   list.Count;
来源：http://nba.xuetiantiany.cn


<!-- 参考信息 -->