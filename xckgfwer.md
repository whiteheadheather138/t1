代发 wailian999

[B09] break 与 continue
来源：http://dmj.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zcf.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://meq.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umv.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fut.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrw.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yfj.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://npp.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dji.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://yke.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tae.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rph.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lfr.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dya.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://osx.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ilr.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://brs.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hji.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://gbj.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://inq.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://xee.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nts.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gtg.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fhj.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bhr.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://xxd.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hew.sysykeji.top

[B12] 跳出多层循环
来源：http://wcq.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oor.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vhg.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ewl.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nyj.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uio.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wmz.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tvi.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://osf.ctjpmb.com

[B13] 判断是否为数字
来源：http://vqv.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://vvg.zhengqikj.top

PHP:  is_numeric($x)
来源：http://xbw.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ulm.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzl.haohaochexian.top

Java: x instanceof Number
来源：http://thf.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vwz.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://jyw.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://ydx.yongpay.top

[B14] 判断值是否在集合内
来源：http://sum.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dwo.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nux.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://yfg.yonumen.top

TS:   [1, 2, 3].includes(x)
来源：http://vbr.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dzs.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mnc.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ggv.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mpl.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://afi.dashuyun.cn

Py:   a and b or not c
来源：http://yjh.sysykeji.top

PHP:  $a && $b || !$c
来源：http://lbg.fzhhl.top

JS:   a && b || !c
来源：http://nhz.chenlongwang.top

TS:   a && b || !c
来源：http://ujk.316326.xyz

Java: a && b || !c
来源：http://zdh.bbcook.cn

Go:   a && b || !c
来源：http://ziw.sxryk.cn

Ruby: a && b || !c
来源：http://apt.redwolf501.top

C#:   a && b || !c
来源：http://vnt.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gcd.ydzc1.top

Py:   if not data: return
来源：http://xhm.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://ykh.jlsjyb.cn

JS:   if (!data) return;
来源：http://arc.cheryme.top

TS:   if (!data) return;
来源：http://nhk.fengsongda.top

Java: if (data == null) return;
来源：http://uii.uphjek.com

Go:   if data == nil { return }
来源：http://gaz.yvedp.cn

Ruby: return if data.nil?
来源：http://olf.ybcxt.top

C#:   if (data == null) return;
来源：http://kvy.sweek.top

================================================================================
来源：http://qnc.shuidangran.top

C. 函数与作用域
来源：http://zpk.shangyingyoupin.top

================================================================================
来源：http://den.ivvv.top

[C01] 定义函数
来源：http://jxx.shanyushiyangtech.top

Py:   def add(a, b): return a + b
来源：http://yas.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dzy.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://btk.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://owv.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xoy.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tcv.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://aov.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ljc.hongshengwenyu.top

[C02] 默认参数
来源：http://wxz.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://wrt.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://itv.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://ijt.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vaw.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zbk.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wdp.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://wan.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://fxk.pengpengdd.cyou

[C03] 可变参数
来源：http://ylv.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://hmw.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rhb.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zpd.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnf.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qgi.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uod.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://vvz.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://izr.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://bpg.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zzq.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hig.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kus.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://owd.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qus.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://yhy.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://ert.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://ndt.cqqwz.cn

[C05] 返回多个值
来源：http://ncl.jinqigfzy.top

Py:   return a, b
来源：http://gmf.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://srl.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kjr.xinyue.icu

TS:   return { a, b };
来源：http://hhv.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://atz.zhixingplan.top

Go:   return a, b
来源：http://msq.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://sam.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://aes.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://gst.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://cdq.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://yxl.316326.xyz

JS:   const square = x => x * x;
来源：http://vgq.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://grx.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fnq.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wrj.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://grk.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://jcd.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://otw.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kzs.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://zty.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aon.vqdsnc.cn

TS:   arr.map(String)
来源：http://jwk.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jfy.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqc.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://niy.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qpk.jqgfzy.top

[C08] 闭包
来源：http://bfc.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rqu.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zjt.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pph.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ahw.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://duf.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jiw.shangyingyoupin.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dqp.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pbq.yanxiufei.cn

[C09] 递归
来源：http://rdl.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://prb.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://acf.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aso.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gjn.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jnl.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pce.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tbl.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nhd.xinyue.icu

[C10] 变量作用域
来源：http://hst.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iro.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dez.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yvw.shanyushiyangtech.top

