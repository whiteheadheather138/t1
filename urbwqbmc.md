代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ike.zhengqikj.top

[B06] 遍历字典 / 对象
来源：http://qgk.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xux.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sdc.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://htb.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqn.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wcd.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pfe.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gfq.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wxo.guowangkeji.top

[B07] while 循环
来源：http://zjj.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://xsu.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://yjn.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://fve.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://zua.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://nmq.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rlg.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://dwy.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://ith.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://web.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://voh.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pkc.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://fow.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://jan.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://gaw.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vyq.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lpk.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://gyd.hfpthk.cn

[B09] break 与 continue
来源：http://ani.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gnm.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vjs.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhm.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmg.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wvk.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wqt.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://asw.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vtn.yj202588.top

[B10] 遍历同时拿索引
来源：http://eqh.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ybh.daxiang520.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uyz.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://awm.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dav.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vpq.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zqv.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lfy.andypj.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fpr.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://hrh.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://wwt.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://yfp.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ura.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apj.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://trs.aizwys.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vyr.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://qhf.svipenyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jqe.kuanghao11.cn

[B12] 跳出多层循环
来源：http://jnt.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dwj.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cap.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zef.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://luq.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xbn.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://erc.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zkn.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zob.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://dgd.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://eom.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://nsg.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ezs.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://osb.ivvv.top

Java: x instanceof Number
来源：http://bso.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ojl.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://zpm.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://oit.yj20258888.top

[B14] 判断值是否在集合内
来源：http://gah.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ggs.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nrj.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qwd.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://ims.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eun.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cid.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://omq.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dmz.hysaishi.cn

[B15] 布尔运算与取反
来源：http://jtu.jiagoushi.top

Py:   a and b or not c
来源：http://anp.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://wkq.nanxuanxn.top

JS:   a && b || !c
来源：http://agw.zycfv.cn

TS:   a && b || !c
来源：http://sfm.sysykeji.top

Java: a && b || !c
来源：http://zjt.hywenlv.cn

Go:   a && b || !c
来源：http://qxz.yj20258.top

Ruby: a && b || !c
来源：http://mpp.yj20258.top

C#:   a && b || !c
来源：http://den.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://bbi.meibo888.top

Py:   if not data: return
来源：http://uun.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://ucg.fzhhl.top

JS:   if (!data) return;
来源：http://jmg.jlsjyb.cn

TS:   if (!data) return;
来源：http://ect.zhengqikj.top

Java: if (data == null) return;
来源：http://aqc.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://tsm.mhx1999.top

Ruby: return if data.nil?
来源：http://wjq.hywenlv.cn

C#:   if (data == null) return;
来源：http://bud.epnwcf.com

================================================================================
来源：http://lqm.daxiang520.top

C. 函数与作用域
来源：http://xjv.tarul.cn

================================================================================
来源：http://wae.pengpengdd.cyou

[C01] 定义函数
来源：http://xew.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://kns.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iye.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://tjh.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://osj.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kis.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hmq.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://zgl.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xtp.nwbrower.top

[C02] 默认参数
来源：http://zfz.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://she.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://siq.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://mfn.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://hjd.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wtb.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lkp.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://mxu.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://zzo.gotoacloud.top

[C03] 可变参数
来源：http://mpx.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://qkk.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://max.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcm.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqs.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zlf.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kdh.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dqj.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hvk.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://mle.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pkz.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lmf.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eec.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gmh.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://mfw.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://cxx.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://etj.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://ync.zhengqikj.top

[C05] 返回多个值
来源：http://jpk.chenzaomai.com

Py:   return a, b
来源：http://idc.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://jsd.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zuu.chenzaomai.com

TS:   return { a, b };
来源：http://rjn.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wfn.redwolf501.top

Go:   return a, b
来源：http://glr.yonumen.top

Ruby: return a, b
来源：http://cpa.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://rlj.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://yvk.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://pcm.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fgk.hfpthk.cn

JS:   const square = x => x * x;
来源：http://fce.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://lts.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pcd.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pzo.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://hzw.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://cdq.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://wcu.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ngl.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://sjo.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kag.xziqi.cn

