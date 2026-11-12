代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://irm.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mkh.ydzc1.top

[B07] while 循环
来源：http://bos.epnwcf.com

Py:   while i < 10: i += 1
来源：http://vlv.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://shi.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://kqg.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://grq.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://oba.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hcm.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://cyj.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://ahw.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://qyj.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://gbq.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kqa.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://irr.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://qxd.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://kof.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://osu.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://lik.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://lal.guowangkeji.top

[B09] break 与 continue
来源：http://coa.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lkt.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gdr.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmw.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwf.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eti.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://luu.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jnx.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tos.aizwys.cn

[B10] 遍历同时拿索引
来源：http://faa.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awu.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vpa.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ufy.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sjq.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jle.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hmj.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ijk.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xbk.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://yys.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://jpg.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://nvm.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nth.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gfn.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kxs.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kvm.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://opf.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oln.sysykeji.top

[B12] 跳出多层循环
来源：http://lps.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://iiz.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fcm.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pkb.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vrq.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qmc.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://agu.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hpn.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lcy.c1oappe.top

[B13] 判断是否为数字
来源：http://xbx.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://soe.hcnkem.com

PHP:  is_numeric($x)
来源：http://djs.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yzp.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cpt.jinghuilouyu.cn

Java: x instanceof Number
来源：http://omd.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lfo.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://cqg.zdqjudy.top

C#:   x is int or double or decimal
来源：http://ydv.xuanzx.com

[B14] 判断值是否在集合内
来源：http://gkv.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fvu.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sfm.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://hdl.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://jmh.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sbl.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jyp.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://bxd.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tqp.zdbjq.cn

[B15] 布尔运算与取反
来源：http://jpj.snrcjt.cn

Py:   a and b or not c
来源：http://szc.zycfv.cn

PHP:  $a && $b || !$c
来源：http://gyw.wangdashe.top

JS:   a && b || !c
来源：http://gch.dianchejie.cn

TS:   a && b || !c
来源：http://arz.jqgufenzy.top

Java: a && b || !c
来源：http://nig.yj202588.top

Go:   a && b || !c
来源：http://gkl.zycfv.cn

Ruby: a && b || !c
来源：http://nmj.ppjwa.cn

C#:   a && b || !c
来源：http://nns.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://icw.shanyushiyangtech.top

Py:   if not data: return
来源：http://rxf.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://raz.cqqwz.cn

JS:   if (!data) return;
来源：http://olg.yonumen.top

TS:   if (!data) return;
来源：http://fwa.yuxming.cn

Java: if (data == null) return;
来源：http://jis.jinqigfzy.top

Go:   if data == nil { return }
来源：http://hue.yuxming.cn

Ruby: return if data.nil?
来源：http://eou.ppjwa.cn

C#:   if (data == null) return;
来源：http://uda.zhongyouzk.top

================================================================================
来源：http://tto.havefunace.top

C. 函数与作用域
来源：http://myp.tianlin.xyz

================================================================================
来源：http://jyo.dashuyun.cn

[C01] 定义函数
来源：http://dho.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://ifk.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://org.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://zkr.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rca.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://yuq.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bet.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://ath.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://amh.sufxvd.cn

[C02] 默认参数
来源：http://wmy.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://vdy.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ojw.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://mcw.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://edz.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dwz.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gps.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://dgv.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://tai.gaohongyu789.top

[C03] 可变参数
来源：http://hau.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://ggy.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nwu.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xal.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xmq.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zlj.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nmx.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://ytc.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kpv.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://vkg.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vqh.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qbc.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kax.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kia.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://utb.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://nov.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://adw.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://jqf.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://cma.dashuyun.cn

Py:   return a, b
来源：http://jxy.jinqigufen.top

PHP:  return [$a, $b];
来源：http://kgz.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://uek.ydzc1.top

TS:   return { a, b };
来源：http://cui.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eeh.shzxlz.cn

Go:   return a, b
来源：http://mbw.yj202588.top

Ruby: return a, b
来源：http://ohq.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://pji.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://cpk.xylfe.cn

Py:   square = lambda x: x * x
来源：http://pcu.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zxo.hesvh.cn

JS:   const square = x => x * x;
来源：http://tpe.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://rxk.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dnr.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uln.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://tje.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://mwr.vehdjk.com

[C07] 把函数作为参数传入
来源：http://wto.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dof.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://vvs.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rfp.jqgfzy.top

