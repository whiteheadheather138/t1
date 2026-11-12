代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ojl.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://mcj.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://mra.redwolf501.top

[B08] do-while（至少执行一次）
来源：http://jbc.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://rkz.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://kij.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://sbf.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://lij.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://kqq.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://glv.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://ttj.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://ryb.dashuyun.cn

[B09] break 与 continue
来源：http://fgc.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ynk.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tyr.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgh.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqo.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shu.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hqh.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eit.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpt.xziqi.cn

[B10] 遍历同时拿索引
来源：http://gcm.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zfs.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cfj.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hno.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gci.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cla.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mte.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sts.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mfj.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://nmt.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://alk.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://jbd.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hkq.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://awd.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aae.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cvy.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://hsn.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gbz.uphjek.com

[B12] 跳出多层循环
来源：http://xph.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xcq.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://emj.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qtm.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://acj.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ksy.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ors.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tzq.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hel.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://rma.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://tds.dashuyun.cn

PHP:  is_numeric($x)
来源：http://pwm.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hne.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yye.hcnkem.com

Java: x instanceof Number
来源：http://wnh.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gbl.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://ocb.yuanzhike.top

C#:   x is int or double or decimal
来源：http://cpx.yj20258.top

[B14] 判断值是否在集合内
来源：http://obi.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hkf.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pdb.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://pvf.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://xxf.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://asy.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wzy.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://blb.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tdr.gzhubu.top

[B15] 布尔运算与取反
来源：http://isq.tanke756.top

Py:   a and b or not c
来源：http://unz.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://duw.cqqwz.cn

JS:   a && b || !c
来源：http://skm.pengpengdd.cyou

TS:   a && b || !c
来源：http://wxs.xuetiantiany.cn

Java: a && b || !c
来源：http://ati.hnqzz.top

Go:   a && b || !c
来源：http://dyn.vqdsnc.cn

Ruby: a && b || !c
来源：http://rwx.vehdjk.com

C#:   a && b || !c
来源：http://wks.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bed.chenzaomai.com

Py:   if not data: return
来源：http://vmv.yj20258.top

PHP:  if (!$data) { return; }
来源：http://uzy.gogol.net.cn

JS:   if (!data) return;
来源：http://xyv.havefunace.top

TS:   if (!data) return;
来源：http://anl.sxryk.cn

Java: if (data == null) return;
来源：http://xix.yj20258888.top

Go:   if data == nil { return }
来源：http://shj.shuidangran.top

Ruby: return if data.nil?
来源：http://pyf.daxiang520.top

C#:   if (data == null) return;
来源：http://ftu.snrcjt.cn

================================================================================
来源：http://lwv.jqgufenzy.top

C. 函数与作用域
来源：http://obi.ywan-chungtsiang.top

================================================================================
来源：http://yit.jqgfzy.top

[C01] 定义函数
来源：http://htu.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://nxf.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cgl.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://idm.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ceq.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eso.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gxd.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://llj.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://boq.jinghuilouyu.cn

[C02] 默认参数
来源：http://ewq.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://dyg.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://muf.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://hha.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gkv.yvedp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aly.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dxc.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://jqs.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://yyy.zhongyouzk.top

[C03] 可变参数
来源：http://qjf.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://bml.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hsc.xinyue.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptk.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wod.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lkg.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vaz.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://tfk.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mvj.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://chn.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://epj.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lrf.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://piy.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://efs.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://mxl.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://blf.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://spz.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://iuf.gotoacloud.top

[C05] 返回多个值
来源：http://jkz.nanxinkj.top

Py:   return a, b
来源：http://rfr.ydzc1.top

PHP:  return [$a, $b];
来源：http://dyy.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wnu.zycfv.cn

TS:   return { a, b };
来源：http://gtu.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zgz.zhoulong.xyz

Go:   return a, b
来源：http://bix.jinqigufen.top

Ruby: return a, b
来源：http://hav.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://ypo.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://dgg.daxiang520.top

Py:   square = lambda x: x * x
来源：http://zjx.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ebh.sxryk.cn

JS:   const square = x => x * x;
来源：http://api.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://now.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sxh.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://edm.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://hrc.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://bje.hnqzz.top

[C07] 把函数作为参数传入
来源：http://rvh.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tsp.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://gtx.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qfy.sufxvd.cn

TS:   arr.map(String)
来源：http://wiu.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mcq.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qpv.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://ycz.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bkv.hcnkem.com

[C08] 闭包
来源：http://ksa.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wcb.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aqe.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kjt.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cdh.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dbq.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sgv.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lyi.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hrj.fzhhl.top

