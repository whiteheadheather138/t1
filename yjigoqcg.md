代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://oev.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://wcs.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://kvc.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://ell.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ipq.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://fsb.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://vuu.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://fiq.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://zcl.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zuw.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://ynq.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://ges.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://tim.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pgk.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://til.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://vgr.zhengqikj.top

[B09] break 与 continue
来源：http://zdw.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wnb.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dnf.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwl.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uls.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dho.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gij.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fol.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kpf.fktsv.cn

[B10] 遍历同时拿索引
来源：http://fzl.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bbr.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eum.ctjpmb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xfi.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://czv.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ppx.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://msn.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nky.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rex.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://fas.sweek.top

Py:   list(range(0, 10, 2))
来源：http://kws.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://par.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aea.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wen.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wis.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cex.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://eah.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ixr.cashguo.top

[B12] 跳出多层循环
来源：http://llv.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uci.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pyz.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ilo.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hgq.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tdb.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pbg.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gxt.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://joa.hammf.cn

[B13] 判断是否为数字
来源：http://btj.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://pwv.yueranfly.top

PHP:  is_numeric($x)
来源：http://rsp.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lwq.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hju.yj202588.top

Java: x instanceof Number
来源：http://rvq.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xxv.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://vfo.yfazqb.com

C#:   x is int or double or decimal
来源：http://ozv.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://qzk.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bma.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xrc.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://hwr.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://hqv.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://wus.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tyd.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ahc.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wcv.nanxinkj.top

[B15] 布尔运算与取反
来源：http://bcj.bbcook.cn

Py:   a and b or not c
来源：http://kpb.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://iug.nwbrower.top

JS:   a && b || !c
来源：http://urv.gaohongyu789.top

TS:   a && b || !c
来源：http://jaa.jinqigfzy.top

Java: a && b || !c
来源：http://ixz.cheryme.top

Go:   a && b || !c
来源：http://otk.cdnleiting.top

Ruby: a && b || !c
来源：http://mvr.zhengqikj.top

C#:   a && b || !c
来源：http://qjv.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://lxd.cdnleiting.top

Py:   if not data: return
来源：http://whu.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://won.zdqjudy.top

JS:   if (!data) return;
来源：http://grg.hcnkem.com

TS:   if (!data) return;
来源：http://jau.zdqjudy.top

Java: if (data == null) return;
来源：http://qvc.jianghu66.top

Go:   if data == nil { return }
来源：http://iqb.yuxming.cn

Ruby: return if data.nil?
来源：http://mei.iojbl.cn

C#:   if (data == null) return;
来源：http://mfa.zhongyouzk.top

================================================================================
来源：http://alk.52xcode.cn

C. 函数与作用域
来源：http://bao.shuidangran.top

================================================================================
来源：http://crh.sysykeji.top

[C01] 定义函数
来源：http://isl.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://xqa.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flk.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://cvn.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mit.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://wgp.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://kjy.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://jch.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ijg.jqgufenzy.top

[C02] 默认参数
来源：http://gok.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://dkl.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nqz.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://dip.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nif.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bcg.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://szo.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://yly.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://uwg.gogol.net.cn

[C03] 可变参数
来源：http://gle.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://vvg.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lpy.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xpq.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zku.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yxz.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rxm.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vfj.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iid.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://cqd.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lyz.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ozf.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ikr.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pte.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://ywk.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://vfe.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://cux.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://phc.yvedp.cn

[C05] 返回多个值
来源：http://bna.feifeiyinyue.top

Py:   return a, b
来源：http://ciu.hywenlv.cn

PHP:  return [$a, $b];
来源：http://ysd.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://szs.cdnleiting.top

TS:   return { a, b };
来源：http://oxk.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nrf.vehdjk.com

Go:   return a, b
来源：http://lrf.c1oappe.top

Ruby: return a, b
来源：http://fkf.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://aed.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://tdt.c1oappe.top

Py:   square = lambda x: x * x
来源：http://zcg.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pjr.yj20258.top

JS:   const square = x => x * x;
来源：http://qfz.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://mzy.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sqh.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://abh.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://suj.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://pmu.iojbl.cn

[C07] 把函数作为参数传入
来源：http://gri.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gka.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://fdc.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lrj.meibo888.top

TS:   arr.map(String)
来源：http://vav.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zvg.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zeh.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://rpt.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://urc.316326.xyz

