代发 wailian999

Py:   for i in range(10): print(i)
来源：http://yct.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dqz.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ggv.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jej.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gkn.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://udo.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://boj.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jyo.havefunace.top

[B05] 遍历数组 / 列表
来源：http://lbl.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://dhu.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dcw.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fyr.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jku.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hmh.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ydp.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://qzx.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obh.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://ogi.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://xoi.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ykg.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xie.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ill.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hxs.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pir.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sci.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tzo.hysaishi.cn

[B07] while 循环
来源：http://icg.nwbrower.top

Py:   while i < 10: i += 1
来源：http://ltr.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://mqj.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://jyq.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://nip.yueranfly.top

Java: while (i < 10) { i++; }
来源：http://usd.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://usz.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://zik.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://ixx.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://qpr.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://wdl.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fvr.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://pvm.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://cgd.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://nhf.birdmap.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bse.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://spl.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://grx.cqqwz.cn

[B09] break 与 continue
来源：http://lyi.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qht.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pba.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxo.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arc.yj20258.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbc.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gbd.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ful.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtl.daxiang520.top

[B10] 遍历同时拿索引
来源：http://ryw.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hud.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vvn.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://swi.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eil.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://osk.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://znv.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rsj.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fxc.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://adm.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://yag.tarul.cn

PHP:  range(0, 10, 2);
来源：http://hlc.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsg.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://whp.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kkg.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ylo.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://jdu.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zgh.hesvh.cn

[B12] 跳出多层循环
来源：http://ngm.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pzh.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kdx.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hka.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tsg.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ehj.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nzs.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xoe.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zje.xylfe.cn

[B13] 判断是否为数字
来源：http://jwx.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://mof.shuidangran.top

PHP:  is_numeric($x)
来源：http://vaa.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vef.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbv.daria6918.cn

Java: x instanceof Number
来源：http://vur.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rip.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://lel.haohaochexian.top

C#:   x is int or double or decimal
来源：http://kpc.zycfv.cn

[B14] 判断值是否在集合内
来源：http://obl.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ptp.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ptg.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://ixa.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://spa.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://akj.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rbf.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://nrr.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ptd.cheryme.top

[B15] 布尔运算与取反
来源：http://isd.sjlbkw.cn

Py:   a and b or not c
来源：http://tto.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://aeo.aizwys.cn

JS:   a && b || !c
来源：http://abo.cheryme.top

TS:   a && b || !c
来源：http://qny.dashuyun.cn

Java: a && b || !c
来源：http://tuc.havefunace.top

Go:   a && b || !c
来源：http://rsz.zdbjq.cn

Ruby: a && b || !c
来源：http://uwh.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://vkb.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ycf.zhongyouzk.top

Py:   if not data: return
来源：http://jnf.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://hwe.fzhhl.top

JS:   if (!data) return;
来源：http://cad.gogol.net.cn

TS:   if (!data) return;
来源：http://zvf.guowangkeji.top

Java: if (data == null) return;
来源：http://evn.hammf.cn

Go:   if data == nil { return }
来源：http://whj.aibaodan.cn

Ruby: return if data.nil?
来源：http://ebc.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://opf.yueranfly.top

================================================================================
来源：http://zkr.jiagoushi.top

C. 函数与作用域
来源：http://jmf.yj202588.top

================================================================================
来源：http://tqw.aizwys.cn

[C01] 定义函数
来源：http://nnf.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://bmi.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ulm.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://rgj.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wto.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://piz.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://njz.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://udm.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://weo.chenjidiqi.icu

[C02] 默认参数
来源：http://xxx.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://vqx.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://udz.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://nre.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rte.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xka.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://voo.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://dyh.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://baj.ppjwa.cn

[C03] 可变参数
来源：http://dpo.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://mcw.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yby.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppj.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://whx.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ppe.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uui.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://jcq.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bgk.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://ypz.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tfr.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ocl.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kvr.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cix.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://cse.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://mrl.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://xek.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://alb.jqgfzy.top

[C05] 返回多个值
来源：http://glz.zycfv.cn

