代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lfx.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hgf.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://den.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jth.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://prs.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://bef.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yos.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mpt.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yyv.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ewq.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yrd.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://tzn.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://woq.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://irg.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://neg.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://usi.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fvl.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ess.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ndf.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hrh.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://atb.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mxc.havefunace.top

[B07] while 循环
来源：http://kbt.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://ryc.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ucb.chenjidiqi.icu

JS:   while (i < 10) { i++; }
来源：http://kfi.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://awg.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://mmm.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zdc.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://tqj.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://uys.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://sgi.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://kjq.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://spj.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://eqq.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://eom.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://vkt.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bni.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://gma.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://gez.vqdsnc.cn

[B09] break 与 continue
来源：http://nkh.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cnh.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ihw.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nta.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wuk.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itf.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://geo.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://enw.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ikh.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://jwf.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oiu.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mof.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lmi.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jaw.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gno.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zpn.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qts.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mex.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://vqx.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://inm.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://oet.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vhg.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vdy.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hca.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mzx.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://iut.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jmx.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://yux.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ier.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tpv.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fib.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cbw.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ube.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bvf.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ccr.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lim.sysykeji.top

[B13] 判断是否为数字
来源：http://ztu.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://tzl.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://nop.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vic.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikn.shzxlz.cn

Java: x instanceof Number
来源：http://byi.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://quw.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://aev.cashguo.top

C#:   x is int or double or decimal
来源：http://gmn.mhx1999.top

[B14] 判断值是否在集合内
来源：http://fsq.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eee.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ypz.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://zds.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://gsl.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ale.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wys.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://dor.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wna.316326.xyz

[B15] 布尔运算与取反
来源：http://vcz.nanxuanxn.top

Py:   a and b or not c
来源：http://rum.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://krq.uphjek.com

JS:   a && b || !c
来源：http://snv.jlsjyb.cn

TS:   a && b || !c
来源：http://toi.daxiang520.top

Java: a && b || !c
来源：http://mso.mhx1999.top

Go:   a && b || !c
来源：http://qtm.hfpthk.cn

Ruby: a && b || !c
来源：http://uvp.zycfv.cn

C#:   a && b || !c
来源：http://ean.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://sqd.yfazqb.com

Py:   if not data: return
来源：http://ciz.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://npk.tianlin.xyz

JS:   if (!data) return;
来源：http://kjl.sweek.top

TS:   if (!data) return;
来源：http://oli.ehwqpu.com

Java: if (data == null) return;
来源：http://whh.nwbrower.top

Go:   if data == nil { return }
来源：http://pvm.cheryme.top

Ruby: return if data.nil?
来源：http://exp.vqdsnc.cn

C#:   if (data == null) return;
来源：http://zqs.ywan-chungtsiang.top

================================================================================
来源：http://rnb.aibaodan.cn

C. 函数与作用域
来源：http://mjr.haohaochexian.top

================================================================================
来源：http://xop.fehbvm.com

[C01] 定义函数
来源：http://agq.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://duz.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bcd.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://muw.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ryz.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wrt.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://gmq.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://wrd.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nno.yj202588.top

[C02] 默认参数
来源：http://xhv.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://yvx.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aoo.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://zyk.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://agt.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nlj.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cka.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://tkk.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://yvy.jianghu66.top

[C03] 可变参数
来源：http://ijg.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://ycf.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://prj.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lch.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zki.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rdr.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ych.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gjp.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://clt.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://hcq.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xvf.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://diz.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ryq.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qnu.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://crr.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://teo.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://ejf.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://jop.feifeiyinyue.top

[C05] 返回多个值
来源：http://euv.zhongyouzk.top

Py:   return a, b
来源：http://tsw.ehwqpu.com

PHP:  return [$a, $b];
来源：http://ofh.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jid.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://lle.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qtx.hesvh.cn

Go:   return a, b
来源：http://ims.dashuyun.cn

Ruby: return a, b
来源：http://keo.hcnkem.com

