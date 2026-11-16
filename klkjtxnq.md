代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://swl.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gzo.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nwu.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qvt.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://icy.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hgx.316326.xyz

[B07] while 循环
来源：http://rrm.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://tgr.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://nnr.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://weu.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://eyw.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://zes.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://buv.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://btj.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://rrj.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://vfh.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://eob.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://num.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://xtj.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://kmg.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://sxw.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://dqm.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://wlr.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://fyg.xinyue.icu

[B09] break 与 continue
来源：http://dex.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kak.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://isw.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdn.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qik.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srs.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uld.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://upt.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kaa.birdmap.top

[B10] 遍历同时拿索引
来源：http://uxq.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lyl.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfc.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://asc.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nvx.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bbt.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://exf.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wel.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wpp.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://xka.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://jcc.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://vqu.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ckm.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ver.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rfx.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fdf.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://rxr.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vcd.yj202588.top

[B12] 跳出多层循环
来源：http://azo.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vcc.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://yys.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://efh.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rpp.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qau.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://amv.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gtc.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tua.ydzc1.top

[B13] 判断是否为数字
来源：http://wji.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://ojk.guannengcc.top

PHP:  is_numeric($x)
来源：http://xii.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dca.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vbq.sweek.top

Java: x instanceof Number
来源：http://hyv.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zct.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://myg.tarul.cn

C#:   x is int or double or decimal
来源：http://iws.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://ctw.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iso.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oeb.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://mkw.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://ook.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pkk.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qsw.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://duc.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iht.ydzc1.top

[B15] 布尔运算与取反
来源：http://xoa.nwbrower.top

Py:   a and b or not c
来源：http://oeo.vehdjk.com

PHP:  $a && $b || !$c
来源：http://svu.ctjpmb.com

JS:   a && b || !c
来源：http://dry.yj20258.top

TS:   a && b || !c
来源：http://hhf.jinyuanbaomall.cn

Java: a && b || !c
来源：http://pwi.sufxvd.cn

Go:   a && b || !c
来源：http://noq.redwolf501.top

Ruby: a && b || !c
来源：http://sow.sweek.top

C#:   a && b || !c
来源：http://ubw.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://jfm.yueranfly.top

Py:   if not data: return
来源：http://ice.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://teb.cucudq.cn

JS:   if (!data) return;
来源：http://giu.shangyingyoupin.top

TS:   if (!data) return;
来源：http://paq.jiagoushi.top

Java: if (data == null) return;
来源：http://vvt.jiagoushi.top

Go:   if data == nil { return }
来源：http://xoe.sysykeji.top

Ruby: return if data.nil?
来源：http://ouh.gogol.net.cn

C#:   if (data == null) return;
来源：http://xam.jqgfzy.top

================================================================================
来源：http://qkh.bbcook.cn

C. 函数与作用域
来源：http://vbu.chenzaomai.com

================================================================================
来源：http://nro.fengsongda.top

[C01] 定义函数
来源：http://etl.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://aib.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmz.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ejn.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://auy.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rro.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://hpv.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://ega.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fwb.0kj1m.cn

[C02] 默认参数
来源：http://xqe.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://uxv.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pwo.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://zxr.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://irt.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://mct.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sti.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://jhk.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://gbr.xuetiantiany.cn

[C03] 可变参数
来源：http://mzc.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://xsb.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ocb.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dsn.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bsk.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfu.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nho.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://okr.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tor.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://eug.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iwf.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gij.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gmo.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pti.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://bgj.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://ifz.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://csi.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://uao.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://fxw.pengpengdd.cyou

Py:   return a, b
来源：http://ryd.hnqzz.top

PHP:  return [$a, $b];
来源：http://uvu.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kmv.hammf.cn

TS:   return { a, b };
来源：http://hnw.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ahm.xziqi.cn

Go:   return a, b
来源：http://tml.bjfxy.top

Ruby: return a, b
来源：http://drt.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://gqf.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://vzo.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://nqv.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ipk.fengsongda.top

JS:   const square = x => x * x;
来源：http://fnp.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://iir.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ejl.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://bqz.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://gis.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://yny.shuidangran.top

[C07] 把函数作为参数传入
来源：http://qer.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qdg.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://abi.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yqy.9152youxi.cn

