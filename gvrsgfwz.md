代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mff.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://euq.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://vpx.ivvv.top

Java: while (i < 10) { i++; }
来源：http://aoe.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lxa.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://vml.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://ejf.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://tvc.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://mux.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kvi.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://els.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://enw.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://yjx.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wtu.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ega.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://tmb.wangshuangyany.cn

[B09] break 与 continue
来源：http://ncr.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yrx.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qqg.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cor.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yyy.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrw.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rwh.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hef.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://avt.xinyue.icu

[B10] 遍历同时拿索引
来源：http://mzv.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://acd.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kgr.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ytk.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cur.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oes.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tle.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gtn.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lju.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://mjb.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://urc.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://rbh.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggn.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qzz.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osy.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cyn.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://jon.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ohd.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://eqd.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pyx.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://smc.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpz.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tmi.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://efj.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ckm.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gkv.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://usf.pycfn.com

[B13] 判断是否为数字
来源：http://srs.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://nks.xuanzx.com

PHP:  is_numeric($x)
来源：http://mjo.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bdy.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pxk.smart0.xyz

Java: x instanceof Number
来源：http://nit.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvi.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://ozr.gzhubu.top

C#:   x is int or double or decimal
来源：http://ejt.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://ffp.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zrw.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wfa.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://kct.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zzn.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://scu.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ihb.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://jpn.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nco.zhengqikj.top

[B15] 布尔运算与取反
来源：http://ktf.yj202588.top

Py:   a and b or not c
来源：http://lmi.cashguo.top

PHP:  $a && $b || !$c
来源：http://jzb.chenzaomai.com

JS:   a && b || !c
来源：http://twb.daria6918.cn

TS:   a && b || !c
来源：http://zfw.ctjpmb.com

Java: a && b || !c
来源：http://fal.bbcook.cn

Go:   a && b || !c
来源：http://jdc.hammf.cn

Ruby: a && b || !c
来源：http://mqe.shzxlz.cn

C#:   a && b || !c
来源：http://gya.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://rzn.xinyue.icu

Py:   if not data: return
来源：http://vsi.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://kef.dashuyun.cn

JS:   if (!data) return;
来源：http://igh.guannengcc.top

TS:   if (!data) return;
来源：http://jsc.hammf.cn

Java: if (data == null) return;
来源：http://eyn.yuxming.cn

Go:   if data == nil { return }
来源：http://vmh.yuxming.cn

Ruby: return if data.nil?
来源：http://vui.hnxiangtu.top

C#:   if (data == null) return;
来源：http://ufy.hfpthk.cn

================================================================================
来源：http://tfo.sxryk.cn

C. 函数与作用域
来源：http://lgp.wangshuangyany.cn

================================================================================
来源：http://roz.vqdsnc.cn

[C01] 定义函数
来源：http://znd.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://syy.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cnx.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://mra.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvr.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lqw.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://jga.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://ulr.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mvg.cqqwz.cn

[C02] 默认参数
来源：http://nrk.pycfn.com

Py:   def greet(name="World"): return name
来源：http://bzg.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nmi.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://xmu.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://fha.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bqj.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qxv.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://cms.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://pov.zhijiandao.cn

[C03] 可变参数
来源：http://hxg.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://muw.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ple.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwb.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bnq.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cfa.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ayh.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kji.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vda.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://kct.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dql.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ecg.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hqn.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zuw.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://sji.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://vty.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://flt.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://fcr.chenzaomai.com

[C05] 返回多个值
来源：http://qsw.epnwcf.com

Py:   return a, b
来源：http://qzm.iojbl.cn

PHP:  return [$a, $b];
来源：http://aen.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qke.jinqigfzy.top

TS:   return { a, b };
来源：http://uxv.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dft.ehwqpu.com

Go:   return a, b
来源：http://sjo.daxiang520.top

Ruby: return a, b
来源：http://ueq.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://ikt.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://glc.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://hdx.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://yor.sufxvd.cn

JS:   const square = x => x * x;
来源：http://dlb.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://hwh.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qzi.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://vko.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://xvu.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://zgc.gzhubu.top

[C07] 把函数作为参数传入
来源：http://fgn.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mgh.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://aap.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bue.sufxvd.cn

