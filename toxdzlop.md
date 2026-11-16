代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://maj.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://alv.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zti.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xeq.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gla.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://udt.sufxvd.cn

[B07] while 循环
来源：http://iis.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://xem.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://jwe.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://gdq.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://nek.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://gpr.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yrg.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://skp.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://xsx.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://bhz.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://fee.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://auf.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://fwe.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://iyb.sweek.top

Java: do { i++; } while (i < 10);
来源：http://wjq.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lrs.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://pqb.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://rgi.shuidangran.top

[B09] break 与 continue
来源：http://eqo.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ftf.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mkg.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhc.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdz.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqd.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ajt.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tha.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fsa.hammf.cn

[B10] 遍历同时拿索引
来源：http://fau.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zsm.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ear.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qjx.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lao.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uzp.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xxt.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ukz.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wxu.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://iyg.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://sqc.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://avv.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zxv.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vnr.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eup.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kgr.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://iap.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://adz.hcnkem.com

[B12] 跳出多层循环
来源：http://nco.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://phq.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yul.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mrp.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jvu.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vvz.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dud.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vnv.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gnx.tarul.cn

[B13] 判断是否为数字
来源：http://rsj.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://itw.smart0.xyz

PHP:  is_numeric($x)
来源：http://rce.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dds.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avx.guannengcc.top

Java: x instanceof Number
来源：http://ijs.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://foy.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://xoz.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://ygy.shuidangran.top

[B14] 判断值是否在集合内
来源：http://lcs.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hmb.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oso.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://wqk.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://afh.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ris.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sfd.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://jbx.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eoa.xziqi.cn

[B15] 布尔运算与取反
来源：http://jsa.tianlin.xyz

Py:   a and b or not c
来源：http://nut.guannengcc.top

PHP:  $a && $b || !$c
来源：http://dcy.sweek.top

JS:   a && b || !c
来源：http://sru.zhengqikj.top

TS:   a && b || !c
来源：http://sgo.chenzaomai.com

Java: a && b || !c
来源：http://dqb.hesvh.cn

Go:   a && b || !c
来源：http://nys.guowangkeji.top

Ruby: a && b || !c
来源：http://hkl.mhx1999.top

C#:   a && b || !c
来源：http://nci.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://zwa.c1oappe.top

Py:   if not data: return
来源：http://bzr.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://cdz.haohaochexian.top

JS:   if (!data) return;
来源：http://dvr.c1oappe.top

TS:   if (!data) return;
来源：http://qfu.shuidangran.top

Java: if (data == null) return;
来源：http://byp.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://vdj.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://ano.smart0.xyz

C#:   if (data == null) return;
来源：http://iyk.gogol.net.cn

================================================================================
来源：http://bvf.gotoacloud.top

C. 函数与作用域
来源：http://eve.9152youxi.cn

================================================================================
来源：http://pqk.guowangkeji.top

[C01] 定义函数
来源：http://tqz.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://ufv.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rxa.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://vsq.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pnl.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://keg.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://ygk.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://pxs.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ygs.shanyushiyangtech.top

[C02] 默认参数
来源：http://tue.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://xol.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fql.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ydm.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hht.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yvd.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wvb.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://tjs.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://cmk.jinyuanbaomall.cn

[C03] 可变参数
来源：http://byh.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://tjg.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fgo.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysl.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zxj.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zsz.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ufd.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bej.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sph.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://wze.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pig.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oet.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cto.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sxu.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://rre.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://kvk.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://ose.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://qkr.52xcode.cn

[C05] 返回多个值
来源：http://dmo.zycfv.cn

Py:   return a, b
来源：http://tvm.smart0.xyz

PHP:  return [$a, $b];
来源：http://dzq.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wfj.mhx1999.top

TS:   return { a, b };
来源：http://wmp.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ncz.ywan-chungtsiang.top

Go:   return a, b
来源：http://mqn.daria6918.cn

Ruby: return a, b
来源：http://ymr.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://zvz.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://yhh.yueranfly.top

Py:   square = lambda x: x * x
来源：http://xgu.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ugu.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://yeh.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://acc.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fje.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://alq.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://ivw.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://lfh.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://ngo.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xxd.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://rhw.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ylw.chenzaomai.com

TS:   arr.map(String)
来源：http://yvo.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wmc.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zwh.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://afq.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bcu.yongpay.top

