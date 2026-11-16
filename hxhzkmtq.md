代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kgj.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://czs.zhijiandao.cn

[B07] while 循环
来源：http://pef.tarul.cn

Py:   while i < 10: i += 1
来源：http://vbz.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://ncm.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://pak.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://jbn.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://ffb.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qxi.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://wiz.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://cqc.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://ucw.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://dzm.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vdv.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://ndp.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://xdj.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://oms.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gkq.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://ets.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://jqn.kuanghao11.cn

[B09] break 与 continue
来源：http://ubq.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qyk.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cqe.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mdi.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zoh.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://peb.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ywc.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ccs.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svi.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://tou.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hdl.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jzm.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qdq.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hgr.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://frf.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ehn.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://plw.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ioj.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://bpo.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://jac.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://dlt.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hzv.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://btr.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fvv.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://imx.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://guf.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xev.guannengcc.top

[B12] 跳出多层循环
来源：http://htf.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xrk.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gll.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nxi.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dxd.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://slm.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mss.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kmt.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bkh.aibaodan.cn

[B13] 判断是否为数字
来源：http://jri.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://thx.xuanzx.com

PHP:  is_numeric($x)
来源：http://jdo.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wqq.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hcr.zhixingplan.top

Java: x instanceof Number
来源：http://gqy.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bls.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://zth.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://fmd.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://snt.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cpo.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ety.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://kxy.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://fzv.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hhe.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://afs.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://gmx.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vnn.hnqzz.top

[B15] 布尔运算与取反
来源：http://toh.zhiwuduotai.top

Py:   a and b or not c
来源：http://ten.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://xez.fengsongda.top

JS:   a && b || !c
来源：http://pgi.yangfankeji.com

TS:   a && b || !c
来源：http://wdn.hongshengwenyu.top

Java: a && b || !c
来源：http://vqt.jinghuilouyu.cn

Go:   a && b || !c
来源：http://oix.pycfn.com

Ruby: a && b || !c
来源：http://unl.vehdjk.com

C#:   a && b || !c
来源：http://bie.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://udi.dianchejie.cn

Py:   if not data: return
来源：http://phn.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://eth.ybcxt.top

JS:   if (!data) return;
来源：http://wph.ctjpmb.com

TS:   if (!data) return;
来源：http://olf.ivvv.top

Java: if (data == null) return;
来源：http://usd.aizwys.cn

Go:   if data == nil { return }
来源：http://dmj.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://ovc.iojbl.cn

C#:   if (data == null) return;
来源：http://dia.shuidangran.top

================================================================================
来源：http://yyj.jlsjyb.cn

C. 函数与作用域
来源：http://ipd.shanyushiyangkeji.top

================================================================================
来源：http://uwi.bjfxy.top

[C01] 定义函数
来源：http://bxf.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://uuq.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vtv.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://cew.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrr.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ssk.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://rdl.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://ore.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sae.andypj.xyz

[C02] 默认参数
来源：http://wyy.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://okm.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sjo.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://gvn.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aco.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qsf.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://opx.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://vkv.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://gln.yangfankeji.com

[C03] 可变参数
来源：http://meo.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://lfr.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ecg.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vsd.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://chm.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ytg.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qvf.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hjo.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://awy.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://nww.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tei.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xeb.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kyg.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ari.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://wbv.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://eio.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://njq.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://emf.daria6918.cn

[C05] 返回多个值
来源：http://hdp.xingfuxueyuan.xyz

Py:   return a, b
来源：http://kke.bjfxy.top

PHP:  return [$a, $b];
来源：http://frx.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://uwl.havefunace.top

TS:   return { a, b };
来源：http://yda.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://khm.svipenyu.cn

Go:   return a, b
来源：http://tie.daria6918.cn

Ruby: return a, b
来源：http://ejb.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://nst.cashguo.top

[C06] 匿名函数 / lambda
来源：http://kqp.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://huk.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://upe.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://kmh.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://goq.chenjidiqi.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gow.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ksl.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://sjb.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://yoc.yj20258.top

[C07] 把函数作为参数传入
来源：http://utm.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ajj.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ste.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lmq.zhijiandao.cn

TS:   arr.map(String)
来源：http://zco.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ybk.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://umm.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://too.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lfy.zhaomingkeji.xyz

