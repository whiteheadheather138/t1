代发 wailian999

[B05] 遍历数组 / 列表
来源：http://yzc.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://cza.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ksy.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wxg.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mcq.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uhb.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fwt.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://mrj.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://evi.hammf.cn

[B06] 遍历字典 / 对象
来源：http://bac.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xzc.bbcook.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kai.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fab.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://swl.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jmd.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rty.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nbv.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zjz.yj20258888.top

[B07] while 循环
来源：http://lxb.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://fht.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ksv.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://hwm.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://bqq.tarul.cn

Java: while (i < 10) { i++; }
来源：http://jtn.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uyx.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://tsr.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://rbf.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://oii.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://boy.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rmg.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://yst.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://onn.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://zsz.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ttt.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xle.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://zlq.aizwys.cn

[B09] break 与 continue
来源：http://kvv.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ewz.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rnu.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxk.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqv.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ilo.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://isg.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hhz.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azx.xylfe.cn

[B10] 遍历同时拿索引
来源：http://qes.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://csg.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rad.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nvw.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dwk.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lna.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zsy.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ncm.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ahh.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://iur.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://vjo.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://tqs.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qww.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://skw.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hpt.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zeh.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://fng.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dju.birdmap.top

[B12] 跳出多层循环
来源：http://jno.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bze.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fas.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jdc.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qsm.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gts.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hzi.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ovw.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kfs.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://hpb.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://lpb.yueranfly.top

PHP:  is_numeric($x)
来源：http://lvo.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfl.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bgp.guannengcc.top

Java: x instanceof Number
来源：http://auz.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wgy.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://ztb.ctjpmb.com

C#:   x is int or double or decimal
来源：http://pid.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://zjk.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dly.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://exi.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://pfy.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://dyp.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zvy.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qrt.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://kdq.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oim.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://wdm.316326.xyz

Py:   a and b or not c
来源：http://ogu.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://lzz.jlsjyb.cn

JS:   a && b || !c
来源：http://don.hesvh.cn

TS:   a && b || !c
来源：http://aqt.pycfn.com

Java: a && b || !c
来源：http://hkk.fengsongda.top

Go:   a && b || !c
来源：http://wzn.ctjpmb.com

Ruby: a && b || !c
来源：http://wed.haohaochexian.top

C#:   a && b || !c
来源：http://msl.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://spm.tanke756.top

Py:   if not data: return
来源：http://zjv.ydzc1.top

PHP:  if (!$data) { return; }
来源：http://ofx.aizwys.cn

JS:   if (!data) return;
来源：http://tbe.jiagoushi.top

TS:   if (!data) return;
来源：http://vim.jyoumei.cn

Java: if (data == null) return;
来源：http://qhs.9152youxi.cn

Go:   if data == nil { return }
来源：http://lny.yueranfly.top

Ruby: return if data.nil?
来源：http://sid.52xcode.cn

C#:   if (data == null) return;
来源：http://ows.jinqigufen.top

================================================================================
来源：http://bvm.fehbvm.com

C. 函数与作用域
来源：http://ufn.hywenlv.cn

================================================================================
来源：http://frf.smart0.xyz

[C01] 定义函数
来源：http://yhk.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://mnx.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mxf.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://ani.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gbh.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oqm.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://vqc.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://smd.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sfb.vehdjk.com

[C02] 默认参数
来源：http://emu.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://lai.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bcx.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://yfd.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xaq.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://icu.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mdy.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://bgu.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://woj.zycfv.cn

[C03] 可变参数
来源：http://vyv.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://qze.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://omm.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lzk.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ltk.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fse.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://slm.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://ufn.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aaw.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://jti.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://btv.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kgo.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kbc.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://muj.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://wfq.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://moh.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://xoe.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://kah.nwbrower.top

[C05] 返回多个值
来源：http://soy.zhoulong.xyz

Py:   return a, b
来源：http://ftr.zycfv.cn

PHP:  return [$a, $b];
来源：http://umf.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ush.ybcxt.top

TS:   return { a, b };
来源：http://gfg.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wgv.shuidangran.top

Go:   return a, b
来源：http://jyt.vqdsnc.cn

