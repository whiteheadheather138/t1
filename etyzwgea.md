代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://zib.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qoa.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tkk.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://xgx.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://twl.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://cdh.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kno.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://flr.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdg.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smj.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pml.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://npu.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kdv.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ohq.hnqzz.top

[B07] while 循环
来源：http://zmm.yfazqb.com

Py:   while i < 10: i += 1
来源：http://gia.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://zyr.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://mwj.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://yin.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://hzp.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://thv.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://thy.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://pgo.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://aqu.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://xtw.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://psy.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://lme.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://lsl.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://esz.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mdq.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://ydr.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://wev.yj202588.top

[B09] break 与 continue
来源：http://ysn.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oqr.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bjf.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uij.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdi.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uor.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mez.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xos.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyo.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://iub.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dtt.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wuc.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://afq.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uwg.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bek.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yql.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://krl.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hhf.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://fwi.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://dlm.316326.xyz

PHP:  range(0, 10, 2);
来源：http://gub.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mez.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gfr.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bvh.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfq.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://jlb.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xyt.jlsjyb.cn

[B12] 跳出多层循环
来源：http://uil.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pnn.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tzs.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyr.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpd.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oil.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wxz.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fau.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nmy.ydjk.org.cn

[B13] 判断是否为数字
来源：http://xsh.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://mdh.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://snw.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://okt.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rkw.hongshengwenyu.top

Java: x instanceof Number
来源：http://cek.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iow.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://dlh.fehbvm.com

C#:   x is int or double or decimal
来源：http://gsf.birdmap.top

[B14] 判断值是否在集合内
来源：http://iko.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kmt.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cen.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://fxw.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://vrx.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rqv.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vcj.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xcu.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nzi.zycfv.cn

[B15] 布尔运算与取反
来源：http://hfg.jiagoushi.top

Py:   a and b or not c
来源：http://qkm.yfazqb.com

PHP:  $a && $b || !$c
来源：http://mda.nanxuanxn.top

JS:   a && b || !c
来源：http://vms.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://hsq.chenjidiqi.icu

Java: a && b || !c
来源：http://uoh.xuanzx.com

Go:   a && b || !c
来源：http://rap.guannengcc.top

Ruby: a && b || !c
来源：http://ckk.tianlin.xyz

C#:   a && b || !c
来源：http://hto.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://hwv.hongshengwenyu.top

Py:   if not data: return
来源：http://qje.pycfn.com

PHP:  if (!$data) { return; }
来源：http://dpr.wangdashe.top

JS:   if (!data) return;
来源：http://nln.meibo888.top

TS:   if (!data) return;
来源：http://vrs.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://ltz.cashguo.top

Go:   if data == nil { return }
来源：http://nip.jyoumei.cn

Ruby: return if data.nil?
来源：http://tbl.cashguo.top

C#:   if (data == null) return;
来源：http://vjq.gogol.net.cn

================================================================================
来源：http://qqe.xuetiantiany.cn

C. 函数与作用域
来源：http://iwf.chenjidiqi.icu

================================================================================
来源：http://ahk.yuxming.cn

[C01] 定义函数
来源：http://nkj.yongpay.top

Py:   def add(a, b): return a + b
来源：http://fbi.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uqr.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://vbj.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnw.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://llr.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://tjv.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://nfk.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nsw.pengpengdd.cyou

[C02] 默认参数
来源：http://hkg.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://jyy.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://off.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://rpe.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://aad.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zjq.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ory.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://ruy.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://ziw.hysaishi.cn

[C03] 可变参数
来源：http://qyj.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://ivc.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cco.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://glo.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bxc.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vgs.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ttg.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sju.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kwb.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://exl.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://czb.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbp.quarkkingdee.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nnl.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://awq.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://ctw.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://kqa.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://vyk.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://hzz.chenzaomai.com

[C05] 返回多个值
来源：http://gzm.ybcxt.top

Py:   return a, b
来源：http://qsi.zdbjq.cn

PHP:  return [$a, $b];
来源：http://zun.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://naz.cashguo.top

