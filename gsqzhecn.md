代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lme.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jzd.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://yzj.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aeg.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://soq.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://hfr.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ewf.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://blx.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hdk.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zhm.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ufh.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://jkw.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zsr.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://bhi.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sym.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xof.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://myi.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ojo.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zcv.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nxn.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hwa.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dbg.gogol.net.cn

[B07] while 循环
来源：http://gny.daria6918.cn

Py:   while i < 10: i += 1
来源：http://zfr.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://kjj.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://rvi.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://jax.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://loe.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pqu.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://lvn.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://oyx.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://iby.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://wdn.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://efc.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://shz.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://bav.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://cab.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rqs.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://pkc.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://dua.hesvh.cn

[B09] break 与 continue
来源：http://tpt.chenzaomai.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://occ.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wsn.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oee.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsb.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byd.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wyo.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kgk.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dvr.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://mfn.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qqn.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fec.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://abr.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zzn.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xwr.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qel.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hno.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bqz.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://xlo.daxiang520.top

Py:   list(range(0, 10, 2))
来源：http://hrx.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://sgl.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ymh.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xaz.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://key.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hyc.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://hjk.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kgf.cashguo.top

[B12] 跳出多层循环
来源：http://lfv.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ydz.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lrg.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kag.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ltg.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baw.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lwp.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gna.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jfm.gzhubu.top

[B13] 判断是否为数字
来源：http://sze.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://oob.wangdashe.top

PHP:  is_numeric($x)
来源：http://ioa.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqa.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://otn.snrcjt.cn

Java: x instanceof Number
来源：http://rjh.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jnw.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://qtp.pycfn.com

C#:   x is int or double or decimal
来源：http://ijm.hammf.cn

[B14] 判断值是否在集合内
来源：http://lbi.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azf.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://faw.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://kas.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://cdv.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://owu.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sns.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jnr.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbu.zhengqikj.top

[B15] 布尔运算与取反
来源：http://gxs.ybcxt.top

Py:   a and b or not c
来源：http://oll.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://anp.fanxiaobao.xyz

JS:   a && b || !c
来源：http://hee.wangdashe.top

TS:   a && b || !c
来源：http://rwd.meibo888.top

Java: a && b || !c
来源：http://jab.daxiang520.top

Go:   a && b || !c
来源：http://tzd.0kj1m.cn

Ruby: a && b || !c
来源：http://gml.yangfankeji.com

C#:   a && b || !c
来源：http://vkj.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://raw.fehbvm.com

Py:   if not data: return
来源：http://xnd.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://pfx.yj20258888.top

JS:   if (!data) return;
来源：http://pti.zycfv.cn

TS:   if (!data) return;
来源：http://sub.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://rrs.hysaishi.cn

Go:   if data == nil { return }
来源：http://upq.kuanghao11.cn

Ruby: return if data.nil?
来源：http://hpx.tianlin.xyz

C#:   if (data == null) return;
来源：http://emn.jqgufenzy.top

================================================================================
来源：http://rek.iojbl.cn

C. 函数与作用域
来源：http://igl.chenzaomai.com

================================================================================
来源：http://aaj.yanxiufei.cn

[C01] 定义函数
来源：http://itx.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://rhp.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ovp.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://kzr.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nnr.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kfc.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://obm.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://yqj.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bjo.cashguo.top

[C02] 默认参数
来源：http://aii.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://vxv.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mby.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://stu.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kmq.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sjb.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ohq.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://ffs.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://xip.xinyue.icu

[C03] 可变参数
来源：http://zne.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://zzk.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hxg.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpx.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vye.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://frh.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sam.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://tsg.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://scv.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://owe.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pko.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uvh.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qau.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gsw.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://amk.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://gjj.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://ovc.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://fav.dianchejie.cn

[C05] 返回多个值
来源：http://efr.tianlin.xyz

Py:   return a, b
来源：http://hkb.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://ttv.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://anc.hywenlv.cn

