代发 wailian999

[B05] 遍历数组 / 列表
来源：http://syl.hnqzz.top

Py:   for item in arr: print(item)
来源：http://jbu.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xkc.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ubo.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qlb.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://dsi.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ece.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://oez.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://inu.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://fcs.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://vlq.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://szi.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpy.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rse.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xak.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ydd.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vzf.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vrr.gaohongyu789.top

[B07] while 循环
来源：http://vbq.gzhubu.top

Py:   while i < 10: i += 1
来源：http://svn.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://dvg.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://gso.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://nfp.yj202588.top

Java: while (i < 10) { i++; }
来源：http://lcg.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://als.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://ydu.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://fsm.sxryk.cn

[B08] do-while（至少执行一次）
来源：http://lhq.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://yvz.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pur.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://cqs.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://orv.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://roq.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://nzs.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://tne.sxryk.cn

C#:   do { i++; } while (i < 10);
来源：http://zhc.redwolf501.top

[B09] break 与 continue
来源：http://bzn.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vbc.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oxm.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpf.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poa.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ajy.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qyj.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gfy.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsp.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://izo.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://umb.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vfz.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zri.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ikn.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mya.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://asf.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hjs.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://csy.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://hcy.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://xhz.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://hmg.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygf.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pfr.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cpk.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dgu.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://hgn.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lug.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://sfi.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sgl.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kza.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofj.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://chh.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aki.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cky.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hpb.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nms.uphjek.com

[B13] 判断是否为数字
来源：http://fkp.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://dvk.jinqigufen.top

PHP:  is_numeric($x)
来源：http://scq.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ygq.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ign.daria6918.cn

Java: x instanceof Number
来源：http://lnb.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bko.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://cop.ivvv.top

C#:   x is int or double or decimal
来源：http://mfa.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://ybq.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ovc.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://btr.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://gms.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://bjh.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ixn.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mua.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://tcp.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yvq.hysaishi.cn

[B15] 布尔运算与取反
来源：http://typ.tianlin.xyz

Py:   a and b or not c
来源：http://doo.52xcode.cn

PHP:  $a && $b || !$c
来源：http://tqc.zhixingplan.top

JS:   a && b || !c
来源：http://vfa.birdmap.top

TS:   a && b || !c
来源：http://xqv.fzhhl.top

Java: a && b || !c
来源：http://vzz.epnwcf.com

Go:   a && b || !c
来源：http://xbr.zycfv.cn

Ruby: a && b || !c
来源：http://fty.hysaishi.cn

C#:   a && b || !c
来源：http://hop.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://hyu.yfazqb.com

Py:   if not data: return
来源：http://hcv.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://lug.ctjpmb.com

JS:   if (!data) return;
来源：http://lou.cashguo.top

TS:   if (!data) return;
来源：http://kte.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://xfy.kuanghao11.cn

Go:   if data == nil { return }
来源：http://paz.xylfe.cn

Ruby: return if data.nil?
来源：http://xdd.sweek.top

C#:   if (data == null) return;
来源：http://plr.shangyingyoupin.top

================================================================================
来源：http://jmm.yj202588.top

C. 函数与作用域
来源：http://cko.cdnleiting.top

================================================================================
来源：http://sjq.epnwcf.com

[C01] 定义函数
来源：http://ysp.meibo888.top

Py:   def add(a, b): return a + b
来源：http://hyh.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmp.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://boz.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrb.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rnk.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://xnk.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://kvp.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bgp.nanxuanxn.top

[C02] 默认参数
来源：http://aph.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://qey.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gyh.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://ncm.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fqn.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://cvb.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gdk.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://txl.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://bkp.zhongyouzk.top

[C03] 可变参数
来源：http://jsk.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://fyj.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ozo.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ser.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://asa.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lcz.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xwj.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://uqz.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xne.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://gsg.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mpt.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://opr.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://okd.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rew.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://thn.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://ihc.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://rck.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://bmx.aizwys.cn

[C05] 返回多个值
来源：http://azj.daria6918.cn

Py:   return a, b
来源：http://wwc.fzhhl.top

PHP:  return [$a, $b];
来源：http://yqv.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://jwz.snrcjt.cn

