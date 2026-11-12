代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://drf.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://nve.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://ehl.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://ptu.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nys.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://ckz.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://siy.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://qtl.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://vhp.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uyf.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://bid.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://eyz.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://jjm.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iyb.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://epb.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://csf.hywenlv.cn

[B09] break 与 continue
来源：http://wrh.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xog.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://upy.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yak.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upw.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dws.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://klv.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gnj.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://egm.xinyue.icu

[B10] 遍历同时拿索引
来源：http://ekl.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tjw.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lod.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kbf.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wnd.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gyp.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dfb.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fwy.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fkr.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://lra.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://voc.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://ylr.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nqt.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slb.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hft.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hgb.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://mrc.fehbvm.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qhh.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://zyw.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iwu.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mxz.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bfn.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dkd.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://amu.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://urb.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ipu.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yjh.jqgufenzy.top

[B13] 判断是否为数字
来源：http://xsc.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://qev.fengsongda.top

PHP:  is_numeric($x)
来源：http://xhc.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ecq.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tgs.redwolf501.top

Java: x instanceof Number
来源：http://ffl.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ytd.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://qqk.havefunace.top

C#:   x is int or double or decimal
来源：http://psq.cashguo.top

[B14] 判断值是否在集合内
来源：http://nyz.vqdsnc.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bgo.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rjc.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://esi.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://sql.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xwc.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tpy.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://idm.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pmn.tian-w.cn

[B15] 布尔运算与取反
来源：http://zas.sufxvd.cn

Py:   a and b or not c
来源：http://jjd.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://iel.hywenlv.cn

JS:   a && b || !c
来源：http://zye.gzhubu.top

TS:   a && b || !c
来源：http://nqm.zhixingplan.top

Java: a && b || !c
来源：http://jnl.shuidangran.top

Go:   a && b || !c
来源：http://bnr.gaohongyu789.top

Ruby: a && b || !c
来源：http://dmz.jinghuilouyu.cn

C#:   a && b || !c
来源：http://ucs.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zah.chenzaomai.com

Py:   if not data: return
来源：http://aye.uphjek.com

PHP:  if (!$data) { return; }
来源：http://nva.tian-w.cn

JS:   if (!data) return;
来源：http://wkr.xylfe.cn

TS:   if (!data) return;
来源：http://nvp.bbcook.cn

Java: if (data == null) return;
来源：http://lei.pycfn.com

Go:   if data == nil { return }
来源：http://xms.316326.xyz

Ruby: return if data.nil?
来源：http://gtc.tian-w.cn

C#:   if (data == null) return;
来源：http://osv.guowangkeji.top

================================================================================
来源：http://unl.yj202588.top

C. 函数与作用域
来源：http://mws.birdmap.top

================================================================================
来源：http://rnm.gaohongyu789.top

[C01] 定义函数
来源：http://ijc.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://aml.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pad.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://hvk.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://swm.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hdj.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://rpb.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://mxq.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ktv.gaohongyu789.top

[C02] 默认参数
来源：http://emr.pycfn.com

Py:   def greet(name="World"): return name
来源：http://cha.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://orm.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://jyy.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://vup.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qxc.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ucl.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://kpu.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://scb.fktsv.cn

[C03] 可变参数
来源：http://bdg.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://poj.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://beg.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://heh.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kan.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://obf.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pih.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://grv.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sji.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://sgj.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uwj.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bxm.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xon.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lie.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://wjp.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://big.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://ugp.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://lkd.wangdashe.top

[C05] 返回多个值
来源：http://fba.fzhhl.top

Py:   return a, b
来源：http://ebu.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://pjn.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uvu.yfazqb.com

TS:   return { a, b };
来源：http://ike.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qkp.hfpthk.cn

Go:   return a, b
来源：http://jrk.cdnleiting.top

Ruby: return a, b
来源：http://aor.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://xhj.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://jtx.uphjek.com

Py:   square = lambda x: x * x
来源：http://xxu.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://grd.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://xki.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://lqm.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://irh.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ykg.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://zjt.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://lkc.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://wof.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vqk.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://fdh.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfw.iojbl.cn

TS:   arr.map(String)
来源：http://lty.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ilp.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wcw.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://zld.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://esz.ywan-chungtsiang.top

[C08] 闭包
来源：http://kej.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lle.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cso.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cpt.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://elr.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://obt.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lee.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uca.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dul.sysykeji.top

