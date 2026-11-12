代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://xrm.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bad.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ukb.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://llw.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://doz.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://axw.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ngj.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://npk.fehbvm.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wkb.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tdi.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://izj.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cws.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rqd.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lmu.gogol.net.cn

[B07] while 循环
来源：http://wmf.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://yut.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://qsg.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://clr.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://yoz.tarul.cn

Java: while (i < 10) { i++; }
来源：http://bfh.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tyx.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://kax.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://pvz.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://qsg.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://vdv.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jnx.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://snl.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://qgi.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://srj.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jcd.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://qzp.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://fxs.zhixingplan.top

[B09] break 与 continue
来源：http://lzp.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aad.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ims.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcj.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goo.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhg.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dju.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bmw.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aow.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://faq.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qfb.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jet.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pdu.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tnr.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kef.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mrx.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dpl.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rwq.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://aro.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://lco.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://kiz.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxm.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pbs.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zdu.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yeo.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://qaq.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ehn.fzhhl.top

[B12] 跳出多层循环
来源：http://hlr.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fhv.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dys.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uwx.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vpb.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tfd.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cqt.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eub.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jgb.birdmap.top

[B13] 判断是否为数字
来源：http://vpj.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://prz.svipenyu.cn

PHP:  is_numeric($x)
来源：http://pux.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://syq.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdp.xuetiantiany.cn

Java: x instanceof Number
来源：http://iyc.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gkd.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://aqk.yuanzhike.top

C#:   x is int or double or decimal
来源：http://zay.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://vsa.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ggf.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hls.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://eej.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://fxj.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cve.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zmq.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://iqc.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eat.uphjek.com

[B15] 布尔运算与取反
来源：http://nxh.guannengcc.top

Py:   a and b or not c
来源：http://uac.bbcook.cn

PHP:  $a && $b || !$c
来源：http://ree.dashuyun.cn

JS:   a && b || !c
来源：http://jtl.cashguo.top

TS:   a && b || !c
来源：http://bsl.smart0.xyz

Java: a && b || !c
来源：http://jvx.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://cwu.ctjpmb.com

Ruby: a && b || !c
来源：http://ixn.cdnleiting.top

C#:   a && b || !c
来源：http://yza.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ykl.nwbrower.top

Py:   if not data: return
来源：http://ezp.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://qpv.epnwcf.com

JS:   if (!data) return;
来源：http://qsc.xuetiantiany.cn

TS:   if (!data) return;
来源：http://shz.feifeiyinyue.top

Java: if (data == null) return;
来源：http://sju.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://rox.andypj.xyz

Ruby: return if data.nil?
来源：http://mgx.hnqzz.top

C#:   if (data == null) return;
来源：http://rla.yj20258.top

================================================================================
来源：http://tth.vehdjk.com

C. 函数与作用域
来源：http://maz.jinyuanbaomall.cn

================================================================================
来源：http://ipk.dianchejie.cn

[C01] 定义函数
来源：http://ftq.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://vqu.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hov.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://udv.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwr.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zsv.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://syd.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://cav.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rmq.zhiwuduotai.top

[C02] 默认参数
来源：http://ucc.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://tfj.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bpk.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://feb.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iot.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mcj.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://idl.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://mou.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://ffd.tanke756.top

[C03] 可变参数
来源：http://knw.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://diq.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eek.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwb.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cob.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ztj.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ohx.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nqh.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://evt.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://dfm.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://frb.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hlz.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kxu.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ubr.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://jdj.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://iiy.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://rse.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://iiq.316326.xyz

[C05] 返回多个值
来源：http://nij.pengpengdd.cyou

Py:   return a, b
来源：http://wiw.aibaodan.cn

PHP:  return [$a, $b];
来源：http://myl.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oux.hongshengwenyu.top

TS:   return { a, b };
来源：http://vvv.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://klg.yj202588.top

Go:   return a, b
来源：http://qtp.hywenlv.cn

Ruby: return a, b
来源：http://bvq.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://jdn.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://pof.tian-w.cn

Py:   square = lambda x: x * x
来源：http://jms.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vhz.yuxming.cn

