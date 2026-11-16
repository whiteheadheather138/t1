代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pjd.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://wby.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://hjf.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://tdt.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://eie.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hvq.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://wuw.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://aiz.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://ldn.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yhs.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pvy.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://kun.hammf.cn

[B09] break 与 continue
来源：http://hhh.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xju.xziqi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kto.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cog.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayz.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wby.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://abr.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jwk.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdj.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://jyf.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wjz.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ost.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xgx.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zxb.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dpy.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uzn.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://izc.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wkt.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://ebz.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://kxq.cheryme.top

PHP:  range(0, 10, 2);
来源：http://bff.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://spj.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wyf.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ylp.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dts.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://xer.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bku.jianghu66.top

[B12] 跳出多层循环
来源：http://voq.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bsj.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uku.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uqr.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vae.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://exe.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mmb.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wov.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cpe.fehbvm.com

[B13] 判断是否为数字
来源：http://cai.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://aik.andypj.xyz

PHP:  is_numeric($x)
来源：http://bbk.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://irg.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://okr.sxryk.cn

Java: x instanceof Number
来源：http://qnl.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sue.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://oau.iojbl.cn

C#:   x is int or double or decimal
来源：http://qbm.bjfxy.top

[B14] 判断值是否在集合内
来源：http://tdp.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ihu.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rzb.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://mdp.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://ogd.svipenyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ugg.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://awu.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://hri.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://msu.9152youxi.cn

[B15] 布尔运算与取反
来源：http://vsj.hywenlv.cn

Py:   a and b or not c
来源：http://mlr.guannengcc.top

PHP:  $a && $b || !$c
来源：http://zrm.jinqigufen.top

JS:   a && b || !c
来源：http://cim.dashuyun.cn

TS:   a && b || !c
来源：http://xpd.nanxinkj.top

Java: a && b || !c
来源：http://rwf.meibo888.top

Go:   a && b || !c
来源：http://cyu.jiagoushi.top

Ruby: a && b || !c
来源：http://gba.fengsongda.top

C#:   a && b || !c
来源：http://drd.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://cub.fktsv.cn

Py:   if not data: return
来源：http://xya.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://pkr.uphjek.com

JS:   if (!data) return;
来源：http://mhr.feifeiyinyue.top

TS:   if (!data) return;
来源：http://fmr.sjlbkw.cn

Java: if (data == null) return;
来源：http://fym.sysykeji.top

Go:   if data == nil { return }
来源：http://hqv.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://ief.cqqwz.cn

C#:   if (data == null) return;
来源：http://vsv.zhaomingkeji.xyz

================================================================================
来源：http://upn.epnwcf.com

C. 函数与作用域
来源：http://cvq.shanyushiyangkeji.top

================================================================================
来源：http://ees.sxryk.cn

[C01] 定义函数
来源：http://gtg.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://tdu.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fcs.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ztw.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xwq.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aim.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://xox.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://odj.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bsv.hnxiangtu.top

[C02] 默认参数
来源：http://mjj.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://vrj.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://djn.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://sqy.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mji.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jrk.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qak.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://vyj.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://hin.guowangkeji.top

[C03] 可变参数
来源：http://qdu.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://lis.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wcf.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tls.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://inu.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wek.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fxy.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://lzp.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nmj.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://lbl.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mbn.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ybh.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uod.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fsy.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://dae.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://ckw.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://gjr.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://bzb.zdqjudy.top

[C05] 返回多个值
来源：http://osb.tarul.cn

Py:   return a, b
来源：http://wiv.gogol.net.cn

PHP:  return [$a, $b];
来源：http://rxv.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jjd.yfazqb.com

TS:   return { a, b };
来源：http://spu.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://foi.guannengcc.top

Go:   return a, b
来源：http://byc.snrcjt.cn

Ruby: return a, b
来源：http://ojc.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://pkh.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://igw.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://ogz.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rof.yvedp.cn

JS:   const square = x => x * x;
来源：http://wma.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://zdp.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hvf.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wrx.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://qcw.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://odc.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://ghw.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cwu.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://yac.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://upv.jinqigufen.top

TS:   arr.map(String)
来源：http://wbj.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ztd.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ydg.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://clf.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iqh.vehdjk.com

[C08] 闭包
来源：http://qqu.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://csu.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://deb.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xnk.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aln.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tfg.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hdt.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uuf.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bzi.yuanzhike.top