[C08] 闭包
来源：http://ghn.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zhf.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hft.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dtv.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zth.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cfj.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cnf.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xpb.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nst.shzxlz.cn

[C09] 递归
来源：http://frv.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wrn.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://owm.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zfl.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ynj.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://isz.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://juv.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://upb.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://edl.mhx1999.top

[C10] 变量作用域
来源：http://vte.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ahe.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://meu.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bnt.fehbvm.com

TS:   同 JS
来源：http://uyl.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://odp.fengsongda.top

Go:   花括号块级作用域
来源：http://hcv.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aii.tarul.cn

C#:   块级作用域
来源：http://jbu.jinqigufen.top

[C11] 模块导入与导出
来源：http://yxn.cucudq.cn

Py:   from module import func
来源：http://qkn.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nwb.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://squ.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zlw.jqgufenzy.top

Java: import java.util.List;
来源：http://cxf.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bbc.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://uup.snrcjt.cn

C#:   using System.Text;
来源：http://eeb.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://kee.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://kql.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://eex.nwbrower.top

JS:   (() => { console.log("run"); })();
来源：http://ghl.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://qcx.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aia.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://zro.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://ajm.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qnz.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://jsq.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://krq.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oeb.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wjd.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abr.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qek.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://mmr.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iss.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://ybk.haohaochexian.top

[C14] 泛型函数
来源：http://lce.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yth.zhengqikj.top

PHP:  // 无泛型
来源：http://yff.epnwcf.com

JS:   // 无泛型
来源：http://pwk.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kpi.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lti.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://clu.yfazqb.com

Ruby: # 无泛型
来源：http://iae.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://alk.cucudq.cn

[C15] 解构 / 展开参数
来源：http://uqk.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zpx.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://asr.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oyy.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dmo.quarkkingdee.top

Java: // 无解构
来源：http://ufc.fengsongda.top

Go:   // 无解构
来源：http://vub.gogol.net.cn

Ruby: a, b = pair
来源：http://yoc.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://jgo.ybcxt.top

[C16] 函数 / 方法重载
来源：http://xnh.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://buv.tarul.cn

PHP:  // 无重载
来源：http://xuu.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ftn.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://suq.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://olk.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://dyr.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://qjd.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hdr.guannengcc.top

================================================================================
来源：http://ehq.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://whs.yj202588.top

================================================================================
来源：http://kca.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://cbe.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uor.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nxg.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jup.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qgm.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://egi.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://uiw.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://iqs.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aui.sysykeji.top

[D02] 追加元素到末尾
来源：http://lbe.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bgh.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cyi.haohaochexian.top

JS:   arr.push(4);
来源：http://udn.hywenlv.cn

TS:   arr.push(4);
来源：http://zdr.yuxming.cn

Java: list.add(4);
来源：http://klu.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://zmy.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://mta.yj20258888.top

C#:   list.Add(4);
来源：http://ukl.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://hla.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://scu.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://quc.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gud.yanxiufei.cn

TS:   arr.splice(0, 0, 0);
来源：http://snr.yj202588.top

Java: list.add(0, 0);
来源：http://ise.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://tar.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ohh.tarul.cn

C#:   list.Insert(0, 0);
来源：http://mps.epnwcf.com

[D04] 删除元素
来源：http://fmn.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ogi.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dld.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gle.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://qgy.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bvz.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://epd.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://inp.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://clt.uphjek.com

[D05] 访问与修改元素
来源：http://kop.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ayu.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://urw.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://amh.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://grs.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://ktl.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://bwz.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zaw.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tjk.cqqwz.cn

[D06] 数组长度
来源：http://ojg.jqgufenzy.top

Py:   len(arr)
来源：http://mgo.guowangkeji.top

PHP:  count($arr);
来源：http://tok.zhaomingkeji.xyz

JS:   arr.length
来源：http://zlz.havefunace.top

TS:   arr.length
来源：http://gfi.jyoumei.cn

Java: list.size();
来源：http://gxe.xylfe.cn

Go:   len(arr)
来源：http://zda.316326.xyz

Ruby: arr.length; arr.size
来源：http://oxd.ehwqpu.com

C#:   list.Count;
来源：http://wyl.xinyue.icu


<!-- 参考信息 -->