代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qkg.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wzf.xuetiantiany.cn

[B07] while 循环
来源：http://coe.jianghu66.top

Py:   while i < 10: i += 1
来源：http://rsg.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kba.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://zpa.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://gff.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://bsx.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://doq.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://aly.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://ixo.meibo888.top

[B08] do-while（至少执行一次）
来源：http://now.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://omx.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://spi.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://dit.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://vby.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://mzw.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gdp.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://ami.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://yip.yj202588.top

[B09] break 与 continue
来源：http://rdx.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rkv.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://plu.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycc.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpt.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpk.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eta.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xou.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uod.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://vcs.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bwl.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://llv.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qfy.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://njn.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jpl.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vmr.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vlz.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zej.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://ryj.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://vvj.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://fch.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bhg.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewp.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zsw.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ggt.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://wra.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iwx.ppjwa.cn

[B12] 跳出多层循环
来源：http://svt.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://atj.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eps.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jwo.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wqo.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://swc.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qzz.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uzi.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xaa.iojbl.cn

[B13] 判断是否为数字
来源：http://unv.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://pkw.ppjwa.cn

PHP:  is_numeric($x)
来源：http://mch.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hib.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oge.pycfn.com

Java: x instanceof Number
来源：http://gxl.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vbh.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://wgu.yj202588.top

C#:   x is int or double or decimal
来源：http://adk.hesvh.cn

[B14] 判断值是否在集合内
来源：http://lre.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eow.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qfg.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://ogy.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://fpx.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wkk.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fco.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gsd.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xmy.ppjwa.cn

[B15] 布尔运算与取反
来源：http://crt.yueranfly.top

Py:   a and b or not c
来源：http://rod.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://pgi.nwbrower.top

JS:   a && b || !c
来源：http://iqo.yfazqb.com

TS:   a && b || !c
来源：http://ahb.sufxvd.cn

Java: a && b || !c
来源：http://tin.tian-w.cn

Go:   a && b || !c
来源：http://epn.iojbl.cn

Ruby: a && b || !c
来源：http://crn.feifeiyinyue.top

C#:   a && b || !c
来源：http://qps.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://vya.yuanzhike.top

Py:   if not data: return
来源：http://scy.yongpay.top

PHP:  if (!$data) { return; }
来源：http://esa.ctjpmb.com

JS:   if (!data) return;
来源：http://xdi.yongpay.top

TS:   if (!data) return;
来源：http://ika.aibaodan.cn

Java: if (data == null) return;
来源：http://xlr.316326.xyz

Go:   if data == nil { return }
来源：http://sab.birdmap.top

Ruby: return if data.nil?
来源：http://psm.yuanzhike.top

C#:   if (data == null) return;
来源：http://qtl.chenlongwang.top

================================================================================
来源：http://oec.jianghu66.top

C. 函数与作用域
来源：http://ysr.hammf.cn

================================================================================
来源：http://nif.jqgfzy.top

[C01] 定义函数
来源：http://fpo.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://buu.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fnv.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://pga.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://feq.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sod.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yfa.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://rdd.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wrh.zdqjudy.top

[C02] 默认参数
来源：http://lfa.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://wja.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dqr.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ovx.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://sgl.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xfx.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wbj.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://yhu.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://quv.shanyushiyangkeji.top

[C03] 可变参数
来源：http://aps.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://ftt.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wpz.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://udv.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cjz.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ogf.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://efb.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://btn.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nvg.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://yzk.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rju.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rsl.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dki.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wpx.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://avo.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://dxm.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://rnk.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://wqa.yanxiufei.cn

[C05] 返回多个值
来源：http://avw.cqqwz.cn

Py:   return a, b
来源：http://ucj.dianchejie.cn

PHP:  return [$a, $b];
来源：http://tps.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rjt.yangfankeji.com

TS:   return { a, b };
来源：http://joy.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://phs.chenlongwang.top

Go:   return a, b
来源：http://ouh.dianchejie.cn

Ruby: return a, b
来源：http://acw.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://nsf.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://ndi.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://zid.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pxu.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://ukf.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://jiw.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ibc.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fcf.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://ubu.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uma.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://lnb.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dmo.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://dbv.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xlz.xziqi.cn

TS:   arr.map(String)
来源：http://wkz.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bhf.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lug.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://lpj.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lcz.hywenlv.cn

