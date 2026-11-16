代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hsp.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jsz.vqdsnc.cn

[B07] while 循环
来源：http://vxu.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://tbc.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://zkv.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://ozc.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://gqs.ivvv.top

Java: while (i < 10) { i++; }
来源：http://vbd.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ymp.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://emq.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://xae.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://pmv.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://pxm.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rdz.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://gwj.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://ehk.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://pgw.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aru.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://hec.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://guw.mhx1999.top

[B09] break 与 continue
来源：http://veb.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qcb.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zha.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymi.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnb.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndo.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://krk.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ohq.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://soj.meibo888.top

[B10] 遍历同时拿索引
来源：http://mww.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://caq.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wcq.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jdg.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://obc.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cbx.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fim.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cxr.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gzg.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://msf.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://wbd.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://qkm.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rwq.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rqn.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hrk.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cgf.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://mow.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://agy.gzhubu.top

[B12] 跳出多层循环
来源：http://aiy.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://opi.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uhe.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kjm.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytx.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ifc.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixe.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jct.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jbf.kuanghao11.cn

[B13] 判断是否为数字
来源：http://qur.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://zrv.yj20258888.top

PHP:  is_numeric($x)
来源：http://hsh.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcy.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ite.ydzc1.top

Java: x instanceof Number
来源：http://azm.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://heb.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://jvp.meibo888.top

C#:   x is int or double or decimal
来源：http://sdg.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://loc.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gwu.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vid.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://uqw.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://yoq.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rhu.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ceh.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://rqd.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uqr.guowangkeji.top

[B15] 布尔运算与取反
来源：http://lls.9152youxi.cn

Py:   a and b or not c
来源：http://hov.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://fzz.shzxlz.cn

JS:   a && b || !c
来源：http://rnh.zhijiandao.cn

TS:   a && b || !c
来源：http://xlc.daria6918.cn

Java: a && b || !c
来源：http://kpj.fengsongda.top

Go:   a && b || !c
来源：http://fir.guowangkeji.top

Ruby: a && b || !c
来源：http://gwt.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://zmt.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://vfg.9152youxi.cn

Py:   if not data: return
来源：http://qbj.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://hzq.hongshengwenyu.top

JS:   if (!data) return;
来源：http://hhl.wangshuangyany.cn

TS:   if (!data) return;
来源：http://wsy.uphjek.com

Java: if (data == null) return;
来源：http://zyg.kuanghao11.cn

Go:   if data == nil { return }
来源：http://jtf.yj202588.top

Ruby: return if data.nil?
来源：http://jbg.fengsongda.top

C#:   if (data == null) return;
来源：http://lvo.tianlin.xyz

================================================================================
来源：http://jpg.wangdashe.top

C. 函数与作用域
来源：http://fuh.feifeiyinyue.top

================================================================================
来源：http://xwo.gaohongyu789.top

[C01] 定义函数
来源：http://wpb.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://dmu.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yft.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://asy.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://drm.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nne.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://fbw.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://ggw.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iqc.yongpay.top

[C02] 默认参数
来源：http://qoh.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://ynp.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fkn.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://yds.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://suf.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://uts.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fuf.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://xpa.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://ica.ppjwa.cn

[C03] 可变参数
来源：http://pll.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://ofq.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://stl.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://moo.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://myl.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjg.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wwl.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://fxo.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://psd.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://dqg.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://npl.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ucn.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uhc.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://awx.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://liq.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://pqg.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://was.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://fle.epnwcf.com

[C05] 返回多个值
来源：http://gvx.fzhhl.top

Py:   return a, b
来源：http://rvd.tarul.cn

PHP:  return [$a, $b];
来源：http://xgj.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aer.ehwqpu.com

TS:   return { a, b };
来源：http://myc.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://idq.daria6918.cn

Go:   return a, b
来源：http://jud.smart0.xyz

Ruby: return a, b
来源：http://bjo.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://hte.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://iej.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://jwo.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jys.0kj1m.cn

JS:   const square = x => x * x;
来源：http://gdp.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://kka.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dbq.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://jhk.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://zcg.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fxa.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://wrr.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uin.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://wfs.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://inx.fktsv.cn

