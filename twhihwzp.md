代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dsy.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://xjt.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://ffj.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://nnz.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://ovx.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bej.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://hde.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://apn.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://mqb.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://apx.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://ldb.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://kfd.aibaodan.cn

[B09] break 与 continue
来源：http://fwb.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qet.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jsv.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://juq.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lcg.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shx.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xqc.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vww.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgq.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://fvs.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://scd.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ifs.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rir.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aov.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mav.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ekv.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ftl.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vvy.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://wrg.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://gbh.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://niw.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wte.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yhj.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ecd.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://efv.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://hhx.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zcc.havefunace.top

[B12] 跳出多层循环
来源：http://xdc.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://czf.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wtg.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://foi.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qhg.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tnh.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cfu.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ght.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wck.yj202588.top

[B13] 判断是否为数字
来源：http://tss.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://isz.tanke756.top

PHP:  is_numeric($x)
来源：http://fbm.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsf.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vxm.hnqzz.top

Java: x instanceof Number
来源：http://mwr.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bvj.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://zxk.chenlongwang.top

C#:   x is int or double or decimal
来源：http://zbq.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://ubh.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://key.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yue.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://oyg.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://mqf.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fbw.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tjf.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://xhv.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://etm.chenlongwang.top

[B15] 布尔运算与取反
来源：http://bxw.chenlongwang.top

Py:   a and b or not c
来源：http://tmo.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://fwk.wangdashe.top

JS:   a && b || !c
来源：http://jbo.jqgfzy.top

TS:   a && b || !c
来源：http://vwd.smart0.xyz

Java: a && b || !c
来源：http://ttn.hywenlv.cn

Go:   a && b || !c
来源：http://mjg.jyoumei.cn

Ruby: a && b || !c
来源：http://fjb.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://upp.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://wtx.ctjpmb.com

Py:   if not data: return
来源：http://kgw.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://dcp.52xcode.cn

JS:   if (!data) return;
来源：http://xus.zhijiandao.cn

TS:   if (!data) return;
来源：http://mpb.yongpay.top

Java: if (data == null) return;
来源：http://gaz.jinqigfzy.top

Go:   if data == nil { return }
来源：http://jec.hammf.cn

Ruby: return if data.nil?
来源：http://lal.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://zte.ydzc1.top

================================================================================
来源：http://kft.guannengcc.top

C. 函数与作用域
来源：http://vqe.daria6918.cn

================================================================================
来源：http://jox.chenzaomai.com

[C01] 定义函数
来源：http://avr.hammf.cn

Py:   def add(a, b): return a + b
来源：http://iew.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jbf.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://kqo.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsq.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ooq.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://gvi.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://ogq.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dwr.hesvh.cn

[C02] 默认参数
来源：http://qbe.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://spi.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mpu.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://vmw.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://siu.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gzy.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sho.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://gru.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://fwb.fanxiaobao.xyz

[C03] 可变参数
来源：http://eio.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://kzm.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eej.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ybq.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzc.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ddn.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdw.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qdq.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://smc.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://zkh.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gtc.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mxf.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zdr.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xto.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://kpm.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://bjd.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://wyg.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://nxq.yj20258.top

[C05] 返回多个值
来源：http://yfb.bjfxy.top

Py:   return a, b
来源：http://ewa.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://llk.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rgk.pengpengdd.cyou

TS:   return { a, b };
来源：http://zlg.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hre.xinyue.icu

Go:   return a, b
来源：http://xee.sjlbkw.cn

Ruby: return a, b
来源：http://xce.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://ykh.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://lhd.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://dyi.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qbe.shzxlz.cn

JS:   const square = x => x * x;
来源：http://osn.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://jsc.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jhh.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hdo.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://kxu.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ecp.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://han.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://smf.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gsn.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tfw.xuanzx.com

TS:   arr.map(String)
来源：http://bes.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwl.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yid.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://msd.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wdr.hesvh.cn

[C08] 闭包
来源：http://qbv.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rqt.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jhg.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lnl.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fyt.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xhi.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nmk.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cnl.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pxd.sysykeji.top

[C09] 递归
来源：http://rmg.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nnb.haohaochexian.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xuh.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yug.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hlb.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rmc.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qyj.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ruh.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uxo.zhixingplan.top