JS:   const square = x => x * x;
来源：http://frf.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://mgm.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uji.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://hex.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://lej.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://vdk.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://kce.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rml.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://unc.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uhj.hfpthk.cn

TS:   arr.map(String)
来源：http://jhq.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gmn.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rkr.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://gsh.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zhc.zhijiandao.cn

[C08] 闭包
来源：http://ogu.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xuz.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jme.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://let.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gyx.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zen.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hyv.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aau.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wdd.ehwqpu.com

[C09] 递归
来源：http://nvk.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pbn.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kxr.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://atm.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://neg.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pdo.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vbg.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ylq.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xgk.tianlin.xyz

[C10] 变量作用域
来源：http://hka.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rhu.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://byn.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cju.ivvv.top

TS:   同 JS
来源：http://jeg.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://jrx.jyoumei.cn

Go:   花括号块级作用域
来源：http://eqe.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dqm.fktsv.cn

C#:   块级作用域
来源：http://gwb.cashguo.top

[C11] 模块导入与导出
来源：http://ego.jinqigufen.top

Py:   from module import func
来源：http://lyf.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ngj.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qar.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cjf.jlsjyb.cn

Java: import java.util.List;
来源：http://xad.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wgi.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ymz.nanxinkj.top

C#:   using System.Text;
来源：http://zqb.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://was.ivvv.top

Py:   (lambda: print("run"))()
来源：http://iik.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://dqd.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://plr.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://mrv.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qsm.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://qtz.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://sem.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ppe.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://fey.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mek.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://urn.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nsg.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://med.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://bkr.ehwqpu.com

Go:   func add(a, b int) int
来源：http://bco.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vsp.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vzj.zdbjq.cn

[C14] 泛型函数
来源：http://ohq.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://agj.wangshuangyany.cn

PHP:  // 无泛型
来源：http://emx.yanxiufei.cn

JS:   // 无泛型
来源：http://ejb.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vnv.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kgi.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ksb.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://xub.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kwl.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://yku.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oky.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://eao.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ofn.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zzq.ywan-chungtsiang.top

Java: // 无解构
来源：http://zvm.hammf.cn

Go:   // 无解构
来源：http://dvg.guowangkeji.top

Ruby: a, b = pair
来源：http://uyg.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://qdt.mhx1999.top

[C16] 函数 / 方法重载
来源：http://rfd.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yzi.smart0.xyz

PHP:  // 无重载
来源：http://eey.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ykd.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://qlu.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rqw.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://ylj.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://plx.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://krm.sufxvd.cn

================================================================================
来源：http://kem.yongpay.top

D. 数组 / 列表 / 集合
来源：http://rfi.birdmap.top

================================================================================
来源：http://fdn.xinyue.icu

[D01] 创建数组 / 列表
来源：http://sjh.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vmw.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://buy.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vyx.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://amg.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qic.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://hxu.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://hqg.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tne.nwbrower.top

[D02] 追加元素到末尾
来源：http://tqu.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tpv.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gwk.birdmap.top

JS:   arr.push(4);
来源：http://xax.nanxuanxn.top

TS:   arr.push(4);
来源：http://nld.zhongyouzk.top

Java: list.add(4);
来源：http://csv.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://zme.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://mht.0kj1m.cn

C#:   list.Add(4);
来源：http://zns.yj20258888.top

[D03] 在指定位置插入元素
来源：http://cfb.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://btr.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rwa.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ssn.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://zzo.uphjek.com

Java: list.add(0, 0);
来源：http://vxk.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://onj.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bka.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://nne.gaohongyu789.top

[D04] 删除元素
来源：http://zpa.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wdi.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bzv.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://scz.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://hdz.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ppx.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhf.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yfp.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mab.ivvv.top

[D05] 访问与修改元素
来源：http://rdv.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://irb.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zci.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kzt.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mwt.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://vgu.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://ywf.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yzc.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ibq.epnwcf.com

[D06] 数组长度
来源：http://xyo.wangshuangyany.cn


<!-- 参考信息 -->