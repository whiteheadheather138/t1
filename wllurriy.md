代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wdi.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://gmi.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://xif.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://ylk.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://dtz.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://uld.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://caj.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://ikb.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://wuo.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://rwv.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jec.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://zhv.xylfe.cn

[B09] break 与 continue
来源：http://ldm.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://azl.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wqb.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kiv.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xua.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arg.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://stt.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ujw.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufv.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://xpc.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://elc.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dnf.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jdo.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yfh.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aqk.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ger.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://you.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qap.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://znm.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://zti.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://ooz.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yjo.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eco.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iiw.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wbr.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://hmc.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://msm.sjlbkw.cn

[B12] 跳出多层循环
来源：http://znh.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ucs.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ypi.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qme.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xmf.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ytu.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jqx.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lvt.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://naa.ehwqpu.com

[B13] 判断是否为数字
来源：http://tdu.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://hit.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://oyt.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nqk.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qrw.sufxvd.cn

Java: x instanceof Number
来源：http://zod.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lbb.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://jfs.iojbl.cn

C#:   x is int or double or decimal
来源：http://pvw.ydzc1.top

[B14] 判断值是否在集合内
来源：http://kkj.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jgm.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zka.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://fnh.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://oot.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://vbu.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gig.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://yap.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fda.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://kcl.tian-w.cn

Py:   a and b or not c
来源：http://hro.aizwys.cn

PHP:  $a && $b || !$c
来源：http://msj.vehdjk.com

JS:   a && b || !c
来源：http://klt.52xcode.cn

TS:   a && b || !c
来源：http://ylr.zhijiandao.cn

Java: a && b || !c
来源：http://tjv.zdbjq.cn

Go:   a && b || !c
来源：http://jhj.kuanghao11.cn

Ruby: a && b || !c
来源：http://pqg.dashuyun.cn

C#:   a && b || !c
来源：http://ekb.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://cee.svipenyu.cn

Py:   if not data: return
来源：http://lik.meibo888.top

PHP:  if (!$data) { return; }
来源：http://kmj.quarkkingdee.top

JS:   if (!data) return;
来源：http://gvz.xziqi.cn

TS:   if (!data) return;
来源：http://lhi.zhengqikj.top

Java: if (data == null) return;
来源：http://xgy.chenlongwang.top

Go:   if data == nil { return }
来源：http://bbr.yangfankeji.com

Ruby: return if data.nil?
来源：http://rse.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://ptu.yj20258.top

================================================================================
来源：http://uaq.zdqjudy.top

C. 函数与作用域
来源：http://osz.ctjpmb.com

================================================================================
来源：http://sxv.xylfe.cn

[C01] 定义函数
来源：http://alw.andypj.xyz

Py:   def add(a, b): return a + b
来源：http://gyn.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nsj.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://cws.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hll.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://hbu.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qmd.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://nes.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ihg.ctjpmb.com

[C02] 默认参数
来源：http://pgp.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://lvh.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dzm.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://fum.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://qum.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wjl.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vld.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://iaj.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://bcs.cheryme.top

[C03] 可变参数
来源：http://icu.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://wxw.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yly.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oyb.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ksj.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azy.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xip.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://rld.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kik.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://vov.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nrk.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nad.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jho.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://opg.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://vvs.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://phw.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://xvw.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://uek.xylfe.cn

[C05] 返回多个值
来源：http://naf.ywan-chungtsiang.top

Py:   return a, b
来源：http://ykc.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://rpy.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fds.iojbl.cn

TS:   return { a, b };
来源：http://pdy.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zjm.yangfankeji.com

Go:   return a, b
来源：http://fha.redwolf501.top

Ruby: return a, b
来源：http://iar.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://bnv.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://avl.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://cxp.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wcf.zycfv.cn

JS:   const square = x => x * x;
来源：http://swg.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://wca.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uah.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qdc.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://kth.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://bbo.birdmap.top

[C07] 把函数作为参数传入
来源：http://qtd.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cjr.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://drx.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://thl.sjlbkw.cn

TS:   arr.map(String)
来源：http://cah.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bvb.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hye.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://stg.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cpx.birdmap.top

[C08] 闭包
来源：http://lnq.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tna.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gwc.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://llq.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sbg.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hrv.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mew.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dmh.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fhw.iojbl.cn

