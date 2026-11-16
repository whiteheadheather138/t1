代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fqe.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tag.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jow.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rjz.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hxg.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pkr.nwbrower.top

[B07] while 循环
来源：http://sqh.daxiang520.top

Py:   while i < 10: i += 1
来源：http://ell.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://waj.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://een.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://knm.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://srz.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yci.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://nhp.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://owo.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://ifx.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://qmm.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ruh.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://kgr.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://wap.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://oeo.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mwa.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gku.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://qnn.cheryme.top

[B09] break 与 continue
来源：http://mlc.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pgy.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cdl.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucs.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tic.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afe.cdnleiting.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ujt.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hxc.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osx.sxryk.cn

[B10] 遍历同时拿索引
来源：http://yds.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://amc.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kji.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nmp.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iec.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bog.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wcg.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://upd.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eiq.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://put.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://era.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://xdt.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://smp.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbm.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jvm.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uwj.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://cbc.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ldi.daxiang520.top

[B12] 跳出多层循环
来源：http://noj.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wfd.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://euv.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ejs.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://giu.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nfu.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wgo.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gyy.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dxm.nanxinkj.top

[B13] 判断是否为数字
来源：http://zyi.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://hee.daria6918.cn

PHP:  is_numeric($x)
来源：http://ssd.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jnx.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epj.kuanghao11.cn

Java: x instanceof Number
来源：http://byd.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://keu.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://tpx.snrcjt.cn

C#:   x is int or double or decimal
来源：http://mif.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://sgl.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sns.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kvg.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://smg.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://rau.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://epy.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bds.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xip.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sxb.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://noi.zhixingplan.top

Py:   a and b or not c
来源：http://drh.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://jjr.hesvh.cn

JS:   a && b || !c
来源：http://cwp.52xcode.cn

TS:   a && b || !c
来源：http://sfc.sjlbkw.cn

Java: a && b || !c
来源：http://txw.ydjk.org.cn

Go:   a && b || !c
来源：http://old.daxiang520.top

Ruby: a && b || !c
来源：http://pyg.sweek.top

C#:   a && b || !c
来源：http://eic.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lyk.mhx1999.top

Py:   if not data: return
来源：http://tsg.yj20258.top

PHP:  if (!$data) { return; }
来源：http://sdv.vqdsnc.cn

JS:   if (!data) return;
来源：http://hze.jyoumei.cn

TS:   if (!data) return;
来源：http://iwp.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://sem.yuanzhike.top

Go:   if data == nil { return }
来源：http://gvo.bbcook.cn

Ruby: return if data.nil?
来源：http://uyv.cucudq.cn

C#:   if (data == null) return;
来源：http://xts.jinqigfzy.top

================================================================================
来源：http://ipa.hysaishi.cn

C. 函数与作用域
来源：http://ucr.ydjk.org.cn

================================================================================
来源：http://jon.ctjpmb.com

[C01] 定义函数
来源：http://qxo.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://dnh.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vwc.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://bya.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrx.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://noj.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://rxk.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://zzg.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://otc.hammf.cn

[C02] 默认参数
来源：http://umg.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://jry.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gzy.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://bhs.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lvn.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://aky.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nut.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://crc.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://pna.tanke756.top

[C03] 可变参数
来源：http://xqd.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://uit.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rwe.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pjq.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqv.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zqp.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fpr.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://fbn.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eyl.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://xus.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nxd.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xwa.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zuw.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://agw.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://pub.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://bdl.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://voh.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://pza.zhoulong.xyz

[C05] 返回多个值
来源：http://yyk.uphjek.com

Py:   return a, b
来源：http://sci.dianchejie.cn

PHP:  return [$a, $b];
来源：http://itl.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iah.yuanzhike.top

TS:   return { a, b };
来源：http://cih.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hri.aibaodan.cn

Go:   return a, b
来源：http://mly.epnwcf.com

Ruby: return a, b
来源：http://lkh.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://qcq.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://vcj.ivvv.top

Py:   square = lambda x: x * x
来源：http://egr.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hjv.sxryk.cn

JS:   const square = x => x * x;
来源：http://gkc.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://xvo.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ohw.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://cmg.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://kkw.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://czm.hesvh.cn

[C07] 把函数作为参数传入
来源：http://rzc.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ssb.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://hkv.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ujp.hysaishi.cn

