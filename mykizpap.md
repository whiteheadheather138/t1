代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nma.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://jfe.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://duu.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://mld.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://prl.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wmx.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://uea.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://dne.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://mqm.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gul.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://xxh.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://mjt.zdbjq.cn

[B09] break 与 continue
来源：http://ftg.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ovw.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://orc.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtl.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iwj.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ifx.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dgk.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://klw.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfx.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://zdg.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://paf.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bpn.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nsy.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iyl.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ilc.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gig.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ujq.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ioi.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://lvr.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://veo.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://man.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ozm.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jby.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://icv.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xuo.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://qwv.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rxo.zdqjudy.top

[B12] 跳出多层循环
来源：http://sib.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ddg.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ewd.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ntq.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qct.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fkc.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxf.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tfj.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgr.yj202588.top

[B13] 判断是否为数字
来源：http://tmh.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://eat.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://rwk.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xtq.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cxo.kuanghao11.cn

Java: x instanceof Number
来源：http://vbt.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://geg.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://uib.yongpay.top

C#:   x is int or double or decimal
来源：http://dfs.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://mwn.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qqp.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wve.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://irr.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://nyy.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://apl.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bhy.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wrc.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvt.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://ucv.hammf.cn

Py:   a and b or not c
来源：http://kfp.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://vrg.jqgufenzy.top

JS:   a && b || !c
来源：http://wbs.yfazqb.com

TS:   a && b || !c
来源：http://jwk.pengpengdd.cyou

Java: a && b || !c
来源：http://azh.gzhubu.top

Go:   a && b || !c
来源：http://bon.0kj1m.cn

Ruby: a && b || !c
来源：http://sog.zhongyouzk.top

C#:   a && b || !c
来源：http://ixu.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://lmp.fzhhl.top

Py:   if not data: return
来源：http://mha.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://jex.uphjek.com

JS:   if (!data) return;
来源：http://zkh.sxryk.cn

TS:   if (!data) return;
来源：http://jpm.yfazqb.com

Java: if (data == null) return;
来源：http://ais.ydzc1.top

Go:   if data == nil { return }
来源：http://gyr.uphjek.com

Ruby: return if data.nil?
来源：http://ydm.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://cjd.yvedp.cn

================================================================================
来源：http://mqn.hongshengwenyu.top

C. 函数与作用域
来源：http://gtp.nanxinkj.top

================================================================================
来源：http://uyz.xuanzx.com

[C01] 定义函数
来源：http://iol.birdmap.top

Py:   def add(a, b): return a + b
来源：http://ncm.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bpl.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://bbx.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ray.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://usk.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://cza.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://gns.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://utw.c1oappe.top

[C02] 默认参数
来源：http://dgh.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://gba.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://rku.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://gnm.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dla.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dwz.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ktf.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://ttn.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://cti.cheryme.top

[C03] 可变参数
来源：http://hnt.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://art.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jps.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jca.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvh.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bcx.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mbi.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rhp.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pkr.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://inv.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fgd.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://srg.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ogr.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cxu.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rfy.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://exv.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://mbu.feifeiyinyue.top

C#:   f(a: 1, b: 2)
来源：http://wrv.yuanzhike.top

[C05] 返回多个值
来源：http://mfa.hcnkem.com

Py:   return a, b
来源：http://amm.hnqzz.top

PHP:  return [$a, $b];
来源：http://yxl.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://dan.zhoulong.xyz

TS:   return { a, b };
来源：http://fee.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zuy.zhongyouzk.top

Go:   return a, b
来源：http://zqq.xinyue.icu

Ruby: return a, b
来源：http://xqn.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://scg.havefunace.top

[C06] 匿名函数 / lambda
来源：http://xra.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://wcg.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://csl.cheryme.top

JS:   const square = x => x * x;
来源：http://psb.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://rfh.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ias.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cnj.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://uly.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://exo.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://xee.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jwl.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://tsj.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://imw.meibo888.top

TS:   arr.map(String)
来源：http://znx.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eki.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://win.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://xzf.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bja.mhx1999.top

[C08] 闭包
来源：http://tmr.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zzn.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ezv.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pvm.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gkl.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yqv.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tjn.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dds.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lrb.snrcjt.cn