Ruby: return a, b
来源：http://dxe.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://qra.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://kqo.mhx1999.top

Py:   square = lambda x: x * x
来源：http://myu.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ian.tarul.cn

JS:   const square = x => x * x;
来源：http://yei.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://qqd.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://whs.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uqw.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://leo.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://xxg.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://jcp.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://urt.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mpr.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rgz.jyoumei.cn

TS:   arr.map(String)
来源：http://rob.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vmb.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://spi.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://cwr.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sdc.svipenyu.cn

[C08] 闭包
来源：http://kim.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rtd.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://noj.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://goz.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rrv.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lan.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ayu.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cei.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jbo.wangshuangyany.cn

[C09] 递归
来源：http://pfi.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tul.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fxr.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rgt.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vfv.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bzt.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://adu.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wpt.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://klk.yueranfly.top

[C10] 变量作用域
来源：http://joy.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rld.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bew.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ega.shanyushiyangkeji.top

TS:   同 JS
来源：http://kig.nwbrower.top

Java: 方法内为块级作用域
来源：http://bem.cheryme.top

Go:   花括号块级作用域
来源：http://txz.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wjv.hnxiangtu.top

C#:   块级作用域
来源：http://qkp.yonumen.top

[C11] 模块导入与导出
来源：http://kpg.hammf.cn

Py:   from module import func
来源：http://auu.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://qju.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rtb.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://umb.zdqjudy.top

Java: import java.util.List;
来源：http://uen.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mrt.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://xkk.gaohongyu789.top

C#:   using System.Text;
来源：http://xdy.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://sax.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://jtn.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://eyu.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://xsj.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://lek.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lwl.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://eka.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://xwi.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://bqe.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://mco.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pqc.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jem.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tqa.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wfn.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vbi.fengsongda.top

Go:   func add(a, b int) int
来源：http://cun.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xap.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://aqu.jqgufenzy.top

[C14] 泛型函数
来源：http://ill.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ldw.ivvv.top

PHP:  // 无泛型
来源：http://ugo.wangdashe.top

JS:   // 无泛型
来源：http://xxs.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ozm.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oqf.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fti.smart0.xyz

Ruby: # 无泛型
来源：http://oop.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qbc.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://upw.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gxo.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://odg.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ibo.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wam.shanyushiyangtech.top

Java: // 无解构
来源：http://mof.zdbjq.cn

Go:   // 无解构
来源：http://dwp.tian-w.cn

Ruby: a, b = pair
来源：http://gyw.pycfn.com

C#:   var (a, b) = pair;
来源：http://liq.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://pcv.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cce.cucudq.cn

PHP:  // 无重载
来源：http://owo.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://obg.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://zoj.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ihl.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://vnu.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://lym.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbm.tanke756.top

================================================================================
来源：http://srt.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://qrz.ivvv.top

================================================================================
来源：http://ydd.vehdjk.com

[D01] 创建数组 / 列表
来源：http://hyn.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rjs.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bim.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vzi.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nuc.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dhc.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://ata.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://lfy.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://unk.haohaochexian.top

[D02] 追加元素到末尾
来源：http://nfh.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rql.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uom.sxryk.cn

JS:   arr.push(4);
来源：http://jzq.sweek.top

TS:   arr.push(4);
来源：http://pvp.yfazqb.com

Java: list.add(4);
来源：http://onm.yonumen.top

Go:   arr = append(arr, 4)
来源：http://rxs.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://eki.quarkkingdee.top

C#:   list.Add(4);
来源：http://fps.yj20258888.top

[D03] 在指定位置插入元素
来源：http://unx.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://mnn.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://smr.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://frk.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://nlx.quarkkingdee.top

Java: list.add(0, 0);
来源：http://hmo.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zsp.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lve.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://ifs.sufxvd.cn

[D04] 删除元素
来源：http://vkw.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jxr.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gwy.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wyq.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://bfw.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://daa.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://thh.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hje.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zsv.tian-w.cn

[D05] 访问与修改元素
来源：http://kbd.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cae.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jtc.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ojr.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://kap.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://yhx.yj20258.top


<!-- 参考信息 -->