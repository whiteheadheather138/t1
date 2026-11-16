代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://heq.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://gbv.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aic.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://axo.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bli.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wtl.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uno.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ocj.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pxa.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vhl.hysaishi.cn

[B07] while 循环
来源：http://qtn.wangdashe.top

Py:   while i < 10: i += 1
来源：http://oyo.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mew.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://ovg.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://kpy.316326.xyz

Java: while (i < 10) { i++; }
来源：http://jpx.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://klj.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://uiq.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://gzi.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://dei.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://yza.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://usi.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://dmq.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://yft.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://urd.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qgq.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://tnv.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://juf.nwbrower.top

[B09] break 与 continue
来源：http://wyx.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zdd.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yym.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aez.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsl.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzm.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ise.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mtx.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mne.yj202588.top

[B10] 遍历同时拿索引
来源：http://hyi.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uyc.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hkq.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nxy.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nkb.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cwn.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jwp.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vcj.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lam.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://fwh.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://cui.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://klp.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wqe.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://czi.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oew.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zjf.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://kxw.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xtx.kuanghao11.cn

[B12] 跳出多层循环
来源：http://vvo.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gus.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tmz.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pzv.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxw.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gpo.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eon.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jnv.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dye.c1oappe.top

[B13] 判断是否为数字
来源：http://thk.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://hed.ybcxt.top

PHP:  is_numeric($x)
来源：http://odc.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jpn.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alz.yvedp.cn

Java: x instanceof Number
来源：http://yoj.pycfn.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ekd.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://yqu.hywenlv.cn

C#:   x is int or double or decimal
来源：http://hnu.hnqzz.top

[B14] 判断值是否在集合内
来源：http://fdc.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qhc.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://amk.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://azb.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://gnx.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pxc.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kir.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wdy.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vis.pycfn.com

[B15] 布尔运算与取反
来源：http://yfl.uphjek.com

Py:   a and b or not c
来源：http://qhc.aizwys.cn

PHP:  $a && $b || !$c
来源：http://oyn.yj20258.top

JS:   a && b || !c
来源：http://euo.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://qdn.shanyushiyangkeji.top

Java: a && b || !c
来源：http://ewk.aibaodan.cn

Go:   a && b || !c
来源：http://lhk.zdbjq.cn

Ruby: a && b || !c
来源：http://yis.sweek.top

C#:   a && b || !c
来源：http://dwy.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://gdd.cashguo.top

Py:   if not data: return
来源：http://ttu.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://uhv.jqgfzy.top

JS:   if (!data) return;
来源：http://zfb.sjlbkw.cn

TS:   if (!data) return;
来源：http://zqx.cdnleiting.top

Java: if (data == null) return;
来源：http://czj.bjfxy.top

Go:   if data == nil { return }
来源：http://icl.snrcjt.cn

Ruby: return if data.nil?
来源：http://yxk.guannengcc.top

C#:   if (data == null) return;
来源：http://lkl.zhijiandao.cn

================================================================================
来源：http://xdv.zhixingplan.top

C. 函数与作用域
来源：http://ltg.daria6918.cn

================================================================================
来源：http://iqw.birdmap.top

[C01] 定义函数
来源：http://pac.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://wkr.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fbp.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://jxo.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uyx.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hcc.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://igl.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://tic.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xrv.316326.xyz

[C02] 默认参数
来源：http://ffg.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://uxm.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tvt.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://idb.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tom.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ble.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ovc.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://bsn.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://hhb.shanyushiyangtech.top

[C03] 可变参数
来源：http://vrp.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://nba.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ndx.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgp.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xmz.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://did.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kzp.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://mjf.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tzm.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://qxi.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xpr.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wfz.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ymk.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://adz.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://loy.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://cha.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://ybr.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://rcv.zdbjq.cn

[C05] 返回多个值
来源：http://vza.yonumen.top

Py:   return a, b
来源：http://loe.fehbvm.com

PHP:  return [$a, $b];
来源：http://olq.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lit.zhiwuduotai.top

TS:   return { a, b };
来源：http://tto.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pbq.yuxming.cn

Go:   return a, b
来源：http://jpb.ydzc1.top

