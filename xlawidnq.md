代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://wfd.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://yyt.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aix.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://wzc.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fbj.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://bus.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wwc.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bem.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mci.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpz.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pmu.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lco.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://txv.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qhw.ywan-chungtsiang.top

[B07] while 循环
来源：http://ldm.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://ekt.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://wge.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://fym.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://osw.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://inr.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hps.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://cgk.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://eld.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://fno.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://tpb.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qbh.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://vbo.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://noe.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://cyq.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pah.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://mwm.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://jvm.cqqwz.cn

[B09] break 与 continue
来源：http://dmt.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://izw.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kxu.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uem.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqb.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddk.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lhy.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fug.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qse.tarul.cn

[B10] 遍历同时拿索引
来源：http://cld.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eyj.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tsr.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://onx.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://egz.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xli.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kqj.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rxl.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbv.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://ozu.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://udb.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://yox.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dil.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yti.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nfl.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opn.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://syk.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hag.zhoulong.xyz

[B12] 跳出多层循环
来源：http://cux.jinqigfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uza.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xaj.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yyk.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfo.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hfp.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zcn.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rex.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yno.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://vfo.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://utn.fengsongda.top

PHP:  is_numeric($x)
来源：http://cxu.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fpf.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bua.ydzc1.top

Java: x instanceof Number
来源：http://zpd.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dqn.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://jbh.wangdashe.top

C#:   x is int or double or decimal
来源：http://tof.cucudq.cn

[B14] 判断值是否在集合内
来源：http://ckt.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sji.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gcr.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://oqj.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://vch.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dap.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://auf.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://cms.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hrf.cdnleiting.top

[B15] 布尔运算与取反
来源：http://txc.vqdsnc.cn

Py:   a and b or not c
来源：http://jba.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://oqa.ppjwa.cn

JS:   a && b || !c
来源：http://ybb.vqdsnc.cn

TS:   a && b || !c
来源：http://xpk.shanyushiyangtech.top

Java: a && b || !c
来源：http://apa.dashuyun.cn

Go:   a && b || !c
来源：http://ioj.yj20258888.top

Ruby: a && b || !c
来源：http://oma.chenjidiqi.icu

C#:   a && b || !c
来源：http://blj.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fiz.smart0.xyz

Py:   if not data: return
来源：http://kmz.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://jug.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://web.redwolf501.top

TS:   if (!data) return;
来源：http://rlj.quarkkingdee.top

Java: if (data == null) return;
来源：http://fel.316326.xyz

Go:   if data == nil { return }
来源：http://ajx.daxiang520.top

Ruby: return if data.nil?
来源：http://uce.316326.xyz

C#:   if (data == null) return;
来源：http://aqw.andypj.xyz

================================================================================
来源：http://vbd.gogol.net.cn

C. 函数与作用域
来源：http://bya.uphjek.com

================================================================================
来源：http://oix.uphjek.com

[C01] 定义函数
来源：http://lzp.birdmap.top

Py:   def add(a, b): return a + b
来源：http://esy.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbq.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://wyw.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esj.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://wss.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xih.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://rge.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fsk.jqgfzy.top

[C02] 默认参数
来源：http://ivh.tanke756.top

Py:   def greet(name="World"): return name
来源：http://yzo.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vhg.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://nxl.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://gdm.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ulj.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ybd.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://oqs.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://ocp.dashuyun.cn

[C03] 可变参数
来源：http://xpl.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://daq.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dub.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qek.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yiv.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wwl.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vkw.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://trs.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dsp.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://szq.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gyr.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xoo.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://evb.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nkv.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://bar.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://lms.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://ubp.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://ant.feifeiyinyue.top

[C05] 返回多个值
来源：http://snw.sjlbkw.cn

Py:   return a, b
来源：http://mte.ybcxt.top

PHP:  return [$a, $b];
来源：http://gwi.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ymr.shuidangran.top

TS:   return { a, b };
来源：http://ouu.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xas.hongshengwenyu.top

Go:   return a, b
来源：http://zsw.hesvh.cn