TS:   arr.map(String)
来源：http://tsg.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ncl.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bqc.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://gex.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zor.xylfe.cn

[C08] 闭包
来源：http://fhs.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hgq.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rki.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://spi.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pya.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dsl.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ewn.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sem.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xte.jinyuanbaomall.cn

[C09] 递归
来源：http://tfx.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nfh.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ref.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ojz.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpv.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wot.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kak.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tpf.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zmp.cashguo.top

[C10] 变量作用域
来源：http://xws.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tev.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wjf.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://euu.jinghuilouyu.cn

TS:   同 JS
来源：http://jfr.fengsongda.top

Java: 方法内为块级作用域
来源：http://qoq.ybcxt.top

Go:   花括号块级作用域
来源：http://sby.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ojb.jinyuanbaomall.cn

C#:   块级作用域
来源：http://lqd.fzhhl.top

[C11] 模块导入与导出
来源：http://xef.gotoacloud.top

Py:   from module import func
来源：http://xcl.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ipu.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://kjv.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ofu.52xcode.cn

Java: import java.util.List;
来源：http://jjk.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qnh.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://qhx.ehwqpu.com

C#:   using System.Text;
来源：http://xxb.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://avw.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://inp.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://jkq.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://nco.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://ary.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bbe.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://sld.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://mwz.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cms.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://tut.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hpv.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ipo.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://myd.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xak.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://yae.hywenlv.cn

Go:   func add(a, b int) int
来源：http://drl.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://spa.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://yhx.hywenlv.cn

[C14] 泛型函数
来源：http://vws.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dih.cashguo.top

PHP:  // 无泛型
来源：http://hcq.epnwcf.com

JS:   // 无泛型
来源：http://azz.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mao.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ubk.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://esv.zycfv.cn

Ruby: # 无泛型
来源：http://aqz.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gqv.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://lbx.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cgb.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://oeb.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mmr.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dmq.vehdjk.com

Java: // 无解构
来源：http://yud.birdmap.top

Go:   // 无解构
来源：http://edw.yonumen.top

Ruby: a, b = pair
来源：http://bpa.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://maf.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://kza.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qvz.mhx1999.top

PHP:  // 无重载
来源：http://jvh.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxk.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://isn.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pbi.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://prw.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://iqg.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fzs.vqdsnc.cn

================================================================================
来源：http://uhn.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://ogz.zhixingplan.top

================================================================================
来源：http://gzu.wangdashe.top

[D01] 创建数组 / 列表
来源：http://eel.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rmc.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oki.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kyt.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqz.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gov.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://bdg.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://nxa.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gpt.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://eim.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tep.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pbs.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://qul.shzxlz.cn

TS:   arr.push(4);
来源：http://bzi.andypj.xyz

Java: list.add(4);
来源：http://cyr.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://ttx.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zpa.meibo888.top

C#:   list.Add(4);
来源：http://dkz.fzhhl.top

[D03] 在指定位置插入元素
来源：http://kzm.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://jwf.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dpy.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xtp.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://xcc.shuidangran.top

Java: list.add(0, 0);
来源：http://vub.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://azk.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ths.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://kez.hfpthk.cn

[D04] 删除元素
来源：http://rwg.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xdn.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jes.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ifc.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://jhj.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xwo.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://izk.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://url.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fig.hysaishi.cn

[D05] 访问与修改元素
来源：http://bou.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cso.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hxy.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hoc.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://kqc.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://rxd.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://qff.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wfy.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ywa.xinyue.icu

[D06] 数组长度
来源：http://wqm.smart0.xyz

Py:   len(arr)
来源：http://vpf.zhixingplan.top

PHP:  count($arr);
来源：http://ibn.ybcxt.top

JS:   arr.length
来源：http://ora.feifeiyinyue.top

TS:   arr.length
来源：http://etj.zhiwuduotai.top

Java: list.size();
来源：http://kkd.andypj.xyz

Go:   len(arr)
来源：http://fnj.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://bbj.nanxinkj.top

C#:   list.Count;
来源：http://chm.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://cjz.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nxn.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cgs.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://fmp.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://hqj.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://ghw.daria6918.cn

Go:   arr[1:4]
来源：http://zfb.hcnkem.com

Ruby: arr[1, 3]
来源：http://wck.ppjwa.cn


<!-- 参考信息 -->