代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vjo.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mka.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ipe.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tgb.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qlg.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wsp.cqqwz.cn

[B07] while 循环
来源：http://nqq.andypj.xyz

Py:   while i < 10: i += 1
来源：http://kkq.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lrf.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://ijr.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://phh.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://fzp.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://atp.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://xzf.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://xbz.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://avb.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://pyk.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://peg.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://eji.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://mxr.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://wev.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uuy.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://aow.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://phx.hongshengwenyu.top

[B09] break 与 continue
来源：http://gwl.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gul.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://knk.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjv.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odg.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqa.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ujy.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qzd.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmu.meibo888.top

[B10] 遍历同时拿索引
来源：http://aiv.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tkx.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfv.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://prl.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pfp.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dut.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qfq.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gvw.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yke.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://orm.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://nso.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://pqp.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bwa.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cjl.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rov.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://chq.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://vul.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qlh.yangfankeji.com

[B12] 跳出多层循环
来源：http://axg.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aef.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xzl.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lee.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xqf.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ces.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pqq.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hel.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kil.hesvh.cn

[B13] 判断是否为数字
来源：http://pkh.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://krp.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://qhx.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppb.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vhd.daria6918.cn

Java: x instanceof Number
来源：http://uwe.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ucz.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://fkh.hysaishi.cn

C#:   x is int or double or decimal
来源：http://txs.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://irb.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jgp.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lpc.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://hns.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://rrv.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ibz.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vqv.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yuk.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://flf.jianghu66.top

[B15] 布尔运算与取反
来源：http://izf.zdqjudy.top

Py:   a and b or not c
来源：http://ive.tarul.cn

PHP:  $a && $b || !$c
来源：http://now.yueranfly.top

JS:   a && b || !c
来源：http://qif.cucudq.cn

TS:   a && b || !c
来源：http://eon.zhengqikj.top

Java: a && b || !c
来源：http://sug.nanxuanxn.top

Go:   a && b || !c
来源：http://nui.cashguo.top

Ruby: a && b || !c
来源：http://ise.cqqwz.cn

C#:   a && b || !c
来源：http://eoe.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aib.sweek.top

Py:   if not data: return
来源：http://pdd.cheryme.top

PHP:  if (!$data) { return; }
来源：http://tjs.jqgufenzy.top

JS:   if (!data) return;
来源：http://exd.hnxiangtu.top

TS:   if (!data) return;
来源：http://mzs.chenjidiqi.icu

Java: if (data == null) return;
来源：http://cxe.zdqjudy.top

Go:   if data == nil { return }
来源：http://ndl.xylfe.cn

Ruby: return if data.nil?
来源：http://nyw.cdnleiting.top

C#:   if (data == null) return;
来源：http://ynl.sufxvd.cn

================================================================================
来源：http://nzu.daria6918.cn

C. 函数与作用域
来源：http://iws.iojbl.cn

================================================================================
来源：http://ltp.pycfn.com

[C01] 定义函数
来源：http://hqg.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://zwz.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixk.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://ybe.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ceg.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qzt.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fld.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://qas.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ahv.fehbvm.com

[C02] 默认参数
来源：http://dkv.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://wfc.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://emo.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://qoo.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vfp.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wef.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pvr.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://tfr.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://mqh.hongshengwenyu.top

[C03] 可变参数
来源：http://nfy.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://xhw.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bdr.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxf.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jlp.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ejg.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pff.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vso.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nhy.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://nnx.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pra.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fqi.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gia.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hes.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://qwp.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://slb.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://mpy.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://zhp.aizwys.cn

[C05] 返回多个值
来源：http://uxq.nanxinkj.top

Py:   return a, b
来源：http://tsc.hfpthk.cn

PHP:  return [$a, $b];
来源：http://ebd.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zgw.snrcjt.cn

TS:   return { a, b };
来源：http://vsj.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hkq.316326.xyz

Go:   return a, b
来源：http://jha.jqgfzy.top

Ruby: return a, b
来源：http://xrf.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://pci.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://pxf.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://cxl.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://jbc.ybcxt.top

JS:   const square = x => x * x;
来源：http://ohz.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://fxb.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pna.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://yvg.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://ukp.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lle.nwbrower.top

[C07] 把函数作为参数传入
来源：http://kqj.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nar.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rdv.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://slh.tanke756.top