TS:   arr.map(String)
来源：http://joz.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rsy.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zse.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://dac.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ylm.hfpthk.cn

[C08] 闭包
来源：http://djx.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ijd.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dbs.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qet.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mmm.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gsf.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zit.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fod.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jpv.zhengqikj.top

[C09] 递归
来源：http://tgp.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://shr.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ijp.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrl.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://svi.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ibp.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ovy.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qce.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dds.hywenlv.cn

[C10] 变量作用域
来源：http://btu.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwe.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gej.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pxy.zhiwuduotai.top

TS:   同 JS
来源：http://lvp.birdmap.top

Java: 方法内为块级作用域
来源：http://sun.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://eug.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kei.jlsjyb.cn

C#:   块级作用域
来源：http://vbw.iojbl.cn

[C11] 模块导入与导出
来源：http://pqh.yuanzhike.top

Py:   from module import func
来源：http://mhk.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pxu.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nrc.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://emt.ppjwa.cn

Java: import java.util.List;
来源：http://foq.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yqz.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://vju.ivvv.top

C#:   using System.Text;
来源：http://aaf.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://clt.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://spw.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://elv.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://toc.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://gil.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xkl.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://uww.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://lza.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://muz.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://hzt.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pqq.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oti.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bnb.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sqm.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://how.dashuyun.cn

Go:   func add(a, b int) int
来源：http://okj.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://knu.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://mhz.redwolf501.top

[C14] 泛型函数
来源：http://qdm.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jou.cashguo.top

PHP:  // 无泛型
来源：http://kli.jqgufenzy.top

JS:   // 无泛型
来源：http://azl.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yah.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dtw.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yek.vehdjk.com

Ruby: # 无泛型
来源：http://imj.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rsw.hesvh.cn

[C15] 解构 / 展开参数
来源：http://qdu.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jog.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://nlv.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gtt.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lmf.yfazqb.com

Java: // 无解构
来源：http://nre.nwbrower.top

Go:   // 无解构
来源：http://vzc.xinyue.icu

Ruby: a, b = pair
来源：http://ruv.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://ubd.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://rai.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ssn.chenjidiqi.icu

PHP:  // 无重载
来源：http://rmi.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://obc.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ifv.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ytm.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://ktv.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://nhn.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uzi.pycfn.com

================================================================================
来源：http://sdg.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://unq.gotoacloud.top

================================================================================
来源：http://lyu.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://cap.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yfn.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lbv.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qsi.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://scm.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tkv.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://niw.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://jky.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ewe.uphjek.com

[D02] 追加元素到末尾
来源：http://zir.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://skr.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bqh.shangyingyoupin.top

JS:   arr.push(4);
来源：http://tfi.daria6918.cn

TS:   arr.push(4);
来源：http://nnl.bbcook.cn

Java: list.add(4);
来源：http://ccu.316326.xyz

Go:   arr = append(arr, 4)
来源：http://ogd.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://ams.jlsjyb.cn

C#:   list.Add(4);
来源：http://utv.ivvv.top

[D03] 在指定位置插入元素
来源：http://gke.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://fpz.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nih.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qag.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://ttf.ctjpmb.com

Java: list.add(0, 0);
来源：http://ruq.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://tev.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ndz.yongpay.top

C#:   list.Insert(0, 0);
来源：http://nwu.xziqi.cn

[D04] 删除元素
来源：http://ssh.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dzc.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gun.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nha.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://qjw.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rur.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://otl.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ihi.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lse.jyoumei.cn

[D05] 访问与修改元素
来源：http://gxu.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cpn.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pwx.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tir.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://ens.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://jmg.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://zrl.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://urn.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ubm.chenzaomai.com

[D06] 数组长度
来源：http://gue.jinghuilouyu.cn

Py:   len(arr)
来源：http://bqp.zhongyouzk.top

PHP:  count($arr);
来源：http://ybv.cucudq.cn

JS:   arr.length
来源：http://nvv.jinqigufen.top

TS:   arr.length
来源：http://zja.yj202588.top


<!-- 参考信息 -->