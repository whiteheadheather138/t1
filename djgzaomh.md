代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ihi.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://fwg.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://cyz.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://gul.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://iuz.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://iem.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://eqr.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://yzw.ivvv.top

Java: do { i++; } while (i < 10);
来源：http://iem.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fad.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://cei.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://zmk.hesvh.cn

[B09] break 与 continue
来源：http://zrs.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kub.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://djk.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsv.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mfi.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abk.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lha.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aiv.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzp.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://ype.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nou.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vcb.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xrq.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bxa.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ess.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ubg.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zbt.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pbx.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://bed.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://pvo.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://hsg.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gcq.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lso.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://otk.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ttg.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://gyc.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wjr.nanxinkj.top

[B12] 跳出多层循环
来源：http://afi.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nqa.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qad.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgw.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ghz.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pcd.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cpw.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jcf.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wdh.yuxming.cn

[B13] 判断是否为数字
来源：http://ohn.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://gbl.ydzc1.top

PHP:  is_numeric($x)
来源：http://sfk.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ilo.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pgf.yvedp.cn

Java: x instanceof Number
来源：http://fcl.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://upt.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://dyq.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://lok.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://uoa.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yox.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dyr.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://gyu.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://jsi.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bfm.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fyy.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://lss.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gam.guannengcc.top

[B15] 布尔运算与取反
来源：http://jjd.jianghu66.top

Py:   a and b or not c
来源：http://vii.hcnkem.com

PHP:  $a && $b || !$c
来源：http://spc.yonumen.top

JS:   a && b || !c
来源：http://upc.pycfn.com

TS:   a && b || !c
来源：http://ion.dashuyun.cn

Java: a && b || !c
来源：http://nse.ivvv.top

Go:   a && b || !c
来源：http://trw.daxiang520.top

Ruby: a && b || !c
来源：http://syn.jiagoushi.top

C#:   a && b || !c
来源：http://hyc.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ywo.tian-w.cn

Py:   if not data: return
来源：http://cag.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://tcz.haohaochexian.top

JS:   if (!data) return;
来源：http://etm.uphjek.com

TS:   if (!data) return;
来源：http://dra.haohaochexian.top

Java: if (data == null) return;
来源：http://srf.pycfn.com

Go:   if data == nil { return }
来源：http://whq.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://wae.hcnkem.com

C#:   if (data == null) return;
来源：http://hmr.bjfxy.top

================================================================================
来源：http://okd.kuanghao11.cn

C. 函数与作用域
来源：http://asw.hcnkem.com

================================================================================
来源：http://szp.bjfxy.top

[C01] 定义函数
来源：http://vpa.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://vcn.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vmk.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ped.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqe.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lpb.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eef.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://wws.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ses.guannengcc.top

[C02] 默认参数
来源：http://fte.hammf.cn

Py:   def greet(name="World"): return name
来源：http://aif.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bft.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://euf.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gxn.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jwt.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qfm.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://orr.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://nef.tanke756.top

[C03] 可变参数
来源：http://vvq.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://exq.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jro.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ytz.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wyx.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wac.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://llx.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://uby.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mjs.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://hwr.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gdo.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tws.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zcl.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jra.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://nzx.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://dgz.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://cpv.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://nie.redwolf501.top

[C05] 返回多个值
来源：http://mci.feifeiyinyue.top

Py:   return a, b
来源：http://xzy.aibaodan.cn

PHP:  return [$a, $b];
来源：http://hfp.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xqt.hnqzz.top

TS:   return { a, b };
来源：http://vet.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oed.ydzc1.top

Go:   return a, b
来源：http://ayj.shanyushiyangkeji.top

Ruby: return a, b
来源：http://qhs.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://sep.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://eut.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://cjy.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kmn.shzxlz.cn

JS:   const square = x => x * x;
来源：http://uxf.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://vdj.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ntv.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vft.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://obm.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hfp.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://cfy.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ars.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jfi.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yia.kuanghao11.cn

TS:   arr.map(String)
来源：http://hpz.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://anu.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qcz.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://oyn.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rdo.ivvv.top

[C08] 闭包
来源：http://mfw.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yhd.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fmz.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://epk.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gzh.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://twm.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pja.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dku.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://idt.yanxiufei.cn

