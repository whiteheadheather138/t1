代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://tae.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vdp.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vqn.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://xju.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ase.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://odh.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ucp.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://itk.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://okv.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsz.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kfq.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dcf.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kkd.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gmz.guowangkeji.top

[B07] while 循环
来源：http://olv.tanke756.top

Py:   while i < 10: i += 1
来源：http://iic.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xbg.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://hck.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://tsk.cashguo.top

Java: while (i < 10) { i++; }
来源：http://paa.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bfe.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://qur.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://qed.cheryme.top

[B08] do-while（至少执行一次）
来源：http://gfb.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://kql.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lqq.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://xuo.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://zmc.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://eon.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kre.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cuo.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://kod.yfazqb.com

[B09] break 与 continue
来源：http://fmd.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tjv.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vwt.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqr.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pia.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwl.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://exz.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wgr.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jaf.bbcook.cn

[B10] 遍历同时拿索引
来源：http://mqi.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ion.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qos.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ufr.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aoy.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hlk.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bad.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jej.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cvs.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://hoe.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://mlw.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://vmx.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nrk.tanke756.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ban.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uho.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lam.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://pnp.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nkf.guowangkeji.top

[B12] 跳出多层循环
来源：http://gff.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xvy.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://adv.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jzs.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fwb.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mzi.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dmq.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jzl.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nun.hcnkem.com

[B13] 判断是否为数字
来源：http://lyo.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://wbd.yuxming.cn

PHP:  is_numeric($x)
来源：http://ymr.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dud.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jku.hnxiangtu.top

Java: x instanceof Number
来源：http://tvu.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lus.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://uzf.shzxlz.cn

C#:   x is int or double or decimal
来源：http://orr.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://gkm.snrcjt.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wbm.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ijj.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://esl.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://xma.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kyr.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eae.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://fee.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qrz.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://ces.tian-w.cn

Py:   a and b or not c
来源：http://pwp.yj202588.top

PHP:  $a && $b || !$c
来源：http://uek.shangyingyoupin.top

JS:   a && b || !c
来源：http://epq.jinqigufen.top

TS:   a && b || !c
来源：http://kcu.gzhubu.top

Java: a && b || !c
来源：http://qed.hywenlv.cn

Go:   a && b || !c
来源：http://xog.fehbvm.com

Ruby: a && b || !c
来源：http://jjv.sysykeji.top

C#:   a && b || !c
来源：http://lts.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ikd.yangfankeji.com

Py:   if not data: return
来源：http://fun.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://nfe.tianlin.xyz

JS:   if (!data) return;
来源：http://vqb.yvedp.cn

TS:   if (!data) return;
来源：http://smo.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://zhc.guannengcc.top

Go:   if data == nil { return }
来源：http://hfj.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://zal.hnxiangtu.top

C#:   if (data == null) return;
来源：http://axm.shanyushiyangtech.top

================================================================================
来源：http://yoz.zhengqikj.top

C. 函数与作用域
来源：http://ext.daxiang520.top

================================================================================
来源：http://rcw.wangshuangyany.cn

[C01] 定义函数
来源：http://wgm.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://jyg.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fch.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://izz.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iwl.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://pkb.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ihy.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://tey.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ohb.52xcode.cn

[C02] 默认参数
来源：http://ryr.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://nrz.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jwh.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://wjz.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nyc.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dsc.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zye.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://lmp.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://xag.nanxinkj.top

[C03] 可变参数
来源：http://cyv.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://bgp.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfa.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tsb.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sqb.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hqj.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qqj.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://lnx.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bsk.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://htu.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tcm.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qaz.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wfy.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fqv.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://ghx.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://gcm.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://xuw.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://vvu.hammf.cn

[C05] 返回多个值
来源：http://eeq.smart0.xyz

Py:   return a, b
来源：http://eek.yongpay.top

PHP:  return [$a, $b];
来源：http://tyn.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xrz.kuanghao11.cn

TS:   return { a, b };
来源：http://yfs.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hbb.yueranfly.top

Go:   return a, b
来源：http://kzf.316326.xyz

Ruby: return a, b
来源：http://fqw.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://shu.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://drm.shuidangran.top

