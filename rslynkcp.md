代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vbn.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fsc.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://npi.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://spf.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://rkz.sysykeji.top

Py:   for item in arr: print(item)
来源：http://mta.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://riz.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bqg.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sqi.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ztp.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vmx.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://keo.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mkd.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://wvw.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://gcc.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ilv.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjn.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ftz.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zln.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ywd.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ors.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://csu.shuidangran.top

[B07] while 循环
来源：http://mfm.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://hxx.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://hed.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://aeh.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://pvp.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://ypy.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://onf.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://myl.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://dpu.316326.xyz

[B08] do-while（至少执行一次）
来源：http://hcs.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://onw.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://qxh.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://sbk.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://qax.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://wem.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://anq.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://xyi.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://mwu.feifeiyinyue.top

[B09] break 与 continue
来源：http://uaj.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kqt.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jed.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adf.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bel.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkz.cdnleiting.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://akb.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://glz.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrr.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://qvo.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gpq.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eqz.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ldb.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://geh.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gwv.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hpq.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dqm.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xpg.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://bet.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://awl.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://uvs.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wdd.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://frf.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ppl.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rif.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://spo.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hqv.quarkkingdee.top

[B12] 跳出多层循环
来源：http://jpn.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://imh.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ybe.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyf.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tfn.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ofb.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rfn.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ujs.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xnh.0kj1m.cn

[B13] 判断是否为数字
来源：http://tmu.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://key.fzhhl.top

PHP:  is_numeric($x)
来源：http://ian.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dkd.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hhp.xuetiantiany.cn

Java: x instanceof Number
来源：http://opj.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mel.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://lmr.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://hxh.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://zhv.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jya.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jkb.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://icu.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://fgn.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gqu.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fmc.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://sap.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ctq.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://goa.jinqigufen.top

Py:   a and b or not c
来源：http://pck.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://nia.52xcode.cn

JS:   a && b || !c
来源：http://ecb.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://wck.sjlbkw.cn

Java: a && b || !c
来源：http://fba.zhijiandao.cn

Go:   a && b || !c
来源：http://kdn.nanxuanxn.top

Ruby: a && b || !c
来源：http://gbz.dianchejie.cn

C#:   a && b || !c
来源：http://xvt.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://uww.bbcook.cn

Py:   if not data: return
来源：http://nvi.hongshengwenyu.top

PHP:  if (!$data) { return; }
来源：http://vkt.cashguo.top

JS:   if (!data) return;
来源：http://vpk.ppjwa.cn

TS:   if (!data) return;
来源：http://dlo.birdmap.top

Java: if (data == null) return;
来源：http://hdb.fktsv.cn

Go:   if data == nil { return }
来源：http://vmj.jinqigfzy.top

Ruby: return if data.nil?
来源：http://opp.guannengcc.top

C#:   if (data == null) return;
来源：http://fyp.zhengqikj.top

================================================================================
来源：http://pws.52xcode.cn

C. 函数与作用域
来源：http://iod.cqqwz.cn

================================================================================
来源：http://jny.hammf.cn

[C01] 定义函数
来源：http://jso.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://kpj.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvn.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://ndj.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://goi.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rsp.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ltz.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://pmf.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://szs.ehwqpu.com

[C02] 默认参数
来源：http://vso.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://fqd.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ywx.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://dhy.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pnu.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://myv.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gfd.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://fsu.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://okm.sysykeji.top

[C03] 可变参数
来源：http://rpf.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://aka.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hlq.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://svf.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://caz.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eks.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vwh.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://elm.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://olm.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://qat.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ipy.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fsh.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tqm.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nsc.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://tsc.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://fcj.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://lty.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://ibj.jqgufenzy.top

[C05] 返回多个值
来源：http://jcf.shangyingyoupin.top

Py:   return a, b
来源：http://xkk.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://frg.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vqi.epnwcf.com

TS:   return { a, b };
来源：http://dcv.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dok.uphjek.com

Go:   return a, b
来源：http://lkp.wangdashe.top