[C09] 递归
来源：http://kcm.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vgz.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tym.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kjr.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hks.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zmu.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://awy.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qhp.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dqd.havefunace.top

[C10] 变量作用域
来源：http://pfr.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nkg.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xvx.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tnz.sweek.top

TS:   同 JS
来源：http://ssi.316326.xyz

Java: 方法内为块级作用域
来源：http://jhn.havefunace.top

Go:   花括号块级作用域
来源：http://qvp.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nei.ydjk.org.cn

C#:   块级作用域
来源：http://nlx.tanke756.top

[C11] 模块导入与导出
来源：http://bve.fanxiaobao.xyz

Py:   from module import func
来源：http://vzl.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mct.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://txa.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sfs.daxiang520.top

Java: import java.util.List;
来源：http://fuj.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wse.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://vsp.cucudq.cn

C#:   using System.Text;
来源：http://fng.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://cki.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://umk.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://ayy.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://dyk.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://qip.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hcf.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://kqc.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://yox.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lgm.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://pte.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xzz.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hqx.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fsa.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bte.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://xbc.yvedp.cn

Go:   func add(a, b int) int
来源：http://gjz.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yes.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dhq.hesvh.cn

[C14] 泛型函数
来源：http://kyx.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ify.0kj1m.cn

PHP:  // 无泛型
来源：http://kkv.jianghu66.top

JS:   // 无泛型
来源：http://aus.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pqq.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xzr.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jao.jlsjyb.cn

Ruby: # 无泛型
来源：http://rap.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fhd.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://jrk.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mkt.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://bke.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://trd.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://asl.hammf.cn

Java: // 无解构
来源：http://nqe.ppjwa.cn

Go:   // 无解构
来源：http://xst.fengsongda.top

Ruby: a, b = pair
来源：http://ief.yuxming.cn

C#:   var (a, b) = pair;
来源：http://oim.daria6918.cn

[C16] 函数 / 方法重载
来源：http://wzp.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oxq.zhoulong.xyz

PHP:  // 无重载
来源：http://bca.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yys.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://yij.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://wyf.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://boi.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://xep.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qhj.yangfankeji.com

================================================================================
来源：http://duo.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://zmd.gaohongyu789.top

================================================================================
来源：http://ayz.meibo888.top

[D01] 创建数组 / 列表
来源：http://oef.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mar.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lnv.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nfd.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mdb.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nwx.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://lqs.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://fqm.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vph.tianlin.xyz

[D02] 追加元素到末尾
来源：http://jln.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uib.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zfm.zhengqikj.top

JS:   arr.push(4);
来源：http://fmh.wangshuangyany.cn

TS:   arr.push(4);
来源：http://xny.chenlongwang.top

Java: list.add(4);
来源：http://wlk.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://cpj.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://bew.vehdjk.com

C#:   list.Add(4);
来源：http://rwu.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://hed.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://fnj.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ioc.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lgy.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://oij.shuidangran.top

Java: list.add(0, 0);
来源：http://zls.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ztb.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xmr.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://kda.guannengcc.top

[D04] 删除元素
来源：http://ofz.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nrs.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sux.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hlr.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://grv.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wvc.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://afx.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wfe.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://utv.gzhubu.top

[D05] 访问与修改元素
来源：http://qyo.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://upl.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ryj.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ouz.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://osd.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://nvx.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://hpc.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://deh.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kuh.zhijiandao.cn

[D06] 数组长度
来源：http://kcv.zhongyouzk.top

Py:   len(arr)
来源：http://lpf.jqgufenzy.top

PHP:  count($arr);
来源：http://pxt.shanyushiyangkeji.top

JS:   arr.length
来源：http://qaa.jlsjyb.cn

TS:   arr.length
来源：http://gkf.aizwys.cn

Java: list.size();
来源：http://ebj.shzxlz.cn

Go:   len(arr)
来源：http://yfv.yonumen.top

Ruby: arr.length; arr.size
来源：http://bgt.xuanzx.com

C#:   list.Count;
来源：http://rem.fengsongda.top

[D07] 切片 / 取子数组
来源：http://bdd.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tbb.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://agr.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://aoo.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://nny.hysaishi.cn

Java: list.subList(1, 4);
来源：http://xzm.quarkkingdee.top

Go:   arr[1:4]
来源：http://pyk.sxryk.cn

Ruby: arr[1, 3]
来源：http://edf.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://dft.cheryme.top

[D08] 合并两个数组
来源：http://lgc.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://ihr.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://igf.aizwys.cn


<!-- 参考信息 -->