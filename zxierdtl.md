代发 wailian999

Py:   for i in range(10): print(i)
来源：http://xfy.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bvv.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eke.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dfb.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bwg.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ohn.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://eur.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ckc.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://ysr.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://dpo.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ssb.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://txe.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uig.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://tpk.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yzx.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://wba.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lxt.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://jrm.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kef.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://thy.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://epm.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zsm.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pbb.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ukb.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iks.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qrc.zhixingplan.top

[B07] while 循环
来源：http://pyo.ydzc1.top

Py:   while i < 10: i += 1
来源：http://uif.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://dwg.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://dfv.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://jzl.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://dpp.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xqq.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://awj.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://syy.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://jmm.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://dss.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eib.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://wvr.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://dcd.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://nwt.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zki.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dzu.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://jmg.jiagoushi.top

[B09] break 与 continue
来源：http://xqw.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xzw.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bgy.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfo.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jut.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjp.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cuz.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jdq.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykz.havefunace.top

[B10] 遍历同时拿索引
来源：http://lsz.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sln.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dcl.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kwa.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://feo.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cyz.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yqq.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xqs.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gtv.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://kkm.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://oxp.birdmap.top

PHP:  range(0, 10, 2);
来源：http://tjb.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tsc.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://luk.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ive.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jnd.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://zzu.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bhh.kuanghao11.cn

[B12] 跳出多层循环
来源：http://myz.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mnx.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://igq.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vih.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wve.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pyh.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wzl.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tsw.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gzx.jyoumei.cn

[B13] 判断是否为数字
来源：http://cqp.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://gcv.sweek.top

PHP:  is_numeric($x)
来源：http://gfa.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbv.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ggj.ehwqpu.com

Java: x instanceof Number
来源：http://vnv.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bek.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://vvq.yj202588.top

C#:   x is int or double or decimal
来源：http://iqu.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://wtn.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jnh.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iig.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://hof.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://xnq.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://opk.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ddl.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://ijg.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tid.mhx1999.top

[B15] 布尔运算与取反
来源：http://udd.epnwcf.com

Py:   a and b or not c
来源：http://ril.sysykeji.top

PHP:  $a && $b || !$c
来源：http://srb.yfazqb.com

JS:   a && b || !c
来源：http://uyu.kuanghao11.cn

TS:   a && b || !c
来源：http://ezq.meibo888.top

Java: a && b || !c
来源：http://xyq.quarkkingdee.top

Go:   a && b || !c
来源：http://lmg.jyoumei.cn

Ruby: a && b || !c
来源：http://ang.jinqigfzy.top

C#:   a && b || !c
来源：http://doo.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://vim.ybcxt.top

Py:   if not data: return
来源：http://qur.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://dpm.daxiang520.top

JS:   if (!data) return;
来源：http://hjx.hfpthk.cn

TS:   if (!data) return;
来源：http://ufj.hammf.cn

Java: if (data == null) return;
来源：http://xmn.daxiang520.top

Go:   if data == nil { return }
来源：http://cgu.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://zlr.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://krl.316326.xyz

================================================================================
来源：http://kne.yj20258.top

C. 函数与作用域
来源：http://jhf.cqqwz.cn

================================================================================
来源：http://ttv.xylfe.cn

[C01] 定义函数
来源：http://cdy.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://uvj.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yjy.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://whs.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lyz.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pde.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kxy.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://sdn.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nqf.sweek.top

[C02] 默认参数
来源：http://btz.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://hlz.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://hyy.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://brj.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://arc.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pca.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mhn.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://xza.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://psj.ydjk.org.cn

[C03] 可变参数
来源：http://wdv.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://gfb.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pqc.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yza.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fqf.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hkm.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://prz.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://lez.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://plj.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://lpd.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sbs.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sxe.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yso.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ief.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://drt.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://bwb.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://xkq.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://nqu.guannengcc.top

[C05] 返回多个值
来源：http://rax.jyoumei.cn

Py:   return a, b
来源：http://oxk.havefunace.top