C#:   return (a, b);              // ValueTuple
来源：http://ywn.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://pwt.shuidangran.top

Py:   square = lambda x: x * x
来源：http://fqz.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ejf.zhixingplan.top

JS:   const square = x => x * x;
来源：http://qbk.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://lns.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://faf.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://ufw.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://xqb.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://dns.sxryk.cn

[C07] 把函数作为参数传入
来源：http://vch.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nqe.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pyr.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://glz.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://jvr.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gvc.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://awr.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://ram.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rdu.9152youxi.cn

[C08] 闭包
来源：http://lql.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://acj.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zqd.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wec.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gmg.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wlm.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ral.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bqa.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vpy.zhijiandao.cn

[C09] 递归
来源：http://afe.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xhc.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tre.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://psy.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpx.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jaj.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://her.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://efp.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vlc.nanxinkj.top

[C10] 变量作用域
来源：http://ifk.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nrj.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ovd.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wse.fzhhl.top

TS:   同 JS
来源：http://ouj.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://yut.yanxiufei.cn

Go:   花括号块级作用域
来源：http://dxh.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://juy.yuanzhike.top

C#:   块级作用域
来源：http://jlv.vqdsnc.cn

[C11] 模块导入与导出
来源：http://xyl.gaohongyu789.top

Py:   from module import func
来源：http://xto.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://brf.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hhb.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zum.hnxiangtu.top

Java: import java.util.List;
来源：http://kax.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mii.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://yta.gzhubu.top

C#:   using System.Text;
来源：http://xma.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://ahf.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://qqx.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://kiq.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://oia.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://ulc.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hrf.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://tvk.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://gja.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://gab.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://doq.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://win.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ucb.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ggw.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yai.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://slj.nanxinkj.top

Go:   func add(a, b int) int
来源：http://xhj.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wdq.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jij.gogol.net.cn

[C14] 泛型函数
来源：http://rps.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pzb.ctjpmb.com

PHP:  // 无泛型
来源：http://btm.zdqjudy.top

JS:   // 无泛型
来源：http://axr.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://quc.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kzv.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kpu.fzhhl.top

Ruby: # 无泛型
来源：http://iha.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ljm.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://qli.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jby.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://sbg.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://enq.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ypy.ywan-chungtsiang.top

Java: // 无解构
来源：http://tay.iojbl.cn

Go:   // 无解构
来源：http://tdb.iojbl.cn

Ruby: a, b = pair
来源：http://mik.andypj.xyz

C#:   var (a, b) = pair;
来源：http://glt.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://yha.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rka.cheryme.top

PHP:  // 无重载
来源：http://mum.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mrg.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://sze.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xkl.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://mff.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://kvd.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbd.daria6918.cn

================================================================================
来源：http://jwy.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://jqd.tianlin.xyz

================================================================================
来源：http://sxd.epnwcf.com

[D01] 创建数组 / 列表
来源：http://nds.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://fbo.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qlz.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pvi.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://cpn.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gpl.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://hpd.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://dsv.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fne.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://ywp.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nlz.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tzg.uphjek.com

JS:   arr.push(4);
来源：http://owj.yj20258.top

TS:   arr.push(4);
来源：http://yip.vehdjk.com

Java: list.add(4);
来源：http://gmi.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://dtu.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://fmo.sjlbkw.cn

C#:   list.Add(4);
来源：http://gjh.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://aiq.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://tuu.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qcm.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fka.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://uje.jinqigufen.top

Java: list.add(0, 0);
来源：http://wqg.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://rdg.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uhq.ivvv.top

C#:   list.Insert(0, 0);
来源：http://jfm.guannengcc.top

[D04] 删除元素
来源：http://rsl.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tog.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jyu.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kgg.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://zuy.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hpn.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wdl.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iuh.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://swn.wangdashe.top

[D05] 访问与修改元素
来源：http://cgb.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpv.dianchejie.cn


<!-- 参考信息 -->