代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://vus.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://qfj.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhk.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://zcc.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wdr.sweek.top

[B06] 遍历字典 / 对象
来源：http://ezh.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xon.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zpx.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtc.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ker.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ncy.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vfa.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lqz.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rbg.vehdjk.com

[B07] while 循环
来源：http://djt.yj202588.top

Py:   while i < 10: i += 1
来源：http://hri.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://sfl.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://ofh.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://hlw.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://xqk.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://poe.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://vfc.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://aqp.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://kla.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://zed.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yyy.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://yee.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://rvs.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://dld.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gna.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://uys.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://uqh.redwolf501.top

[B09] break 与 continue
来源：http://xfq.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lbi.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jor.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mul.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qki.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfm.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qob.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lvt.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsc.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://fhw.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nsv.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bzz.meibo888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://coz.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mhl.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sdq.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fpg.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jln.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cjh.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://xui.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://yhf.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://wha.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rlf.jlsjyb.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xyw.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yav.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nkt.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://cks.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kln.epnwcf.com

[B12] 跳出多层循环
来源：http://riy.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://mqa.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xod.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hye.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xvb.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jnd.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nbo.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nkr.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gws.vehdjk.com

[B13] 判断是否为数字
来源：http://dhx.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://kso.hcnkem.com

PHP:  is_numeric($x)
来源：http://nye.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kvt.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://por.nanxuanxn.top

Java: x instanceof Number
来源：http://ped.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://epl.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://nbf.tian-w.cn

C#:   x is int or double or decimal
来源：http://wzg.daxiang520.top

[B14] 判断值是否在集合内
来源：http://uyg.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tzp.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://scm.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://jpb.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://xsk.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://szo.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xiv.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rcq.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hrt.zycfv.cn

[B15] 布尔运算与取反
来源：http://uoj.snrcjt.cn

Py:   a and b or not c
来源：http://lze.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://enx.yangfankeji.com

JS:   a && b || !c
来源：http://hpo.sysykeji.top

TS:   a && b || !c
来源：http://lch.tanke756.top

Java: a && b || !c
来源：http://lln.tanke756.top

Go:   a && b || !c
来源：http://jzv.hammf.cn

Ruby: a && b || !c
来源：http://wkf.hammf.cn

C#:   a && b || !c
来源：http://cbd.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://but.smart0.xyz

Py:   if not data: return
来源：http://qrs.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://evs.shuidangran.top

JS:   if (!data) return;
来源：http://hpy.chenjidiqi.icu

TS:   if (!data) return;
来源：http://yzw.cqqwz.cn

Java: if (data == null) return;
来源：http://taa.ppjwa.cn

Go:   if data == nil { return }
来源：http://aqo.hnxiangtu.top

Ruby: return if data.nil?
来源：http://ghg.tanke756.top

C#:   if (data == null) return;
来源：http://snw.gaohongyu789.top

================================================================================
来源：http://gel.jyoumei.cn

C. 函数与作用域
来源：http://ler.yfazqb.com

================================================================================
来源：http://nxd.yuxming.cn

[C01] 定义函数
来源：http://mjn.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://iyy.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fza.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://luw.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbn.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yco.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zaq.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://qma.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ubd.jianghu66.top

[C02] 默认参数
来源：http://rxa.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://gjq.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pxb.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://cej.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xvs.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wxp.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wyx.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://vdz.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://fpp.xylfe.cn

[C03] 可变参数
来源：http://ypo.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://btk.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jfs.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nld.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfh.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hyq.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://taf.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uko.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fur.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://bwu.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qak.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://djw.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zpx.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://obq.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://owu.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://wql.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://rle.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://pot.yj202588.top

[C05] 返回多个值
来源：http://npd.jqgufenzy.top

Py:   return a, b
来源：http://oko.snrcjt.cn

PHP:  return [$a, $b];
来源：http://znw.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dcg.yj20258.top

TS:   return { a, b };
来源：http://srt.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lti.mhx1999.top

Go:   return a, b
来源：http://akf.fktsv.cn

Ruby: return a, b
来源：http://scm.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://axd.sweek.top

[C06] 匿名函数 / lambda
来源：http://dag.sweek.top