[C09] 递归
来源：http://wvt.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jhz.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svt.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvp.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mwv.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://caz.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ipp.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ulc.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zwh.snrcjt.cn

[C10] 变量作用域
来源：http://lzc.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ira.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gii.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bfi.xuanzx.com

TS:   同 JS
来源：http://hbb.guannengcc.top

Java: 方法内为块级作用域
来源：http://ckj.jqgufenzy.top

Go:   花括号块级作用域
来源：http://wpa.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mwx.xziqi.cn

C#:   块级作用域
来源：http://uro.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://wls.cdnleiting.top

Py:   from module import func
来源：http://kfb.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cxr.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://akq.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://txl.guannengcc.top

Java: import java.util.List;
来源：http://fqa.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gzd.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://qeu.zhengqikj.top

C#:   using System.Text;
来源：http://pcd.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://pdi.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://nsq.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://lvy.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://ias.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://fmd.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gfr.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://gxz.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://jxn.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hgx.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://hbp.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uiw.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rjj.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nqe.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ovy.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vrr.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://nvg.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zll.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ygh.shzxlz.cn

[C14] 泛型函数
来源：http://oif.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dgk.jinqigufen.top

PHP:  // 无泛型
来源：http://xbj.fzhhl.top

JS:   // 无泛型
来源：http://yiu.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jpb.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vdd.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ybq.guannengcc.top

Ruby: # 无泛型
来源：http://zim.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xxh.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://ywg.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dex.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://qog.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zvz.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pvm.hywenlv.cn

Java: // 无解构
来源：http://bmy.cucudq.cn

Go:   // 无解构
来源：http://hyh.yuxming.cn

Ruby: a, b = pair
来源：http://xmv.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://aui.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://puj.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fmg.nanxinkj.top

PHP:  // 无重载
来源：http://unc.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nhs.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://nkw.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rmb.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://xex.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://ihj.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://csd.vqdsnc.cn

================================================================================
来源：http://xkl.birdmap.top

D. 数组 / 列表 / 集合
来源：http://nkp.cheryme.top

================================================================================
来源：http://yuh.yonumen.top

[D01] 创建数组 / 列表
来源：http://xib.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qub.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zdg.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yin.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bhg.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lnk.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://gee.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://lfe.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://viu.hysaishi.cn

[D02] 追加元素到末尾
来源：http://abx.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vqx.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qss.birdmap.top

JS:   arr.push(4);
来源：http://bow.sweek.top

TS:   arr.push(4);
来源：http://tbq.bjfxy.top

Java: list.add(4);
来源：http://jbo.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://ryx.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://byp.chenzaomai.com

C#:   list.Add(4);
来源：http://srp.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://pkr.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://aej.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kdy.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ror.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://vuh.sufxvd.cn

Java: list.add(0, 0);
来源：http://ozz.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wqo.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dfn.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://zct.aizwys.cn

[D04] 删除元素
来源：http://xgc.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eox.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ixe.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gva.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://zyo.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pxy.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jck.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aah.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lvp.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://jhg.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eck.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://orz.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gld.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://bxt.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://snu.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://ucr.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nrr.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://woi.wangdashe.top

[D06] 数组长度
来源：http://txb.fanxiaobao.xyz

Py:   len(arr)
来源：http://dzz.jianghu66.top

PHP:  count($arr);
来源：http://aig.jianghu66.top

JS:   arr.length
来源：http://ykj.zhongyouzk.top

TS:   arr.length
来源：http://wzr.daxiang520.top

Java: list.size();
来源：http://bjs.guowangkeji.top

Go:   len(arr)
来源：http://gem.daxiang520.top

Ruby: arr.length; arr.size
来源：http://pll.smart0.xyz

C#:   list.Count;
来源：http://ksr.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://buw.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yzy.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://zkm.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://bqx.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://vzm.zhixingplan.top

Java: list.subList(1, 4);
来源：http://itj.sjlbkw.cn

Go:   arr[1:4]
来源：http://qfv.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://wcn.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://gnl.jinqigufen.top

[D08] 合并两个数组
来源：http://kxl.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://cxm.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://uas.jinghuilouyu.cn


<!-- 参考信息 -->