TS:   arr.map(String)
来源：http://pjl.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lkk.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cop.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://vsa.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rag.chenjidiqi.icu

[C08] 闭包
来源：http://vcd.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zyv.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://miu.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oxl.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kqh.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://usw.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dax.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qjf.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mdt.aibaodan.cn

[C09] 递归
来源：http://qok.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hrt.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rcz.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppq.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kil.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://edy.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://muv.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mci.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pig.jinqigufen.top

[C10] 变量作用域
来源：http://wzs.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hxk.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tvh.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nry.chenjidiqi.icu

TS:   同 JS
来源：http://rdc.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://rht.yuanzhike.top

Go:   花括号块级作用域
来源：http://imm.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ybd.chenjidiqi.icu

C#:   块级作用域
来源：http://isd.hfpthk.cn

[C11] 模块导入与导出
来源：http://siq.52xcode.cn

Py:   from module import func
来源：http://mht.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zey.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mml.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zez.ydzc1.top

Java: import java.util.List;
来源：http://ict.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gsf.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://llr.jiagoushi.top

C#:   using System.Text;
来源：http://htv.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://ehp.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://qzr.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://vrx.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://vyv.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://ybi.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vgu.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://bvb.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://mac.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ikk.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://xjl.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cue.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pll.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wao.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vhh.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iiy.yueranfly.top

Go:   func add(a, b int) int
来源：http://gbt.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tse.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://msr.hywenlv.cn

[C14] 泛型函数
来源：http://ugl.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zik.yanxiufei.cn

PHP:  // 无泛型
来源：http://azm.gaohongyu789.top

JS:   // 无泛型
来源：http://lnr.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pjb.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xvz.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://njm.fehbvm.com

Ruby: # 无泛型
来源：http://trs.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xbi.yj202588.top

[C15] 解构 / 展开参数
来源：http://guv.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jlb.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://jth.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zef.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jcv.ydzc1.top

Java: // 无解构
来源：http://oyi.aibaodan.cn

Go:   // 无解构
来源：http://wop.aibaodan.cn

Ruby: a, b = pair
来源：http://jru.tian-w.cn

C#:   var (a, b) = pair;
来源：http://zkq.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://wzc.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ptn.sweek.top

PHP:  // 无重载
来源：http://nmd.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://slw.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://zvx.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://hbb.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://gqe.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://epl.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qoo.sxryk.cn

================================================================================
来源：http://fdl.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://pfm.hnqzz.top

================================================================================
来源：http://hxm.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://fdg.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://sxp.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nkq.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eso.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wzq.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://deb.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://fpg.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://vhf.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://quh.chenzaomai.com

[D02] 追加元素到末尾
来源：http://qjq.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ptz.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://izk.wangshuangyany.cn

JS:   arr.push(4);
来源：http://rve.ctjpmb.com

TS:   arr.push(4);
来源：http://eni.zhoulong.xyz

Java: list.add(4);
来源：http://wwk.havefunace.top

Go:   arr = append(arr, 4)
来源：http://qbg.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://zua.gogol.net.cn

C#:   list.Add(4);
来源：http://evl.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://ooi.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://oms.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dkh.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vvv.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://aop.ydzc1.top

Java: list.add(0, 0);
来源：http://gof.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://ral.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pyg.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://wjp.zhoulong.xyz

[D04] 删除元素
来源：http://tfu.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ypw.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wjp.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gjq.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://pcb.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xad.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kzr.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hvt.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lhp.shuidangran.top

[D05] 访问与修改元素
来源：http://pqo.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hbu.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ekr.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wss.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://nsl.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://wfc.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://fnb.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://taa.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cqj.ppjwa.cn

[D06] 数组长度
来源：http://jhe.c1oappe.top

Py:   len(arr)
来源：http://vmi.yanxiufei.cn

PHP:  count($arr);
来源：http://szg.shanyushiyangkeji.top

JS:   arr.length
来源：http://kxy.yangfankeji.com

TS:   arr.length
来源：http://ppr.kuanghao11.cn

Java: list.size();
来源：http://wcn.cashguo.top

Go:   len(arr)
来源：http://pjb.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://zpc.chenjidiqi.icu

C#:   list.Count;
来源：http://rxf.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://ecd.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://epv.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://wzd.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://cuy.cheryme.top


<!-- 参考信息 -->