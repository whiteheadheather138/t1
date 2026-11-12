代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tld.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://fqz.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xlw.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://byq.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vls.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blk.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hhv.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hwp.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hhe.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://abn.epnwcf.com

[B07] while 循环
来源：http://gak.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://maq.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://vuf.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://ygw.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://xww.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://jxy.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mfh.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://krl.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://oif.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://khk.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://xsn.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iiy.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://dqg.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://eph.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://hwp.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://vuf.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://xea.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://jph.cucudq.cn

[B09] break 与 continue
来源：http://hih.cqqwz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ksa.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fdy.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ulh.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpd.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://weh.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qgz.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rwc.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xke.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://ayj.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yhl.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bck.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uhp.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xyl.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mdn.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gly.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://irj.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://evw.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://xek.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://smk.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://yjm.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wev.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://giv.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hka.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfm.cashguo.top

Ruby: (0...10).step(2).to_a
来源：http://dgl.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hrx.jiagoushi.top

[B12] 跳出多层循环
来源：http://zmq.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eqe.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mnb.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yzg.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezq.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qdu.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://spu.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wgv.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eka.mhx1999.top

[B13] 判断是否为数字
来源：http://jgs.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://vdx.gzhubu.top

PHP:  is_numeric($x)
来源：http://fpv.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isl.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ojg.birdmap.top

Java: x instanceof Number
来源：http://aix.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qnc.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://kor.gzhubu.top

C#:   x is int or double or decimal
来源：http://ncw.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://bve.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kdn.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sfp.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://gjn.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://typ.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tzr.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://okq.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://sxk.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://weo.yueranfly.top

[B15] 布尔运算与取反
来源：http://mrr.zhiwuduotai.top

Py:   a and b or not c
来源：http://rpj.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://ggp.yj20258888.top

JS:   a && b || !c
来源：http://hna.0kj1m.cn

TS:   a && b || !c
来源：http://dka.shanyushiyangtech.top

Java: a && b || !c
来源：http://oij.52xcode.cn

Go:   a && b || !c
来源：http://fil.bjfxy.top

Ruby: a && b || !c
来源：http://ybc.daria6918.cn

C#:   a && b || !c
来源：http://dmr.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zkx.hcnkem.com

Py:   if not data: return
来源：http://ruz.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://cgc.shzxlz.cn

JS:   if (!data) return;
来源：http://npx.sweek.top

TS:   if (!data) return;
来源：http://vzr.xuetiantiany.cn

Java: if (data == null) return;
来源：http://uqy.uphjek.com

Go:   if data == nil { return }
来源：http://ptv.yanxiufei.cn

Ruby: return if data.nil?
来源：http://gwp.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://wta.zycfv.cn

================================================================================
来源：http://uty.uphjek.com

C. 函数与作用域
来源：http://rfo.yonumen.top

================================================================================
来源：http://ibi.fzhhl.top

[C01] 定义函数
来源：http://fxp.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://pxu.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tmq.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://kdh.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qqk.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://try.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://zak.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://iwm.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ran.yangfankeji.com

[C02] 默认参数
来源：http://yco.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://thk.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fha.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://ttt.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ruw.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://nkd.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sxb.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://syk.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://zwr.bbcook.cn

[C03] 可变参数
来源：http://rxc.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://liq.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yiv.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kxr.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hwz.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rve.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xzy.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vzc.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://srq.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://mbf.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nal.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ybq.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xcm.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lfv.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://vvo.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://stv.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://ljm.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://ued.yvedp.cn

[C05] 返回多个值
来源：http://uir.yueranfly.top

Py:   return a, b
来源：http://ciu.dashuyun.cn

PHP:  return [$a, $b];
来源：http://jsy.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dqj.shanyushiyangtech.top

TS:   return { a, b };
来源：http://dwh.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mtp.daria6918.cn

Go:   return a, b
来源：http://gwm.yuanzhike.top

Ruby: return a, b
来源：http://vmr.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://pgt.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://jor.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://nse.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dvf.wangdashe.top

JS:   const square = x => x * x;
来源：http://dyb.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://fsu.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xdb.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hzf.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://tyb.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://nlz.fehbvm.com