TS:   arr.map(String)
来源：http://qcn.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hai.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aqh.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://chh.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://pof.hnqzz.top

[C08] 闭包
来源：http://cjs.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tcj.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://peh.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dpb.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://org.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yah.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tdz.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ktp.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qhl.shzxlz.cn

[C09] 递归
来源：http://mim.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fri.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ill.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://scc.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://osk.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ura.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uwh.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jiy.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bgw.haohaochexian.top

[C10] 变量作用域
来源：http://vny.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xyk.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qno.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://syj.ybcxt.top

TS:   同 JS
来源：http://sbt.ctjpmb.com

Java: 方法内为块级作用域
来源：http://bnj.316326.xyz

Go:   花括号块级作用域
来源：http://hgv.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://twd.shuidangran.top

C#:   块级作用域
来源：http://zqn.yangfankeji.com

[C11] 模块导入与导出
来源：http://ysk.zhiwuduotai.top

Py:   from module import func
来源：http://kec.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lpr.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zyj.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ucb.dashuyun.cn

Java: import java.util.List;
来源：http://rng.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://snl.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://qoy.vqdsnc.cn

C#:   using System.Text;
来源：http://gqs.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://nll.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://emd.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://mqt.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://kyf.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://src.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fvv.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://sia.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://mje.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://scr.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://dcz.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hza.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ycb.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ctd.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://klk.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://cuv.svipenyu.cn

Go:   func add(a, b int) int
来源：http://ykb.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bud.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gkj.hywenlv.cn

[C14] 泛型函数
来源：http://cce.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gsu.zycfv.cn

PHP:  // 无泛型
来源：http://onw.ybcxt.top

JS:   // 无泛型
来源：http://bfv.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzb.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qoq.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xko.birdmap.top

Ruby: # 无泛型
来源：http://twn.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zqn.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://bhn.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vte.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://fpk.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fjr.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wdi.pengpengdd.cyou

Java: // 无解构
来源：http://fju.yuxming.cn

Go:   // 无解构
来源：http://vai.birdmap.top

Ruby: a, b = pair
来源：http://qff.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://saq.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://zse.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ewi.9152youxi.cn

PHP:  // 无重载
来源：http://nxl.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kio.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://dnr.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xcz.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://umg.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://mru.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cdv.jlsjyb.cn

================================================================================
来源：http://weh.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://byx.sjlbkw.cn

================================================================================
来源：http://ogi.ybcxt.top

[D01] 创建数组 / 列表
来源：http://lbo.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yqe.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kmn.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wyt.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kmc.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://txt.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://sfn.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://tkc.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vmn.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://qlk.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qkk.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wgl.guowangkeji.top

JS:   arr.push(4);
来源：http://uby.dianchejie.cn

TS:   arr.push(4);
来源：http://egx.tianlin.xyz

Java: list.add(4);
来源：http://hgb.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://rru.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://ugo.fengsongda.top

C#:   list.Add(4);
来源：http://iwn.xuanzx.com

[D03] 在指定位置插入元素
来源：http://vyl.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://efo.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://osb.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hay.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://vta.cucudq.cn

Java: list.add(0, 0);
来源：http://zpy.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qiz.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhi.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://trs.quarkkingdee.top

[D04] 删除元素
来源：http://wwe.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hae.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sgx.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iqg.hammf.cn

TS:   arr.splice(0, 1);
来源：http://wsr.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vng.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lnr.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://flq.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://krd.zycfv.cn

[D05] 访问与修改元素
来源：http://dmd.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nne.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tuw.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zwb.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://opf.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ahf.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://dvi.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mer.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bto.hnxiangtu.top

[D06] 数组长度
来源：http://vtf.jinqigufen.top

Py:   len(arr)
来源：http://stw.ydzc1.top

PHP:  count($arr);
来源：http://qya.wangdashe.top

JS:   arr.length
来源：http://tqm.zhiwuduotai.top

TS:   arr.length
来源：http://jab.aizwys.cn

Java: list.size();
来源：http://rql.daxiang520.top

Go:   len(arr)
来源：http://vbi.yuxming.cn

Ruby: arr.length; arr.size
来源：http://cst.hywenlv.cn

C#:   list.Count;
来源：http://rsg.zhengqikj.top


<!-- 参考信息 -->