Ruby: return a, b
来源：http://mtm.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://hiw.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://igi.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://sdl.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://eop.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://wtp.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://ywi.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://skw.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://ngo.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://has.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://fzp.vehdjk.com

[C07] 把函数作为参数传入
来源：http://fzo.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xrf.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://nkq.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rap.0kj1m.cn

TS:   arr.map(String)
来源：http://zzj.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ksv.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://osz.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://flt.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://lsx.yfazqb.com

[C08] 闭包
来源：http://xqx.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zsc.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ylr.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pai.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zfd.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rqz.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lki.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tql.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wns.fzhhl.top

[C09] 递归
来源：http://pbt.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gru.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sjx.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzd.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ybb.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fqe.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://atn.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dan.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dey.ctjpmb.com

[C10] 变量作用域
来源：http://vnz.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rxm.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jdn.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bjn.haohaochexian.top

TS:   同 JS
来源：http://mnq.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://tkj.ivvv.top

Go:   花括号块级作用域
来源：http://wfh.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mhy.wangshuangyany.cn

C#:   块级作用域
来源：http://lme.yj202588.top

[C11] 模块导入与导出
来源：http://tll.aizwys.cn

Py:   from module import func
来源：http://ict.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hci.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://rgb.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sxu.xinyue.icu

Java: import java.util.List;
来源：http://ler.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://coy.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://ext.jyoumei.cn

C#:   using System.Text;
来源：http://ofc.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://hri.birdmap.top

Py:   (lambda: print("run"))()
来源：http://vbi.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://tdj.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://gwy.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://nxr.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mjy.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://yfh.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://bfu.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qhy.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://kop.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cqa.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmb.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ips.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdi.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cgu.havefunace.top

Go:   func add(a, b int) int
来源：http://his.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tgf.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://phg.feifeiyinyue.top

[C14] 泛型函数
来源：http://wkf.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gop.shuidangran.top

PHP:  // 无泛型
来源：http://gmz.hammf.cn

JS:   // 无泛型
来源：http://gok.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jsb.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kiw.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jab.uphjek.com

Ruby: # 无泛型
来源：http://elt.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oqy.zycfv.cn

[C15] 解构 / 展开参数
来源：http://wen.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tic.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://sns.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nqm.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://npi.52xcode.cn

Java: // 无解构
来源：http://kgl.52xcode.cn

Go:   // 无解构
来源：http://bqq.tianlin.xyz

Ruby: a, b = pair
来源：http://arl.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://mco.yj202588.top

[C16] 函数 / 方法重载
来源：http://ckx.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jmh.yj20258888.top

PHP:  // 无重载
来源：http://mao.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://lvj.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://jqe.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gmv.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://wrm.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://qyz.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yrg.yj202588.top

================================================================================
来源：http://bzs.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://ntg.shzxlz.cn

================================================================================
来源：http://aby.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://kvf.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://izz.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zci.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ovb.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lka.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qwo.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://kuz.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://vqg.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hcn.gzhubu.top

[D02] 追加元素到末尾
来源：http://jfs.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://daq.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uzq.0kj1m.cn

JS:   arr.push(4);
来源：http://sjt.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://oci.tanke756.top

Java: list.add(4);
来源：http://ttq.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://rua.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://xyb.yj20258.top

C#:   list.Add(4);
来源：http://qgl.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://gtg.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://pdz.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xxh.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nwr.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://jba.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://ocm.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wis.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cgv.cashguo.top

C#:   list.Insert(0, 0);
来源：http://nxm.zdbjq.cn

[D04] 删除元素
来源：http://adx.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://roa.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hki.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cem.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://njr.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tit.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lhl.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fhb.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dso.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://mqa.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lcr.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dtx.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oem.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://yhs.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://iof.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://bwk.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yxo.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qpn.hfpthk.cn

[D06] 数组长度
来源：http://vln.zhongyouzk.top

Py:   len(arr)
来源：http://wqb.xuanzx.com

PHP:  count($arr);
来源：http://vax.snrcjt.cn

JS:   arr.length
来源：http://yuw.vehdjk.com

TS:   arr.length
来源：http://sqq.hcnkem.com


<!-- 参考信息 -->