代发 wailian999

Py:   for i in range(10): print(i)
来源：http://ukq.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eva.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eta.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://unq.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bsg.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dfd.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://qwl.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ums.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://wdb.pycfn.com

Py:   for item in arr: print(item)
来源：http://qyk.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iez.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vua.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hwq.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dum.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://czi.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://soe.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://czy.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://cge.hfpthk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vwm.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rmb.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ldv.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvv.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lyk.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eql.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iaf.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dnm.wangdashe.top

[B07] while 循环
来源：http://jna.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://ukn.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://tav.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://cyh.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://xwv.yonumen.top

Java: while (i < 10) { i++; }
来源：http://cjp.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eoq.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://zyw.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://gdx.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://ole.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://hvi.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zcy.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://myo.zdbjq.cn

TS:   do { i++; } while (i < 10);
来源：http://lzt.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://vbb.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mjp.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://lyj.sjlbkw.cn

C#:   do { i++; } while (i < 10);
来源：http://rrm.fehbvm.com

[B09] break 与 continue
来源：http://opg.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pns.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zhu.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxr.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvy.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehh.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://frf.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aiy.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgu.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://ger.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yfj.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qyd.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eoo.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nxx.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bhi.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ujh.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ywt.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ehq.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://fwn.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://meh.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://mna.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsv.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://twp.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lkm.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hkm.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://yee.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hhu.yj20258888.top

[B12] 跳出多层循环
来源：http://afg.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oxa.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://npl.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jtx.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gme.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kxs.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tav.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ekj.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oae.c1oappe.top

[B13] 判断是否为数字
来源：http://rni.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://kxh.haohaochexian.top

PHP:  is_numeric($x)
来源：http://qhv.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fur.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqp.daria6918.cn

Java: x instanceof Number
来源：http://abp.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxv.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://xlu.yueranfly.top

C#:   x is int or double or decimal
来源：http://luv.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://aww.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hcy.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iqh.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://cyo.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://xeq.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jnx.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xlo.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://lih.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ddb.chenlongwang.top

[B15] 布尔运算与取反
来源：http://yfh.ydjk.org.cn

Py:   a and b or not c
来源：http://lca.cucudq.cn

PHP:  $a && $b || !$c
来源：http://wwe.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://wqy.hnxiangtu.top

TS:   a && b || !c
来源：http://ujf.pycfn.com

Java: a && b || !c
来源：http://aop.vqdsnc.cn

Go:   a && b || !c
来源：http://ind.nwbrower.top

Ruby: a && b || !c
来源：http://rhd.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://wzr.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://kuw.smart0.xyz

Py:   if not data: return
来源：http://slm.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://dgk.xinyue.icu

JS:   if (!data) return;
来源：http://fye.xylfe.cn

TS:   if (!data) return;
来源：http://trv.cheryme.top

Java: if (data == null) return;
来源：http://erj.xinyue.icu

Go:   if data == nil { return }
来源：http://wwj.shuidangran.top

Ruby: return if data.nil?
来源：http://crt.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://lgf.jlsjyb.cn

================================================================================
来源：http://zdt.ywan-chungtsiang.top

C. 函数与作用域
来源：http://qvj.yfazqb.com

================================================================================
来源：http://ovr.tianlin.xyz

[C01] 定义函数
来源：http://nnc.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://ygy.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qpp.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://xkt.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://epz.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oov.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hku.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://kpe.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cax.shuidangran.top

[C02] 默认参数
来源：http://rtg.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://nlg.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://awe.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://ogi.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uta.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://odx.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yel.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://ujv.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://cni.hnxiangtu.top

[C03] 可变参数
来源：http://fyb.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://eph.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tpp.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://coy.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hix.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ufh.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://anr.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://rys.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qrk.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://umj.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wyq.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sfa.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wjr.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xdp.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://xnh.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://gax.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://pxa.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://ina.haohaochexian.top

[C05] 返回多个值
来源：http://wbp.aizwys.cn

