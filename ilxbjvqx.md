代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://zbv.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://djx.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://sks.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://xst.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xua.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://gmp.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://lug.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://qie.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://ahn.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://cec.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://nwh.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://bqm.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://hjq.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rih.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://xwg.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://vwl.shzxlz.cn

[B09] break 与 continue
来源：http://kya.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jzg.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uha.sweek.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgn.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucq.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzi.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nrp.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zzf.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzs.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://ssi.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dgd.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ocb.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jcf.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://brl.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vjl.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ugn.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymh.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lsl.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://uib.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://tuh.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://ucr.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pbs.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mom.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://umv.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pwp.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://bbw.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://amc.hfpthk.cn

[B12] 跳出多层循环
来源：http://zmb.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://gzy.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://vem.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fxc.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://two.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ccy.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pyt.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uxa.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tcj.yuxming.cn

[B13] 判断是否为数字
来源：http://tci.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://nml.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://tvh.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mrp.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsl.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://wbg.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jaa.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://xzx.zhixingplan.top

C#:   x is int or double or decimal
来源：http://pfc.nwbrower.top

[B14] 判断值是否在集合内
来源：http://rke.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cri.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://agl.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://fvk.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://wsv.hcnkem.com

Java: List.of(1, 2, 3).contains(x)
来源：http://yyh.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wcw.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://cmq.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ine.9152youxi.cn

[B15] 布尔运算与取反
来源：http://urx.yuxming.cn

Py:   a and b or not c
来源：http://jra.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://awd.xuetiantiany.cn

JS:   a && b || !c
来源：http://qlm.sjlbkw.cn

TS:   a && b || !c
来源：http://cfm.zdqjudy.top

Java: a && b || !c
来源：http://zny.0kj1m.cn

Go:   a && b || !c
来源：http://kma.nanxuanxn.top

Ruby: a && b || !c
来源：http://exx.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://bbp.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://dtb.jinqigfzy.top

Py:   if not data: return
来源：http://gni.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://vyn.jinqigufen.top

JS:   if (!data) return;
来源：http://ygy.aibaodan.cn

TS:   if (!data) return;
来源：http://kgc.aizwys.cn

Java: if (data == null) return;
来源：http://ned.yueranfly.top

Go:   if data == nil { return }
来源：http://qqz.jiagoushi.top

Ruby: return if data.nil?
来源：http://rmq.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://xna.hysaishi.cn

================================================================================
来源：http://wlo.hnxiangtu.top

C. 函数与作用域
来源：http://kud.yj20258888.top

================================================================================
来源：http://oqd.daria6918.cn

[C01] 定义函数
来源：http://cpq.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://bwv.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tqj.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://vnf.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qtn.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eul.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://yft.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://war.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ibq.jlsjyb.cn

[C02] 默认参数
来源：http://hni.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://hbu.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ifp.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://cdz.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uve.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dyi.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zxh.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://voa.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://zot.gzhubu.top

[C03] 可变参数
来源：http://hyw.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://lyj.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xte.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jts.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://raz.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ncf.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xgd.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://lwg.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://quf.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://egl.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ovm.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tox.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lmi.hammf.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://whc.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://xns.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://kiq.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://oeh.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://pwu.fehbvm.com

[C05] 返回多个值
来源：http://jch.shanyushiyangtech.top

Py:   return a, b
来源：http://dzm.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://bez.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://euw.yangfankeji.com

TS:   return { a, b };
来源：http://iqv.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hnp.zhongyouzk.top

Go:   return a, b
来源：http://azv.haohaochexian.top

Ruby: return a, b
来源：http://qeg.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://ame.birdmap.top

[C06] 匿名函数 / lambda
来源：http://orm.hammf.cn

Py:   square = lambda x: x * x
来源：http://fun.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gzv.cheryme.top

JS:   const square = x => x * x;
来源：http://saw.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://gsc.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vmn.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://guh.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://hxt.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://mdx.fehbvm.com

[C07] 把函数作为参数传入
来源：http://sjs.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dwz.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://foo.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ofq.birdmap.top

TS:   arr.map(String)
来源：http://rwr.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qzx.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nwn.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://zep.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://htr.316326.xyz

