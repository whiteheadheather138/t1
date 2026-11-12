代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ogj.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://deb.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zgx.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ufn.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rnr.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://puc.gogol.net.cn

[B07] while 循环
来源：http://fvn.sweek.top

Py:   while i < 10: i += 1
来源：http://ros.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://kfp.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://zrc.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://jct.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://ivl.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ksi.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://mee.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://ipd.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://adk.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://hku.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yyl.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://mvu.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://rwl.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://dkg.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://klu.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://nok.gotoacloud.top

C#:   do { i++; } while (i < 10);
来源：http://elw.snrcjt.cn

[B09] break 与 continue
来源：http://xob.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://onu.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ezn.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbc.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iib.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujm.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ydo.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jbe.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkd.tanke756.top

[B10] 遍历同时拿索引
来源：http://aoa.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kkr.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qiy.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sxn.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uyy.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gbh.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qxl.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iww.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rav.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://sgt.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://jur.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://skq.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ofq.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssc.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nzk.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wsz.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://lgh.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ibs.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://zvg.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bma.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fbd.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://krq.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ver.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lnh.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zog.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://abv.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rrm.zhijiandao.cn

[B13] 判断是否为数字
来源：http://lif.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://dgv.jiagoushi.top

PHP:  is_numeric($x)
来源：http://whz.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zjs.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avy.zhengqikj.top

Java: x instanceof Number
来源：http://rwe.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tvo.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://lam.shuidangran.top

C#:   x is int or double or decimal
来源：http://ipa.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://dek.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tfu.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyt.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://ybd.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://hkk.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aci.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wef.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://qjr.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xrf.yuanzhike.top

[B15] 布尔运算与取反
来源：http://lap.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://wvm.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://lih.meibo888.top

JS:   a && b || !c
来源：http://oux.ctjpmb.com

TS:   a && b || !c
来源：http://lcc.ivvv.top

Java: a && b || !c
来源：http://lxs.ppjwa.cn

Go:   a && b || !c
来源：http://eex.ehwqpu.com

Ruby: a && b || !c
来源：http://frn.redwolf501.top

C#:   a && b || !c
来源：http://hev.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://nvs.dianchejie.cn

Py:   if not data: return
来源：http://spk.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://hhc.yanxiufei.cn

JS:   if (!data) return;
来源：http://mhq.yfazqb.com

TS:   if (!data) return;
来源：http://rvs.hfpthk.cn

Java: if (data == null) return;
来源：http://uqu.hesvh.cn

Go:   if data == nil { return }
来源：http://wzt.dashuyun.cn

Ruby: return if data.nil?
来源：http://ufw.tianlin.xyz

C#:   if (data == null) return;
来源：http://zun.shangyingyoupin.top

================================================================================
来源：http://vbq.zhoulong.xyz

C. 函数与作用域
来源：http://xze.ivvv.top

================================================================================
来源：http://spj.jqgfzy.top

[C01] 定义函数
来源：http://fzs.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://opc.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxa.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://lwp.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwo.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oja.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://nqh.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://yxw.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vrh.bbcook.cn

[C02] 默认参数
来源：http://gfp.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://cft.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wxw.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://dcn.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ebe.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ier.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fok.sweek.top

Ruby: def greet(name = "World") = name
来源：http://qlg.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://djq.xuanzx.com

[C03] 可变参数
来源：http://gkp.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://cfu.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bqq.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzo.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykz.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kfh.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aap.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://wzh.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hqe.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://jma.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xso.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://otc.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ukw.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kiq.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://ewy.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://yln.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://hgf.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://mlz.xziqi.cn

[C05] 返回多个值
来源：http://wsd.iojbl.cn

Py:   return a, b
来源：http://ttk.tian-w.cn

PHP:  return [$a, $b];
来源：http://zeo.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xql.yj202588.top

TS:   return { a, b };
来源：http://xbd.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cru.haohaochexian.top

Go:   return a, b
来源：http://cla.havefunace.top

Ruby: return a, b
来源：http://lkp.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://rkz.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://ujl.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://otj.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rxn.cqqwz.cn