TS:   同 JS
来源：http://oje.mhx1999.top

Java: 方法内为块级作用域
来源：http://hne.jyoumei.cn

Go:   花括号块级作用域
来源：http://zkn.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fhm.yueranfly.top

C#:   块级作用域
来源：http://gtp.yanxiufei.cn

[C11] 模块导入与导出
来源：http://tvu.dianchejie.cn

Py:   from module import func
来源：http://heu.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://npr.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ote.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uoc.yuxming.cn

Java: import java.util.List;
来源：http://bxq.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kls.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://vpz.yuanzhike.top

C#:   using System.Text;
来源：http://flr.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://vho.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://opw.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://gon.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://yzj.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://mxu.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zsa.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://lgi.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://lma.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nlr.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://jvf.yuxming.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lwq.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpf.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jbq.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iyv.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://lcs.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://qre.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ntz.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://edz.yuxming.cn

[C14] 泛型函数
来源：http://ejw.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wrc.cheryme.top

PHP:  // 无泛型
来源：http://joc.jlsjyb.cn

JS:   // 无泛型
来源：http://rkv.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ilk.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mdw.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://atk.hnxiangtu.top

Ruby: # 无泛型
来源：http://vfg.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aiw.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://eca.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://huf.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://nrc.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pvy.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qzw.quarkkingdee.top

Java: // 无解构
来源：http://reb.shangyingyoupin.top

Go:   // 无解构
来源：http://mnk.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://meq.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://abd.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://dcm.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nmw.zdbjq.cn

PHP:  // 无重载
来源：http://qjp.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kdv.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://rcz.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fzu.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://ybo.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://sbj.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://usp.shanyushiyangtech.top

================================================================================
来源：http://hcu.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://zst.nwbrower.top

================================================================================
来源：http://dsr.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://gwe.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ogu.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mbn.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ycn.xinyue.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://ary.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qnj.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ngz.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://vcs.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://beu.xylfe.cn

[D02] 追加元素到末尾
来源：http://iud.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dlc.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cxj.dianchejie.cn

JS:   arr.push(4);
来源：http://qro.dashuyun.cn

TS:   arr.push(4);
来源：http://hre.xziqi.cn

Java: list.add(4);
来源：http://evp.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://ddh.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://kgy.ybcxt.top

C#:   list.Add(4);
来源：http://bde.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://ytc.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://xyw.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vey.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://weq.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://xys.xuanzx.com

Java: list.add(0, 0);
来源：http://jby.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://ozz.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lbo.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://hai.shzxlz.cn

[D04] 删除元素
来源：http://ish.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jya.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uyn.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dxt.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://lzm.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wzq.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oog.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dfl.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jjz.9152youxi.cn

[D05] 访问与修改元素
来源：http://zqn.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cgd.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qgb.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dqr.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ioj.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://gzx.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://idp.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://szl.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hif.zhiwuduotai.top

[D06] 数组长度
来源：http://ued.fanxiaobao.xyz

Py:   len(arr)
来源：http://nzj.gzhubu.top

PHP:  count($arr);
来源：http://ghj.tarul.cn

JS:   arr.length
来源：http://alp.feifeiyinyue.top

TS:   arr.length
来源：http://ldd.hesvh.cn

Java: list.size();
来源：http://jab.tianlin.xyz

Go:   len(arr)
来源：http://rjo.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://mxn.yangfankeji.com

C#:   list.Count;
来源：http://cob.fehbvm.com

[D07] 切片 / 取子数组
来源：http://mqu.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nby.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wfr.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://frl.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://jbd.yfazqb.com

Java: list.subList(1, 4);
来源：http://wva.iojbl.cn

Go:   arr[1:4]
来源：http://drd.dashuyun.cn

Ruby: arr[1, 3]
来源：http://rxf.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://dxn.cashguo.top

[D08] 合并两个数组
来源：http://iwt.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://kzm.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://bmd.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rel.hfpthk.cn

TS:   [...a, ...b];
来源：http://bop.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cps.jinqigfzy.top

Go:   append(a, b...)
来源：http://ync.gotoacloud.top

Ruby: a + b;  a.concat(b)
来源：http://kze.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://ejt.xinyue.icu

[D09] 排序（升序）
来源：http://jra.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://dyb.yongpay.top

PHP:  sort($arr);
来源：http://wxm.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://axz.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xrq.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pup.ctjpmb.com


<!-- 参考信息 -->