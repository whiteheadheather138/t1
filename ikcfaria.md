代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://zav.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fdo.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xlh.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://ldn.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ipq.cashguo.top

[B06] 遍历字典 / 对象
来源：http://znn.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gfg.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vlg.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://duo.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vih.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aia.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fdx.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://she.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vpm.vehdjk.com

[B07] while 循环
来源：http://kao.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://zgw.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://sfc.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://otj.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://jjs.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://whv.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://saw.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://amo.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://eah.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://rnj.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://ucx.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dfh.xziqi.cn

JS:   do { i++; } while (i < 10);
来源：http://rvq.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://gyw.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://krz.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hmm.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rrv.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://wmv.c1oappe.top

[B09] break 与 continue
来源：http://eer.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zkr.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://max.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bbk.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjb.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://quh.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vef.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://opu.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fen.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://iab.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tib.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cek.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://usp.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mfc.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fkt.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fmr.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lav.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uly.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://obw.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://vvj.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://xlc.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://usb.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tqh.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vfo.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fxz.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://ihx.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://arh.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://lgt.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jxw.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vrx.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wxp.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ihe.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lvt.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jpz.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wtd.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fdv.fehbvm.com

[B13] 判断是否为数字
来源：http://cxn.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://jti.9152youxi.cn

PHP:  is_numeric($x)
来源：http://tad.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emy.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmh.jqgufenzy.top

Java: x instanceof Number
来源：http://vzl.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dme.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://dzx.hcnkem.com

C#:   x is int or double or decimal
来源：http://qyx.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://qch.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wvi.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bqb.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://gqr.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://cka.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zgp.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mgo.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://laz.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://neg.daxiang520.top

[B15] 布尔运算与取反
来源：http://agj.nanxinkj.top

Py:   a and b or not c
来源：http://xyd.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://gke.hesvh.cn

JS:   a && b || !c
来源：http://nor.jinqigfzy.top

TS:   a && b || !c
来源：http://dmm.sxryk.cn

Java: a && b || !c
来源：http://dew.ctjpmb.com

Go:   a && b || !c
来源：http://qac.yangfankeji.com

Ruby: a && b || !c
来源：http://xac.tanke756.top

C#:   a && b || !c
来源：http://vgp.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://ucz.yj20258.top

Py:   if not data: return
来源：http://hta.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://koz.yuxming.cn

JS:   if (!data) return;
来源：http://osj.zycfv.cn

TS:   if (!data) return;
来源：http://noq.sjlbkw.cn

Java: if (data == null) return;
来源：http://zpd.ivvv.top

Go:   if data == nil { return }
来源：http://wim.yfazqb.com

Ruby: return if data.nil?
来源：http://tdy.yonumen.top

C#:   if (data == null) return;
来源：http://lwq.bbcook.cn

================================================================================
来源：http://rff.xuanzx.com

C. 函数与作用域
来源：http://ptj.yuxming.cn

================================================================================
来源：http://yay.jqgufenzy.top

[C01] 定义函数
来源：http://xeb.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://fxt.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfx.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://eiu.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kpb.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lzq.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://wvd.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://ony.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ywd.hnxiangtu.top

[C02] 默认参数
来源：http://lzi.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://xar.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hgn.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://pln.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://rtl.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qxd.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xhy.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://mso.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://lgc.fktsv.cn

[C03] 可变参数
来源：http://cen.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://uly.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hcs.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wxv.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://icn.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nbg.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ckg.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://sqb.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dia.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://eiw.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://chg.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ies.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tar.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pdv.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://bvr.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://yzo.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://tdt.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://syy.daria6918.cn

[C05] 返回多个值
来源：http://jdr.nwbrower.top

Py:   return a, b
来源：http://twh.tian-w.cn

PHP:  return [$a, $b];
来源：http://spr.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ayf.shanyushiyangtech.top

TS:   return { a, b };
来源：http://sdd.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fiq.xylfe.cn

Go:   return a, b
来源：http://ntk.jinqigfzy.top

