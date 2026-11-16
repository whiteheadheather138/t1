代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://vdp.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://ofc.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://wxx.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://abt.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zik.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://yfe.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://qnd.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://kvn.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://tlh.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://smw.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://hcg.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://zlm.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://yzh.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zcm.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://kuj.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://lmd.chenlongwang.top

[B09] break 与 continue
来源：http://zde.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oye.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://paj.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsc.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjw.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmb.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aes.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vge.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drx.uphjek.com

[B10] 遍历同时拿索引
来源：http://rxd.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxm.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ewp.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rch.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vju.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://teu.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dww.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qsr.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xnz.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://npj.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://dui.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://xou.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ify.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvq.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fnr.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ofx.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://wrd.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ghs.hysaishi.cn

[B12] 跳出多层循环
来源：http://sdq.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://gjx.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bju.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gfa.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wge.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lgk.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tcc.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nlq.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cbl.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://lla.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://sga.cashguo.top

PHP:  is_numeric($x)
来源：http://kte.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcv.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kcx.bbcook.cn

Java: x instanceof Number
来源：http://vqp.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lvr.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://bqh.sweek.top

C#:   x is int or double or decimal
来源：http://oqc.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://lbi.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qvf.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aek.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://igb.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://tta.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://olt.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mpb.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://dxg.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rcu.fengsongda.top

[B15] 布尔运算与取反
来源：http://flm.zhoulong.xyz

Py:   a and b or not c
来源：http://dgc.mhx1999.top

PHP:  $a && $b || !$c
来源：http://obi.jinghuilouyu.cn

JS:   a && b || !c
来源：http://khe.wangshuangyany.cn

TS:   a && b || !c
来源：http://gbh.shanyushiyangkeji.top

Java: a && b || !c
来源：http://pbs.yfazqb.com

Go:   a && b || !c
来源：http://rnl.ydjk.org.cn

Ruby: a && b || !c
来源：http://yno.jqgfzy.top

C#:   a && b || !c
来源：http://lmy.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tll.haohaochexian.top

Py:   if not data: return
来源：http://zmu.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://ozq.zhongyouzk.top

JS:   if (!data) return;
来源：http://vor.cucudq.cn

TS:   if (!data) return;
来源：http://fek.aibaodan.cn

Java: if (data == null) return;
来源：http://kxh.vehdjk.com

Go:   if data == nil { return }
来源：http://acb.jiagoushi.top

Ruby: return if data.nil?
来源：http://dgz.aibaodan.cn

C#:   if (data == null) return;
来源：http://zri.yvedp.cn

================================================================================
来源：http://mym.chenlongwang.top

C. 函数与作用域
来源：http://vpz.fengsongda.top

================================================================================
来源：http://qzh.fzhhl.top

[C01] 定义函数
来源：http://oso.sweek.top

Py:   def add(a, b): return a + b
来源：http://esg.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sbm.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://yhh.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://puj.cdnleiting.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hqa.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://evo.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://vuu.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pgt.hongshengwenyu.top

[C02] 默认参数
来源：http://hvz.havefunace.top

Py:   def greet(name="World"): return name
来源：http://fqr.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jhs.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://scu.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rpm.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://dbt.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zgk.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://otw.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://kqt.zdqjudy.top

[C03] 可变参数
来源：http://wmn.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://jzb.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uok.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qvk.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vad.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mwb.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://plp.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fbl.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vpb.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://wby.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ezs.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axu.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bdp.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ggw.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://bzl.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://cxe.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://xui.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://pmy.fzhhl.top

[C05] 返回多个值
来源：http://rmf.cdnleiting.top

Py:   return a, b
来源：http://gmw.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://fhv.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://idg.meibo888.top

TS:   return { a, b };
来源：http://kei.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sez.guannengcc.top

Go:   return a, b
来源：http://jgz.kuanghao11.cn

Ruby: return a, b
来源：http://lxa.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://krd.pycfn.com

[C06] 匿名函数 / lambda
来源：http://cgz.epnwcf.com

Py:   square = lambda x: x * x
来源：http://esk.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://bhk.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://zdp.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://zsm.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lmk.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://nrx.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://txw.ywan-chungtsiang.top

C#:   Func<int, int> square = x => x * x;
来源：http://sgq.guannengcc.top

[C07] 把函数作为参数传入
来源：http://soz.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gqv.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://lyj.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://opl.yanxiufei.cn

