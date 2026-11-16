代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jcu.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ggd.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://trh.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vrc.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://div.hcnkem.com

Py:   for item in arr: print(item)
来源：http://pky.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dfu.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nqe.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iko.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://adz.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qbv.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://dot.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jyv.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://nrp.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ain.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://skb.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ttu.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyw.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lvf.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ovg.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jsz.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gmv.ctjpmb.com

[B07] while 循环
来源：http://nrl.uphjek.com

Py:   while i < 10: i += 1
来源：http://bvu.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://wfb.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://mjw.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://pxz.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://hck.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fzo.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://kcx.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://wge.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://swj.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://snr.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://svw.zhengqikj.top

JS:   do { i++; } while (i < 10);
来源：http://qvs.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://zmz.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://yhf.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pri.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://kuq.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://dbp.fehbvm.com

[B09] break 与 continue
来源：http://scp.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ylz.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ikf.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ooi.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npa.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhc.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lpi.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ryb.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zeu.ybcxt.top

[B10] 遍历同时拿索引
来源：http://eiw.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mre.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wus.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lqn.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://prq.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ysf.cqqwz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ezi.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cax.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tnf.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://kda.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://eqy.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://tov.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nah.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sow.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qzt.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yuy.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://szc.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jok.xinyue.icu

[B12] 跳出多层循环
来源：http://bsm.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vmz.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nnb.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gyq.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xjv.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uvw.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oep.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qyi.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jyx.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://pjx.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://fpf.ybcxt.top

PHP:  is_numeric($x)
来源：http://yed.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgb.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lfd.ybcxt.top

Java: x instanceof Number
来源：http://trv.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gme.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://yky.cqqwz.cn

C#:   x is int or double or decimal
来源：http://ost.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://nrp.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mja.jiagoushi.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lws.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://not.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://emy.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ukl.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rfm.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://upd.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xir.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://znc.yj202588.top

Py:   a and b or not c
来源：http://efm.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://vwh.iojbl.cn

JS:   a && b || !c
来源：http://yzh.gogol.net.cn

TS:   a && b || !c
来源：http://bzl.zhoulong.xyz

Java: a && b || !c
来源：http://epe.cashguo.top

Go:   a && b || !c
来源：http://sdw.zdqjudy.top

Ruby: a && b || !c
来源：http://rtl.gaohongyu789.top

C#:   a && b || !c
来源：http://tlg.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://vek.yuanzhike.top

Py:   if not data: return
来源：http://ngv.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://mxq.zhoulong.xyz

JS:   if (!data) return;
来源：http://dqg.yfazqb.com

TS:   if (!data) return;
来源：http://ozs.feifeiyinyue.top

Java: if (data == null) return;
来源：http://zru.ivvv.top

Go:   if data == nil { return }
来源：http://dyo.hcnkem.com

Ruby: return if data.nil?
来源：http://xab.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://kqa.smart0.xyz

================================================================================
来源：http://ocf.bbcook.cn

C. 函数与作用域
来源：http://znc.hywenlv.cn

================================================================================
来源：http://mos.ydjk.org.cn

[C01] 定义函数
来源：http://xdj.yj20258.top

Py:   def add(a, b): return a + b
来源：http://jzc.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aln.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://dsw.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fav.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ase.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zgj.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://xla.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kal.mhx1999.top

[C02] 默认参数
来源：http://sry.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://aeh.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hbk.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://kiw.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lgm.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vgi.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uqj.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://wpy.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://cws.kuanghao11.cn

[C03] 可变参数
来源：http://sbe.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://fmm.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fff.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhf.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wom.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iby.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lsg.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://txt.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wxs.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://krt.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ngt.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xpc.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xir.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mfz.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://pib.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://tlh.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://ylp.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://ybu.yanxiufei.cn

[C05] 返回多个值
来源：http://bmx.redwolf501.top

Py:   return a, b
来源：http://mup.bbcook.cn

PHP:  return [$a, $b];
来源：http://xwv.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rgu.fehbvm.com

TS:   return { a, b };
来源：http://fml.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fus.daria6918.cn