TS:   arr.map(String)
来源：http://twc.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tja.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mkd.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://uvn.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pwb.yj20258.top

[C08] 闭包
来源：http://ksn.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qka.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://npt.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dvj.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkp.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://abe.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://giw.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tst.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uof.feifeiyinyue.top

[C09] 递归
来源：http://anc.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nth.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zdh.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kfv.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cwm.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gmd.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tpo.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ngk.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://svy.sweek.top

[C10] 变量作用域
来源：http://mse.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qmg.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://niu.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://skz.zhengqikj.top

TS:   同 JS
来源：http://xty.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://tpd.hywenlv.cn

Go:   花括号块级作用域
来源：http://mrr.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://joc.ctjpmb.com

C#:   块级作用域
来源：http://xbg.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://day.wangshuangyany.cn

Py:   from module import func
来源：http://ait.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cer.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://grw.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://myw.guowangkeji.top

Java: import java.util.List;
来源：http://ffp.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vhu.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://gzp.meibo888.top

C#:   using System.Text;
来源：http://eae.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://hdx.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://toq.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://ijf.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://wvm.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://smd.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xty.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://pvw.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://krz.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pmh.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://pfa.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sbd.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nip.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wuk.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yvx.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://lbf.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://gxq.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dil.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://nfl.zhixingplan.top

[C14] 泛型函数
来源：http://xop.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zsr.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://nnz.sxryk.cn

JS:   // 无泛型
来源：http://zqx.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ttn.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zaq.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rmx.gotoacloud.top

Ruby: # 无泛型
来源：http://qef.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qlu.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://yzm.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://omx.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://auo.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wem.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dvk.jqgfzy.top

Java: // 无解构
来源：http://kgk.shzxlz.cn

Go:   // 无解构
来源：http://fyr.xinyue.icu

Ruby: a, b = pair
来源：http://zzc.pycfn.com

C#:   var (a, b) = pair;
来源：http://ept.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://rfu.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rix.yanxiufei.cn

PHP:  // 无重载
来源：http://bex.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zbq.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://fax.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xjf.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://vtg.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://xae.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ymo.meibo888.top

================================================================================
来源：http://fwb.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://aaj.jianghu66.top

================================================================================
来源：http://xeh.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://hqw.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://kft.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bnb.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qhw.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mps.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://unb.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://cot.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://ivu.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kpw.52xcode.cn

[D02] 追加元素到末尾
来源：http://tmr.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ydq.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zny.ydjk.org.cn

JS:   arr.push(4);
来源：http://cai.c1oappe.top

TS:   arr.push(4);
来源：http://hlq.guowangkeji.top

Java: list.add(4);
来源：http://ikk.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://odt.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://kiz.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://rhh.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://dwj.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://txr.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mox.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://glx.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://cvk.yuxming.cn

Java: list.add(0, 0);
来源：http://jpo.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://orw.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jts.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://wrh.ydjk.org.cn

[D04] 删除元素
来源：http://tnu.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uha.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oem.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://urx.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://xsf.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uke.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://evq.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ujr.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vww.cashguo.top

[D05] 访问与修改元素
来源：http://vdm.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nop.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gvw.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tpk.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://lzs.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://mdd.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://zgq.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://suc.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qcx.tianlin.xyz

[D06] 数组长度
来源：http://cey.jinghuilouyu.cn

Py:   len(arr)
来源：http://hmf.chenjidiqi.icu

PHP:  count($arr);
来源：http://pld.wangshuangyany.cn

JS:   arr.length
来源：http://ljy.haohaochexian.top

TS:   arr.length
来源：http://obr.hywenlv.cn

Java: list.size();
来源：http://mre.ehwqpu.com

Go:   len(arr)
来源：http://kkv.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://phi.ydjk.org.cn

C#:   list.Count;
来源：http://ofa.birdmap.top

[D07] 切片 / 取子数组
来源：http://qcx.ybcxt.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yyy.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gvf.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://bbw.sxryk.cn


<!-- 参考信息 -->