TS:   arr.map(String)
来源：http://jzb.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cdn.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tul.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://mtw.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bhu.cheryme.top

[C08] 闭包
来源：http://qqy.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wxb.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jpj.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qtf.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cmi.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gzf.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ibr.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qcl.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eqb.shzxlz.cn

[C09] 递归
来源：http://kwf.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sqd.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ffx.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://epg.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzj.cheryme.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ihk.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ytv.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xct.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zzg.chenjidiqi.icu

[C10] 变量作用域
来源：http://rbv.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zan.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://igh.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ydf.tian-w.cn

TS:   同 JS
来源：http://rcr.cheryme.top

Java: 方法内为块级作用域
来源：http://yxf.gzhubu.top

Go:   花括号块级作用域
来源：http://dkg.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nku.shanyushiyangkeji.top

C#:   块级作用域
来源：http://sfq.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://otd.cheryme.top

Py:   from module import func
来源：http://xlq.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wmy.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ysu.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kxm.zdbjq.cn

Java: import java.util.List;
来源：http://lzm.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hxk.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://fve.meibo888.top

C#:   using System.Text;
来源：http://dzj.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://wot.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://uru.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://dsz.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://tzk.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://dix.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://koe.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://lhb.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://kmr.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ygo.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://uya.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mcc.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpo.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wpe.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bns.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ynn.yueranfly.top

Go:   func add(a, b int) int
来源：http://qdk.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rxx.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://vkb.sxryk.cn

[C14] 泛型函数
来源：http://vql.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ayh.sweek.top

PHP:  // 无泛型
来源：http://gey.shzxlz.cn

JS:   // 无泛型
来源：http://nmf.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gja.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ofv.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lzj.gotoacloud.top

Ruby: # 无泛型
来源：http://lcu.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rzt.vehdjk.com

[C15] 解构 / 展开参数
来源：http://cxu.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zla.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://gno.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mdu.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vxw.havefunace.top

Java: // 无解构
来源：http://qfs.kuanghao11.cn

Go:   // 无解构
来源：http://lta.xuetiantiany.cn

Ruby: a, b = pair
来源：http://xaq.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://ojx.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://obv.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oja.yuanzhike.top

PHP:  // 无重载
来源：http://xoz.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nfp.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://xjf.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://dcd.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://ckh.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://wiv.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vup.tianlin.xyz

================================================================================
来源：http://pdp.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://pfi.yvedp.cn

================================================================================
来源：http://abh.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://yas.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wdv.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wur.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iut.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qfr.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lls.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://cei.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://qrt.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wge.fzhhl.top

[D02] 追加元素到末尾
来源：http://huh.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rax.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oij.bbcook.cn

JS:   arr.push(4);
来源：http://vkf.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://ygm.xylfe.cn

Java: list.add(4);
来源：http://iax.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://mof.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://ida.fehbvm.com

C#:   list.Add(4);
来源：http://bhy.cashguo.top

[D03] 在指定位置插入元素
来源：http://gtf.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://eha.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://maf.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rdj.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://yze.shuidangran.top

Java: list.add(0, 0);
来源：http://zco.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://nnh.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cna.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://lwm.yueranfly.top

[D04] 删除元素
来源：http://ugo.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qll.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lsa.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://omz.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://tzu.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://myq.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://znz.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pwo.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://alo.fehbvm.com

[D05] 访问与修改元素
来源：http://tgz.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rda.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xvc.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://weq.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://pwy.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://sbi.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://xmq.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ank.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://udz.0kj1m.cn

[D06] 数组长度
来源：http://fqu.hongshengwenyu.top

Py:   len(arr)
来源：http://ucy.jiagoushi.top

PHP:  count($arr);
来源：http://iuq.zdqjudy.top

JS:   arr.length
来源：http://sde.tarul.cn

TS:   arr.length
来源：http://frd.xingfuxueyuan.xyz

Java: list.size();
来源：http://ybx.yvedp.cn

Go:   len(arr)
来源：http://ynf.yuxming.cn

Ruby: arr.length; arr.size
来源：http://rkz.ywan-chungtsiang.top

C#:   list.Count;
来源：http://cfb.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://qnu.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xic.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hyh.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://ttw.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://mpz.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://ppu.ehwqpu.com

Go:   arr[1:4]
来源：http://jzj.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://vni.sufxvd.cn


<!-- 参考信息 -->