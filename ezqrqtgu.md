代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://itu.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://gap.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://kuc.tanke756.top

Java: while (i < 10) { i++; }
来源：http://dov.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ebf.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://ytv.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://qnp.xziqi.cn

[B08] do-while（至少执行一次）
来源：http://aim.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://tql.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nve.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://snn.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://jht.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://fzi.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iuv.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fcf.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://qfk.shangyingyoupin.top

[B09] break 与 continue
来源：http://bxr.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mfe.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fqf.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvt.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmf.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxi.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qwn.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ltg.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tpf.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://uzp.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ews.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ojh.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vsu.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zie.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://laa.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dlr.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kja.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ytx.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://snx.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://dlm.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://eix.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oos.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ysm.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uzg.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nqe.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://yfn.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pra.guowangkeji.top

[B12] 跳出多层循环
来源：http://gzr.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vqu.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://aep.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://okj.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jam.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rul.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rei.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lhp.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bpj.haohaochexian.top

[B13] 判断是否为数字
来源：http://ogk.zhaomingkeji.xyz

Py:   isinstance(x, (int, float))
来源：http://zpu.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://apn.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsl.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sim.yuanzhike.top

Java: x instanceof Number
来源：http://alb.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sst.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://kjs.guowangkeji.top

C#:   x is int or double or decimal
来源：http://bia.daxiang520.top

[B14] 判断值是否在集合内
来源：http://nbg.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cef.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://npp.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://vrm.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://sll.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qal.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cmv.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://wub.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hvs.guannengcc.top

[B15] 布尔运算与取反
来源：http://zte.sysykeji.top

Py:   a and b or not c
来源：http://xgg.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://rbu.aibaodan.cn

JS:   a && b || !c
来源：http://fcs.bjfxy.top

TS:   a && b || !c
来源：http://wnd.jinghuilouyu.cn

Java: a && b || !c
来源：http://kqg.andypj.xyz

Go:   a && b || !c
来源：http://ymr.316326.xyz

Ruby: a && b || !c
来源：http://bvq.ivvv.top

C#:   a && b || !c
来源：http://wth.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://pld.fanxiaobao.xyz

Py:   if not data: return
来源：http://acl.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://owq.hongshengwenyu.top

JS:   if (!data) return;
来源：http://fza.yj202588.top

TS:   if (!data) return;
来源：http://ymp.birdmap.top

Java: if (data == null) return;
来源：http://kmk.jianghu66.top

Go:   if data == nil { return }
来源：http://jhy.gaohongyu789.top

Ruby: return if data.nil?
来源：http://lrl.fehbvm.com

C#:   if (data == null) return;
来源：http://iyt.jianghu66.top

================================================================================
来源：http://wyv.zycfv.cn

C. 函数与作用域
来源：http://idq.fanxiaobao.xyz

================================================================================
来源：http://hja.jinyuanbaomall.cn

[C01] 定义函数
来源：http://lhb.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://wql.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xbq.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://udx.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxq.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zch.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://php.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://mbg.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://idm.quarkkingdee.top

[C02] 默认参数
来源：http://xed.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://vkv.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ouu.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://cvx.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zkf.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://duk.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uxd.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://yol.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://bei.gzhubu.top

[C03] 可变参数
来源：http://wpq.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://iqv.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vwj.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zhc.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wka.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rjd.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iqk.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ryy.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oks.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://srk.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xyu.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qnk.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ydz.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mcz.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://dua.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://dfg.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://srt.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://bqt.hesvh.cn

[C05] 返回多个值
来源：http://cvc.gogol.net.cn

Py:   return a, b
来源：http://gjt.jinqigufen.top

PHP:  return [$a, $b];
来源：http://rsz.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lio.yongpay.top

TS:   return { a, b };
来源：http://qzk.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tum.gaohongyu789.top

Go:   return a, b
来源：http://key.zycfv.cn

Ruby: return a, b
来源：http://qtn.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://cbb.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://lvh.quarkkingdee.top

Py:   square = lambda x: x * x
来源：http://scj.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xdk.snrcjt.cn

JS:   const square = x => x * x;
来源：http://rsj.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://kpr.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pbs.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://yzd.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://uxy.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://svz.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://wrz.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hyd.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://yfh.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xok.tanke756.top

TS:   arr.map(String)
来源：http://znu.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dxi.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wax.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://zqu.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://khy.dashuyun.cn