PHP:  return [$a, $b];
来源：http://ixa.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oja.yuxming.cn

TS:   return { a, b };
来源：http://uyu.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oml.bbcook.cn

Go:   return a, b
来源：http://cnr.316326.xyz

Ruby: return a, b
来源：http://nkz.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ghj.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://gif.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://bxm.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tjh.gogol.net.cn

JS:   const square = x => x * x;
来源：http://pcz.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://fva.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hnu.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://sdc.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://jpx.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://krj.bjfxy.top

[C07] 把函数作为参数传入
来源：http://awi.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zbb.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://utq.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fan.hywenlv.cn

TS:   arr.map(String)
来源：http://qeb.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ceg.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tyb.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://dln.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://izr.cqqwz.cn

[C08] 闭包
来源：http://qio.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ieh.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qgh.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qri.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mzi.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dcj.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pgi.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pcj.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://chq.yuanzhike.top

[C09] 递归
来源：http://pfn.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lum.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jgt.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://duv.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://och.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qcf.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lpz.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://adb.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qkr.ybcxt.top

[C10] 变量作用域
来源：http://rpk.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ohy.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kib.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sgm.nanxinkj.top

TS:   同 JS
来源：http://ffy.chenzaomai.com

Java: 方法内为块级作用域
来源：http://ftk.andypj.xyz

Go:   花括号块级作用域
来源：http://xbj.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rjt.aibaodan.cn

C#:   块级作用域
来源：http://xmf.xuanzx.com

[C11] 模块导入与导出
来源：http://zsj.guannengcc.top

Py:   from module import func
来源：http://fxf.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tzl.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vdl.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aka.ydzc1.top

Java: import java.util.List;
来源：http://sjs.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sxx.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://nmf.meibo888.top

C#:   using System.Text;
来源：http://joq.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://efp.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://etz.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://vov.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://agn.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://mtt.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fcd.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://fdq.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://ajc.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nwp.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://gqd.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hxq.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gkl.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lzx.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rkd.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bbh.daria6918.cn

Go:   func add(a, b int) int
来源：http://udp.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqb.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://vxl.gogol.net.cn

[C14] 泛型函数
来源：http://dqv.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tte.hcnkem.com

PHP:  // 无泛型
来源：http://jfy.epnwcf.com

JS:   // 无泛型
来源：http://qai.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dxu.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nmc.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://erj.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://uat.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fkb.fktsv.cn

[C15] 解构 / 展开参数
来源：http://xwd.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tsm.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://xhe.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rce.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jpa.zhengqikj.top

Java: // 无解构
来源：http://clh.cdnleiting.top

Go:   // 无解构
来源：http://fou.hnqzz.top

Ruby: a, b = pair
来源：http://itm.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://tvd.yj202588.top

[C16] 函数 / 方法重载
来源：http://ann.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pfo.bbcook.cn

PHP:  // 无重载
来源：http://puq.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ctw.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://ijg.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zat.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://iub.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://dwg.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xqp.ybcxt.top

================================================================================
来源：http://ktl.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://oik.aibaodan.cn

================================================================================
来源：http://oxx.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://kci.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mja.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jcd.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://twd.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cnb.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://omg.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://kfr.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://bpn.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wyb.fehbvm.com

[D02] 追加元素到末尾
来源：http://dza.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://foh.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bfa.yuanzhike.top

JS:   arr.push(4);
来源：http://lry.tanke756.top

TS:   arr.push(4);
来源：http://yxh.ydjk.org.cn

Java: list.add(4);
来源：http://zds.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://yue.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://ngf.yj20258888.top

C#:   list.Add(4);
来源：http://uwm.cucudq.cn

[D03] 在指定位置插入元素
来源：http://oxz.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://uus.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dje.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lim.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://zao.smart0.xyz

Java: list.add(0, 0);
来源：http://hxt.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://hfa.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qdr.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://qah.zhixingplan.top

[D04] 删除元素
来源：http://lxm.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pnt.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xhv.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://npj.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://osx.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ykk.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bzu.fktsv.cn


<!-- 参考信息 -->