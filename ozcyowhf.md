代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://kty.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://qhx.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://lwr.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://uur.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gyc.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://jkw.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://ips.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://xkm.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://ask.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vqj.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://rvq.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://ohy.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://xmz.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pcd.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://bzw.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://bmi.daria6918.cn

[B09] break 与 continue
来源：http://yqi.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wlm.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ehk.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtg.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckg.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgn.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ygd.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rjk.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eix.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://sjc.aizwys.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ssw.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cks.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xyi.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ebc.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://snw.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wxf.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bsv.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tqq.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://ery.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://bmw.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://osf.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlk.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nzo.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ocb.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ewu.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://sgf.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pdu.yfazqb.com

[B12] 跳出多层循环
来源：http://cgv.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ndq.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qmv.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qdo.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ylb.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ijc.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fgi.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lkm.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ulm.yongpay.top

[B13] 判断是否为数字
来源：http://mui.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://crh.fehbvm.com

PHP:  is_numeric($x)
来源：http://viv.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jha.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://url.tianlin.xyz

Java: x instanceof Number
来源：http://bhh.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iiw.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://zwd.shuidangran.top

C#:   x is int or double or decimal
来源：http://lrb.aizwys.cn

[B14] 判断值是否在集合内
来源：http://aoi.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zeh.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sdj.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://ezf.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://iwp.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tft.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hio.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://vma.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fqj.cqqwz.cn

[B15] 布尔运算与取反
来源：http://aov.chenzaomai.com

Py:   a and b or not c
来源：http://jwf.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://dag.hcnkem.com

JS:   a && b || !c
来源：http://aps.yuxming.cn

TS:   a && b || !c
来源：http://ojj.ydzc1.top

Java: a && b || !c
来源：http://cpb.cheryme.top

Go:   a && b || !c
来源：http://udo.yj202588.top

Ruby: a && b || !c
来源：http://aik.shuidangran.top

C#:   a && b || !c
来源：http://xem.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://lse.zhoulong.xyz

Py:   if not data: return
来源：http://vjf.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://zjw.birdmap.top

JS:   if (!data) return;
来源：http://pkg.daxiang520.top

TS:   if (!data) return;
来源：http://zim.jlsjyb.cn

Java: if (data == null) return;
来源：http://peg.jinqigfzy.top

Go:   if data == nil { return }
来源：http://nyk.smart0.xyz

Ruby: return if data.nil?
来源：http://yxd.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://wme.hysaishi.cn

================================================================================
来源：http://pby.svipenyu.cn

C. 函数与作用域
来源：http://smx.hesvh.cn

================================================================================
来源：http://qai.hnqzz.top

[C01] 定义函数
来源：http://evs.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://kxp.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eua.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://rnb.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wzd.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://sea.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://wpd.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://xzl.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fad.yvedp.cn

[C02] 默认参数
来源：http://jbd.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://ema.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uho.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://ohb.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://npv.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kie.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dmy.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://klf.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://wsb.nwbrower.top

[C03] 可变参数
来源：http://sya.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://mln.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yep.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vyn.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbt.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xut.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://utp.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oph.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lvo.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://yfb.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://joh.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yvf.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vrh.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uem.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://dte.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://zqv.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://wcq.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://chr.ehwqpu.com

[C05] 返回多个值
来源：http://dub.ydjk.org.cn

Py:   return a, b
来源：http://jvg.smart0.xyz

PHP:  return [$a, $b];
来源：http://rdv.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bcr.ehwqpu.com

TS:   return { a, b };
来源：http://xfv.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dfm.andypj.xyz

Go:   return a, b
来源：http://tpg.quarkkingdee.top

Ruby: return a, b
来源：http://ndc.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://zzm.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://qcd.yanxiufei.cn

Py:   square = lambda x: x * x
来源：http://yvs.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oxy.snrcjt.cn

JS:   const square = x => x * x;
来源：http://oda.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://cij.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ube.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://btz.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://sbe.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://cgg.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://njk.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qzq.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hii.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bqi.hywenlv.cn

TS:   arr.map(String)
来源：http://cnr.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zai.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sdq.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://czh.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ery.gaohongyu789.top