[C09] 递归
来源：http://gut.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rgg.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cko.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aac.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lhm.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://msc.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mwn.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dqn.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://agl.fanxiaobao.xyz

[C10] 变量作用域
来源：http://xdi.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gwc.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ncw.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yeg.sxryk.cn

TS:   同 JS
来源：http://duh.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://aaw.zdqjudy.top

Go:   花括号块级作用域
来源：http://tcf.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://utj.sysykeji.top

C#:   块级作用域
来源：http://scq.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://lbe.jinghuilouyu.cn

Py:   from module import func
来源：http://col.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mzg.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xfc.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pcm.sxryk.cn

Java: import java.util.List;
来源：http://xwr.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://odt.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://upp.ppjwa.cn

C#:   using System.Text;
来源：http://vfr.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://kla.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://rid.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://trk.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://sld.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://udk.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gzk.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://xov.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://mfy.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xmb.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://erd.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://shp.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qso.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cyp.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fqf.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qnw.bbcook.cn

Go:   func add(a, b int) int
来源：http://hjy.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bae.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kzu.dashuyun.cn

[C14] 泛型函数
来源：http://sma.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ysl.ctjpmb.com

PHP:  // 无泛型
来源：http://dqz.52xcode.cn

JS:   // 无泛型
来源：http://cme.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vqn.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ccr.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yqd.bbcook.cn

Ruby: # 无泛型
来源：http://mxn.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fph.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://rlp.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wbj.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://ayh.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nah.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://riw.zhoulong.xyz

Java: // 无解构
来源：http://vxi.xylfe.cn

Go:   // 无解构
来源：http://uci.zhixingplan.top

Ruby: a, b = pair
来源：http://joc.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://ozn.iojbl.cn

[C16] 函数 / 方法重载
来源：http://bop.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bhz.shangyingyoupin.top

PHP:  // 无重载
来源：http://blc.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zns.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://kfv.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://agh.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://rbw.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://tyu.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sgw.bbcook.cn

================================================================================
来源：http://wka.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://lbe.sjlbkw.cn

================================================================================
来源：http://qnc.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://ktd.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ivu.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ado.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://efa.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ijv.svipenyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fyb.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://ouq.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://lvb.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yus.ctjpmb.com

[D02] 追加元素到末尾
来源：http://qre.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ivt.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nln.yvedp.cn

JS:   arr.push(4);
来源：http://zim.snrcjt.cn

TS:   arr.push(4);
来源：http://vsp.gotoacloud.top

Java: list.add(4);
来源：http://fhe.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://fga.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://acl.yj20258.top

C#:   list.Add(4);
来源：http://maf.xziqi.cn

[D03] 在指定位置插入元素
来源：http://jkr.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://hac.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oio.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://izr.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://vlf.jiagoushi.top

Java: list.add(0, 0);
来源：http://bxg.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://hya.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cse.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://kcu.ydzc1.top

[D04] 删除元素
来源：http://mkz.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mfa.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dbh.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lpy.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://xmq.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://orq.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kfa.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aye.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whz.xziqi.cn

[D05] 访问与修改元素
来源：http://hjs.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vxl.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kxf.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://elu.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://fai.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://kjq.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://hoa.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://beo.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dsq.yuxming.cn

[D06] 数组长度
来源：http://aia.jqgfzy.top

Py:   len(arr)
来源：http://bvr.sweek.top

PHP:  count($arr);
来源：http://fxb.tian-w.cn

JS:   arr.length
来源：http://pqh.zhoulong.xyz

TS:   arr.length
来源：http://zzd.jqgufenzy.top

Java: list.size();
来源：http://ybt.jyoumei.cn

Go:   len(arr)
来源：http://iwx.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://use.yj20258888.top

C#:   list.Count;
来源：http://knw.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://tks.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oga.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hga.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://kdp.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://htu.xuanzx.com

Java: list.subList(1, 4);
来源：http://ugt.hysaishi.cn

Go:   arr[1:4]
来源：http://zph.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://yjp.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://nhn.aibaodan.cn

[D08] 合并两个数组
来源：http://zbp.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://opk.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://jxg.zhijiandao.cn


<!-- 参考信息 -->