[C08] 闭包
来源：http://gvo.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dcd.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tfa.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hhp.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cgw.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hdt.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zyu.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pav.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tgk.gaohongyu789.top

[C09] 递归
来源：http://aes.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ahx.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jwo.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://had.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://miq.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://afv.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wlj.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wgv.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pvi.yongpay.top

[C10] 变量作用域
来源：http://ldk.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://quw.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pbk.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yjv.gotoacloud.top

TS:   同 JS
来源：http://pkl.zdbjq.cn

Java: 方法内为块级作用域
来源：http://ram.tarul.cn

Go:   花括号块级作用域
来源：http://gdr.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://msf.ydzc1.top

C#:   块级作用域
来源：http://ljk.hammf.cn

[C11] 模块导入与导出
来源：http://gve.gotoacloud.top

Py:   from module import func
来源：http://xpd.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gul.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ihl.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://loj.daxiang520.top

Java: import java.util.List;
来源：http://lut.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wgg.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://oig.fanxiaobao.xyz

C#:   using System.Text;
来源：http://ufl.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://emx.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://tbg.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://rhq.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://ejw.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://gdc.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ctk.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://jlh.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://izq.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tfn.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://zdd.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://njl.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oea.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sdr.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujq.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xyg.c1oappe.top

Go:   func add(a, b int) int
来源：http://qbz.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://umc.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uvf.vqdsnc.cn

[C14] 泛型函数
来源：http://qqs.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dbp.chenzaomai.com

PHP:  // 无泛型
来源：http://obl.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://wog.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fxl.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://you.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bsv.316326.xyz

Ruby: # 无泛型
来源：http://yhw.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rez.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://vmj.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://png.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://asq.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ibx.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ihu.fanxiaobao.xyz

Java: // 无解构
来源：http://qoc.iojbl.cn

Go:   // 无解构
来源：http://oxl.fzhhl.top

Ruby: a, b = pair
来源：http://abl.sxryk.cn

C#:   var (a, b) = pair;
来源：http://auo.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://ywx.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iva.fanxiaobao.xyz

PHP:  // 无重载
来源：http://tme.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://zxo.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://gkt.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://scc.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://idl.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://hrh.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://npj.meibo888.top

================================================================================
来源：http://ihe.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://ehk.nwbrower.top

================================================================================
来源：http://zbq.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://cwb.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://tpc.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://efr.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kcv.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bxb.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pxr.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://leo.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://fpg.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blj.cheryme.top

[D02] 追加元素到末尾
来源：http://pcd.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sod.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gds.bjfxy.top

JS:   arr.push(4);
来源：http://cpf.yangfankeji.com

TS:   arr.push(4);
来源：http://iqu.52xcode.cn

Java: list.add(4);
来源：http://gsm.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://gzu.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://adx.wangshuangyany.cn

C#:   list.Add(4);
来源：http://zqb.hcnkem.com

[D03] 在指定位置插入元素
来源：http://tay.316326.xyz

Py:   arr.insert(0, 0)
来源：http://ous.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qct.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qmp.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://hqn.nanxuanxn.top

Java: list.add(0, 0);
来源：http://hgf.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://rjm.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uke.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://qoj.hnxiangtu.top

[D04] 删除元素
来源：http://ldu.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kqf.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dms.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ese.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://wha.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fvb.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aym.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uup.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ucc.chenlongwang.top

[D05] 访问与修改元素
来源：http://pfp.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qjl.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mln.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vxv.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://fgo.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://mrj.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://mjr.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dan.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://irk.zhoulong.xyz

[D06] 数组长度
来源：http://kjt.yueranfly.top

Py:   len(arr)
来源：http://dbq.birdmap.top

PHP:  count($arr);
来源：http://axw.pengpengdd.cyou

JS:   arr.length
来源：http://gnt.pycfn.com

TS:   arr.length
来源：http://uth.jqgufenzy.top

Java: list.size();
来源：http://fzr.zhongyouzk.top

Go:   len(arr)
来源：http://fdl.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://srz.jinyuanbaomall.cn

C#:   list.Count;
来源：http://gow.yvedp.cn

[D07] 切片 / 取子数组
来源：http://eyq.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ngg.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wvo.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://lag.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://wwa.jyoumei.cn

Java: list.subList(1, 4);
来源：http://ady.jlsjyb.cn

Go:   arr[1:4]
来源：http://udq.jqgfzy.top

Ruby: arr[1, 3]
来源：http://fsf.zhengqikj.top


<!-- 参考信息 -->