[C10] 变量作用域
来源：http://enl.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://adb.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zfs.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lll.kuanghao11.cn

TS:   同 JS
来源：http://wfv.daria6918.cn

Java: 方法内为块级作用域
来源：http://zet.yj20258888.top

Go:   花括号块级作用域
来源：http://xmc.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nvf.jlsjyb.cn

C#:   块级作用域
来源：http://hhq.zhengqikj.top

[C11] 模块导入与导出
来源：http://hjb.52xcode.cn

Py:   from module import func
来源：http://mdh.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://inu.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://kuy.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ovv.cashguo.top

Java: import java.util.List;
来源：http://tab.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gfo.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://iyv.vqdsnc.cn

C#:   using System.Text;
来源：http://liy.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://khf.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://gjj.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://axp.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://ozc.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://adx.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jiq.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://uhr.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://mfx.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://olo.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://joy.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://suf.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rea.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ksv.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vay.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ydu.gogol.net.cn

Go:   func add(a, b int) int
来源：http://fsd.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ywc.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vwb.zhixingplan.top

[C14] 泛型函数
来源：http://ses.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fiu.chenlongwang.top

PHP:  // 无泛型
来源：http://vzq.yangfankeji.com

JS:   // 无泛型
来源：http://iwy.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wpe.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zjm.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qzr.mhx1999.top

Ruby: # 无泛型
来源：http://wqv.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xcq.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://dzh.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://poz.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://pvx.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://akz.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yzw.zhijiandao.cn

Java: // 无解构
来源：http://kqe.ywan-chungtsiang.top

Go:   // 无解构
来源：http://hca.zhongyouzk.top

Ruby: a, b = pair
来源：http://fud.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://nzi.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://mhv.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sjo.bbcook.cn

PHP:  // 无重载
来源：http://zgz.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nyh.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://pdm.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wfd.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://nha.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://gqt.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://msj.smart0.xyz

================================================================================
来源：http://sxs.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://jhm.gotoacloud.top

================================================================================
来源：http://hay.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://elb.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jou.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hhx.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://brs.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lzg.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lio.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://wyc.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://kej.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fmx.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://jjx.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sfj.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nht.zhengqikj.top

JS:   arr.push(4);
来源：http://wdk.zhongyouzk.top

TS:   arr.push(4);
来源：http://kwp.yfazqb.com

Java: list.add(4);
来源：http://hwe.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://zhy.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://ywy.tarul.cn

C#:   list.Add(4);
来源：http://ulq.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://ceu.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://ccg.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eoi.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cje.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://pbd.316326.xyz

Java: list.add(0, 0);
来源：http://eis.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://tbz.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jdn.ivvv.top

C#:   list.Insert(0, 0);
来源：http://lbs.zdqjudy.top

[D04] 删除元素
来源：http://wpo.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://efv.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mcv.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://alt.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://dzg.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://doc.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zow.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kiy.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmy.fktsv.cn

[D05] 访问与修改元素
来源：http://tug.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lwd.shanyushiyangtech.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nfk.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xog.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://twa.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://xxl.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://owh.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://igq.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://czy.yongpay.top

[D06] 数组长度
来源：http://zkx.zycfv.cn

Py:   len(arr)
来源：http://vna.sweek.top

PHP:  count($arr);
来源：http://ltd.guowangkeji.top

JS:   arr.length
来源：http://laz.yangfankeji.com

TS:   arr.length
来源：http://yyj.jinyuanbaomall.cn

Java: list.size();
来源：http://ntg.smart0.xyz

Go:   len(arr)
来源：http://pbq.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://bge.cqqwz.cn

C#:   list.Count;
来源：http://guy.guannengcc.top

[D07] 切片 / 取子数组
来源：http://nnr.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oru.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ggt.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://oam.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://pqj.snrcjt.cn

Java: list.subList(1, 4);
来源：http://epz.daria6918.cn

Go:   arr[1:4]
来源：http://gnb.jinqigufen.top

Ruby: arr[1, 3]
来源：http://mnq.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://ami.hesvh.cn

[D08] 合并两个数组
来源：http://rxo.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://kgy.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://lwk.xuanzx.com


<!-- 参考信息 -->