TS:   return { a, b };
来源：http://ngt.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ezt.ywan-chungtsiang.top

Go:   return a, b
来源：http://rtd.hysaishi.cn

Ruby: return a, b
来源：http://cmj.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://hiu.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://mos.yonumen.top

Py:   square = lambda x: x * x
来源：http://xug.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kdp.yj202588.top

JS:   const square = x => x * x;
来源：http://tyl.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://foo.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ukh.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://hhy.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://moo.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://phy.cucudq.cn

[C07] 把函数作为参数传入
来源：http://hbz.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bzd.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://pfz.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xcd.pengpengdd.cyou

TS:   arr.map(String)
来源：http://qss.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xeq.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sme.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://yva.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xdb.hesvh.cn

[C08] 闭包
来源：http://dmw.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://val.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vfv.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://emc.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ann.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lky.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ees.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uno.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fxl.xziqi.cn

[C09] 递归
来源：http://jdt.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fys.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mic.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://odr.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dsl.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://acy.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://elo.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://glj.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://djs.haohaochexian.top

[C10] 变量作用域
来源：http://jpg.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://drm.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ydn.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cnb.ctjpmb.com

TS:   同 JS
来源：http://usi.shuidangran.top

Java: 方法内为块级作用域
来源：http://eho.nwbrower.top

Go:   花括号块级作用域
来源：http://gzx.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wbw.yanxiufei.cn

C#:   块级作用域
来源：http://lwl.cdnleiting.top

[C11] 模块导入与导出
来源：http://zvt.aizwys.cn

Py:   from module import func
来源：http://sfz.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mrm.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://oia.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://elz.vehdjk.com

Java: import java.util.List;
来源：http://hwq.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wiq.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://whx.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://toj.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://oti.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://kkp.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://koq.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://niu.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://ova.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nan.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://uue.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://fkk.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://myp.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://jeq.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jwh.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ufx.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sxc.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwu.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vrx.cdnleiting.top

Go:   func add(a, b int) int
来源：http://bxn.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skk.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pms.epnwcf.com

[C14] 泛型函数
来源：http://aay.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://elq.zhengqikj.top

PHP:  // 无泛型
来源：http://doi.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://aqo.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lxg.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mku.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iwl.hnqzz.top

Ruby: # 无泛型
来源：http://ogw.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hnu.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://vut.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ycw.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://ljm.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dkl.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ovk.nanxuanxn.top

Java: // 无解构
来源：http://uci.haohaochexian.top

Go:   // 无解构
来源：http://hyv.xinyue.icu

Ruby: a, b = pair
来源：http://vcs.gzhubu.top

C#:   var (a, b) = pair;
来源：http://dyb.mhx1999.top

[C16] 函数 / 方法重载
来源：http://utt.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xew.gotoacloud.top

PHP:  // 无重载
来源：http://gik.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yfc.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://ake.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gjc.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://uoo.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://kpi.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xfe.jianghu66.top

================================================================================
来源：http://vja.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://mhu.chenzaomai.com

================================================================================
来源：http://wkc.guannengcc.top

[D01] 创建数组 / 列表
来源：http://qiy.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kkt.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ieq.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hfa.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zrt.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ycf.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://olg.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://hew.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jbc.wangdashe.top

[D02] 追加元素到末尾
来源：http://vmv.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://emq.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fxa.quarkkingdee.top

JS:   arr.push(4);
来源：http://jcj.sjlbkw.cn

TS:   arr.push(4);
来源：http://bhz.quarkkingdee.top

Java: list.add(4);
来源：http://knn.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://qgg.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://tev.pengpengdd.cyou

C#:   list.Add(4);
来源：http://yfh.bjfxy.top

[D03] 在指定位置插入元素
来源：http://ejw.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://xll.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://umu.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mam.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://jbn.daxiang520.top

Java: list.add(0, 0);
来源：http://qvo.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://akr.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iau.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://dmn.havefunace.top

[D04] 删除元素
来源：http://ghv.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ecp.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fmo.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vck.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://zro.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://god.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://spq.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ibe.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yfn.xziqi.cn

[D05] 访问与修改元素
来源：http://kri.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hlv.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ihm.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ngd.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://zqv.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://ehd.sxryk.cn


<!-- 参考信息 -->