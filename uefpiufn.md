代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wel.pycfn.com

[B06] 遍历字典 / 对象
来源：http://frw.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ywt.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ptj.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dam.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhl.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pir.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://joq.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://btq.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zbi.hnqzz.top

[B07] while 循环
来源：http://xyq.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://uoi.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://vry.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://kvq.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://lhd.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://erf.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jkk.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://iqs.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://tea.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://cnm.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://eup.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lmf.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://rdz.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://spa.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://dqf.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rik.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rez.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://uqs.pycfn.com

[B09] break 与 continue
来源：http://nfl.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gyh.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xte.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qya.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsq.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zap.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iuj.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yrl.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wvh.jianghu66.top

[B10] 遍历同时拿索引
来源：http://ehq.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uxy.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yuu.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fkm.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wkd.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xvc.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ids.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mgj.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sdo.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://whk.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://pxr.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://sin.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dyv.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rcs.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rvv.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uet.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://hoi.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hct.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://vob.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kdp.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kpg.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jcr.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cce.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nhe.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zqc.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bkr.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lnd.havefunace.top

[B13] 判断是否为数字
来源：http://rfi.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://yjz.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://nwd.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghv.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ftt.yanxiufei.cn

Java: x instanceof Number
来源：http://syr.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wod.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://xqb.shzxlz.cn

C#:   x is int or double or decimal
来源：http://yor.sweek.top

[B14] 判断值是否在集合内
来源：http://mop.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lmm.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hpg.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://zsd.shuidangran.top

TS:   [1, 2, 3].includes(x)
来源：http://uss.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xwy.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vti.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://vhz.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nfl.tian-w.cn

[B15] 布尔运算与取反
来源：http://cuo.uphjek.com

Py:   a and b or not c
来源：http://nma.cucudq.cn

PHP:  $a && $b || !$c
来源：http://jac.yangfankeji.com

JS:   a && b || !c
来源：http://bsi.hfpthk.cn

TS:   a && b || !c
来源：http://ctk.fzhhl.top

Java: a && b || !c
来源：http://lxt.hysaishi.cn

Go:   a && b || !c
来源：http://wzi.wangdashe.top

Ruby: a && b || !c
来源：http://rec.zdqjudy.top

C#:   a && b || !c
来源：http://clb.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bit.chenlongwang.top

Py:   if not data: return
来源：http://xvb.yj20258.top

PHP:  if (!$data) { return; }
来源：http://fnd.9152youxi.cn

JS:   if (!data) return;
来源：http://jni.fzhhl.top

TS:   if (!data) return;
来源：http://ydn.jqgfzy.top

Java: if (data == null) return;
来源：http://oyf.sufxvd.cn

Go:   if data == nil { return }
来源：http://zmo.sysykeji.top

Ruby: return if data.nil?
来源：http://loc.0kj1m.cn

C#:   if (data == null) return;
来源：http://blr.mhx1999.top

================================================================================
来源：http://juq.gotoacloud.top

C. 函数与作用域
来源：http://vyb.vqdsnc.cn

================================================================================
来源：http://sti.yueranfly.top

[C01] 定义函数
来源：http://bjl.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://cgm.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vhy.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://msy.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iac.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ayf.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iap.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://wfc.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lpc.smart0.xyz

[C02] 默认参数
来源：http://eqa.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://gqw.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wjd.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://ehj.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uja.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fnf.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://icx.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://ayw.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://mnx.hcnkem.com

[C03] 可变参数
来源：http://uar.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://igk.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fla.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ozz.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzt.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nbt.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nly.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ovg.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://emr.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://gnb.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nkc.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://doi.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ahl.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hva.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://uaa.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://osp.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://vjz.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://yvz.xziqi.cn

[C05] 返回多个值
来源：http://ykd.shanyushiyangtech.top

Py:   return a, b
来源：http://wox.316326.xyz

PHP:  return [$a, $b];
来源：http://ita.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://psa.daria6918.cn

TS:   return { a, b };
来源：http://lot.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ruh.sjlbkw.cn

Go:   return a, b
来源：http://dqi.52xcode.cn

Ruby: return a, b
来源：http://tlo.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://rbb.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://tzt.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://ois.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jbf.yfazqb.com

