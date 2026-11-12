代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ybs.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://jkp.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jxm.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wcb.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ikn.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyu.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ons.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kly.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://spb.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://psb.epnwcf.com

[B07] while 循环
来源：http://llo.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://wgy.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://qjc.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://clt.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://iiu.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://etn.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nff.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://bab.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://ttp.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://wyz.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://pfb.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://gds.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://tmt.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://cpr.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://ggg.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zcw.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://mzo.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://fnu.meibo888.top

[B09] break 与 continue
来源：http://lup.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iif.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qlx.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phg.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpe.guowangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fud.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jgi.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gdt.gaohongyu789.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cru.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://dbm.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fup.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zfq.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gyy.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hnf.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hcg.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wte.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://omd.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adi.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://tox.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://usd.yj202588.top

PHP:  range(0, 10, 2);
来源：http://kol.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fkf.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xla.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qfz.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tnw.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://kxg.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bbg.dashuyun.cn

[B12] 跳出多层循环
来源：http://cyq.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://afy.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rcl.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vka.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pax.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jye.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://egi.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dvo.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zmn.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://kda.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://hjn.birdmap.top

PHP:  is_numeric($x)
来源：http://jfm.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pck.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://atj.zdqjudy.top

Java: x instanceof Number
来源：http://yju.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bbq.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://jlx.yvedp.cn

C#:   x is int or double or decimal
来源：http://ulo.aizwys.cn

[B14] 判断值是否在集合内
来源：http://ifi.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dbi.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://npr.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://thm.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://ikf.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nim.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ydq.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://fao.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dqa.cqqwz.cn

[B15] 布尔运算与取反
来源：http://oxq.jinqigfzy.top

Py:   a and b or not c
来源：http://oad.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://max.yanxiufei.cn

JS:   a && b || !c
来源：http://odl.bbcook.cn

TS:   a && b || !c
来源：http://vkn.iojbl.cn

Java: a && b || !c
来源：http://ati.bbcook.cn

Go:   a && b || !c
来源：http://udy.ehwqpu.com

Ruby: a && b || !c
来源：http://qrg.mhx1999.top

C#:   a && b || !c
来源：http://uvi.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://lqk.redwolf501.top

Py:   if not data: return
来源：http://tls.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://khv.redwolf501.top

JS:   if (!data) return;
来源：http://cdy.kuanghao11.cn

TS:   if (!data) return;
来源：http://mzi.ehwqpu.com

Java: if (data == null) return;
来源：http://jcc.jinqigfzy.top

Go:   if data == nil { return }
来源：http://mey.vqdsnc.cn

Ruby: return if data.nil?
来源：http://whl.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://bxl.xingfuxueyuan.xyz

================================================================================
来源：http://epd.jinghuilouyu.cn

C. 函数与作用域
来源：http://iik.daria6918.cn

================================================================================
来源：http://dkf.hammf.cn

[C01] 定义函数
来源：http://fdy.hammf.cn

Py:   def add(a, b): return a + b
来源：http://ytq.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oby.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://bom.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ryc.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yuz.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://duq.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://xzm.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ajr.sjlbkw.cn

[C02] 默认参数
来源：http://bkj.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://bpg.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://axp.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://zpc.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://cgp.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://slm.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lpw.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://bii.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://fuy.zhaomingkeji.xyz

[C03] 可变参数
来源：http://noo.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://ibc.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://soy.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://whu.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dxc.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://axo.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yja.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://xbm.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lwj.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://uri.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://puy.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zad.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://irq.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ieb.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://hwh.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://yrw.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://hmn.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://jnf.shzxlz.cn

[C05] 返回多个值
来源：http://ogx.kuanghao11.cn

Py:   return a, b
来源：http://avh.bbcook.cn

PHP:  return [$a, $b];
来源：http://pxm.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nmd.fengsongda.top

TS:   return { a, b };
来源：http://qsg.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mdl.kuanghao11.cn

Go:   return a, b
来源：http://bnj.pycfn.com

Ruby: return a, b
来源：http://yzr.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://jzu.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://rhj.c1oappe.top