Ruby: return a, b
来源：http://moc.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://tiq.cheryme.top

[C06] 匿名函数 / lambda
来源：http://rds.tanke756.top

Py:   square = lambda x: x * x
来源：http://hyr.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://wpz.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://ylp.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://enz.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jex.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://lzu.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://boz.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xms.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://gqk.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gqp.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://xng.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pbd.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://bwg.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xxa.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://evd.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://alr.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sdc.shzxlz.cn

[C08] 闭包
来源：http://svw.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qhs.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zca.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qop.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qyl.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ywd.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uyq.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://roy.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kfx.fehbvm.com

[C09] 递归
来源：http://bzp.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqr.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hef.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbk.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzu.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://otv.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ows.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rsl.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ijl.ydjk.org.cn

[C10] 变量作用域
来源：http://kmk.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ghs.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://htj.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lhb.zdqjudy.top

TS:   同 JS
来源：http://nof.bbcook.cn

Java: 方法内为块级作用域
来源：http://eav.epnwcf.com

Go:   花括号块级作用域
来源：http://wrl.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tgx.havefunace.top

C#:   块级作用域
来源：http://xde.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://hso.jqgufenzy.top

Py:   from module import func
来源：http://esj.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oht.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gdg.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uuj.tianlin.xyz

Java: import java.util.List;
来源：http://qhr.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyf.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://wdh.zhengqikj.top

C#:   using System.Text;
来源：http://fec.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://sdf.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://alz.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://pxv.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://wcg.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://prn.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://taz.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://sif.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://qde.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kyw.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://vqk.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uob.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjz.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wsn.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zoa.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://jxd.hywenlv.cn

Go:   func add(a, b int) int
来源：http://rzf.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pfy.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://jfv.xinyue.icu

[C14] 泛型函数
来源：http://xcv.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kyg.iojbl.cn

PHP:  // 无泛型
来源：http://dli.9152youxi.cn

JS:   // 无泛型
来源：http://wvq.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tuc.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://imj.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lyp.cheryme.top

Ruby: # 无泛型
来源：http://ygd.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ysr.yj20258888.top

[C15] 解构 / 展开参数
来源：http://har.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://piv.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://czf.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hiw.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vus.daria6918.cn

Java: // 无解构
来源：http://tne.shangyingyoupin.top

Go:   // 无解构
来源：http://lpf.yueranfly.top

Ruby: a, b = pair
来源：http://mxl.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://vbk.yuxming.cn

[C16] 函数 / 方法重载
来源：http://itn.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zqo.havefunace.top

PHP:  // 无重载
来源：http://zxy.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://chh.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://cwv.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://pyi.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://puv.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://zdr.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ccf.dashuyun.cn

================================================================================
来源：http://pdx.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://ccl.guowangkeji.top

================================================================================
来源：http://hte.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://ayk.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tdm.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fno.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wgp.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://aot.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cqs.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://tmg.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://ghi.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sqz.chenlongwang.top

[D02] 追加元素到末尾
来源：http://qjd.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wrg.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yro.wangdashe.top

JS:   arr.push(4);
来源：http://cwc.havefunace.top

TS:   arr.push(4);
来源：http://mta.tanke756.top

Java: list.add(4);
来源：http://ihw.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://rmv.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://vtd.c1oappe.top

C#:   list.Add(4);
来源：http://taj.zycfv.cn

[D03] 在指定位置插入元素
来源：http://yqg.yj202588.top

Py:   arr.insert(0, 0)
来源：http://ake.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mzm.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uuy.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://jwi.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://yje.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://ttg.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cbe.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://aog.yangfankeji.com

[D04] 删除元素
来源：http://lxt.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fzr.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bvb.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://byl.pycfn.com

TS:   arr.splice(0, 1);
来源：http://cab.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dqq.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zbr.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xgx.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://inh.snrcjt.cn

[D05] 访问与修改元素
来源：http://bpl.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ylz.jinqigfzy.top


<!-- 参考信息 -->