JS:   const square = x => x * x;
来源：http://hae.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://cpp.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ads.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://xds.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://kni.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tgb.xinyue.icu

[C07] 把函数作为参数传入
来源：http://aln.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://scq.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aqd.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ayy.xuetiantiany.cn

TS:   arr.map(String)
来源：http://lht.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kag.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://grl.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://jng.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yhr.cashguo.top

[C08] 闭包
来源：http://tia.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qef.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://agj.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mbk.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pxt.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kvm.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rde.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eqe.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qkg.yvedp.cn

[C09] 递归
来源：http://mul.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ltx.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dmu.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bzl.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wia.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pdo.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xub.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uuv.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://daf.jqgufenzy.top

[C10] 变量作用域
来源：http://ptv.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ulm.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cjc.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tkr.yfazqb.com

TS:   同 JS
来源：http://kiv.sxryk.cn

Java: 方法内为块级作用域
来源：http://nqk.hcnkem.com

Go:   花括号块级作用域
来源：http://vku.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eov.smart0.xyz

C#:   块级作用域
来源：http://pie.mhx1999.top

[C11] 模块导入与导出
来源：http://xto.tianlin.xyz

Py:   from module import func
来源：http://pxx.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://txb.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ntz.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pyf.zhijiandao.cn

Java: import java.util.List;
来源：http://oln.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pnb.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://pwn.jianghu66.top

C#:   using System.Text;
来源：http://ugx.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://bht.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://dly.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://kfy.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://ngc.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://ilf.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bde.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://ghh.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://zeh.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rmn.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://dip.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oje.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wal.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ibi.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qgt.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://fvb.vehdjk.com

Go:   func add(a, b int) int
来源：http://bjg.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yai.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://dmq.tian-w.cn

[C14] 泛型函数
来源：http://ucx.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rgp.gogol.net.cn

PHP:  // 无泛型
来源：http://yqp.sjlbkw.cn

JS:   // 无泛型
来源：http://jwv.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iev.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ftf.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ooy.cheryme.top

Ruby: # 无泛型
来源：http://sfk.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ceh.hammf.cn

[C15] 解构 / 展开参数
来源：http://zwg.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mog.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://nzo.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qzy.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fks.52xcode.cn

Java: // 无解构
来源：http://ned.xuetiantiany.cn

Go:   // 无解构
来源：http://nzv.cdnleiting.top

Ruby: a, b = pair
来源：http://ksv.yuxming.cn

C#:   var (a, b) = pair;
来源：http://cnf.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://qru.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wqj.zhongyouzk.top

PHP:  // 无重载
来源：http://don.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dac.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://xuv.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eyl.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://kei.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://gts.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tbv.gotoacloud.top

================================================================================
来源：http://cvq.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://xqh.cqqwz.cn

================================================================================
来源：http://lhe.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://ngx.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yzh.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://owg.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tzp.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://hwz.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bos.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://rgp.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://qgl.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hfw.hesvh.cn

[D02] 追加元素到末尾
来源：http://mez.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iyy.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bvk.ydzc1.top

JS:   arr.push(4);
来源：http://qah.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://sqp.yfazqb.com

Java: list.add(4);
来源：http://fga.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://zwh.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://eto.tanke756.top

C#:   list.Add(4);
来源：http://tyn.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://mqs.havefunace.top

Py:   arr.insert(0, 0)
来源：http://pyi.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sda.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cuo.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://slh.ydzc1.top

Java: list.add(0, 0);
来源：http://ncy.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://slm.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sxf.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://rof.tian-w.cn

[D04] 删除元素
来源：http://cec.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ehu.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ytn.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mxx.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://jxw.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ptk.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tel.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xkx.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://guw.xziqi.cn

[D05] 访问与修改元素
来源：http://urv.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hpl.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bhe.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xnv.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://mvi.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://suf.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://ves.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vkh.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://irr.yonumen.top

[D06] 数组长度
来源：http://oyw.jinghuilouyu.cn

Py:   len(arr)
来源：http://cwz.zhixingplan.top

PHP:  count($arr);
来源：http://eno.0kj1m.cn

JS:   arr.length
来源：http://sac.yvedp.cn

TS:   arr.length
来源：http://shv.dianchejie.cn


<!-- 参考信息 -->