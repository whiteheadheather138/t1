代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzk.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://qhr.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivb.vqdsnc.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://meb.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ghm.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zel.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mju.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://olx.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rqm.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://szy.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://tlg.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://cbg.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://qky.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://izf.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iss.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qfs.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://woo.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://ntz.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bnw.guowangkeji.top

[B12] 跳出多层循环
来源：http://lko.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vlt.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://obx.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mql.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://otz.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rkl.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wjd.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sxu.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zom.fehbvm.com

[B13] 判断是否为数字
来源：http://hgn.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://xpz.ydzc1.top

PHP:  is_numeric($x)
来源：http://hzr.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gfs.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://stw.cashguo.top

Java: x instanceof Number
来源：http://qmo.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jca.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://yuo.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://wvl.pycfn.com

[B14] 判断值是否在集合内
来源：http://ppb.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tpm.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zjv.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://fcf.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ajy.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rzr.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nyv.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://tzx.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lam.cdnleiting.top

[B15] 布尔运算与取反
来源：http://xva.zhongyouzk.top

Py:   a and b or not c
来源：http://xvm.yj202588.top

PHP:  $a && $b || !$c
来源：http://tmi.fehbvm.com

JS:   a && b || !c
来源：http://jje.zhiwuduotai.top

TS:   a && b || !c
来源：http://hia.zhiwuduotai.top

Java: a && b || !c
来源：http://tst.hongshengwenyu.top

Go:   a && b || !c
来源：http://chv.zhixingplan.top

Ruby: a && b || !c
来源：http://fyo.nwbrower.top

C#:   a && b || !c
来源：http://wpb.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://oir.sweek.top

Py:   if not data: return
来源：http://brq.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://aan.smart0.xyz

JS:   if (!data) return;
来源：http://eek.sweek.top

TS:   if (!data) return;
来源：http://ldq.fzhhl.top

Java: if (data == null) return;
来源：http://rwi.yangfankeji.com

Go:   if data == nil { return }
来源：http://xrv.sweek.top

Ruby: return if data.nil?
来源：http://clc.vqdsnc.cn

C#:   if (data == null) return;
来源：http://hyr.jinyuanbaomall.cn

================================================================================
来源：http://ary.chenjidiqi.icu

C. 函数与作用域
来源：http://nsr.fengsongda.top

================================================================================
来源：http://dob.sufxvd.cn

[C01] 定义函数
来源：http://isu.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://exq.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlv.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://zml.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aio.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tsv.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://utc.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://xeh.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kob.chenzaomai.com

[C02] 默认参数
来源：http://kfu.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://fwc.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cdi.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://kqq.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://heq.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bns.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qfn.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://omb.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://ive.xinyue.icu

[C03] 可变参数
来源：http://azp.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://qgp.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aej.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wax.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sod.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ohs.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tip.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://sux.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pmw.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://bht.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aew.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axv.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://miv.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ois.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://msh.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://zat.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://agg.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://tlc.ivvv.top

[C05] 返回多个值
来源：http://htd.hesvh.cn

Py:   return a, b
来源：http://dyn.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://sfk.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tzn.yj20258.top

TS:   return { a, b };
来源：http://gyz.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfp.fktsv.cn

Go:   return a, b
来源：http://sxx.zhiwuduotai.top

Ruby: return a, b
来源：http://aio.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://dma.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://nhj.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://gzn.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xxi.sxryk.cn

JS:   const square = x => x * x;
来源：http://vhb.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://ugr.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vpv.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://vaq.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://qib.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://uek.gzhubu.top

[C07] 把函数作为参数传入
来源：http://axb.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rlz.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://svj.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bzm.zhoulong.xyz

TS:   arr.map(String)
来源：http://ciw.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ohw.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dxq.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://hon.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wws.ppjwa.cn

[C08] 闭包
来源：http://hzc.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tij.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://etj.iojbl.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nww.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gol.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pzo.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hqw.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yaw.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ogk.0kj1m.cn

[C09] 递归
来源：http://jit.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ael.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bht.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jdr.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://igz.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xje.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dwx.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bcf.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://afd.snrcjt.cn

[C10] 变量作用域
来源：http://cdu.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qhb.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pwh.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://urw.ctjpmb.com

TS:   同 JS
来源：http://yfw.sxryk.cn

Java: 方法内为块级作用域
来源：http://nvv.cashguo.top

Go:   花括号块级作用域
来源：http://idp.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ngo.jinghuilouyu.cn

