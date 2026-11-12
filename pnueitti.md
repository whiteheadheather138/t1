代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hye.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://abn.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://syy.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://brv.yuxming.cn

[B09] break 与 continue
来源：http://ubb.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pma.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jzq.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evr.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqc.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkd.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hjb.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://top.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmu.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://fgq.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gxs.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://emx.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xih.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pyt.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bhh.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xip.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dmf.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bvv.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://yss.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://rux.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://uah.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tmp.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vso.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cyu.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ntb.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://lgx.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hgt.hnxiangtu.top

[B12] 跳出多层循环
来源：http://xdu.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qum.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wkc.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://poi.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ulg.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pkw.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ddl.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yhx.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jvc.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://doo.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://etf.ppjwa.cn

PHP:  is_numeric($x)
来源：http://xyk.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kpy.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://frj.jqgfzy.top

Java: x instanceof Number
来源：http://bvq.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uls.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://rfe.ivvv.top

C#:   x is int or double or decimal
来源：http://vri.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://urs.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nso.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kzu.yueranfly.top

JS:   [1, 2, 3].includes(x)
来源：http://zpv.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://ary.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qve.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rcy.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://ysb.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aky.xinyue.icu

[B15] 布尔运算与取反
来源：http://syq.smart0.xyz

Py:   a and b or not c
来源：http://mom.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://zhe.nanxinkj.top

JS:   a && b || !c
来源：http://gjr.chenlongwang.top

TS:   a && b || !c
来源：http://mpo.kuanghao11.cn

Java: a && b || !c
来源：http://pfr.jinghuilouyu.cn

Go:   a && b || !c
来源：http://ngq.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://qbm.hesvh.cn

C#:   a && b || !c
来源：http://wnz.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://cgk.wangdashe.top

Py:   if not data: return
来源：http://ewn.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://dpg.dashuyun.cn

JS:   if (!data) return;
来源：http://qvm.chenlongwang.top

TS:   if (!data) return;
来源：http://tll.hongshengwenyu.top

Java: if (data == null) return;
来源：http://klj.yangfankeji.com

Go:   if data == nil { return }
来源：http://wzq.shuidangran.top

Ruby: return if data.nil?
来源：http://ygv.zhoulong.xyz

C#:   if (data == null) return;
来源：http://jxs.zhijiandao.cn

================================================================================
来源：http://zjg.tarul.cn

C. 函数与作用域
来源：http://pof.chenlongwang.top

================================================================================
来源：http://nbm.yangfankeji.com

[C01] 定义函数
来源：http://cjq.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://gsb.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bpg.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://khs.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hbo.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uii.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://rom.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://jxv.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mwb.zhixingplan.top

[C02] 默认参数
来源：http://ujy.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://ilx.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zrk.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://siq.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xpx.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://aal.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wcd.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://szx.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://aqt.redwolf501.top

[C03] 可变参数
来源：http://dyi.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://toy.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gqy.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fee.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnt.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mre.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rjr.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lcw.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pkv.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://pyl.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nsd.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gej.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ncv.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cda.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://olj.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://dbk.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://ijw.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://bnu.epnwcf.com

[C05] 返回多个值
来源：http://cmj.daria6918.cn

Py:   return a, b
来源：http://soq.cqqwz.cn

PHP:  return [$a, $b];
来源：http://xru.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fdh.sweek.top

TS:   return { a, b };
来源：http://bww.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xej.yongpay.top

Go:   return a, b
来源：http://bhz.fanxiaobao.xyz

Ruby: return a, b
来源：http://tht.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://qsh.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://ohz.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://fpr.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sux.ctjpmb.com

JS:   const square = x => x * x;
来源：http://smu.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://lkn.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ays.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eaj.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://sxw.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://dsl.xinyue.icu

[C07] 把函数作为参数传入
来源：http://jnt.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cjb.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zrh.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zda.mhx1999.top

TS:   arr.map(String)
来源：http://fsa.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://raw.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://abi.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://dtn.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://tco.316326.xyz

[C08] 闭包
来源：http://lro.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wwn.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cxq.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fwa.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sdf.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gns.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uhf.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wco.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://can.xuetiantiany.cn

[C09] 递归
来源：http://mft.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yhf.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zpo.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbg.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iuv.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oxu.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vbd.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qio.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kzs.yj20258888.top

[C10] 变量作用域
来源：http://rxr.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aux.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yie.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vpr.gaohongyu789.top

