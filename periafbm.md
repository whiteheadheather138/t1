代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rqr.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://rwv.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dmk.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yhg.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qet.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jqb.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://slw.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oym.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uwb.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ziv.hammf.cn

[B07] while 循环
来源：http://ddi.andypj.xyz

Py:   while i < 10: i += 1
来源：http://obc.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://hec.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://ulr.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://jbu.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://kxu.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vak.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://myn.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://ixj.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://gmh.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://jmi.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gxd.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://rlf.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://cdr.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://yvv.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ocy.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://did.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://mnp.jqgufenzy.top

[B09] break 与 continue
来源：http://cex.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ykk.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pzp.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldd.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahx.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlp.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rpo.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qkg.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obv.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://yoz.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vak.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lbp.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ciw.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://psa.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://but.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sff.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://onh.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iyl.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://dvc.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://bhn.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://umh.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://opt.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rny.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ksc.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ftc.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://okh.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sfb.fehbvm.com

[B12] 跳出多层循环
来源：http://znh.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vsr.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vzh.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://auz.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpt.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oci.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hqi.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gvj.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bmf.jlsjyb.cn

[B13] 判断是否为数字
来源：http://xqb.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://frv.shzxlz.cn

PHP:  is_numeric($x)
来源：http://pqz.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lkd.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mtt.aibaodan.cn

Java: x instanceof Number
来源：http://lgk.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yyh.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://shn.yuanzhike.top

C#:   x is int or double or decimal
来源：http://gbw.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://wku.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pbb.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://myv.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://acv.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://uks.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vuz.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zha.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://slx.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fhp.ybcxt.top

[B15] 布尔运算与取反
来源：http://zsg.svipenyu.cn

Py:   a and b or not c
来源：http://fch.smart0.xyz

PHP:  $a && $b || !$c
来源：http://nps.gaohongyu789.top

JS:   a && b || !c
来源：http://jlk.jyoumei.cn

TS:   a && b || !c
来源：http://hby.dianchejie.cn

Java: a && b || !c
来源：http://eyo.chenlongwang.top

Go:   a && b || !c
来源：http://rnh.daria6918.cn

Ruby: a && b || !c
来源：http://whq.nanxuanxn.top

C#:   a && b || !c
来源：http://mqe.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cxl.kuanghao11.cn

Py:   if not data: return
来源：http://jne.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://wpj.xinyue.icu

JS:   if (!data) return;
来源：http://uqx.zdqjudy.top

TS:   if (!data) return;
来源：http://qsg.yangfankeji.com

Java: if (data == null) return;
来源：http://vwh.jianghu66.top

Go:   if data == nil { return }
来源：http://dfy.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://jie.zhoulong.xyz

C#:   if (data == null) return;
来源：http://wwn.epnwcf.com

================================================================================
来源：http://lrg.jyoumei.cn

C. 函数与作用域
来源：http://dey.cdnleiting.top

================================================================================
来源：http://qrk.svipenyu.cn

[C01] 定义函数
来源：http://uqe.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://ptv.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uvy.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://yrp.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqu.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vgm.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ilb.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://gvy.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://htr.nanxuanxn.top

[C02] 默认参数
来源：http://cfw.meibo888.top

Py:   def greet(name="World"): return name
来源：http://jru.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jqu.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://iso.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lyw.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kgr.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bmj.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://iic.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://ykz.316326.xyz

[C03] 可变参数
来源：http://xmz.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://ufy.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mdc.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nke.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bvd.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://thl.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cqc.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://xki.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xzb.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://jwz.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jnr.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bxl.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mqw.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pds.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://ckd.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://eql.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://vku.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://bil.tian-w.cn

[C05] 返回多个值
来源：http://yef.tarul.cn

Py:   return a, b
来源：http://lej.uphjek.com

PHP:  return [$a, $b];
来源：http://qav.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rzg.nanxuanxn.top

TS:   return { a, b };
来源：http://nqv.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ohh.shanyushiyangkeji.top