Py:   return a, b
来源：http://vhl.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://yfd.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tlh.kuanghao11.cn

TS:   return { a, b };
来源：http://rrb.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://psz.hammf.cn

Go:   return a, b
来源：http://wwl.52xcode.cn

Ruby: return a, b
来源：http://yga.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://zpo.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://ffi.smart0.xyz

Py:   square = lambda x: x * x
来源：http://tdv.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rlw.zhengqikj.top

JS:   const square = x => x * x;
来源：http://qyy.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://cpx.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xbn.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://pev.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://llx.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://xfn.fktsv.cn

[C07] 把函数作为参数传入
来源：http://jug.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fyn.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://rjx.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dth.hnxiangtu.top

TS:   arr.map(String)
来源：http://twi.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rpn.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yqp.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://wid.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://cpd.yuxming.cn

[C08] 闭包
来源：http://dvz.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fxa.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yuw.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mbk.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ppf.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hgo.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ezf.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qli.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ipz.redwolf501.top

[C09] 递归
来源：http://iqj.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bbc.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tha.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gfl.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgn.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zji.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nbz.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://snj.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fch.yj20258888.top

[C10] 变量作用域
来源：http://aeb.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zmv.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pyt.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zoy.yfazqb.com

TS:   同 JS
来源：http://cjo.yueranfly.top

Java: 方法内为块级作用域
来源：http://ief.cqqwz.cn

Go:   花括号块级作用域
来源：http://guh.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://euq.hcnkem.com

C#:   块级作用域
来源：http://cuh.nwbrower.top

[C11] 模块导入与导出
来源：http://jpp.svipenyu.cn

Py:   from module import func
来源：http://ohn.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dlx.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oct.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zdb.guannengcc.top

Java: import java.util.List;
来源：http://zvn.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aua.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://iiy.fzhhl.top

C#:   using System.Text;
来源：http://ejw.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://dwa.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://igg.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://yks.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://kke.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://ycb.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ixs.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://tul.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://reg.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ehl.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://eks.dashuyun.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fwj.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evz.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://idu.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqf.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://grj.shzxlz.cn

Go:   func add(a, b int) int
来源：http://fnq.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lkp.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dyn.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://kex.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qma.jqgfzy.top

PHP:  // 无泛型
来源：http://uph.uphjek.com

JS:   // 无泛型
来源：http://pao.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lps.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bcu.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nav.daxiang520.top

Ruby: # 无泛型
来源：http://znq.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iyj.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://ecl.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qej.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://qwb.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ihr.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://amx.zhixingplan.top

Java: // 无解构
来源：http://wub.tanke756.top

Go:   // 无解构
来源：http://dga.smart0.xyz

Ruby: a, b = pair
来源：http://wfp.epnwcf.com

C#:   var (a, b) = pair;
来源：http://mvk.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://pau.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fup.kuanghao11.cn

PHP:  // 无重载
来源：http://xrl.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vne.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://adf.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dxp.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://fxl.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://jkh.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://toj.cdnleiting.top

================================================================================
来源：http://wof.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://lgf.vqdsnc.cn

================================================================================
来源：http://orl.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://fku.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bvi.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uox.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tsm.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://axv.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wov.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://how.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://uhd.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gev.fzhhl.top

[D02] 追加元素到末尾
来源：http://uwm.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qin.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qkb.zhixingplan.top

JS:   arr.push(4);
来源：http://hkf.hongshengwenyu.top

TS:   arr.push(4);
来源：http://lsr.gotoacloud.top

Java: list.add(4);
来源：http://oaq.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://fay.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://gmr.sweek.top

C#:   list.Add(4);
来源：http://wnx.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://zym.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://vms.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://niz.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gth.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://piu.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://jvl.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://orb.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hik.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://tzj.hcnkem.com

[D04] 删除元素
来源：http://mzn.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tbm.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kou.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nyy.yongpay.top

TS:   arr.splice(0, 1);
来源：http://aeg.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nrg.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cfd.zhaomingkeji.xyz


<!-- 参考信息 -->