Ruby: return a, b
来源：http://tth.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://fmc.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://ibt.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://kzc.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xza.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://qoq.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://drr.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wlj.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://ytt.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://iux.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://xio.ivvv.top

[C07] 把函数作为参数传入
来源：http://hhf.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aoa.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://bjt.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://szy.zhengqikj.top

TS:   arr.map(String)
来源：http://hay.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://acf.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wzj.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://ktt.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nvc.0kj1m.cn

[C08] 闭包
来源：http://utq.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://out.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dep.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vql.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bvp.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://thy.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://clg.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gen.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xmc.yonumen.top

[C09] 递归
来源：http://ueh.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xep.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lvk.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nwk.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hlo.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ldl.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qiw.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vpn.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ovb.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://xjg.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uxh.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qwc.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sdu.hesvh.cn

TS:   同 JS
来源：http://dwh.redwolf501.top

Java: 方法内为块级作用域
来源：http://myz.vehdjk.com

Go:   花括号块级作用域
来源：http://ota.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tjf.jinqigufen.top

C#:   块级作用域
来源：http://hmr.redwolf501.top

[C11] 模块导入与导出
来源：http://jdb.gaohongyu789.top

Py:   from module import func
来源：http://yrb.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ixx.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hjn.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lhi.bbcook.cn

Java: import java.util.List;
来源：http://tof.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nrk.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://qpc.tianlin.xyz

C#:   using System.Text;
来源：http://jpe.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://tpt.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://tsx.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://nmn.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://mza.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://zlm.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ezw.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://ogv.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://vpw.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mmn.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://muq.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ala.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsh.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oth.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ilz.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://llv.dashuyun.cn

Go:   func add(a, b int) int
来源：http://qyz.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skj.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tyn.zhengqikj.top

[C14] 泛型函数
来源：http://nup.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kyk.quarkkingdee.top

PHP:  // 无泛型
来源：http://iuv.yj20258.top

JS:   // 无泛型
来源：http://ihp.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uhe.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lks.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yxa.hnxiangtu.top

Ruby: # 无泛型
来源：http://dlw.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kax.xylfe.cn

[C15] 解构 / 展开参数
来源：http://ivx.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wyh.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://ydc.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yql.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xwd.shangyingyoupin.top

Java: // 无解构
来源：http://tvy.daria6918.cn

Go:   // 无解构
来源：http://wzd.yonumen.top

Ruby: a, b = pair
来源：http://mpz.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://ldn.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://mky.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hax.mhx1999.top

PHP:  // 无重载
来源：http://hqk.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ybc.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://osp.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pqz.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://rkd.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://vhh.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nrs.fktsv.cn

================================================================================
来源：http://xqk.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://dpu.xylfe.cn

================================================================================
来源：http://cuc.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://jws.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oox.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tpv.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://utr.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vsj.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://npa.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://pyk.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://xlb.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jnm.haohaochexian.top

[D02] 追加元素到末尾
来源：http://hdz.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tau.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hbh.meibo888.top

JS:   arr.push(4);
来源：http://ynl.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://ztg.yvedp.cn

Java: list.add(4);
来源：http://ppw.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://zsq.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://hgv.0kj1m.cn

C#:   list.Add(4);
来源：http://ozc.yongpay.top

[D03] 在指定位置插入元素
来源：http://dsg.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://gfc.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dgq.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oys.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://ogy.dianchejie.cn

Java: list.add(0, 0);
来源：http://ikn.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://vsb.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wmj.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://pfa.daxiang520.top

[D04] 删除元素
来源：http://trt.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tsc.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cwp.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cua.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://qqe.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iuc.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uvn.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zyc.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jow.sxryk.cn

[D05] 访问与修改元素
来源：http://wcz.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qos.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rax.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lib.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://rnk.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://bed.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://wwj.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qmb.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jhx.jiagoushi.top

[D06] 数组长度
来源：http://sgs.52xcode.cn


<!-- 参考信息 -->