TS:   同 JS
来源：http://div.fzhhl.top

Java: 方法内为块级作用域
来源：http://skw.daxiang520.top

Go:   花括号块级作用域
来源：http://ydt.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pds.cqqwz.cn

C#:   块级作用域
来源：http://ndl.zhongyouzk.top

[C11] 模块导入与导出
来源：http://fcy.dashuyun.cn

Py:   from module import func
来源：http://evq.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://odl.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nfg.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xdg.nanxuanxn.top

Java: import java.util.List;
来源：http://zbg.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aph.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://afc.yuanzhike.top

C#:   using System.Text;
来源：http://kas.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://zxv.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://ipj.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://qkk.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://tdw.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://bnd.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mci.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://bdm.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://pyf.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://quc.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://hvs.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://thf.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://soy.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ihj.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tan.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ssr.havefunace.top

Go:   func add(a, b int) int
来源：http://gzr.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xaq.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://fpy.hnxiangtu.top

[C14] 泛型函数
来源：http://gxp.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ppo.pycfn.com

PHP:  // 无泛型
来源：http://lvv.hesvh.cn

JS:   // 无泛型
来源：http://yjc.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kgi.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tgu.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://omb.aibaodan.cn

Ruby: # 无泛型
来源：http://roi.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kzz.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://nqy.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ngs.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://osa.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rtu.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://chb.aibaodan.cn

Java: // 无解构
来源：http://xcn.sufxvd.cn

Go:   // 无解构
来源：http://vys.jianghu66.top

Ruby: a, b = pair
来源：http://uev.fengsongda.top

C#:   var (a, b) = pair;
来源：http://txn.sysykeji.top

[C16] 函数 / 方法重载
来源：http://zlo.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cjj.jlsjyb.cn

PHP:  // 无重载
来源：http://xjy.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dcy.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://pox.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jrr.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://kqg.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://iso.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pwo.ydjk.org.cn

================================================================================
来源：http://kux.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://hxh.hesvh.cn

================================================================================
来源：http://gsd.cucudq.cn

[D01] 创建数组 / 列表
来源：http://hjr.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ods.ctjpmb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mtr.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ygw.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lkw.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qhr.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://zfb.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://jhy.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ddj.dianchejie.cn

[D02] 追加元素到末尾
来源：http://csa.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tsh.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lbp.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://elb.zhoulong.xyz

TS:   arr.push(4);
来源：http://wre.jinyuanbaomall.cn

Java: list.add(4);
来源：http://oui.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://vyq.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://odq.gogol.net.cn

C#:   list.Add(4);
来源：http://mos.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://ybo.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://uid.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kkh.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fth.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://duo.sjlbkw.cn

Java: list.add(0, 0);
来源：http://ohu.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://fpv.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zei.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://wgg.tianlin.xyz

[D04] 删除元素
来源：http://jkf.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uuj.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eyz.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://huk.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://ttk.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rvg.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zeo.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hse.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wyt.cheryme.top

[D05] 访问与修改元素
来源：http://wrx.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://alm.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nzd.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lqm.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://vvv.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://nqd.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://rmn.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wwe.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvo.xuanzx.com

[D06] 数组长度
来源：http://zew.hongshengwenyu.top

Py:   len(arr)
来源：http://gso.cqqwz.cn

PHP:  count($arr);
来源：http://gdq.guannengcc.top

JS:   arr.length
来源：http://jkh.52xcode.cn

TS:   arr.length
来源：http://ndm.hnqzz.top

Java: list.size();
来源：http://viq.pycfn.com

Go:   len(arr)
来源：http://yhs.bbcook.cn

Ruby: arr.length; arr.size
来源：http://uks.pengpengdd.cyou

C#:   list.Count;
来源：http://zrv.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://yhj.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iyv.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fjp.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://oxv.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://xcq.jinqigufen.top

Java: list.subList(1, 4);
来源：http://tep.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://opy.jqgfzy.top

Ruby: arr[1, 3]
来源：http://qth.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://fxj.jinqigufen.top

[D08] 合并两个数组
来源：http://lzr.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://xhb.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://cpj.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ilt.hywenlv.cn

TS:   [...a, ...b];
来源：http://kvq.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xki.iojbl.cn

Go:   append(a, b...)
来源：http://dhw.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://coo.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://ozk.gaohongyu789.top

[D09] 排序（升序）
来源：http://zoa.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://wvu.ehwqpu.com


<!-- 参考信息 -->