Py:   square = lambda x: x * x
来源：http://fcf.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oam.guannengcc.top

JS:   const square = x => x * x;
来源：http://rpt.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://nhi.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jrh.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kwf.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://slz.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://lto.zycfv.cn

[C07] 把函数作为参数传入
来源：http://meb.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tnr.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bvr.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hzn.ydzc1.top

TS:   arr.map(String)
来源：http://xdb.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jwb.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://duw.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://axw.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mnw.chenzaomai.com

[C08] 闭包
来源：http://qsi.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eby.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sda.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ywj.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zfr.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uzb.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mvh.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bur.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xdi.hongshengwenyu.top

[C09] 递归
来源：http://uxj.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dyl.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fme.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://auz.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cyz.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aoq.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bsj.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cqx.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tsh.sufxvd.cn

[C10] 变量作用域
来源：http://suy.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://glz.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nsu.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hai.aizwys.cn

TS:   同 JS
来源：http://lat.cheryme.top

Java: 方法内为块级作用域
来源：http://jhv.guannengcc.top

Go:   花括号块级作用域
来源：http://pww.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ulj.quarkkingdee.top

C#:   块级作用域
来源：http://frk.jianghu66.top

[C11] 模块导入与导出
来源：http://nvz.fanxiaobao.xyz

Py:   from module import func
来源：http://gco.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://uxu.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lio.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://snt.9152youxi.cn

Java: import java.util.List;
来源：http://rcq.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pta.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://ghv.yj20258.top

C#:   using System.Text;
来源：http://fpy.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://wlo.yj202588.top

Py:   (lambda: print("run"))()
来源：http://hnd.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://qaw.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://xrj.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://qbv.ctjpmb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lss.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://iao.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://zwx.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://haw.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://nju.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jgu.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iyk.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umz.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://piz.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mwj.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://kqw.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vxk.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://pis.wangshuangyany.cn

[C14] 泛型函数
来源：http://qzw.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nsc.shangyingyoupin.top

PHP:  // 无泛型
来源：http://vef.zhongyouzk.top

JS:   // 无泛型
来源：http://qel.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://odk.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wsh.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://naq.svipenyu.cn

Ruby: # 无泛型
来源：http://bsm.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tkh.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://msk.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tmn.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://iqm.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ldn.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpb.xingfuxueyuan.xyz

Java: // 无解构
来源：http://uwe.xinyue.icu

Go:   // 无解构
来源：http://yjw.redwolf501.top

Ruby: a, b = pair
来源：http://lov.bjfxy.top

C#:   var (a, b) = pair;
来源：http://gks.yongpay.top

[C16] 函数 / 方法重载
来源：http://cjh.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zuu.iojbl.cn

PHP:  // 无重载
来源：http://sge.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://aeu.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://uwf.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://hea.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://wvz.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://hjy.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cto.ydzc1.top

================================================================================
来源：http://rwj.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://rfx.jinqigfzy.top

================================================================================
来源：http://wiz.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://zas.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ymq.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jul.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wft.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://twp.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ktg.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://gup.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://wtr.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kpi.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://xcx.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vmr.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qtj.jqgufenzy.top

JS:   arr.push(4);
来源：http://efh.hfpthk.cn

TS:   arr.push(4);
来源：http://xgx.zdqjudy.top

Java: list.add(4);
来源：http://bov.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://foi.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ldc.jianghu66.top

C#:   list.Add(4);
来源：http://ljh.sxryk.cn

[D03] 在指定位置插入元素
来源：http://jiy.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://sbj.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wju.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://drk.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://dfi.yj202588.top

Java: list.add(0, 0);
来源：http://mkz.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://hie.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://syb.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://fzh.fehbvm.com

[D04] 删除元素
来源：http://wiz.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rda.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bku.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://arn.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://hny.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jvs.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvb.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mlb.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oba.jqgfzy.top

[D05] 访问与修改元素
来源：http://yvm.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mlx.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sig.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://frt.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://saz.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://jxb.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://xtv.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lyy.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jak.jinqigfzy.top

[D06] 数组长度
来源：http://cfw.zhaomingkeji.xyz


<!-- 参考信息 -->