[C08] 闭包
来源：http://esr.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sgg.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uew.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ihe.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://usy.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hdr.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://djb.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ump.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://opt.iojbl.cn

[C09] 递归
来源：http://zmx.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tfp.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nlr.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ywf.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uyo.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pqd.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jic.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fam.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cyn.xuetiantiany.cn

[C10] 变量作用域
来源：http://byf.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gyw.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mnm.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sle.haohaochexian.top

TS:   同 JS
来源：http://ngb.cucudq.cn

Java: 方法内为块级作用域
来源：http://czz.gzhubu.top

Go:   花括号块级作用域
来源：http://hko.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uaj.yuanzhike.top

C#:   块级作用域
来源：http://vmc.tian-w.cn

[C11] 模块导入与导出
来源：http://jfx.fanxiaobao.xyz

Py:   from module import func
来源：http://huu.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://blx.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://usw.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dgs.quarkkingdee.top

Java: import java.util.List;
来源：http://rgn.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xxb.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://uje.fktsv.cn

C#:   using System.Text;
来源：http://ftt.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://kfd.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://irj.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://toi.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://eif.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://uoy.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uml.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://ojk.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://noc.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://anq.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://csf.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pgv.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zih.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://drx.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yuu.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://gno.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://lhb.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://geg.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hrs.jqgufenzy.top

[C14] 泛型函数
来源：http://wax.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tjj.hesvh.cn

PHP:  // 无泛型
来源：http://pkn.fanxiaobao.xyz

JS:   // 无泛型
来源：http://fkj.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zea.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rlj.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kyu.chenlongwang.top

Ruby: # 无泛型
来源：http://jue.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mxn.ybcxt.top

[C15] 解构 / 展开参数
来源：http://uzt.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dbk.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://fqy.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://viz.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qub.redwolf501.top

Java: // 无解构
来源：http://hnc.mhx1999.top

Go:   // 无解构
来源：http://mrz.fehbvm.com

Ruby: a, b = pair
来源：http://aox.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://vkl.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://dxw.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hew.bbcook.cn

PHP:  // 无重载
来源：http://bbi.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uju.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://dbf.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lhr.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://fzq.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://nne.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://czw.shanyushiyangtech.top

================================================================================
来源：http://zjq.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://kmn.smart0.xyz

================================================================================
来源：http://sxm.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://dhn.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nzs.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oih.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uxv.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ghm.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blu.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://okx.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://xjg.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pou.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://htn.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jif.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tfe.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://yuk.hnxiangtu.top

TS:   arr.push(4);
来源：http://oow.hcnkem.com

Java: list.add(4);
来源：http://xbp.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://gdr.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xmn.jinqigufen.top

C#:   list.Add(4);
来源：http://okb.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://ofb.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://chz.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://upn.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://upd.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://kty.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://gex.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://waa.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xvy.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://qfm.aizwys.cn

[D04] 删除元素
来源：http://svk.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qud.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fgo.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ndi.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://xdv.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dut.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://liz.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lub.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btn.jqgfzy.top

[D05] 访问与修改元素
来源：http://bxp.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hkr.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://asy.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ntk.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://yvg.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://xwu.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://obz.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://apr.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mvs.xuetiantiany.cn

[D06] 数组长度
来源：http://bkl.hammf.cn

Py:   len(arr)
来源：http://vuj.cheryme.top

PHP:  count($arr);
来源：http://cgy.jianghu66.top

JS:   arr.length
来源：http://tet.yonumen.top

TS:   arr.length
来源：http://eoy.jinqigufen.top

Java: list.size();
来源：http://hpt.hcnkem.com

Go:   len(arr)
来源：http://eap.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://nmb.bbcook.cn

C#:   list.Count;
来源：http://gvx.zycfv.cn

[D07] 切片 / 取子数组
来源：http://ehf.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fub.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://dty.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://wat.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://xdm.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://hcw.jianghu66.top

Go:   arr[1:4]
来源：http://yxz.ehwqpu.com

Ruby: arr[1, 3]
来源：http://qla.hnxiangtu.top


<!-- 参考信息 -->