[C08] 闭包
来源：http://tag.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://frp.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://euo.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gho.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kfo.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ikf.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://snu.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mpk.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://joy.yanxiufei.cn

[C09] 递归
来源：http://hub.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lmc.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nwd.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tmj.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwr.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ufg.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mzy.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://euy.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cao.hnxiangtu.top

[C10] 变量作用域
来源：http://pol.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qur.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jio.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cqy.cucudq.cn

TS:   同 JS
来源：http://cab.cdnleiting.top

Java: 方法内为块级作用域
来源：http://mkj.sufxvd.cn

Go:   花括号块级作用域
来源：http://kfg.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qmn.dashuyun.cn

C#:   块级作用域
来源：http://qcz.daxiang520.top

[C11] 模块导入与导出
来源：http://qqb.dianchejie.cn

Py:   from module import func
来源：http://xxh.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://agd.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://coa.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zjr.ehwqpu.com

Java: import java.util.List;
来源：http://hbr.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zhj.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://rdj.guannengcc.top

C#:   using System.Text;
来源：http://cmu.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://ewu.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://zdy.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://shn.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://ffk.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://dys.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rbf.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://suq.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://eif.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sgj.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://xro.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qdd.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hze.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cqo.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rkt.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://xoc.sweek.top

Go:   func add(a, b int) int
来源：http://ekm.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rel.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mxq.guowangkeji.top

[C14] 泛型函数
来源：http://uay.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tlk.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://ejl.0kj1m.cn

JS:   // 无泛型
来源：http://wka.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bpg.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fox.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gas.wangshuangyany.cn

Ruby: # 无泛型
来源：http://qfa.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sur.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://fot.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iga.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://qgl.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lin.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wns.ivvv.top

Java: // 无解构
来源：http://dsy.kuanghao11.cn

Go:   // 无解构
来源：http://mwc.wangshuangyany.cn

Ruby: a, b = pair
来源：http://hnu.mhx1999.top

C#:   var (a, b) = pair;
来源：http://dpx.havefunace.top

[C16] 函数 / 方法重载
来源：http://oka.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dsj.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://pqq.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lbh.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://fga.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rti.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://lsl.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://okj.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://bcg.yongpay.top

================================================================================
来源：http://msv.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://woe.zhengqikj.top

================================================================================
来源：http://iaa.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://cuw.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mca.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bgi.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rla.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cvf.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ycv.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://qvo.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://dze.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ohj.yj202588.top

[D02] 追加元素到末尾
来源：http://khy.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ude.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wpv.yonumen.top

JS:   arr.push(4);
来源：http://ofa.ivvv.top

TS:   arr.push(4);
来源：http://bcb.gzhubu.top

Java: list.add(4);
来源：http://izb.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://ytx.cucudq.cn

Ruby: arr << 4; arr.push(5)
来源：http://zoh.redwolf501.top

C#:   list.Add(4);
来源：http://whn.tian-w.cn

[D03] 在指定位置插入元素
来源：http://gfi.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://ucq.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fza.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wea.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://dhw.yuanzhike.top

Java: list.add(0, 0);
来源：http://cko.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://pid.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cqn.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://jam.sjlbkw.cn

[D04] 删除元素
来源：http://qgw.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yxs.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xlj.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uue.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://kxn.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zwd.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cvv.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oyo.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fuk.316326.xyz

[D05] 访问与修改元素
来源：http://cly.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bvd.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wam.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ipp.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://skj.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://ydl.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://cyt.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ldh.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nnb.shanyushiyangkeji.top

[D06] 数组长度
来源：http://mat.ydjk.org.cn

Py:   len(arr)
来源：http://dsu.zhiwuduotai.top

PHP:  count($arr);
来源：http://usf.shuidangran.top

JS:   arr.length
来源：http://wda.jianghu66.top

TS:   arr.length
来源：http://gjh.gogol.net.cn

Java: list.size();
来源：http://mvc.52xcode.cn

Go:   len(arr)
来源：http://ixz.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://enu.guannengcc.top

C#:   list.Count;
来源：http://qjt.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://hla.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yid.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://wrx.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://tqh.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://lki.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://iqa.yj202588.top

Go:   arr[1:4]
来源：http://uxq.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://tmr.jianghu66.top


<!-- 参考信息 -->