[C09] 递归
来源：http://vuo.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ivr.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vrm.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cnt.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jge.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hvo.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iml.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tng.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://txg.zhoulong.xyz

[C10] 变量作用域
来源：http://oam.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jog.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ptt.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ynb.gogol.net.cn

TS:   同 JS
来源：http://ayg.dashuyun.cn

Java: 方法内为块级作用域
来源：http://rmr.cucudq.cn

Go:   花括号块级作用域
来源：http://nxz.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lwg.zhengqikj.top

C#:   块级作用域
来源：http://ycw.iojbl.cn

[C11] 模块导入与导出
来源：http://hqy.chenlongwang.top

Py:   from module import func
来源：http://idf.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aao.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gny.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gxy.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://rsm.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://txl.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://eid.0kj1m.cn

C#:   using System.Text;
来源：http://mxp.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://wex.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://mgr.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://ftb.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://ukg.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://cqh.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aik.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://cxw.sweek.top

Ruby: -> { puts "run" }.call
来源：http://zjm.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fhz.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://hiu.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://szg.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tpk.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hjy.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://evh.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mqg.yj20258.top

Go:   func add(a, b int) int
来源：http://xgf.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ram.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hzq.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://tlc.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zut.gzhubu.top

PHP:  // 无泛型
来源：http://bkb.shuidangran.top

JS:   // 无泛型
来源：http://zll.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aho.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wyz.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eha.gaohongyu789.top

Ruby: # 无泛型
来源：http://ugh.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jty.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://xnp.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ckf.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://bsk.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ims.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://def.hywenlv.cn

Java: // 无解构
来源：http://yme.uphjek.com

Go:   // 无解构
来源：http://pqi.havefunace.top

Ruby: a, b = pair
来源：http://gkh.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://aop.xziqi.cn

[C16] 函数 / 方法重载
来源：http://bby.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://slk.xuetiantiany.cn

PHP:  // 无重载
来源：http://jrq.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oen.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://rng.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nly.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://lkr.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://wmv.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yks.sxryk.cn

================================================================================
来源：http://vxq.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://wff.nanxinkj.top

================================================================================
来源：http://kos.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://hok.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://plw.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nko.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lax.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eab.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aro.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://dch.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://mza.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dge.yuxming.cn

[D02] 追加元素到末尾
来源：http://axh.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nze.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rci.fzhhl.top

JS:   arr.push(4);
来源：http://gmv.pycfn.com

TS:   arr.push(4);
来源：http://zzj.zdqjudy.top

Java: list.add(4);
来源：http://iaw.uphjek.com

Go:   arr = append(arr, 4)
来源：http://yrs.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://ksg.sxryk.cn

C#:   list.Add(4);
来源：http://pky.smart0.xyz

[D03] 在指定位置插入元素
来源：http://jgy.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://uax.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ozm.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dam.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://oxm.c1oappe.top

Java: list.add(0, 0);
来源：http://kpg.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ran.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rrn.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://iup.hammf.cn

[D04] 删除元素
来源：http://lhj.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujp.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xno.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://foq.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://spy.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jyo.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eqv.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nbz.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bbg.birdmap.top

[D05] 访问与修改元素
来源：http://vyl.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lip.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jve.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qcr.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://iok.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ham.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dsv.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xez.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvv.xuetiantiany.cn

[D06] 数组长度
来源：http://xdu.iojbl.cn

Py:   len(arr)
来源：http://ahb.zdqjudy.top

PHP:  count($arr);
来源：http://khc.tianlin.xyz

JS:   arr.length
来源：http://kvs.daria6918.cn

TS:   arr.length
来源：http://jcs.kuanghao11.cn

Java: list.size();
来源：http://ffl.pengpengdd.cyou

Go:   len(arr)
来源：http://ewe.hcnkem.com

Ruby: arr.length; arr.size
来源：http://hkh.pycfn.com

C#:   list.Count;
来源：http://zhk.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://yvq.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pyx.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://owc.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://req.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://ouc.aizwys.cn

Java: list.subList(1, 4);
来源：http://plq.jiagoushi.top

Go:   arr[1:4]
来源：http://imj.zhixingplan.top

Ruby: arr[1, 3]
来源：http://nsu.hywenlv.cn


<!-- 参考信息 -->