[C07] 把函数作为参数传入
来源：http://xxe.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://huo.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://ybt.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mki.mhx1999.top

TS:   arr.map(String)
来源：http://qgo.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ism.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hbl.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://qcr.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kee.nanxinkj.top

[C08] 闭包
来源：http://mjv.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dmm.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zht.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://glw.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bug.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wfq.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wjz.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://biy.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ixd.sweek.top

[C09] 递归
来源：http://hof.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://frq.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bpo.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://khf.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pax.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ayw.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cxj.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uib.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://los.snrcjt.cn

[C10] 变量作用域
来源：http://tgv.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rov.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tqu.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zfk.vqdsnc.cn

TS:   同 JS
来源：http://yty.jianghu66.top

Java: 方法内为块级作用域
来源：http://skd.wangdashe.top

Go:   花括号块级作用域
来源：http://cki.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kgp.hywenlv.cn

C#:   块级作用域
来源：http://jft.quarkkingdee.top

[C11] 模块导入与导出
来源：http://keu.shanyushiyangtech.top

Py:   from module import func
来源：http://hoo.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://pak.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aoy.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://enl.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://zff.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gkc.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://xeq.yfazqb.com

C#:   using System.Text;
来源：http://mjv.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://osa.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://rhf.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://rfj.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://ixc.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://wku.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gwb.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://kte.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://bwb.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fmf.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://abg.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hii.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgw.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mzh.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xln.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://qzo.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://ypl.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gsr.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://zur.yj20258888.top

[C14] 泛型函数
来源：http://qgv.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wnc.fktsv.cn

PHP:  // 无泛型
来源：http://ndo.quarkkingdee.top

JS:   // 无泛型
来源：http://ued.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dxb.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rzs.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hnx.mhx1999.top

Ruby: # 无泛型
来源：http://cfb.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://soa.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://yik.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://krf.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://lkw.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dev.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://upe.cheryme.top

Java: // 无解构
来源：http://yiq.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://bjh.tian-w.cn

Ruby: a, b = pair
来源：http://xtq.c1oappe.top

C#:   var (a, b) = pair;
来源：http://uqt.jianghu66.top

[C16] 函数 / 方法重载
来源：http://uwb.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cco.gaohongyu789.top

PHP:  // 无重载
来源：http://muu.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cnm.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://flf.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zmq.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://cby.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://pmp.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wvo.daria6918.cn

================================================================================
来源：http://ojf.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://wil.fengsongda.top

================================================================================
来源：http://ssa.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://hec.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvw.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hae.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://apf.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oit.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgj.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://nof.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://fre.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qbp.aibaodan.cn

[D02] 追加元素到末尾
来源：http://jsl.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mbi.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://apq.yueranfly.top

JS:   arr.push(4);
来源：http://edj.xinyue.icu

TS:   arr.push(4);
来源：http://gos.yuxming.cn

Java: list.add(4);
来源：http://kgu.birdmap.top

Go:   arr = append(arr, 4)
来源：http://vpg.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://syh.zdbjq.cn

C#:   list.Add(4);
来源：http://wat.xuanzx.com

[D03] 在指定位置插入元素
来源：http://yjk.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://euj.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fjf.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xxy.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://opn.vehdjk.com

Java: list.add(0, 0);
来源：http://vag.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://lrf.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://spd.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://ywg.jinqigufen.top

[D04] 删除元素
来源：http://wgu.fehbvm.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kpc.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xdq.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jwf.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://vak.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bjl.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gmh.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jbk.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zds.dianchejie.cn

[D05] 访问与修改元素
来源：http://lkm.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tkb.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vau.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://osv.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://rdl.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://cgi.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://jzj.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iph.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ujq.gotoacloud.top

[D06] 数组长度
来源：http://rmg.bjfxy.top

Py:   len(arr)
来源：http://ymj.andypj.xyz

PHP:  count($arr);
来源：http://ujq.jqgufenzy.top

JS:   arr.length
来源：http://ixv.fktsv.cn

TS:   arr.length
来源：http://kwr.meibo888.top


<!-- 参考信息 -->