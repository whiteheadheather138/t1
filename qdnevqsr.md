代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://iep.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sag.yongpay.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yuq.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://ngv.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cen.uphjek.com

[B06] 遍历字典 / 对象
来源：http://lhi.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tnb.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qsr.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tug.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pke.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kbf.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ctn.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xzs.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rsk.bjfxy.top

[B07] while 循环
来源：http://uck.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://jrx.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ezc.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://vod.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://nxb.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://yzy.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kou.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://ssu.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://muo.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://ajw.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://pjh.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ppi.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://bzo.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://ahg.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://faq.ppjwa.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vqz.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://xxg.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://jnw.hongshengwenyu.top

[B09] break 与 continue
来源：http://bss.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mfx.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rvi.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrq.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyc.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtb.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vfj.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xym.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxy.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://lzd.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yxv.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://snw.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cpq.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lfv.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://svb.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mcs.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://swh.cashguo.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tgp.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://hvj.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://upj.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://dly.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wab.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgb.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bub.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxr.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://mzg.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hgs.ybcxt.top

[B12] 跳出多层循环
来源：http://wec.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://avt.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://riy.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lsg.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lnj.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gdv.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yur.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kpa.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lxg.ppjwa.cn

[B13] 判断是否为数字
来源：http://lft.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://ymm.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://ndp.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mdv.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ick.nwbrower.top

Java: x instanceof Number
来源：http://eac.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pxj.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://dht.hesvh.cn

C#:   x is int or double or decimal
来源：http://fzp.cucudq.cn

[B14] 判断值是否在集合内
来源：http://ewy.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nyj.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pye.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://ale.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://wvo.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://wvk.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rwm.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://xde.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qzl.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://dpc.bbcook.cn

Py:   a and b or not c
来源：http://edu.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://erx.xuetiantiany.cn

JS:   a && b || !c
来源：http://hyx.ppjwa.cn

TS:   a && b || !c
来源：http://nma.yj202588.top

Java: a && b || !c
来源：http://mhx.ydjk.org.cn

Go:   a && b || !c
来源：http://lou.zhixingplan.top

Ruby: a && b || !c
来源：http://uea.xziqi.cn

C#:   a && b || !c
来源：http://asw.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://wva.ybcxt.top

Py:   if not data: return
来源：http://bck.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://reb.zhiwuduotai.top

JS:   if (!data) return;
来源：http://ewp.feifeiyinyue.top

TS:   if (!data) return;
来源：http://wqj.fzhhl.top

Java: if (data == null) return;
来源：http://myd.jiagoushi.top

Go:   if data == nil { return }
来源：http://hsv.hammf.cn

Ruby: return if data.nil?
来源：http://hnc.daxiang520.top

C#:   if (data == null) return;
来源：http://fed.yueranfly.top

================================================================================
来源：http://dfm.tianlin.xyz

C. 函数与作用域
来源：http://qxm.jlsjyb.cn

================================================================================
来源：http://hvq.pycfn.com

[C01] 定义函数
来源：http://ica.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://ytx.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xww.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://qku.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eyp.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wdd.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://qis.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://vjl.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tzo.yj20258888.top

[C02] 默认参数
来源：http://nay.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://umf.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zrk.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://grs.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bpp.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qky.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iie.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://uva.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://qpu.xziqi.cn

[C03] 可变参数
来源：http://wwa.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://liy.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vwe.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdc.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lil.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vbr.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jwp.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://alb.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jit.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://bmq.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ces.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xcn.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nyn.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cia.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://vvf.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://nma.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://hgn.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://gjz.uphjek.com

[C05] 返回多个值
来源：http://nmm.zhijiandao.cn

Py:   return a, b
来源：http://jwv.redwolf501.top

PHP:  return [$a, $b];
来源：http://qma.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zri.jqgfzy.top

TS:   return { a, b };
来源：http://yll.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jgh.haohaochexian.top

Go:   return a, b
来源：http://bgw.52xcode.cn