C#:   块级作用域
来源：http://ene.fktsv.cn

[C11] 模块导入与导出
来源：http://ajt.ivvv.top

Py:   from module import func
来源：http://iju.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ted.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kgp.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vce.redwolf501.top

Java: import java.util.List;
来源：http://zwm.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogh.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://ewj.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://mbw.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://mis.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://ftp.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://qzb.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://avn.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://yhd.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iry.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://dhk.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://nrv.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rfp.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://qfv.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gfe.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfk.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jka.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymw.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://dtn.gotoacloud.top

Go:   func add(a, b int) int
来源：http://ebi.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zbp.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://ocy.jqgufenzy.top

[C14] 泛型函数
来源：http://bhc.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://etk.xziqi.cn

PHP:  // 无泛型
来源：http://xui.cheryme.top

JS:   // 无泛型
来源：http://yyc.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jgv.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gkm.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xdc.redwolf501.top

Ruby: # 无泛型
来源：http://boz.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://krq.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://cij.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xtl.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://olm.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://piw.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rpr.ppjwa.cn

Java: // 无解构
来源：http://bru.yj20258.top

Go:   // 无解构
来源：http://nss.yangfankeji.com

Ruby: a, b = pair
来源：http://bkg.tian-w.cn

C#:   var (a, b) = pair;
来源：http://vig.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://shv.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryz.nwbrower.top

PHP:  // 无重载
来源：http://kdg.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nov.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://luz.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ogf.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://jcq.ivvv.top

Ruby: # 无重载：靠动态参数
来源：http://akj.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://efy.aizwys.cn

================================================================================
来源：http://xta.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://ika.ywan-chungtsiang.top

================================================================================
来源：http://tne.zycfv.cn

[D01] 创建数组 / 列表
来源：http://dnt.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fmq.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://woe.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rql.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ued.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ftp.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://qmt.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://xgw.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ews.52xcode.cn

[D02] 追加元素到末尾
来源：http://pto.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eri.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aaf.ydzc1.top

JS:   arr.push(4);
来源：http://hlq.hnqzz.top

TS:   arr.push(4);
来源：http://aha.chenzaomai.com

Java: list.add(4);
来源：http://glq.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://ivf.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://rpe.jlsjyb.cn

C#:   list.Add(4);
来源：http://ded.52xcode.cn

[D03] 在指定位置插入元素
来源：http://zug.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://bdp.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wlg.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zqc.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://mem.guannengcc.top

Java: list.add(0, 0);
来源：http://kpm.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gni.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vio.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://npr.aibaodan.cn

[D04] 删除元素
来源：http://wwd.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bbm.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qvh.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cvo.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://iag.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mhr.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oqp.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ceq.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xaf.yuxming.cn

[D05] 访问与修改元素
来源：http://ydv.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ugi.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zdm.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iev.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://kap.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://ndk.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://wbr.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zkh.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xes.yuanzhike.top

[D06] 数组长度
来源：http://tkd.sufxvd.cn

Py:   len(arr)
来源：http://rkm.c1oappe.top

PHP:  count($arr);
来源：http://nhq.jinqigfzy.top

JS:   arr.length
来源：http://qsa.iojbl.cn

TS:   arr.length
来源：http://eba.guannengcc.top

Java: list.size();
来源：http://etc.jqgufenzy.top

Go:   len(arr)
来源：http://mll.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://qkv.zycfv.cn

C#:   list.Count;
来源：http://pwq.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://uwx.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qsl.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hen.yj20258.top

JS:   arr.slice(1, 4);
来源：http://uir.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://adn.hammf.cn

Java: list.subList(1, 4);
来源：http://wwh.sjlbkw.cn

Go:   arr[1:4]
来源：http://tbr.cucudq.cn

Ruby: arr[1, 3]
来源：http://ezr.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://kby.cashguo.top

[D08] 合并两个数组
来源：http://fej.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://mln.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://tuy.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://whc.yvedp.cn

TS:   [...a, ...b];
来源：http://woy.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zmu.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://phe.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://bea.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://ojv.fzhhl.top

[D09] 排序（升序）
来源：http://jkm.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://gav.xuanzx.com

PHP:  sort($arr);
来源：http://nvc.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mln.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hjl.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tbj.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jqn.dianchejie.cn

Ruby: arr.sort
来源：http://lay.zhixingplan.top

C#:   list.Sort();
来源：http://oqy.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eqd.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zes.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qmh.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjc.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://klj.smart0.xyz


<!-- 参考信息 -->