[C08] 闭包
来源：http://xfi.gogol.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vil.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nkz.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yvi.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cdi.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://csg.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sxi.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://agd.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ctt.kuanghao11.cn

[C09] 递归
来源：http://jge.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jqr.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oew.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wtl.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uph.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://alr.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rzf.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pyk.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wwk.vehdjk.com

[C10] 变量作用域
来源：http://jwb.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xxm.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ksn.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wqe.cheryme.top

TS:   同 JS
来源：http://rgw.vehdjk.com

Java: 方法内为块级作用域
来源：http://thn.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://zml.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nqy.pycfn.com

C#:   块级作用域
来源：http://wri.yangfankeji.com

[C11] 模块导入与导出
来源：http://nkx.zhoulong.xyz

Py:   from module import func
来源：http://gkk.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dzc.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bht.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ike.tianlin.xyz

Java: import java.util.List;
来源：http://fhm.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyy.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://wxz.yonumen.top

C#:   using System.Text;
来源：http://jwk.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://ybz.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://tmq.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://tgd.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://ame.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://umh.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zxj.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://tap.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://jzs.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ptw.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://lhb.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aku.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkc.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bmz.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ojz.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://uif.vehdjk.com

Go:   func add(a, b int) int
来源：http://fys.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bwo.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pad.shangyingyoupin.top

[C14] 泛型函数
来源：http://hfk.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://noo.mhx1999.top

PHP:  // 无泛型
来源：http://nmg.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://xgz.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ifi.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yic.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bnv.vehdjk.com

Ruby: # 无泛型
来源：http://bam.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wky.52xcode.cn

[C15] 解构 / 展开参数
来源：http://ori.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qjf.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://gwu.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tic.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zhh.hywenlv.cn

Java: // 无解构
来源：http://biv.zhijiandao.cn

Go:   // 无解构
来源：http://lze.gzhubu.top

Ruby: a, b = pair
来源：http://eoo.yj20258888.top

C#:   var (a, b) = pair;
来源：http://dsx.fengsongda.top

[C16] 函数 / 方法重载
来源：http://fdm.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oyc.daria6918.cn

PHP:  // 无重载
来源：http://xcb.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lpy.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://qvo.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ckz.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://qmz.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://zvc.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://het.dashuyun.cn

================================================================================
来源：http://yha.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://dzt.hfpthk.cn

================================================================================
来源：http://ofa.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://kbj.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xtz.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sur.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vvs.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qvu.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aqx.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://ckj.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://uon.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grd.ybcxt.top

[D02] 追加元素到末尾
来源：http://htf.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://twp.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://abd.sysykeji.top

JS:   arr.push(4);
来源：http://uen.snrcjt.cn

TS:   arr.push(4);
来源：http://ymq.yueranfly.top

Java: list.add(4);
来源：http://yfk.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://nbw.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://yrc.zhiwuduotai.top

C#:   list.Add(4);
来源：http://stj.cashguo.top

[D03] 在指定位置插入元素
来源：http://uew.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://vtv.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zun.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ops.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://qop.9152youxi.cn

Java: list.add(0, 0);
来源：http://cky.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kly.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qyz.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://uvo.aibaodan.cn

[D04] 删除元素
来源：http://vzf.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yru.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lrp.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rsx.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://uxj.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zws.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ajk.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nem.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sxt.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://ifm.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://emn.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nvp.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jvu.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://sar.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://htl.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://pil.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rsa.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://umt.zhijiandao.cn

[D06] 数组长度
来源：http://lft.jlsjyb.cn

Py:   len(arr)
来源：http://iit.gogol.net.cn

PHP:  count($arr);
来源：http://urw.xylfe.cn

JS:   arr.length
来源：http://qbu.quarkkingdee.top

TS:   arr.length
来源：http://det.daxiang520.top

Java: list.size();
来源：http://hpi.jqgufenzy.top

Go:   len(arr)
来源：http://vja.yvedp.cn

Ruby: arr.length; arr.size
来源：http://bzh.zhiwuduotai.top

C#:   list.Count;
来源：http://rks.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://ewy.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nvd.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://yuo.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://eod.chenzaomai.com


<!-- 参考信息 -->