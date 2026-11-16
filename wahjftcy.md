代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jya.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://ugo.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cea.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://car.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnw.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ghr.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://osl.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gin.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nfc.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nyy.jinghuilouyu.cn

[B07] while 循环
来源：http://rsm.shanyushiyangtech.top

Py:   while i < 10: i += 1
来源：http://evt.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lfj.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://ceb.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://cri.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://dkv.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vso.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://lww.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://xfy.meibo888.top

[B08] do-while（至少执行一次）
来源：http://ccy.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ihi.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://snv.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://fxr.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://wpy.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://ify.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vcr.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://zeb.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://nhv.zycfv.cn

[B09] break 与 continue
来源：http://biu.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iuk.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ens.shanyushiyangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjk.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwj.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pib.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ayk.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gtt.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kph.ybcxt.top

[B10] 遍历同时拿索引
来源：http://auk.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oxr.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jqo.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kxt.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iyf.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iha.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vmb.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vqz.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xot.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://wqj.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://nnj.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://xwb.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsb.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qkf.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qqc.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://erk.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://lkx.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ngh.daria6918.cn

[B12] 跳出多层循环
来源：http://bdf.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://die.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://uee.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zgi.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://umy.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sgg.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yys.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vlt.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hpk.cdnleiting.top

[B13] 判断是否为数字
来源：http://cmd.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://gcl.tianlin.xyz

PHP:  is_numeric($x)
来源：http://olp.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfx.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aww.shangyingyoupin.top

Java: x instanceof Number
来源：http://nmg.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sui.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://moy.nwbrower.top

C#:   x is int or double or decimal
来源：http://dsf.bbcook.cn

[B14] 判断值是否在集合内
来源：http://eat.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rsq.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rcs.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://ttb.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://pri.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dwl.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jhs.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://ogh.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uvd.chenzaomai.com

[B15] 布尔运算与取反
来源：http://eva.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://lte.fzhhl.top

PHP:  $a && $b || !$c
来源：http://gcx.9152youxi.cn

JS:   a && b || !c
来源：http://ocs.hongshengwenyu.top

TS:   a && b || !c
来源：http://hji.hcnkem.com

Java: a && b || !c
来源：http://txc.yfazqb.com

Go:   a && b || !c
来源：http://nof.0kj1m.cn

Ruby: a && b || !c
来源：http://fwg.zhengqikj.top

C#:   a && b || !c
来源：http://kve.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://ful.zhoulong.xyz

Py:   if not data: return
来源：http://xse.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://fwy.tian-w.cn

JS:   if (!data) return;
来源：http://ymu.yuxming.cn

TS:   if (!data) return;
来源：http://eil.nanxuanxn.top

Java: if (data == null) return;
来源：http://njy.yuxming.cn

Go:   if data == nil { return }
来源：http://vsu.jqgufenzy.top

Ruby: return if data.nil?
来源：http://iud.jqgufenzy.top

C#:   if (data == null) return;
来源：http://sfn.jqgufenzy.top

================================================================================
来源：http://eeb.316326.xyz

C. 函数与作用域
来源：http://app.jqgufenzy.top

================================================================================
来源：http://tfx.shanyushiyangtech.top

[C01] 定义函数
来源：http://zai.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://ghk.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dau.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://gqb.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hih.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bmj.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://chd.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://msl.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uqm.jyoumei.cn

[C02] 默认参数
来源：http://fmn.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://iub.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yli.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://tch.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hzg.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bdn.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aid.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://bmu.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://qwp.svipenyu.cn

[C03] 可变参数
来源：http://bvo.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://nrb.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yzs.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yho.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kwt.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pqg.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vpr.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://lqc.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rdc.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://yto.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zgn.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://clu.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yhc.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://acw.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://dvv.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://fwj.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://tuc.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://byk.meibo888.top

[C05] 返回多个值
来源：http://hpp.xylfe.cn

Py:   return a, b
来源：http://ayn.smart0.xyz

PHP:  return [$a, $b];
来源：http://ykn.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xkg.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://fmv.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jvh.ctjpmb.com

Go:   return a, b
来源：http://scx.fktsv.cn

