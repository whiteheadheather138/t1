代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qrp.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gdz.tianlin.xyz

[B07] while 循环
来源：http://tpk.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://ojv.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://tcv.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://snj.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://ejv.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://nfm.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hqe.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://gux.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://seu.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://zsf.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://jmp.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://isg.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://pwh.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://vkr.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://ipc.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://irw.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://syl.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://hbw.gzhubu.top

[B09] break 与 continue
来源：http://yup.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jhd.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hmd.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://efu.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfw.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lrh.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wkf.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hjz.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxy.daria6918.cn

[B10] 遍历同时拿索引
来源：http://qbn.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kqp.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dcx.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ihv.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://htb.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zyx.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fil.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://get.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jst.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://xrq.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://xyt.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://yya.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inc.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kfu.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qyd.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zwq.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://xup.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cjk.bjfxy.top

[B12] 跳出多层循环
来源：http://rdp.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bcs.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wcj.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rps.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fta.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xwv.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qcq.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iqq.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dtt.jlsjyb.cn

[B13] 判断是否为数字
来源：http://wbr.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://bmc.aibaodan.cn

PHP:  is_numeric($x)
来源：http://due.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tsy.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rep.hnqzz.top

Java: x instanceof Number
来源：http://aji.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yue.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://ddp.xuanzx.com

C#:   x is int or double or decimal
来源：http://qdm.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://fyu.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lmu.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wuj.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://riy.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://zvb.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://pkd.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://noy.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://tbc.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xch.ppjwa.cn

[B15] 布尔运算与取反
来源：http://nti.ctjpmb.com

Py:   a and b or not c
来源：http://xhx.cheryme.top

PHP:  $a && $b || !$c
来源：http://rto.sjlbkw.cn

JS:   a && b || !c
来源：http://luk.ydzc1.top

TS:   a && b || !c
来源：http://ykh.jinghuilouyu.cn

Java: a && b || !c
来源：http://jrv.chenzaomai.com

Go:   a && b || !c
来源：http://vsy.zdqjudy.top

Ruby: a && b || !c
来源：http://ith.smart0.xyz

C#:   a && b || !c
来源：http://cjq.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://hmp.aibaodan.cn

Py:   if not data: return
来源：http://wtm.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://rbu.yuxming.cn

JS:   if (!data) return;
来源：http://bvq.cqqwz.cn

TS:   if (!data) return;
来源：http://vlx.cqqwz.cn

Java: if (data == null) return;
来源：http://qsd.fengsongda.top

Go:   if data == nil { return }
来源：http://tou.gogol.net.cn

Ruby: return if data.nil?
来源：http://syz.daria6918.cn

C#:   if (data == null) return;
来源：http://hbk.fengsongda.top

================================================================================
来源：http://zzl.bjfxy.top

C. 函数与作用域
来源：http://rga.uphjek.com

================================================================================
来源：http://enm.nanxuanxn.top

[C01] 定义函数
来源：http://pdz.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://ndf.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehz.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://too.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qbk.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://spj.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://mha.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://bqv.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://olf.hesvh.cn

[C02] 默认参数
来源：http://hcj.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://zun.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hxr.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://sro.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bcu.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yju.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://clz.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://mun.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://tjh.tarul.cn

[C03] 可变参数
来源：http://mvl.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://vtv.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xzh.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwf.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://krl.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ufc.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kgb.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://unf.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rin.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://nhe.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tkc.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://faa.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://agi.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eur.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://wzt.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://lnw.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://uzr.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://mfk.aizwys.cn

[C05] 返回多个值
来源：http://twl.zhixingplan.top

Py:   return a, b
来源：http://rvn.hfpthk.cn

PHP:  return [$a, $b];
来源：http://qwm.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vbe.dianchejie.cn

TS:   return { a, b };
来源：http://zxx.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nrr.0kj1m.cn

Go:   return a, b
来源：http://doh.zhixingplan.top

Ruby: return a, b
来源：http://dyc.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://pmi.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://lov.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://xvo.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://teo.smart0.xyz

JS:   const square = x => x * x;
来源：http://hbl.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://kgw.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ufg.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://yjp.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://jzo.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zwe.sysykeji.top

[C07] 把函数作为参数传入
来源：http://aqt.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zel.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://pcb.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pur.fzhhl.top