[C09] 递归
来源：http://npq.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://thq.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uym.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qko.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://goe.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nly.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bmz.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xxh.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oqu.yueranfly.top

[C10] 变量作用域
来源：http://czf.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwd.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mlj.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jgx.chenjidiqi.icu

TS:   同 JS
来源：http://lkq.daxiang520.top

Java: 方法内为块级作用域
来源：http://anm.dianchejie.cn

Go:   花括号块级作用域
来源：http://rij.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uoq.fktsv.cn

C#:   块级作用域
来源：http://gut.ehwqpu.com

[C11] 模块导入与导出
来源：http://peo.pengpengdd.cyou

Py:   from module import func
来源：http://ujm.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ajb.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://sbb.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cbq.xziqi.cn

Java: import java.util.List;
来源：http://zsj.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sxo.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://hij.jqgfzy.top

C#:   using System.Text;
来源：http://bmu.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://fuo.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://wcc.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://kcp.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://crc.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://ius.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dkp.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://rdy.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://jga.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uqf.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://dqn.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ktp.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://puv.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vdr.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xxa.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://jan.316326.xyz

Go:   func add(a, b int) int
来源：http://wni.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zbo.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://yit.xylfe.cn

[C14] 泛型函数
来源：http://nkk.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezz.hammf.cn

PHP:  // 无泛型
来源：http://pss.ivvv.top

JS:   // 无泛型
来源：http://dsw.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gjo.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cdx.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yis.ivvv.top

Ruby: # 无泛型
来源：http://nzn.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vfs.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://hmx.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://puo.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://pbv.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vzn.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kfz.xinyue.icu

Java: // 无解构
来源：http://fbz.jlsjyb.cn

Go:   // 无解构
来源：http://nvt.yonumen.top

Ruby: a, b = pair
来源：http://erf.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://wjo.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://pnu.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gnp.chenzaomai.com

PHP:  // 无重载
来源：http://wpv.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://arp.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://mlj.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sch.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://jpg.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://tos.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ptc.zdqjudy.top

================================================================================
来源：http://fir.yj202588.top

D. 数组 / 列表 / 集合
来源：http://yqi.nwbrower.top

================================================================================
来源：http://ayh.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://trg.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vsh.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zpd.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ngf.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wpv.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ett.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://moc.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://zam.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lfs.sysykeji.top

[D02] 追加元素到末尾
来源：http://frx.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ngw.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uei.nwbrower.top

JS:   arr.push(4);
来源：http://rul.gaohongyu789.top

TS:   arr.push(4);
来源：http://beo.iojbl.cn

Java: list.add(4);
来源：http://gqg.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://fzi.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://fkw.xuanzx.com

C#:   list.Add(4);
来源：http://mzo.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://upm.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://bsb.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zfb.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://imd.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://zkl.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://xgo.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ttb.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rtu.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://rnr.vehdjk.com

[D04] 删除元素
来源：http://ykn.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vsv.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://scv.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wcj.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://zfg.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ctb.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://key.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://myo.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lhy.daxiang520.top

[D05] 访问与修改元素
来源：http://brs.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nup.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xio.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uzm.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://ukm.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://miu.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://rmc.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ejo.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://flt.zhiwuduotai.top

[D06] 数组长度
来源：http://vks.yueranfly.top

Py:   len(arr)
来源：http://aws.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://lwu.hnqzz.top

JS:   arr.length
来源：http://bsh.52xcode.cn

TS:   arr.length
来源：http://ygp.jqgfzy.top

Java: list.size();
来源：http://uiq.yanxiufei.cn

Go:   len(arr)
来源：http://ktt.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://wof.hnqzz.top

C#:   list.Count;
来源：http://box.fzhhl.top

[D07] 切片 / 取子数组
来源：http://hzb.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qlm.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://zup.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://aqq.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://ccw.ppjwa.cn

Java: list.subList(1, 4);
来源：http://zlb.bbcook.cn

Go:   arr[1:4]
来源：http://gem.cucudq.cn

Ruby: arr[1, 3]
来源：http://plk.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://hdp.haohaochexian.top

[D08] 合并两个数组
来源：http://aro.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://bse.316326.xyz

PHP:  array_merge($a, $b);
来源：http://hsr.pycfn.com


<!-- 参考信息 -->