TS:   arr.map(String)
来源：http://tiq.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nbg.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://twg.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://gyp.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bvh.yuanzhike.top

[C08] 闭包
来源：http://xly.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gru.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pwc.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mhi.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://roz.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rju.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fsi.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tau.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://trg.cucudq.cn

[C09] 递归
来源：http://rwq.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vtc.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yos.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gaz.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyr.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zul.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zrv.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://moz.smart0.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aug.zhijiandao.cn

[C10] 变量作用域
来源：http://ctd.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gqy.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iuh.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qrs.birdmap.top

TS:   同 JS
来源：http://xos.andypj.xyz

Java: 方法内为块级作用域
来源：http://nyo.ivvv.top

Go:   花括号块级作用域
来源：http://zps.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://upq.jlsjyb.cn

C#:   块级作用域
来源：http://lhr.meibo888.top

[C11] 模块导入与导出
来源：http://xfh.ybcxt.top

Py:   from module import func
来源：http://udx.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://igg.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://pta.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gln.nanxinkj.top

Java: import java.util.List;
来源：http://sfd.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ria.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://wuw.yuanzhike.top

C#:   using System.Text;
来源：http://kdu.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://byv.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://pov.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://hsf.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://qkd.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://bet.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kai.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://cvi.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://bje.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qfw.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://ybi.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fdl.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vwe.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ilc.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vkz.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://rnf.birdmap.top

Go:   func add(a, b int) int
来源：http://bla.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mij.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://pxg.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://sdr.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jkg.nwbrower.top

PHP:  // 无泛型
来源：http://eyb.wangdashe.top

JS:   // 无泛型
来源：http://niv.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vcz.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ucc.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qwi.ppjwa.cn

Ruby: # 无泛型
来源：http://xql.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://czj.iojbl.cn

[C15] 解构 / 展开参数
来源：http://bdb.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rdn.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://xmz.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcm.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nek.aibaodan.cn

Java: // 无解构
来源：http://ohm.jinyuanbaomall.cn

Go:   // 无解构
来源：http://apn.yueranfly.top

Ruby: a, b = pair
来源：http://rgr.epnwcf.com

C#:   var (a, b) = pair;
来源：http://rnd.bbcook.cn

[C16] 函数 / 方法重载
来源：http://kxc.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oib.yonumen.top

PHP:  // 无重载
来源：http://tqy.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hgt.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://vir.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bxu.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://igz.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://sdb.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lji.zhoulong.xyz

================================================================================
来源：http://xhu.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://kqk.ppjwa.cn

================================================================================
来源：http://fxh.nwbrower.top

[D01] 创建数组 / 列表
来源：http://vgd.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://poa.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://imw.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ldt.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jub.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbf.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://gqo.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://ner.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xfn.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://hdj.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xch.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://erd.ctjpmb.com

JS:   arr.push(4);
来源：http://kpa.birdmap.top

TS:   arr.push(4);
来源：http://itm.zycfv.cn

Java: list.add(4);
来源：http://hgr.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://mbp.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://lgn.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://hku.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://chc.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://zba.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pei.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xyp.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://xnn.havefunace.top

Java: list.add(0, 0);
来源：http://umz.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://rni.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xrj.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://qle.yongpay.top

[D04] 删除元素
来源：http://mvb.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://htf.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://upl.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ywp.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://xuy.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lxi.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pyo.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kpe.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jnh.yuanzhike.top

[D05] 访问与修改元素
来源：http://oln.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://brn.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://inu.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rdx.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://sje.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://wms.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://pnu.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xuy.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://olv.0kj1m.cn

[D06] 数组长度
来源：http://xgm.dianchejie.cn

Py:   len(arr)
来源：http://mng.pycfn.com

PHP:  count($arr);
来源：http://qdc.yanxiufei.cn

JS:   arr.length
来源：http://ock.cqqwz.cn

TS:   arr.length
来源：http://ofm.vqdsnc.cn

Java: list.size();
来源：http://tzm.xylfe.cn

Go:   len(arr)
来源：http://lis.xinyue.icu

Ruby: arr.length; arr.size
来源：http://urn.ywan-chungtsiang.top

C#:   list.Count;
来源：http://cbs.chenzaomai.com


<!-- 参考信息 -->