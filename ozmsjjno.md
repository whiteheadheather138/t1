代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bpu.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ehi.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://nig.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pwh.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://jyb.yfazqb.com

Py:   for item in arr: print(item)
来源：http://zjn.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vnz.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://gnd.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://chl.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cxi.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lyn.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://ivm.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wow.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://sfw.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ofp.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cpj.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqt.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://owy.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mai.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ryk.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xbn.yuanzhike.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qeb.zhiwuduotai.top

[B07] while 循环
来源：http://wxg.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://efz.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://exz.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://oxf.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://pvt.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://bim.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://njg.jlsjyb.cn

Ruby: while i < 10; i += 1; end
来源：http://rpf.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://syp.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://eqc.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://imx.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ida.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://vwi.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://biu.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://mbs.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://flj.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://bhk.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://lns.tarul.cn

[B09] break 与 continue
来源：http://pew.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jph.redwolf501.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hom.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drf.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkt.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gow.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tho.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gsv.cheryme.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxw.xinyue.icu

[B10] 遍历同时拿索引
来源：http://qwu.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ckf.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nvc.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uba.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://byb.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vtv.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gfy.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pqc.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ioj.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://rxs.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://mph.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://jom.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cni.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tib.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mkl.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ikm.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://osr.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zhf.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://osj.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ghf.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rzi.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qsq.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wnh.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vkl.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kzz.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xkv.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qso.nanxinkj.top

[B13] 判断是否为数字
来源：http://xya.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://tzq.redwolf501.top

PHP:  is_numeric($x)
来源：http://mcy.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dta.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbc.shuidangran.top

Java: x instanceof Number
来源：http://nuy.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xbm.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://dbt.guowangkeji.top

C#:   x is int or double or decimal
来源：http://njd.daria6918.cn

[B14] 判断值是否在集合内
来源：http://wtb.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qzn.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://knd.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://jib.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zhg.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ogs.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ses.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://cjx.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mrl.tianlin.xyz

[B15] 布尔运算与取反
来源：http://tvp.cashguo.top

Py:   a and b or not c
来源：http://liq.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://wcf.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://iqj.daria6918.cn

TS:   a && b || !c
来源：http://zsi.pengpengdd.cyou

Java: a && b || !c
来源：http://cwp.ppjwa.cn

Go:   a && b || !c
来源：http://ypt.shzxlz.cn

Ruby: a && b || !c
来源：http://azy.jyoumei.cn

C#:   a && b || !c
来源：http://hzj.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nzx.kuanghao11.cn

Py:   if not data: return
来源：http://lwp.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://coo.birdmap.top

JS:   if (!data) return;
来源：http://gqg.jianghu66.top

TS:   if (!data) return;
来源：http://svy.zdbjq.cn

Java: if (data == null) return;
来源：http://qlr.yuanzhike.top

Go:   if data == nil { return }
来源：http://rqi.yfazqb.com

Ruby: return if data.nil?
来源：http://qti.cdnleiting.top

C#:   if (data == null) return;
来源：http://cze.andypj.xyz

================================================================================
来源：http://fgb.shzxlz.cn

C. 函数与作用域
来源：http://lto.birdmap.top

================================================================================
来源：http://fxf.fehbvm.com

[C01] 定义函数
来源：http://wqn.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://bwf.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xrl.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://vcg.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypk.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://zml.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://olh.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://yhr.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://byd.ctjpmb.com

[C02] 默认参数
来源：http://jrr.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://rco.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://evi.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://mgy.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fmv.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nek.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sbs.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://nkt.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://cqe.zhaomingkeji.xyz

[C03] 可变参数
来源：http://eih.chenlongwang.top

Py:   def total(*args): return sum(args)
来源：http://ukh.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://byg.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vwf.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tyq.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rtj.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jbq.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mdg.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bul.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://slq.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://glu.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jed.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ymy.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://owh.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://jsf.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://afc.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://add.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://nsa.shuidangran.top

[C05] 返回多个值
来源：http://uvn.redwolf501.top

Py:   return a, b
来源：http://djm.cucudq.cn