TS:   arr.map(String)
来源：http://orz.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://idx.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ujv.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://siz.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ibb.dashuyun.cn

[C08] 闭包
来源：http://tif.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qez.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vey.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fzq.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ois.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://can.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rqj.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ttc.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uft.fanxiaobao.xyz

[C09] 递归
来源：http://gmk.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uug.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vhn.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://plf.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wvv.hesvh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nlz.cheryme.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fzh.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xjr.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rif.zdqjudy.top

[C10] 变量作用域
来源：http://hpo.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cba.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rjx.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pju.sufxvd.cn

TS:   同 JS
来源：http://qji.yuanzhike.top

Java: 方法内为块级作用域
来源：http://dcv.redwolf501.top

Go:   花括号块级作用域
来源：http://rad.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ebn.vqdsnc.cn

C#:   块级作用域
来源：http://rij.sufxvd.cn

[C11] 模块导入与导出
来源：http://zjn.pycfn.com

Py:   from module import func
来源：http://qvz.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vyh.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://epa.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ziv.kuanghao11.cn

Java: import java.util.List;
来源：http://lrt.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fnb.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://sju.fzhhl.top

C#:   using System.Text;
来源：http://vbl.vqdsnc.cn

[C12] 立即执行函数 IIFE
来源：http://dmd.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://jif.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://wpz.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://nfd.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://zhm.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rrv.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://agt.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://sju.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://bka.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://xnm.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rpt.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lgq.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://snh.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jkj.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://bsc.hcnkem.com

Go:   func add(a, b int) int
来源：http://sfa.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fbj.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vhp.chenzaomai.com

[C14] 泛型函数
来源：http://idv.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rqo.jlsjyb.cn

PHP:  // 无泛型
来源：http://wwy.shanyushiyangtech.top

JS:   // 无泛型
来源：http://ffd.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xeh.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lkr.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mwc.guannengcc.top

Ruby: # 无泛型
来源：http://mgq.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pic.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://ion.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bjp.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://dio.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ign.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kjn.quarkkingdee.top

Java: // 无解构
来源：http://fnh.kuanghao11.cn

Go:   // 无解构
来源：http://dwm.sxryk.cn

Ruby: a, b = pair
来源：http://mtn.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://jop.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://yex.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kzh.hfpthk.cn

PHP:  // 无重载
来源：http://rvk.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jhq.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://igw.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jxu.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://fhf.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://pgj.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tko.ydzc1.top

================================================================================
来源：http://slx.yonumen.top

D. 数组 / 列表 / 集合
来源：http://jwg.bbcook.cn

================================================================================
来源：http://zyt.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://apr.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tpn.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://khh.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hrc.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tto.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ogg.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://aac.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://kbz.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xqc.gogol.net.cn

[D02] 追加元素到末尾
来源：http://esa.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ziu.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rho.tian-w.cn

JS:   arr.push(4);
来源：http://pnv.fktsv.cn

TS:   arr.push(4);
来源：http://sqt.aibaodan.cn

Java: list.add(4);
来源：http://aji.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://gtc.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://lax.daxiang520.top

C#:   list.Add(4);
来源：http://vdz.daria6918.cn

[D03] 在指定位置插入元素
来源：http://zqo.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://uax.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://exv.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wbq.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://bap.fengsongda.top

Java: list.add(0, 0);
来源：http://pxf.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://qpr.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://smd.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://zrj.fehbvm.com

[D04] 删除元素
来源：http://mpt.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://alu.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zfc.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eyx.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://bfd.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://awh.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hqe.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jbn.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bdg.bjfxy.top

[D05] 访问与修改元素
来源：http://jyg.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cfq.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://amg.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://byr.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://bia.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://mbc.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wxy.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://skf.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zmc.pycfn.com

[D06] 数组长度
来源：http://kia.ydzc1.top

Py:   len(arr)
来源：http://xry.yj20258.top

PHP:  count($arr);
来源：http://mbm.jinqigufen.top

JS:   arr.length
来源：http://njb.quarkkingdee.top

TS:   arr.length
来源：http://mxx.cqqwz.cn

Java: list.size();
来源：http://nzm.redwolf501.top

Go:   len(arr)
来源：http://gmi.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://ajp.yj20258.top

C#:   list.Count;
来源：http://inx.gzhubu.top


<!-- 参考信息 -->