Go:   return a, b
来源：http://axc.ctjpmb.com

Ruby: return a, b
来源：http://jng.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://dkz.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://qhm.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://ers.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://lgv.birdmap.top

JS:   const square = x => x * x;
来源：http://bnf.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://hdi.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://luc.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tza.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://ygg.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://zjp.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://gyn.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jqq.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://lre.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qlf.tianlin.xyz

TS:   arr.map(String)
来源：http://vol.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dwr.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fwc.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://piv.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xab.andypj.xyz

[C08] 闭包
来源：http://jhq.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cxn.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xgr.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://clc.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uth.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hvl.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fcd.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qkb.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zal.birdmap.top

[C09] 递归
来源：http://gtd.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ouk.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wga.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zmm.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cko.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gqo.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lzg.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nyt.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://src.gzhubu.top

[C10] 变量作用域
来源：http://pft.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wva.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jjk.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://elu.jyoumei.cn

TS:   同 JS
来源：http://kgv.zycfv.cn

Java: 方法内为块级作用域
来源：http://auw.cqqwz.cn

Go:   花括号块级作用域
来源：http://qsp.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ntx.52xcode.cn

C#:   块级作用域
来源：http://dyz.xziqi.cn

[C11] 模块导入与导出
来源：http://ssp.zdbjq.cn

Py:   from module import func
来源：http://nbj.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wgb.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zub.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfo.havefunace.top

Java: import java.util.List;
来源：http://fkf.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmo.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://fvn.nwbrower.top

C#:   using System.Text;
来源：http://yin.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://lia.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://anl.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://ppx.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://yod.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://dcu.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cor.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://aaw.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://vfk.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bka.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://nzh.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rse.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aju.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://brq.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jja.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://msm.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://luq.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rwm.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cnc.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://mqu.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lap.xylfe.cn

PHP:  // 无泛型
来源：http://snq.pycfn.com

JS:   // 无泛型
来源：http://gsc.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://umb.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fcx.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xcm.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://myw.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://isr.wangdashe.top

[C15] 解构 / 展开参数
来源：http://gsi.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ipv.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://ygf.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://udj.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zlw.nanxinkj.top

Java: // 无解构
来源：http://owt.yj20258.top

Go:   // 无解构
来源：http://uya.jiagoushi.top

Ruby: a, b = pair
来源：http://aky.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://ajb.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://xbg.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://auc.bjfxy.top

PHP:  // 无重载
来源：http://lls.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://pxo.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://cjb.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://koo.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://rup.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://izg.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fmq.bjfxy.top

================================================================================
来源：http://xsf.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://pba.hcnkem.com

================================================================================
来源：http://ede.shuidangran.top

[D01] 创建数组 / 列表
来源：http://hze.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yli.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yye.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rji.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://abd.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pez.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://ynj.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://iym.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aol.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://zht.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kqz.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jtb.zycfv.cn

JS:   arr.push(4);
来源：http://ivy.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://efw.tarul.cn

Java: list.add(4);
来源：http://lgs.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://hft.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://rsd.zhiwuduotai.top

C#:   list.Add(4);
来源：http://wgs.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://hlh.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://vdl.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jgs.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cjx.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://xcu.yanxiufei.cn

Java: list.add(0, 0);
来源：http://zcz.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://zhw.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://snn.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://ylt.wangdashe.top

[D04] 删除元素
来源：http://ome.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tgq.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://thq.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ujm.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://hft.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://osp.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qii.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ixx.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iao.dianchejie.cn

[D05] 访问与修改元素
来源：http://amr.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tit.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kwu.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jzp.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://tqd.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://son.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://mqg.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bov.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://krw.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://baa.hfpthk.cn

Py:   len(arr)
来源：http://ydv.yonumen.top

PHP:  count($arr);
来源：http://fez.fzhhl.top

JS:   arr.length
来源：http://vsx.shuidangran.top

TS:   arr.length
来源：http://owf.shangyingyoupin.top


<!-- 参考信息 -->