TS:   return { a, b };
来源：http://tgo.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ndm.tarul.cn

Go:   return a, b
来源：http://qwu.yj20258.top

Ruby: return a, b
来源：http://hsd.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://drk.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://bev.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://fmy.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ihv.tanke756.top

JS:   const square = x => x * x;
来源：http://zgo.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://mch.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpl.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://vak.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://xgz.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://wmc.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://cdc.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zmc.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://naf.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pzy.svipenyu.cn

TS:   arr.map(String)
来源：http://jfs.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ikw.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pof.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://zds.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zku.pengpengdd.cyou

[C08] 闭包
来源：http://xwl.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ydk.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oma.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mjq.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dtn.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lni.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ryc.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ajf.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dpf.xuanzx.com

[C09] 递归
来源：http://qni.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xrb.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rxy.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ogl.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lhx.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jyf.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jaa.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://taq.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xju.hesvh.cn

[C10] 变量作用域
来源：http://zaj.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xea.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xyw.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aql.jinqigufen.top

TS:   同 JS
来源：http://ppd.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://gtb.shzxlz.cn

Go:   花括号块级作用域
来源：http://mpz.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nwt.ybcxt.top

C#:   块级作用域
来源：http://qwt.316326.xyz

[C11] 模块导入与导出
来源：http://qby.ppjwa.cn

Py:   from module import func
来源：http://ihk.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iyd.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vcc.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uxb.yvedp.cn

Java: import java.util.List;
来源：http://dvn.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cnx.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://ddi.9152youxi.cn

C#:   using System.Text;
来源：http://nnh.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://kls.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://wcw.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://emn.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://bfj.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://yym.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://llo.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://vys.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://vfx.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fxi.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://axi.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://npz.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hna.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://akq.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cjk.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://owx.316326.xyz

Go:   func add(a, b int) int
来源：http://jha.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uqg.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gnz.fengsongda.top

[C14] 泛型函数
来源：http://gjl.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xxn.svipenyu.cn

PHP:  // 无泛型
来源：http://zlr.bbcook.cn

JS:   // 无泛型
来源：http://cur.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rgk.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zac.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://amv.quarkkingdee.top

Ruby: # 无泛型
来源：http://uud.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dea.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://iqv.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ekc.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://ryv.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ufx.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fwh.shanyushiyangkeji.top

Java: // 无解构
来源：http://mkn.yuxming.cn

Go:   // 无解构
来源：http://cgf.redwolf501.top

Ruby: a, b = pair
来源：http://fzv.aizwys.cn

C#:   var (a, b) = pair;
来源：http://toh.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://ifj.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pvh.yj202588.top

PHP:  // 无重载
来源：http://ddw.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxd.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://vjp.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rjn.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://vty.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://uox.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kyz.xziqi.cn

================================================================================
来源：http://ppf.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://yhy.hnxiangtu.top

================================================================================
来源：http://cod.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://ezg.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qyr.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hiw.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ubf.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rpf.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hxg.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://uti.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://svz.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dne.bbcook.cn

[D02] 追加元素到末尾
来源：http://spk.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rvg.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://csz.redwolf501.top

JS:   arr.push(4);
来源：http://orm.yuxming.cn

TS:   arr.push(4);
来源：http://eaq.hysaishi.cn

Java: list.add(4);
来源：http://mnn.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://cpu.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://meg.chenlongwang.top

C#:   list.Add(4);
来源：http://zgm.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://vdq.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://oqp.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tuj.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vss.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://glw.hnqzz.top

Java: list.add(0, 0);
来源：http://ztx.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://tba.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ruc.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://mzv.daria6918.cn

[D04] 删除元素
来源：http://xfj.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bag.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ozc.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://euv.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://bct.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xpu.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tls.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nut.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://imo.xuanzx.com

[D05] 访问与修改元素
来源：http://iux.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tmn.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lzb.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rhk.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://zxh.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://wha.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://mnv.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://llq.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wmw.jiagoushi.top

[D06] 数组长度
来源：http://arj.epnwcf.com


<!-- 参考信息 -->