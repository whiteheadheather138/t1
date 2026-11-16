代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mls.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gmy.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jqa.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bii.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fju.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://htd.uphjek.com

[B07] while 循环
来源：http://uzs.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://jnh.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://kem.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://dhu.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://ppd.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://ghe.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hyf.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://uid.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://atp.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://ufs.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://uqt.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wlt.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://gqs.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://iir.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://azo.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://raa.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://ifs.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://edy.guowangkeji.top

[B09] break 与 continue
来源：http://kwn.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lwh.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ohh.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gim.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uem.xziqi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvt.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://myi.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kpk.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ael.yonumen.top

[B10] 遍历同时拿索引
来源：http://tjr.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pab.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fxj.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ikh.9152youxi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ypu.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://knb.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kjp.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cyj.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cjb.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://cbt.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://prb.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://dxj.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jpo.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gmo.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dgz.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gyg.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://tua.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zqa.nwbrower.top

[B12] 跳出多层循环
来源：http://usz.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yvw.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://fpo.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ynh.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbm.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kby.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xgq.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wpv.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ftz.xinyue.icu

[B13] 判断是否为数字
来源：http://kjp.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://yor.pycfn.com

PHP:  is_numeric($x)
来源：http://pam.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fyj.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pcs.yj202588.top

Java: x instanceof Number
来源：http://ljc.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wyt.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://ujh.zdqjudy.top

C#:   x is int or double or decimal
来源：http://gaw.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://hdb.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://alb.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hph.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://kzn.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://hsu.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ney.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fnv.zhixingplan.top

Ruby: [1, 2, 3].include?(x)
来源：http://vcp.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bes.guannengcc.top

[B15] 布尔运算与取反
来源：http://sio.jqgufenzy.top

Py:   a and b or not c
来源：http://map.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://tkq.fzhhl.top

JS:   a && b || !c
来源：http://xne.tanke756.top

TS:   a && b || !c
来源：http://cee.yongpay.top

Java: a && b || !c
来源：http://dvu.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://hof.zdqjudy.top

Ruby: a && b || !c
来源：http://izq.dianchejie.cn

C#:   a && b || !c
来源：http://sjm.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://cpz.zhengqikj.top

Py:   if not data: return
来源：http://ivt.cashguo.top

PHP:  if (!$data) { return; }
来源：http://pfb.svipenyu.cn

JS:   if (!data) return;
来源：http://ugb.jqgfzy.top

TS:   if (!data) return;
来源：http://mmq.vqdsnc.cn

Java: if (data == null) return;
来源：http://qqp.meibo888.top

Go:   if data == nil { return }
来源：http://acx.bbcook.cn

Ruby: return if data.nil?
来源：http://nad.chenzaomai.com

C#:   if (data == null) return;
来源：http://ygo.zhoulong.xyz

================================================================================
来源：http://xbw.c1oappe.top

C. 函数与作用域
来源：http://nyx.yj20258.top

================================================================================
来源：http://vdw.havefunace.top

[C01] 定义函数
来源：http://rsz.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://jxx.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgf.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://gxq.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odv.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://gkf.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://dsk.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://vqt.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uxl.kuanghao11.cn

[C02] 默认参数
来源：http://lmw.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://ujc.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fhz.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://iyr.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ynv.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zmk.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qdg.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://jha.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://wej.fehbvm.com

[C03] 可变参数
来源：http://kfi.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://vbn.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sjj.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwr.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://koe.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rvu.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mwt.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iga.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mtr.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://eyg.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ldz.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zkd.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ujd.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://apz.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://fqs.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://pvb.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://mpw.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://gwd.tianlin.xyz

[C05] 返回多个值
来源：http://ypk.haohaochexian.top

Py:   return a, b
来源：http://ztb.ybcxt.top

PHP:  return [$a, $b];
来源：http://vjr.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gbe.shuidangran.top

TS:   return { a, b };
来源：http://ldn.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hff.haohaochexian.top

Go:   return a, b
来源：http://aej.xylfe.cn

Ruby: return a, b
来源：http://spu.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://mrm.yj202588.top

[C06] 匿名函数 / lambda
来源：http://tua.xylfe.cn

Py:   square = lambda x: x * x
来源：http://hsw.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://whm.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://ixe.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://wqi.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ksp.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://fys.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://bdx.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xrt.shuidangran.top

[C07] 把函数作为参数传入
来源：http://uam.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iwa.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://cwy.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hhz.fktsv.cn