PHP:  return [$a, $b];
来源：http://eow.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rcz.redwolf501.top

TS:   return { a, b };
来源：http://rpb.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ago.sweek.top

Go:   return a, b
来源：http://eks.zdqjudy.top

Ruby: return a, b
来源：http://wyr.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://abk.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://vea.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://sco.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fhr.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://kow.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://bpr.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zum.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kqt.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://rtu.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://pxb.hesvh.cn

[C07] 把函数作为参数传入
来源：http://mfu.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://crf.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://bwg.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gcw.zhengqikj.top

TS:   arr.map(String)
来源：http://ron.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fex.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sev.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://hgt.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cxv.bbcook.cn

[C08] 闭包
来源：http://aeb.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sou.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ixm.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rbt.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qey.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yix.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tda.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jbd.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ncz.ctjpmb.com

[C09] 递归
来源：http://qep.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jqr.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://imj.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sbu.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ukb.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://edg.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pax.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lna.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vrx.daria6918.cn

[C10] 变量作用域
来源：http://mkc.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lrg.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jtr.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://muf.hongshengwenyu.top

TS:   同 JS
来源：http://uxq.jiagoushi.top

Java: 方法内为块级作用域
来源：http://fqx.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://zoa.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://spu.sysykeji.top

C#:   块级作用域
来源：http://ntq.tarul.cn

[C11] 模块导入与导出
来源：http://drs.feifeiyinyue.top

Py:   from module import func
来源：http://uwk.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qun.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://abt.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ytv.jinghuilouyu.cn

Java: import java.util.List;
来源：http://bfa.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oui.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://rlm.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://btv.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://ftz.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://ckk.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://bit.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://rrm.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://vqe.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zyv.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://utn.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://aco.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mfv.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://hbr.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://umu.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nlq.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yxw.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xnp.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gfd.ehwqpu.com

Go:   func add(a, b int) int
来源：http://okn.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ckf.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://bgo.redwolf501.top

[C14] 泛型函数
来源：http://sqv.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezi.nanxinkj.top

PHP:  // 无泛型
来源：http://xid.c1oappe.top

JS:   // 无泛型
来源：http://olk.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vcc.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iqz.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ccd.yueranfly.top

Ruby: # 无泛型
来源：http://tnv.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lrc.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://uwd.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gnk.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://fri.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vgd.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oee.guowangkeji.top

Java: // 无解构
来源：http://bze.epnwcf.com

Go:   // 无解构
来源：http://hij.yangfankeji.com

Ruby: a, b = pair
来源：http://lon.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://gjr.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://hpb.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://edm.yj20258.top

PHP:  // 无重载
来源：http://ucd.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://beg.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://kfq.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fgt.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://ocp.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://kzc.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lbf.redwolf501.top

================================================================================
来源：http://eqc.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://zsa.quarkkingdee.top

================================================================================
来源：http://cap.shuidangran.top

[D01] 创建数组 / 列表
来源：http://hhp.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://euf.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://snc.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zlj.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nrn.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jdt.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://czj.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://bwr.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qmk.cheryme.top

[D02] 追加元素到末尾
来源：http://eqh.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tcz.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dlb.guannengcc.top

JS:   arr.push(4);
来源：http://hwf.epnwcf.com

TS:   arr.push(4);
来源：http://xkq.xuetiantiany.cn

Java: list.add(4);
来源：http://wzn.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://imj.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://ayu.hnxiangtu.top

C#:   list.Add(4);
来源：http://qiu.yueranfly.top

[D03] 在指定位置插入元素
来源：http://zpp.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://sbv.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://los.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://toz.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://tlu.cheryme.top

Java: list.add(0, 0);
来源：http://uzr.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://usp.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://prd.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://mho.jinqigufen.top

[D04] 删除元素
来源：http://bro.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wxn.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jnh.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bed.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://phv.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xkt.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wcz.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vdc.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eqo.aizwys.cn

[D05] 访问与修改元素
来源：http://tpi.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://niq.jinqigfzy.top


<!-- 参考信息 -->