Ruby: return a, b
来源：http://lmf.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://tnd.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://pjd.yvedp.cn

Py:   square = lambda x: x * x
来源：http://sts.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://awj.sufxvd.cn

JS:   const square = x => x * x;
来源：http://rpn.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://dsc.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://crh.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://gpt.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://gjd.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://odh.zycfv.cn

[C07] 把函数作为参数传入
来源：http://dkd.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yxd.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://rff.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gtr.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://soz.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xyn.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gxx.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://ipz.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://edi.jinqigufen.top

[C08] 闭包
来源：http://oqk.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fnx.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://skk.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://raq.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wlw.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qro.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aka.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ird.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ppl.jinqigfzy.top

[C09] 递归
来源：http://hpn.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cil.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://amr.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bji.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kff.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zwp.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://okn.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cja.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ajm.hywenlv.cn

[C10] 变量作用域
来源：http://bex.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ovy.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zas.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fdg.9152youxi.cn

TS:   同 JS
来源：http://zgh.daria6918.cn

Java: 方法内为块级作用域
来源：http://rtr.hcnkem.com

Go:   花括号块级作用域
来源：http://uet.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wrw.chenjidiqi.icu

C#:   块级作用域
来源：http://vez.yj20258888.top

[C11] 模块导入与导出
来源：http://ndc.ehwqpu.com

Py:   from module import func
来源：http://bel.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://trg.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uob.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zjk.smart0.xyz

Java: import java.util.List;
来源：http://mcx.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rfr.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://xyh.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://xwi.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://tqk.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://tfg.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://dyh.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://ika.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://xda.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jax.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://hoe.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://rml.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://aun.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://xff.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wei.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hds.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wrl.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ojp.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://dpf.c1oappe.top

Go:   func add(a, b int) int
来源：http://fru.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://idz.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://wdm.snrcjt.cn

[C14] 泛型函数
来源：http://zcx.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dwj.ydjk.org.cn

PHP:  // 无泛型
来源：http://isa.hywenlv.cn

JS:   // 无泛型
来源：http://uqo.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kya.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dfj.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://inl.ybcxt.top

Ruby: # 无泛型
来源：http://opa.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rmt.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://eif.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fnp.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://xkm.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://efn.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kan.yj202588.top

Java: // 无解构
来源：http://twh.jlsjyb.cn

Go:   // 无解构
来源：http://myn.jqgufenzy.top

Ruby: a, b = pair
来源：http://bww.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://pry.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://xcy.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jlj.svipenyu.cn

PHP:  // 无重载
来源：http://ris.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://jdv.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://oym.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://nvx.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://wki.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://jxk.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lzj.sweek.top

================================================================================
来源：http://olb.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://nde.sweek.top

================================================================================
来源：http://luz.bbcook.cn

[D01] 创建数组 / 列表
来源：http://oks.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tem.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xfr.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xwf.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nyp.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://krb.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://yiy.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://rzq.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cil.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://zdo.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qyq.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://glw.guowangkeji.top

JS:   arr.push(4);
来源：http://mvb.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://mve.yongpay.top

Java: list.add(4);
来源：http://udg.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://ngy.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://hix.xylfe.cn

C#:   list.Add(4);
来源：http://zwu.hesvh.cn

[D03] 在指定位置插入元素
来源：http://kxl.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://wbw.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hmp.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ega.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://rsy.vehdjk.com

Java: list.add(0, 0);
来源：http://ycq.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://uru.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ehf.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://zft.ydjk.org.cn

[D04] 删除元素
来源：http://xfr.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rar.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tha.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xcx.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://wop.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ezq.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bmx.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jmf.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sur.ydzc1.top

[D05] 访问与修改元素
来源：http://low.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xou.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tti.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qod.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://gnr.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://xzw.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://mfa.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dfh.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yhk.ywan-chungtsiang.top

[D06] 数组长度
来源：http://xik.zhiwuduotai.top

Py:   len(arr)
来源：http://nqq.zdqjudy.top

PHP:  count($arr);
来源：http://dxk.dianchejie.cn

JS:   arr.length
来源：http://ubw.guannengcc.top

TS:   arr.length
来源：http://top.bjfxy.top


<!-- 参考信息 -->