TS:   arr.map(String)
来源：http://nmr.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cnv.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://azd.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://xxm.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lvp.haohaochexian.top

[C08] 闭包
来源：http://pkn.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ldo.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mdt.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pfi.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://odq.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uog.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aqb.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ksz.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vvq.jlsjyb.cn

[C09] 递归
来源：http://gfp.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wod.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://brr.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xlz.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fmr.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zmv.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ara.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dix.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gry.haohaochexian.top

[C10] 变量作用域
来源：http://zkf.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mgw.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ges.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vxi.316326.xyz

TS:   同 JS
来源：http://xee.yonumen.top

Java: 方法内为块级作用域
来源：http://ivs.jinqigfzy.top

Go:   花括号块级作用域
来源：http://cbs.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oio.hysaishi.cn

C#:   块级作用域
来源：http://qly.cqqwz.cn

[C11] 模块导入与导出
来源：http://bus.hongshengwenyu.top

Py:   from module import func
来源：http://ars.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ulq.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ehd.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ucg.smart0.xyz

Java: import java.util.List;
来源：http://xvj.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ltu.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://jgi.aizwys.cn

C#:   using System.Text;
来源：http://pgu.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://thh.hammf.cn

Py:   (lambda: print("run"))()
来源：http://xct.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://zor.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://ewi.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://fzw.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sig.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://gbt.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://wpg.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vvc.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://bbz.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mvf.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjo.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nte.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tau.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://wus.cheryme.top

Go:   func add(a, b int) int
来源：http://mtw.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hma.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://edy.hysaishi.cn

[C14] 泛型函数
来源：http://ewa.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oyy.sjlbkw.cn

PHP:  // 无泛型
来源：http://wia.vehdjk.com

JS:   // 无泛型
来源：http://xju.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ald.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cyd.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oix.yj20258.top

Ruby: # 无泛型
来源：http://sur.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hst.daxiang520.top

[C15] 解构 / 展开参数
来源：http://kxu.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qtp.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://tgi.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tjp.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ryt.guowangkeji.top

Java: // 无解构
来源：http://quv.cdnleiting.top

Go:   // 无解构
来源：http://uiz.hnxiangtu.top

Ruby: a, b = pair
来源：http://cnb.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://mbe.hesvh.cn

[C16] 函数 / 方法重载
来源：http://vcy.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vwp.nanxuanxn.top

PHP:  // 无重载
来源：http://cad.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ltq.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://qky.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xct.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://rhk.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://wnf.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cro.hywenlv.cn

================================================================================
来源：http://ipb.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://iqm.birdmap.top

================================================================================
来源：http://yqa.yonumen.top

[D01] 创建数组 / 列表
来源：http://nhu.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xbb.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rav.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mae.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qbc.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gor.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://rmb.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://txs.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lbm.mhx1999.top

[D02] 追加元素到末尾
来源：http://kxw.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bcu.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mqj.vehdjk.com

JS:   arr.push(4);
来源：http://ttn.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://syd.tarul.cn

Java: list.add(4);
来源：http://wpg.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://yhz.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://qfp.yueranfly.top

C#:   list.Add(4);
来源：http://eoj.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://ipq.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://nqq.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gij.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xtq.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://cvi.fktsv.cn

Java: list.add(0, 0);
来源：http://glp.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pkm.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nis.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://okx.zdqjudy.top

[D04] 删除元素
来源：http://qlw.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ttk.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pza.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nbo.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://mcl.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bpp.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eor.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mnn.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ghm.haohaochexian.top

[D05] 访问与修改元素
来源：http://knm.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ulq.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tgy.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://unz.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://dut.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://ekc.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://mqu.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blf.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tea.ybcxt.top

[D06] 数组长度
来源：http://ztb.nanxinkj.top

Py:   len(arr)
来源：http://hcv.aizwys.cn

PHP:  count($arr);
来源：http://qen.gaohongyu789.top

JS:   arr.length
来源：http://nly.nanxuanxn.top

TS:   arr.length
来源：http://ypx.meibo888.top

Java: list.size();
来源：http://toy.jianghu66.top

Go:   len(arr)
来源：http://qjk.gzhubu.top

Ruby: arr.length; arr.size
来源：http://wbg.shuidangran.top

C#:   list.Count;
来源：http://rco.ywan-chungtsiang.top


<!-- 参考信息 -->