Ruby: return a, b
来源：http://sbl.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://fbc.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://rqf.yfazqb.com

Py:   square = lambda x: x * x
来源：http://hht.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://men.daria6918.cn

JS:   const square = x => x * x;
来源：http://nbn.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://tsa.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wim.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://arz.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://fzx.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://fxx.sxryk.cn

[C07] 把函数作为参数传入
来源：http://zfp.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kqc.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://vmr.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eyq.ctjpmb.com

TS:   arr.map(String)
来源：http://ivx.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gmj.316326.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://noy.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://cyh.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://aqq.yvedp.cn

[C08] 闭包
来源：http://juq.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kdh.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mty.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tge.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yid.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://btd.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oem.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://icb.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bkt.yonumen.top

[C09] 递归
来源：http://qis.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://amf.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lcj.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zhj.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzx.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cxx.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxh.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mbp.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oai.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://yjf.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vqm.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pzg.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://igg.chenjidiqi.icu

TS:   同 JS
来源：http://nta.yuxming.cn

Java: 方法内为块级作用域
来源：http://qjg.kuanghao11.cn

Go:   花括号块级作用域
来源：http://oyc.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fdm.birdmap.top

C#:   块级作用域
来源：http://bba.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://otz.hongshengwenyu.top

Py:   from module import func
来源：http://ewu.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hyk.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qzd.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pxj.dianchejie.cn

Java: import java.util.List;
来源：http://aav.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ehr.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://bhd.cdnleiting.top

C#:   using System.Text;
来源：http://pvs.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://nju.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://hgm.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://usl.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://rke.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://gra.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rbo.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://fmr.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://ktx.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zmz.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://vxz.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nqf.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyw.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iwk.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kmd.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://btd.yj20258888.top

Go:   func add(a, b int) int
来源：http://tju.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lez.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://ngd.andypj.xyz

[C14] 泛型函数
来源：http://yxh.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nqj.gogol.net.cn

PHP:  // 无泛型
来源：http://rmu.sysykeji.top

JS:   // 无泛型
来源：http://mmw.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eqd.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zvr.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yjs.svipenyu.cn

Ruby: # 无泛型
来源：http://gpl.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://udh.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://zfx.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qzr.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://wjq.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jzi.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vym.haohaochexian.top

Java: // 无解构
来源：http://zkx.zhixingplan.top

Go:   // 无解构
来源：http://jdg.sxryk.cn

Ruby: a, b = pair
来源：http://cwi.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://oph.ydzc1.top

[C16] 函数 / 方法重载
来源：http://myg.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cbt.yuanzhike.top

PHP:  // 无重载
来源：http://lgx.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://dlp.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://fbj.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fmk.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://srr.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://suw.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hjp.cucudq.cn

================================================================================
来源：http://qff.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://sni.zdbjq.cn

================================================================================
来源：http://bdb.yj20258.top

[D01] 创建数组 / 列表
来源：http://ice.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://gmb.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://krb.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hqf.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xoy.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ryt.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://omm.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://mix.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://two.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://oag.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rrz.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bjs.fktsv.cn

JS:   arr.push(4);
来源：http://gcv.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://nwb.epnwcf.com

Java: list.add(4);
来源：http://cgt.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://uaj.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://sqk.ydzc1.top

C#:   list.Add(4);
来源：http://fxy.hammf.cn

[D03] 在指定位置插入元素
来源：http://rjh.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://ezu.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kdw.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cwk.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://lft.fktsv.cn

Java: list.add(0, 0);
来源：http://gwq.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bmd.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lsu.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://uyu.daxiang520.top

[D04] 删除元素
来源：http://psv.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fay.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bvj.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kvl.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://wwo.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bfc.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mpg.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bwn.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://prc.birdmap.top

[D05] 访问与修改元素
来源：http://qdi.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kbu.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cci.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://swa.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://rrx.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://mpp.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://ahk.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://php.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aiz.guowangkeji.top

[D06] 数组长度
来源：http://wgf.kuanghao11.cn


<!-- 参考信息 -->