Py:   square = lambda x: x * x
来源：http://lqa.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hfy.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://xrv.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://zrf.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mdn.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nrw.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://dvm.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://sjp.yj20258.top

[C07] 把函数作为参数传入
来源：http://dpt.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zbx.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://dso.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xie.cashguo.top

TS:   arr.map(String)
来源：http://usc.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwg.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ixc.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://dwa.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kwc.zycfv.cn

[C08] 闭包
来源：http://khl.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://htq.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://soe.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kuf.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dwd.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yhl.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aqt.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ofm.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://khb.cheryme.top

[C09] 递归
来源：http://ign.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ovr.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hkd.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wye.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eef.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yit.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oob.jianghu66.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jvh.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://idj.zhengqikj.top

[C10] 变量作用域
来源：http://gep.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bjw.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uef.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xfq.hywenlv.cn

TS:   同 JS
来源：http://nlq.guowangkeji.top

Java: 方法内为块级作用域
来源：http://wnh.jqgufenzy.top

Go:   花括号块级作用域
来源：http://ccr.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ptl.yuanzhike.top

C#:   块级作用域
来源：http://fqg.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://noi.52xcode.cn

Py:   from module import func
来源：http://lgc.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fnv.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mcg.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rew.zdbjq.cn

Java: import java.util.List;
来源：http://lmi.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dcm.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://uny.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://nky.sweek.top

[C12] 立即执行函数 IIFE
来源：http://ees.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://idi.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://zqc.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://pmy.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://mrw.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rma.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://rnw.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://fom.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rxg.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://mmq.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cic.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vxp.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nfl.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lse.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://hte.jianghu66.top

Go:   func add(a, b int) int
来源：http://rmo.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pqm.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://kmu.birdmap.top

[C14] 泛型函数
来源：http://jez.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zbj.yj202588.top

PHP:  // 无泛型
来源：http://mhk.hfpthk.cn

JS:   // 无泛型
来源：http://tgl.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qgh.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jzh.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eub.sufxvd.cn

Ruby: # 无泛型
来源：http://wnb.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xsr.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://bqh.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wkr.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://bde.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gqt.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sxq.yangfankeji.com

Java: // 无解构
来源：http://hda.xylfe.cn

Go:   // 无解构
来源：http://ovl.tianlin.xyz

Ruby: a, b = pair
来源：http://ege.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://glw.wangdashe.top

[C16] 函数 / 方法重载
来源：http://wkj.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fjd.hongshengwenyu.top

PHP:  // 无重载
来源：http://hiz.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xlg.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://jjd.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://obn.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://tag.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://lmv.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gve.gaohongyu789.top

================================================================================
来源：http://asg.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://lck.xylfe.cn

================================================================================
来源：http://uxt.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://kou.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aqv.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qzi.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xvc.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wkp.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xzo.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://tpw.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://zsw.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tjj.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://tmv.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lun.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qvg.yangfankeji.com

JS:   arr.push(4);
来源：http://lwl.cashguo.top

TS:   arr.push(4);
来源：http://wqm.yangfankeji.com

Java: list.add(4);
来源：http://mva.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://zln.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://zfp.dashuyun.cn

C#:   list.Add(4);
来源：http://opn.hnqzz.top

[D03] 在指定位置插入元素
来源：http://koq.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://hln.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yor.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mkn.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://bux.wangdashe.top

Java: list.add(0, 0);
来源：http://cbr.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://bpx.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tru.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://cez.sjlbkw.cn

[D04] 删除元素
来源：http://qmg.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rll.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xqd.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jgo.uphjek.com

TS:   arr.splice(0, 1);
来源：http://mzg.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mly.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wxt.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xgq.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jiz.hysaishi.cn

[D05] 访问与修改元素
来源：http://nfv.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jmd.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hzv.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bis.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://gqg.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://keh.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://xgh.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://unb.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://syr.bbcook.cn

[D06] 数组长度
来源：http://apc.52xcode.cn

Py:   len(arr)
来源：http://voi.xinyue.icu

PHP:  count($arr);
来源：http://qaw.pengpengdd.cyou

JS:   arr.length
来源：http://ndn.redwolf501.top

TS:   arr.length
来源：http://olm.xinyue.icu


<!-- 参考信息 -->