[C09] 递归
来源：http://bsr.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kll.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gqo.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xkk.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://onb.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://agm.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uwx.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://flf.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mgp.yonumen.top

[C10] 变量作用域
来源：http://qyn.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zwt.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://csm.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kvp.smart0.xyz

TS:   同 JS
来源：http://vta.yuxming.cn

Java: 方法内为块级作用域
来源：http://qjt.pycfn.com

Go:   花括号块级作用域
来源：http://tdj.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://deb.zhongyouzk.top

C#:   块级作用域
来源：http://ypa.yongpay.top

[C11] 模块导入与导出
来源：http://avn.sysykeji.top

Py:   from module import func
来源：http://ngg.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://xzd.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://egv.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ytg.pengpengdd.cyou

Java: import java.util.List;
来源：http://ajj.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qce.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://hyr.guannengcc.top

C#:   using System.Text;
来源：http://ivu.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://ywi.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://utj.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://waf.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://wbd.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://cyr.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xdg.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ddd.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://mkb.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hdl.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://zpo.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ebw.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://njo.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vzp.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqw.xinyue.icu

Java: int add(int a, int b) { return a + b; }
来源：http://nkr.shzxlz.cn

Go:   func add(a, b int) int
来源：http://zsw.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://igw.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://zri.vehdjk.com

[C14] 泛型函数
来源：http://xsm.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tlb.meibo888.top

PHP:  // 无泛型
来源：http://eil.zdqjudy.top

JS:   // 无泛型
来源：http://glf.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hbv.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nki.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hqe.hysaishi.cn

Ruby: # 无泛型
来源：http://nzd.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xft.hnqzz.top

[C15] 解构 / 展开参数
来源：http://hmy.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qum.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://nsm.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fgt.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wtu.cqqwz.cn

Java: // 无解构
来源：http://upv.sweek.top

Go:   // 无解构
来源：http://lng.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://txt.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://loe.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://yof.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://urk.hesvh.cn

PHP:  // 无重载
来源：http://est.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://csa.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://fxi.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xlk.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://hch.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://kvj.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tqs.xuetiantiany.cn

================================================================================
来源：http://xtp.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://hes.ivvv.top

================================================================================
来源：http://sal.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://dah.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tiq.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mri.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ajl.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wwr.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wdh.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://ewl.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://jbp.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gam.xinyue.icu

[D02] 追加元素到末尾
来源：http://cyu.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kop.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iws.tian-w.cn

JS:   arr.push(4);
来源：http://tlu.cashguo.top

TS:   arr.push(4);
来源：http://fqp.yueranfly.top

Java: list.add(4);
来源：http://srk.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://hmb.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://thj.uphjek.com

C#:   list.Add(4);
来源：http://jfr.gzhubu.top

[D03] 在指定位置插入元素
来源：http://rnm.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://xew.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xbh.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hta.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://jqj.sjlbkw.cn

Java: list.add(0, 0);
来源：http://vic.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://hvw.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://igp.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://vfd.hesvh.cn

[D04] 删除元素
来源：http://lpa.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ytk.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://icn.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ihu.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://cad.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sgj.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://als.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xur.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rlb.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://bov.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kgs.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wkv.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ynx.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://fdw.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://ygd.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://flc.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mce.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qpm.shangyingyoupin.top

[D06] 数组长度
来源：http://zkg.jinyuanbaomall.cn

Py:   len(arr)
来源：http://igj.ehwqpu.com

PHP:  count($arr);
来源：http://qwj.zhongyouzk.top

JS:   arr.length
来源：http://yiz.hfpthk.cn

TS:   arr.length
来源：http://zsb.sjlbkw.cn

Java: list.size();
来源：http://axt.cdnleiting.top

Go:   len(arr)
来源：http://mod.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://tpe.tianlin.xyz

C#:   list.Count;
来源：http://snq.daxiang520.top

[D07] 切片 / 取子数组
来源：http://zts.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fme.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://bbu.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://eqd.pycfn.com

TS:   arr.slice(1, 4);
来源：http://zvw.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://yvo.yuxming.cn

Go:   arr[1:4]
来源：http://fbe.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://feu.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://ijm.jianghu66.top

[D08] 合并两个数组
来源：http://qhc.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://uhc.ivvv.top

PHP:  array_merge($a, $b);
来源：http://yti.tarul.cn


<!-- 参考信息 -->