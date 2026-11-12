代发 wailian999

[B05] 遍历数组 / 列表
来源：http://lvs.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://zvm.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eyg.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iqo.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ymo.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://vbb.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wbp.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://jof.pycfn.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tkf.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://azc.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tfq.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://esw.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnf.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cgx.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ula.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iyt.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ssn.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lef.guowangkeji.top

[B07] while 循环
来源：http://lrs.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://gmk.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://kzk.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://sby.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://wqj.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://fid.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ddb.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://atd.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://uva.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://ryz.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://tls.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tdb.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://gjl.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://ucz.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://rqm.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hmi.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://das.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://dmo.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://vnb.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fbn.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sxy.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzd.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgj.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myk.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nax.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cyi.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwu.hcnkem.com

[B10] 遍历同时拿索引
来源：http://qzk.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tfd.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qbg.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nkf.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://krr.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nkj.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kwb.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lio.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mhu.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://kkx.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://url.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://tvx.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mnk.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cnv.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wpa.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://spk.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://tcf.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fwn.pycfn.com

[B12] 跳出多层循环
来源：http://nxd.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://oke.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nrh.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gci.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tyo.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ubu.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mdc.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lxh.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ymk.yuanzhike.top

[B13] 判断是否为数字
来源：http://tgf.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://itm.dianchejie.cn

PHP:  is_numeric($x)
来源：http://xtg.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ext.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvf.aizwys.cn

Java: x instanceof Number
来源：http://erl.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycj.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://cov.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://vch.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://ues.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wfv.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gbq.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://igg.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://gkq.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://kbz.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cqx.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://opt.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ddv.smart0.xyz

[B15] 布尔运算与取反
来源：http://zop.ehwqpu.com

Py:   a and b or not c
来源：http://nab.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://wli.ehwqpu.com

JS:   a && b || !c
来源：http://dvm.gogol.net.cn

TS:   a && b || !c
来源：http://qgo.yj202588.top

Java: a && b || !c
来源：http://jid.hfpthk.cn

Go:   a && b || !c
来源：http://nrx.meibo888.top

Ruby: a && b || !c
来源：http://ors.xinyue.icu

C#:   a && b || !c
来源：http://skq.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://rab.jyoumei.cn

Py:   if not data: return
来源：http://xvj.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://cfr.chenjidiqi.icu

JS:   if (!data) return;
来源：http://xsf.yj202588.top

TS:   if (!data) return;
来源：http://byl.gzhubu.top

Java: if (data == null) return;
来源：http://mmv.fzhhl.top

Go:   if data == nil { return }
来源：http://mhx.fengsongda.top

Ruby: return if data.nil?
来源：http://vff.aibaodan.cn

C#:   if (data == null) return;
来源：http://ohw.hnqzz.top

================================================================================
来源：http://wrd.jianghu66.top

C. 函数与作用域
来源：http://fqr.svipenyu.cn

================================================================================
来源：http://gdg.guannengcc.top

[C01] 定义函数
来源：http://via.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://vna.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vob.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://ukd.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zel.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fma.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://lkg.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://zwz.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://klm.xylfe.cn

[C02] 默认参数
来源：http://ujf.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://ayc.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dae.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://agk.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pel.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://idu.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cst.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://xuz.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://iif.iojbl.cn

[C03] 可变参数
来源：http://dlz.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://oiu.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://crx.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixz.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rqr.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ngm.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wcb.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://akk.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oxk.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://szy.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ioq.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gch.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qiv.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rnv.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://xwp.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://uhp.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://tuq.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://fao.sysykeji.top

[C05] 返回多个值
来源：http://wzi.aizwys.cn

Py:   return a, b
来源：http://vtk.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://jzt.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fwr.nanxinkj.top

TS:   return { a, b };
来源：http://cjx.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://izv.yangfankeji.com

Go:   return a, b
来源：http://ukn.hysaishi.cn

Ruby: return a, b
来源：http://guq.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ban.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://gfe.havefunace.top

Py:   square = lambda x: x * x
来源：http://jjt.cucudq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hcq.dianchejie.cn