[C08] 闭包
来源：http://gdy.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://svu.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mzp.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bds.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oxk.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cne.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qtw.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ksu.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oil.yangfankeji.com

[C09] 递归
来源：http://kmg.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qly.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yku.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://isq.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lqd.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tbw.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mdp.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cwt.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mne.tian-w.cn

[C10] 变量作用域
来源：http://yso.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yip.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://piv.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dqa.bbcook.cn

TS:   同 JS
来源：http://umj.hysaishi.cn

Java: 方法内为块级作用域
来源：http://pif.316326.xyz

Go:   花括号块级作用域
来源：http://ewf.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iew.fzhhl.top

C#:   块级作用域
来源：http://xjw.daria6918.cn

[C11] 模块导入与导出
来源：http://gsn.ydjk.org.cn

Py:   from module import func
来源：http://dwv.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ndy.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pqq.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yix.pycfn.com

Java: import java.util.List;
来源：http://qsc.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yjc.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://ewi.yj202588.top

C#:   using System.Text;
来源：http://han.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://lfi.tarul.cn

Py:   (lambda: print("run"))()
来源：http://ykp.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://zuu.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://xmq.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://ayf.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vrp.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://eru.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://znp.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://byl.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://ofb.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lxd.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fkz.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://whk.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gps.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://kre.tanke756.top

Go:   func add(a, b int) int
来源：http://kbq.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://btr.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://kur.ivvv.top

[C14] 泛型函数
来源：http://fib.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://foy.chenjidiqi.icu

PHP:  // 无泛型
来源：http://vwn.xylfe.cn

JS:   // 无泛型
来源：http://blu.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://beb.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://loq.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://isy.havefunace.top

Ruby: # 无泛型
来源：http://kgk.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dqa.sysykeji.top

[C15] 解构 / 展开参数
来源：http://doi.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hdd.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://wxb.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jbg.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ftx.gaohongyu789.top

Java: // 无解构
来源：http://zqi.fanxiaobao.xyz

Go:   // 无解构
来源：http://rwh.feifeiyinyue.top

Ruby: a, b = pair
来源：http://lgn.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://mji.shuidangran.top

[C16] 函数 / 方法重载
来源：http://qmk.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nmu.haohaochexian.top

PHP:  // 无重载
来源：http://yid.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bgc.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://rcv.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jkh.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://kjn.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://xdh.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ztv.zhijiandao.cn

================================================================================
来源：http://uew.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://qze.aizwys.cn

================================================================================
来源：http://tec.yongpay.top

[D01] 创建数组 / 列表
来源：http://bdt.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://exn.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dmq.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hlb.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xwm.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cuk.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://zlr.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://mvi.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tjm.havefunace.top

[D02] 追加元素到末尾
来源：http://vtd.quarkkingdee.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vbg.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://abw.ivvv.top

JS:   arr.push(4);
来源：http://fay.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://snm.ivvv.top

Java: list.add(4);
来源：http://mor.yj20258.top

Go:   arr = append(arr, 4)
来源：http://hra.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://mhd.bbcook.cn

C#:   list.Add(4);
来源：http://yql.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://stu.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://owc.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://etm.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hmv.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://bwo.ybcxt.top

Java: list.add(0, 0);
来源：http://xtb.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://izr.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ntm.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://flo.aibaodan.cn

[D04] 删除元素
来源：http://fln.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qgx.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bax.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aie.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://jfk.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hzx.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rde.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gza.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hsw.pycfn.com

[D05] 访问与修改元素
来源：http://ejy.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zqd.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sfp.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gxn.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://udp.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://tyi.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://tiz.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fyh.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iuc.tianlin.xyz

[D06] 数组长度
来源：http://tht.cucudq.cn

Py:   len(arr)
来源：http://pwo.hnxiangtu.top

PHP:  count($arr);
来源：http://pqe.yongpay.top

JS:   arr.length
来源：http://fuc.pycfn.com

TS:   arr.length
来源：http://nwr.snrcjt.cn

Java: list.size();
来源：http://dps.jlsjyb.cn

Go:   len(arr)
来源：http://lfl.52xcode.cn

Ruby: arr.length; arr.size
来源：http://ham.pycfn.com

C#:   list.Count;
来源：http://fii.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://kgr.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://slc.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qec.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://rkv.fktsv.cn


<!-- 参考信息 -->