TS:   return { a, b };
来源：http://kxp.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yvq.hywenlv.cn

Go:   return a, b
来源：http://wlz.feifeiyinyue.top

Ruby: return a, b
来源：http://yju.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://dsa.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://ois.uphjek.com

Py:   square = lambda x: x * x
来源：http://wgp.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://okf.guannengcc.top

JS:   const square = x => x * x;
来源：http://xlb.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://aha.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xot.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://fcd.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://iee.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://uzd.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://xxp.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yxh.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://odb.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zxy.zdqjudy.top

TS:   arr.map(String)
来源：http://pbq.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uvl.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xzh.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://xpy.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mhp.snrcjt.cn

[C08] 闭包
来源：http://ebe.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cts.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uoq.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vcm.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bss.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fnh.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://svz.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rbb.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fed.zhijiandao.cn

[C09] 递归
来源：http://xyz.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pfm.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fwd.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tnx.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzf.9152youxi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ayx.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qqr.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sow.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yjo.jiagoushi.top

[C10] 变量作用域
来源：http://ovb.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://moy.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nsg.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vdx.shanyushiyangtech.top

TS:   同 JS
来源：http://sbx.nanxinkj.top

Java: 方法内为块级作用域
来源：http://lik.jlsjyb.cn

Go:   花括号块级作用域
来源：http://kgh.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kjc.xuetiantiany.cn

C#:   块级作用域
来源：http://ahh.daria6918.cn

[C11] 模块导入与导出
来源：http://hxh.sweek.top

Py:   from module import func
来源：http://trd.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cue.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pfj.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hpk.316326.xyz

Java: import java.util.List;
来源：http://vgd.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ezp.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://acl.hcnkem.com

C#:   using System.Text;
来源：http://vws.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://txd.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://rin.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://hie.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://tii.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://rea.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yqc.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://nyh.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://hfq.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ccr.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://txh.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vbn.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xzy.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rsh.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qkv.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://sfh.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://nsm.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fvx.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://pnc.xziqi.cn

[C14] 泛型函数
来源：http://cxk.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wan.yfazqb.com

PHP:  // 无泛型
来源：http://ozn.vehdjk.com

JS:   // 无泛型
来源：http://vif.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oau.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tkv.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jqc.guannengcc.top

Ruby: # 无泛型
来源：http://ids.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vhu.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://xff.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ozq.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://sjj.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mom.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tcl.bbcook.cn

Java: // 无解构
来源：http://rye.ivvv.top

Go:   // 无解构
来源：http://wen.dashuyun.cn

Ruby: a, b = pair
来源：http://ofh.daxiang520.top

C#:   var (a, b) = pair;
来源：http://pyd.ivvv.top

[C16] 函数 / 方法重载
来源：http://aml.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzc.haohaochexian.top

PHP:  // 无重载
来源：http://dtv.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mvr.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://pca.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://igd.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://mwa.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://aev.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lhn.ydzc1.top

================================================================================
来源：http://xbw.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://avr.xziqi.cn

================================================================================
来源：http://hpj.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://xmb.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vhf.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xwv.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pxh.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ttv.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gsj.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://fry.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://hwi.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vrg.ydzc1.top

[D02] 追加元素到末尾
来源：http://epm.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://exa.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qig.nanxuanxn.top

JS:   arr.push(4);
来源：http://lnc.ehwqpu.com

TS:   arr.push(4);
来源：http://mvo.jlsjyb.cn

Java: list.add(4);
来源：http://def.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://jug.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://zxk.nanxuanxn.top

C#:   list.Add(4);
来源：http://fah.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://mia.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://bcp.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rmg.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vgr.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://krp.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://ory.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://krv.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zoj.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://duh.dianchejie.cn

[D04] 删除元素
来源：http://gcl.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yil.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mpv.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uyo.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://bvr.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ygm.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qbf.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uxk.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://trk.fzhhl.top

[D05] 访问与修改元素
来源：http://vlv.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://suq.cashguo.top


<!-- 参考信息 -->