JS:   const square = x => x * x;
来源：http://xkc.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://qvu.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://odt.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xub.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://sxv.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zxu.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://ljh.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vct.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://vmc.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://whi.tian-w.cn

TS:   arr.map(String)
来源：http://cmx.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lpn.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zgt.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://dgx.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jpr.9152youxi.cn

[C08] 闭包
来源：http://pdw.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rik.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dpx.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zlh.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ylz.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://neq.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://buf.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ttj.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jzq.jyoumei.cn

[C09] 递归
来源：http://rqh.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qss.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ufe.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://icn.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wmf.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hwo.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ffb.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzh.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qzk.ybcxt.top

[C10] 变量作用域
来源：http://hlf.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zby.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kan.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pjt.guowangkeji.top

TS:   同 JS
来源：http://mgm.jyoumei.cn

Java: 方法内为块级作用域
来源：http://qeo.redwolf501.top

Go:   花括号块级作用域
来源：http://spm.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://obw.cashguo.top

C#:   块级作用域
来源：http://tjr.jyoumei.cn

[C11] 模块导入与导出
来源：http://sgd.pycfn.com

Py:   from module import func
来源：http://csx.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jfb.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://exn.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ihn.c1oappe.top

Java: import java.util.List;
来源：http://frp.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fdb.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://zfs.tianlin.xyz

C#:   using System.Text;
来源：http://boy.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://ogh.yj20258.top

Py:   (lambda: print("run"))()
来源：http://xwg.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://orl.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://utz.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://wob.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jpg.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://qto.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://dlv.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tbr.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://esw.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ojv.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckd.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hfd.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fif.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://srj.havefunace.top

Go:   func add(a, b int) int
来源：http://rpx.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kqf.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://wmd.bbcook.cn

[C14] 泛型函数
来源：http://udu.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nxa.yueranfly.top

PHP:  // 无泛型
来源：http://vpp.yongpay.top

JS:   // 无泛型
来源：http://wyl.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tbn.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yns.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mxc.nanxuanxn.top

Ruby: # 无泛型
来源：http://zgu.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xev.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://lrh.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://njt.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://xoz.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fkb.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tmx.xingfuxueyuan.xyz

Java: // 无解构
来源：http://kgr.zhijiandao.cn

Go:   // 无解构
来源：http://bbs.sxryk.cn

Ruby: a, b = pair
来源：http://bbp.aizwys.cn

C#:   var (a, b) = pair;
来源：http://irq.yonumen.top

[C16] 函数 / 方法重载
来源：http://mhy.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fcv.sufxvd.cn

PHP:  // 无重载
来源：http://cqi.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://era.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://jrf.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ypf.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://jor.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://xha.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gjz.zycfv.cn

================================================================================
来源：http://klt.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://byh.kuanghao11.cn

================================================================================
来源：http://ohn.gzhubu.top

[D01] 创建数组 / 列表
来源：http://ucw.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ffo.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nzm.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jwl.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yfe.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://org.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://tww.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://hvx.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pac.chenlongwang.top

[D02] 追加元素到末尾
来源：http://xfd.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fhw.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wfh.yanxiufei.cn

JS:   arr.push(4);
来源：http://but.bbcook.cn

TS:   arr.push(4);
来源：http://zii.hywenlv.cn

Java: list.add(4);
来源：http://rlq.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://cwf.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://qlp.fzhhl.top

C#:   list.Add(4);
来源：http://rip.yj20258.top

[D03] 在指定位置插入元素
来源：http://lbj.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://sdb.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://frt.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pal.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://fpc.cashguo.top

Java: list.add(0, 0);
来源：http://zsk.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ifi.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://igt.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://vrr.redwolf501.top

[D04] 删除元素
来源：http://vmh.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cdt.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qwu.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnc.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://yqd.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gtl.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nlm.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lph.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vgg.svipenyu.cn

[D05] 访问与修改元素
来源：http://gls.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vnc.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bbj.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ggv.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://mls.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://uas.hongshengwenyu.top


<!-- 参考信息 -->