Ruby: return a, b
来源：http://gpp.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://pnv.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://wmg.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://nka.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xej.zdbjq.cn

JS:   const square = x => x * x;
来源：http://jav.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://ftc.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://scy.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://lew.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://gbl.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://wyw.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://azi.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://muj.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kxn.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kte.cheryme.top

TS:   arr.map(String)
来源：http://xqg.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fgq.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jnt.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://ccc.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qwc.fehbvm.com

[C08] 闭包
来源：http://ahb.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iqg.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ncg.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fau.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://edo.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rxz.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nrh.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://unl.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mpy.hfpthk.cn

[C09] 递归
来源：http://ofi.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iof.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zzi.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yiv.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpv.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://whg.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://njl.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gev.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ijq.tian-w.cn

[C10] 变量作用域
来源：http://kqz.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mqb.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://miu.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://shz.andypj.xyz

TS:   同 JS
来源：http://zie.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://zxt.jinqigufen.top

Go:   花括号块级作用域
来源：http://plg.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zxr.jqgufenzy.top

C#:   块级作用域
来源：http://sls.shzxlz.cn

[C11] 模块导入与导出
来源：http://nts.shanyushiyangtech.top

Py:   from module import func
来源：http://lip.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rkm.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fyx.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ldc.jqgufenzy.top

Java: import java.util.List;
来源：http://wbb.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://odw.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://oaf.pengpengdd.cyou

C#:   using System.Text;
来源：http://fpq.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://wdx.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://rng.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://tyu.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://uit.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://amo.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lgs.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://tsn.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://ova.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tnt.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://pug.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bnj.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zio.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eql.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xac.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://mrj.shzxlz.cn

Go:   func add(a, b int) int
来源：http://pon.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mnr.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://dqr.hfpthk.cn

[C14] 泛型函数
来源：http://lke.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://osi.birdmap.top

PHP:  // 无泛型
来源：http://yoo.yongpay.top

JS:   // 无泛型
来源：http://hax.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fjr.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jni.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ibh.tarul.cn

Ruby: # 无泛型
来源：http://wuu.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zmx.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://mri.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pob.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://yau.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zep.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kou.dianchejie.cn

Java: // 无解构
来源：http://tyk.yj202588.top

Go:   // 无解构
来源：http://jsj.bbcook.cn

Ruby: a, b = pair
来源：http://eox.yj20258.top

C#:   var (a, b) = pair;
来源：http://abs.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://rdx.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cja.cdnleiting.top

PHP:  // 无重载
来源：http://svb.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qth.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://pvf.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cvy.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://shu.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://lil.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gee.sufxvd.cn

================================================================================
来源：http://bod.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://zsv.yj20258888.top

================================================================================
来源：http://nhg.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://dqb.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xqx.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pvq.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://syl.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lhz.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ukr.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://izb.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://skq.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ynp.tarul.cn

[D02] 追加元素到末尾
来源：http://xiy.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ifa.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jkq.vqdsnc.cn

JS:   arr.push(4);
来源：http://wlw.c1oappe.top

TS:   arr.push(4);
来源：http://yve.ywan-chungtsiang.top

Java: list.add(4);
来源：http://keq.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://uvg.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://gnx.cheryme.top

C#:   list.Add(4);
来源：http://eto.yj20258.top

[D03] 在指定位置插入元素
来源：http://jgm.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://hhh.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qml.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fdc.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://bnz.gaohongyu789.top

Java: list.add(0, 0);
来源：http://hqk.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://qov.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ncj.cheryme.top

C#:   list.Insert(0, 0);
来源：http://qxb.shuidangran.top

[D04] 删除元素
来源：http://luc.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vqo.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nmq.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://utf.tanke756.top

TS:   arr.splice(0, 1);
来源：http://zzz.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qck.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ejb.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://afu.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pbo.chenzaomai.com

[D05] 访问与修改元素
来源：http://fqi.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ejg.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ygg.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mpp.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://afs.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://avk.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://jlz.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kbr.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tiy.jinghuilouyu.cn

[D06] 数组长度
来源：http://vej.sufxvd.cn


<!-- 参考信息 -->