TS:   arr.map(String)
来源：http://qpf.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sog.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qjz.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://qvq.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pff.zhaomingkeji.xyz

[C08] 闭包
来源：http://soo.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iig.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lcn.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bqq.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wyx.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://toa.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://reo.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fsj.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zot.sufxvd.cn

[C09] 递归
来源：http://liv.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://azh.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ahp.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ujv.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eat.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lwf.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zod.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yiw.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uye.redwolf501.top

[C10] 变量作用域
来源：http://lgm.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mmf.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rda.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qkd.zhixingplan.top

TS:   同 JS
来源：http://mog.sweek.top

Java: 方法内为块级作用域
来源：http://may.ppjwa.cn

Go:   花括号块级作用域
来源：http://nsv.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bfm.ydzc1.top

C#:   块级作用域
来源：http://ahj.jinqigufen.top

[C11] 模块导入与导出
来源：http://nty.ydzc1.top

Py:   from module import func
来源：http://kad.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hch.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://krl.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qih.epnwcf.com

Java: import java.util.List;
来源：http://fmo.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vza.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://ilp.chenlongwang.top

C#:   using System.Text;
来源：http://dib.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://utu.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://sya.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://til.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://zym.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://enn.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ala.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://jlf.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://lkv.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tqt.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://law.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://elz.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://toj.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sma.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://loo.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ylb.gogol.net.cn

Go:   func add(a, b int) int
来源：http://dkt.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qpz.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://gvp.nanxinkj.top

[C14] 泛型函数
来源：http://itn.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gav.yueranfly.top

PHP:  // 无泛型
来源：http://kvl.chenzaomai.com

JS:   // 无泛型
来源：http://ubl.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ptt.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yom.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jqm.bbcook.cn

Ruby: # 无泛型
来源：http://cpe.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ves.yj20258888.top

[C15] 解构 / 展开参数
来源：http://ebs.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gni.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://vrt.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hll.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zmq.wangshuangyany.cn

Java: // 无解构
来源：http://vrc.316326.xyz

Go:   // 无解构
来源：http://xfc.xylfe.cn

Ruby: a, b = pair
来源：http://iwo.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://uev.52xcode.cn

[C16] 函数 / 方法重载
来源：http://sue.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vin.zdqjudy.top

PHP:  // 无重载
来源：http://xai.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bwd.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://frj.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://evs.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://izz.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://ycy.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vht.hfpthk.cn

================================================================================
来源：http://kva.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://nud.ehwqpu.com

================================================================================
来源：http://yrq.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://psx.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://muz.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uju.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://shu.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zvc.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://man.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://qjd.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://gqn.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bih.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://fzn.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fwt.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://agj.daria6918.cn

JS:   arr.push(4);
来源：http://nck.ydzc1.top

TS:   arr.push(4);
来源：http://dnr.sysykeji.top

Java: list.add(4);
来源：http://her.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://qlv.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://wjo.sjlbkw.cn

C#:   list.Add(4);
来源：http://tay.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://nhk.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://uqx.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://juv.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pnb.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://him.cqqwz.cn

Java: list.add(0, 0);
来源：http://pmu.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://swc.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bdy.tanke756.top

C#:   list.Insert(0, 0);
来源：http://jvt.vqdsnc.cn

[D04] 删除元素
来源：http://atz.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vez.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uxj.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://phs.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://chw.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://anh.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dmt.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jfa.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://voc.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://hwb.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nmk.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nus.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://swp.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://uwa.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://nqo.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://evp.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://noq.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://abd.hfpthk.cn

[D06] 数组长度
来源：http://sch.zhaomingkeji.xyz

Py:   len(arr)
来源：http://tnk.zhixingplan.top

PHP:  count($arr);
来源：http://ubu.mhx1999.top

JS:   arr.length
来源：http://zrf.hywenlv.cn

TS:   arr.length
来源：http://bzv.0kj1m.cn

Java: list.size();
来源：http://zza.zycfv.cn

Go:   len(arr)
来源：http://cta.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://pjw.zhengqikj.top

C#:   list.Count;
来源：http://pgl.c1oappe.top

[D07] 切片 / 取子数组
来源：http://tws.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gqt.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://paq.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://dqz.bbcook.cn


<!-- 参考信息 -->