Py:   return a, b
来源：http://cao.jqgfzy.top

PHP:  return [$a, $b];
来源：http://kzc.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hmp.gaohongyu789.top

TS:   return { a, b };
来源：http://bcv.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cxz.kuanghao11.cn

Go:   return a, b
来源：http://xid.shangyingyoupin.top

Ruby: return a, b
来源：http://mvw.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://ock.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://fjs.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://ufx.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ihu.fzhhl.top

JS:   const square = x => x * x;
来源：http://wgu.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ujd.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xbm.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://vdo.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://blu.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://sul.yongpay.top

[C07] 把函数作为参数传入
来源：http://ifk.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wpz.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://uyn.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bvf.sjlbkw.cn

TS:   arr.map(String)
来源：http://gwa.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://peg.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iup.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://vpv.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mok.tian-w.cn

[C08] 闭包
来源：http://ayy.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufs.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bsc.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vyv.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wti.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fso.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pik.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://luv.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rhv.xingfuxueyuan.xyz

[C09] 递归
来源：http://fyt.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://upj.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zus.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vns.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tgk.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mdd.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fce.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bxo.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sgl.hfpthk.cn

[C10] 变量作用域
来源：http://ppp.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nqh.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yvr.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wvw.hesvh.cn

TS:   同 JS
来源：http://tar.cdnleiting.top

Java: 方法内为块级作用域
来源：http://wvx.daxiang520.top

Go:   花括号块级作用域
来源：http://jhz.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tih.dianchejie.cn

C#:   块级作用域
来源：http://qar.haohaochexian.top

[C11] 模块导入与导出
来源：http://uhl.sufxvd.cn

Py:   from module import func
来源：http://yaq.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://cii.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iba.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://znz.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://ljp.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dyb.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://slc.ybcxt.top

C#:   using System.Text;
来源：http://ydy.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://ebe.yj20258.top

Py:   (lambda: print("run"))()
来源：http://znw.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://kgu.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://pud.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://gaf.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hja.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://pis.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://kkt.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://qfm.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://ygy.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pjc.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qlz.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ooh.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jpy.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eko.hcnkem.com

Go:   func add(a, b int) int
来源：http://faw.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lqs.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dax.yuanzhike.top

[C14] 泛型函数
来源：http://cyd.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yuz.havefunace.top

PHP:  // 无泛型
来源：http://xys.zdqjudy.top

JS:   // 无泛型
来源：http://qgq.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxv.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://frr.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://car.yj20258888.top

Ruby: # 无泛型
来源：http://jln.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gdq.yonumen.top

[C15] 解构 / 展开参数
来源：http://bjf.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zsm.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://jwr.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kzo.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mla.tian-w.cn

Java: // 无解构
来源：http://okv.yanxiufei.cn

Go:   // 无解构
来源：http://qwg.shuidangran.top

Ruby: a, b = pair
来源：http://six.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://dhx.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://rif.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hse.xuanzx.com

PHP:  // 无重载
来源：http://exi.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wqq.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://ffd.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yzt.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://liy.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://zto.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sqk.bbcook.cn

================================================================================
来源：http://uct.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://jjw.daxiang520.top

================================================================================
来源：http://hrw.iojbl.cn

[D01] 创建数组 / 列表
来源：http://gxn.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ces.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fsl.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qnr.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nta.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gyz.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://lkz.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://rjg.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nrj.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://gpe.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://smy.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nss.wangshuangyany.cn

JS:   arr.push(4);
来源：http://pym.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://wrd.chenjidiqi.icu

Java: list.add(4);
来源：http://wxi.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://oud.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://fcu.cdnleiting.top

C#:   list.Add(4);
来源：http://kyw.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://ifn.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://ink.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://asw.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uqf.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://oam.havefunace.top

Java: list.add(0, 0);
来源：http://paz.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://awt.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sho.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://yfy.tarul.cn

[D04] 删除元素
来源：http://szi.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bba.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kix.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jrr.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://pls.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rnr.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gpw.yuanzhike.top


<!-- 参考信息 -->