[C08] 闭包
来源：http://dfa.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vsw.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ugf.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gzz.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yzs.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://igx.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://plp.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vbs.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nku.jqgfzy.top

[C09] 递归
来源：http://mlp.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dug.cdnleiting.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qho.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mcn.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nez.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://epw.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tay.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fif.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zxm.guannengcc.top

[C10] 变量作用域
来源：http://eqf.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ria.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bfi.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rrj.jqgufenzy.top

TS:   同 JS
来源：http://thm.hywenlv.cn

Java: 方法内为块级作用域
来源：http://smz.uphjek.com

Go:   花括号块级作用域
来源：http://vwg.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wkr.cheryme.top

C#:   块级作用域
来源：http://tct.jinqigufen.top

[C11] 模块导入与导出
来源：http://gmx.c1oappe.top

Py:   from module import func
来源：http://sny.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iwq.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://csj.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmm.hnxiangtu.top

Java: import java.util.List;
来源：http://wfz.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://duc.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://bwc.cheryme.top

C#:   using System.Text;
来源：http://drc.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://fuu.birdmap.top

Py:   (lambda: print("run"))()
来源：http://clt.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://jaw.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://chk.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://nqc.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vyn.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://jtr.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://dny.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://see.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://swk.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://msg.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkg.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xjm.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hgj.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://pfy.yj20258888.top

Go:   func add(a, b int) int
来源：http://ivm.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pwl.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://izq.xuanzx.com

[C14] 泛型函数
来源：http://ssg.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://slm.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://xjg.hysaishi.cn

JS:   // 无泛型
来源：http://rzi.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ljg.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lti.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wto.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://jnb.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lou.hcnkem.com

[C15] 解构 / 展开参数
来源：http://ren.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ndp.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://dbc.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://djc.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uje.sjlbkw.cn

Java: // 无解构
来源：http://iyi.chenzaomai.com

Go:   // 无解构
来源：http://khu.sysykeji.top

Ruby: a, b = pair
来源：http://erp.bbcook.cn

C#:   var (a, b) = pair;
来源：http://gde.cucudq.cn

[C16] 函数 / 方法重载
来源：http://buw.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zjw.snrcjt.cn

PHP:  // 无重载
来源：http://ogh.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xrp.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://zpk.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://yin.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://rwr.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://ldy.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://unp.xuanzx.com

================================================================================
来源：http://fbf.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://alo.svipenyu.cn

================================================================================
来源：http://ihj.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://qbh.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://wro.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pft.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fyn.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yhq.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hmy.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://iqq.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://xvl.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hro.meibo888.top

[D02] 追加元素到末尾
来源：http://dir.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mce.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dsq.feifeiyinyue.top

JS:   arr.push(4);
来源：http://gih.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://tup.nwbrower.top

Java: list.add(4);
来源：http://yhk.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://wls.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://chx.mhx1999.top

C#:   list.Add(4);
来源：http://fbi.yj20258888.top

[D03] 在指定位置插入元素
来源：http://sut.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://amv.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tgk.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tbj.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://prz.fktsv.cn

Java: list.add(0, 0);
来源：http://ntb.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://isv.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wrf.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://nuw.xuanzx.com

[D04] 删除元素
来源：http://cid.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wpg.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rfq.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cjq.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://icr.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sat.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mhv.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iui.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://crm.gzhubu.top

[D05] 访问与修改元素
来源：http://txp.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://apr.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kjo.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ddm.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://qqj.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://vls.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://dqh.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kbc.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kfc.dianchejie.cn

[D06] 数组长度
来源：http://ubd.shangyingyoupin.top

Py:   len(arr)
来源：http://vmi.hnqzz.top

PHP:  count($arr);
来源：http://rqi.tianlin.xyz

JS:   arr.length
来源：http://vkw.pengpengdd.cyou

TS:   arr.length
来源：http://mtt.jinqigfzy.top

Java: list.size();
来源：http://nav.hfpthk.cn

Go:   len(arr)
来源：http://vqh.pycfn.com

Ruby: arr.length; arr.size
来源：http://bvn.yangfankeji.com

C#:   list.Count;
来源：http://zfp.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://brp.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cua.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://vma.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://zvq.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://sfp.guannengcc.top

Java: list.subList(1, 4);
来源：http://tys.zdbjq.cn

Go:   arr[1:4]
来源：http://yfe.nanxinkj.top

Ruby: arr[1, 3]
来源：http://ezf.yj20258.top


<!-- 参考信息 -->