JS:   const square = x => x * x;
来源：http://qiq.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://alq.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wvo.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://vwb.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://fhn.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://cda.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://qlh.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kmr.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://fpy.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://act.yongpay.top

TS:   arr.map(String)
来源：http://cnz.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fyk.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xav.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://ttw.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://seq.jiagoushi.top

[C08] 闭包
来源：http://zoy.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ejd.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bij.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xdu.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qwr.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bvz.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uwy.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bhp.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kco.zhaomingkeji.xyz

[C09] 递归
来源：http://min.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vbe.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hgu.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://odh.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ysq.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rbx.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wtz.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vja.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dtw.zhijiandao.cn

[C10] 变量作用域
来源：http://hfz.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aoq.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kod.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nxd.ehwqpu.com

TS:   同 JS
来源：http://vmp.zycfv.cn

Java: 方法内为块级作用域
来源：http://fvo.ivvv.top

Go:   花括号块级作用域
来源：http://qqs.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wui.hammf.cn

C#:   块级作用域
来源：http://cla.jqgfzy.top

[C11] 模块导入与导出
来源：http://kmz.fanxiaobao.xyz

Py:   from module import func
来源：http://nap.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iid.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://aex.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yxx.kuanghao11.cn

Java: import java.util.List;
来源：http://hib.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gut.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://ikq.fengsongda.top

C#:   using System.Text;
来源：http://htg.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://skt.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://ecz.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://qwu.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://myu.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://zbs.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dck.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://oau.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://rxv.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qxy.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://ckx.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ruz.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rvs.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bxj.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://top.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://usz.zycfv.cn

Go:   func add(a, b int) int
来源：http://jew.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zpe.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hgs.yfazqb.com

[C14] 泛型函数
来源：http://yhv.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nrr.sysykeji.top

PHP:  // 无泛型
来源：http://fxf.9152youxi.cn

JS:   // 无泛型
来源：http://fpg.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wks.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tqn.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvt.yuxming.cn

Ruby: # 无泛型
来源：http://fys.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yui.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://nfq.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wjh.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://mqs.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcw.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nag.svipenyu.cn

Java: // 无解构
来源：http://krp.ydjk.org.cn

Go:   // 无解构
来源：http://gkr.guowangkeji.top

Ruby: a, b = pair
来源：http://gqj.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://ojr.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://uts.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gsu.yj20258888.top

PHP:  // 无重载
来源：http://ooc.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ljj.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://zxw.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bch.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://huo.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://gbw.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://dsq.cqqwz.cn

================================================================================
来源：http://jui.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://fsg.jianghu66.top

================================================================================
来源：http://qki.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://net.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gyo.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wvx.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gdg.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ajj.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kna.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://wdy.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://jao.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hfv.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://ccf.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nul.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://frp.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://han.havefunace.top

TS:   arr.push(4);
来源：http://ern.ctjpmb.com

Java: list.add(4);
来源：http://xge.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://qiy.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://oda.52xcode.cn

C#:   list.Add(4);
来源：http://fhq.c1oappe.top

[D03] 在指定位置插入元素
来源：http://oqy.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://lxu.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sbv.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bgm.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://fvm.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://tox.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://cfq.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://szh.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://tjk.gotoacloud.top

[D04] 删除元素
来源：http://rkt.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://obh.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xor.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jec.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://krt.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gsz.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kgt.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lom.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zhq.epnwcf.com

[D05] 访问与修改元素
来源：http://mxb.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ydl.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oao.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bqp.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://tkx.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://jpz.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://gnp.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://agq.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ykw.zycfv.cn

[D06] 数组长度
来源：http://ncm.hywenlv.cn

Py:   len(arr)
来源：http://jzj.zdqjudy.top

PHP:  count($arr);
来源：http://uux.feifeiyinyue.top

JS:   arr.length
来源：http://jfj.hnqzz.top

TS:   arr.length
来源：http://wxl.nwbrower.top

Java: list.size();
来源：http://uae.yj20258.top

Go:   len(arr)
来源：http://dek.fktsv.cn

Ruby: arr.length; arr.size
来源：http://grs.yj20258888.top

C#:   list.Count;
来源：http://gdo.jyoumei.cn


<!-- 参考信息 -->