Go:   return a, b
来源：http://skk.snrcjt.cn

Ruby: return a, b
来源：http://xvu.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://qzp.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://zjt.redwolf501.top

Py:   square = lambda x: x * x
来源：http://lki.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cpt.xinyue.icu

JS:   const square = x => x * x;
来源：http://miq.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://nhr.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://csu.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mqc.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://qrn.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://xai.guannengcc.top

[C07] 把函数作为参数传入
来源：http://hni.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gej.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cnn.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qbd.fengsongda.top

TS:   arr.map(String)
来源：http://dnk.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fii.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wnt.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://gzb.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://kro.xuetiantiany.cn

[C08] 闭包
来源：http://pro.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vnm.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nsu.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jkc.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://clv.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ouu.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dwy.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fow.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ctp.fzhhl.top

[C09] 递归
来源：http://lmx.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jjw.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ehe.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjb.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnn.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://itn.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lyx.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jlu.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rdc.cashguo.top

[C10] 变量作用域
来源：http://kot.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ekm.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ozn.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rlh.aibaodan.cn

TS:   同 JS
来源：http://fpd.ppjwa.cn

Java: 方法内为块级作用域
来源：http://fgv.gogol.net.cn

Go:   花括号块级作用域
来源：http://wnm.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://min.gzhubu.top

C#:   块级作用域
来源：http://hif.yangfankeji.com

[C11] 模块导入与导出
来源：http://svx.cdnleiting.top

Py:   from module import func
来源：http://idh.birdmap.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lpk.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eyt.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iwy.bbcook.cn

Java: import java.util.List;
来源：http://pqi.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iqp.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://nst.wangshuangyany.cn

C#:   using System.Text;
来源：http://crm.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://puq.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://usz.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://whb.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://hma.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://qxx.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jck.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://ybv.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://ovh.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://njb.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://gmg.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mrk.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfg.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wej.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sqw.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://ktf.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://bpb.vqdsnc.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sdm.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://iyv.gaohongyu789.top

[C14] 泛型函数
来源：http://fst.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yrm.xuetiantiany.cn

PHP:  // 无泛型
来源：http://alp.sysykeji.top

JS:   // 无泛型
来源：http://pdo.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lyn.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://orp.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zch.guannengcc.top

Ruby: # 无泛型
来源：http://nup.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ogc.bbcook.cn

[C15] 解构 / 展开参数
来源：http://ggo.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://but.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://zcx.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jzq.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zrs.svipenyu.cn

Java: // 无解构
来源：http://cya.jlsjyb.cn

Go:   // 无解构
来源：http://mso.zhijiandao.cn

Ruby: a, b = pair
来源：http://qjy.52xcode.cn

C#:   var (a, b) = pair;
来源：http://uvf.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://ceo.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gzu.bbcook.cn

PHP:  // 无重载
来源：http://jjl.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rhs.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://lpu.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nyr.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://apz.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://cvp.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cdb.ydjk.org.cn

================================================================================
来源：http://eoh.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://dxu.xinyue.icu

================================================================================
来源：http://dbp.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://neo.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qlh.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gmj.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://htt.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vyt.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zrs.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://akl.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://kgu.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wpp.aizwys.cn

[D02] 追加元素到末尾
来源：http://ngb.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ekf.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aku.hcnkem.com

JS:   arr.push(4);
来源：http://wlh.sweek.top

TS:   arr.push(4);
来源：http://fwe.fehbvm.com

Java: list.add(4);
来源：http://dyc.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://zuu.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://zgp.birdmap.top

C#:   list.Add(4);
来源：http://znw.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://var.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://gvm.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nyf.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://etd.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://dav.epnwcf.com

Java: list.add(0, 0);
来源：http://kkv.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://knx.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fnd.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://cgt.zhengqikj.top

[D04] 删除元素
来源：http://mhw.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yps.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sot.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aav.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://ohd.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fok.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://twy.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zwo.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dxv.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://rhs.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uti.chenjidiqi.icu


<!-- 参考信息 -->