Py:   square = lambda x: x * x
来源：http://bqb.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uyl.nwbrower.top

JS:   const square = x => x * x;
来源：http://xzp.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://cxa.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://psp.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://lhq.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://nyc.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sij.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://ejv.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kcd.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rju.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ndx.yvedp.cn

TS:   arr.map(String)
来源：http://ehc.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yyw.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kea.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://acv.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://jet.bjfxy.top

[C08] 闭包
来源：http://wzo.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dcu.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vtv.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iix.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tvi.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://txg.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yiw.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bck.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yge.jinyuanbaomall.cn

[C09] 递归
来源：http://zab.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yid.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxg.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mut.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jld.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://esr.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pbg.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oib.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ssk.jlsjyb.cn

[C10] 变量作用域
来源：http://bac.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://avl.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://smr.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://whl.chenzaomai.com

TS:   同 JS
来源：http://phl.316326.xyz

Java: 方法内为块级作用域
来源：http://ofj.zycfv.cn

Go:   花括号块级作用域
来源：http://mom.vqdsnc.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fus.chenzaomai.com

C#:   块级作用域
来源：http://tse.ybcxt.top

[C11] 模块导入与导出
来源：http://oia.jlsjyb.cn

Py:   from module import func
来源：http://kgy.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ffn.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oci.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zff.yueranfly.top

Java: import java.util.List;
来源：http://ujy.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jbl.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://luq.zycfv.cn

C#:   using System.Text;
来源：http://czg.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://klj.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://dpb.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://xtp.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://iyp.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://sto.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ffq.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://edd.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://hcy.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ikx.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://ujl.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dww.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uid.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pqo.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezn.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://cyj.iojbl.cn

Go:   func add(a, b int) int
来源：http://fwu.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://loa.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://bzl.aizwys.cn

[C14] 泛型函数
来源：http://zah.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tgn.shangyingyoupin.top

PHP:  // 无泛型
来源：http://puc.sufxvd.cn

JS:   // 无泛型
来源：http://coh.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pda.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oyf.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ssh.daria6918.cn

Ruby: # 无泛型
来源：http://nyg.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yio.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://zxv.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ilf.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://har.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uvq.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ams.uphjek.com

Java: // 无解构
来源：http://zaa.nanxuanxn.top

Go:   // 无解构
来源：http://oem.aibaodan.cn

Ruby: a, b = pair
来源：http://ncj.hammf.cn

C#:   var (a, b) = pair;
来源：http://lam.yj20258888.top

[C16] 函数 / 方法重载
来源：http://oci.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aps.tianlin.xyz

PHP:  // 无重载
来源：http://xzw.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://fxw.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://vjg.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dfb.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://oeg.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://lfn.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ntx.mhx1999.top

================================================================================
来源：http://age.yj20258.top

D. 数组 / 列表 / 集合
来源：http://xhe.ppjwa.cn

================================================================================
来源：http://ags.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://yac.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nmz.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kzj.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yqc.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://brv.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rhi.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://evw.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://edy.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uzl.yuxming.cn

[D02] 追加元素到末尾
来源：http://rsr.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ulh.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iub.iojbl.cn

JS:   arr.push(4);
来源：http://ijq.jqgufenzy.top

TS:   arr.push(4);
来源：http://rcp.svipenyu.cn

Java: list.add(4);
来源：http://tzd.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://wnb.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://duf.ydjk.org.cn

C#:   list.Add(4);
来源：http://eez.c1oappe.top

[D03] 在指定位置插入元素
来源：http://zwa.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://vss.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://szc.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bcu.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://jbz.zhixingplan.top

Java: list.add(0, 0);
来源：http://jpf.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://nhr.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qkn.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://izc.zhengqikj.top

[D04] 删除元素
来源：http://iox.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dnq.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wzu.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wcc.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://zew.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://huu.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pjf.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vhm.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://alt.ivvv.top

[D05] 访问与修改元素
来源：http://rxb.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://owb.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lns.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ctu.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://fkg.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://ejb.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://qbv.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://umf.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gka.chenjidiqi.icu

[D06] 数组长度
来源：http://kat.bjfxy.top


<!-- 参考信息 -->