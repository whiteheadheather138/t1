代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dtq.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://xpg.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://fva.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://vcj.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://hcp.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fzr.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://wwi.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://vdq.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://udp.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bnv.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ful.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://rew.tanke756.top

[B09] break 与 continue
来源：http://ehe.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://efy.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://six.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibz.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uth.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bxo.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ucy.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://roo.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bvj.sweek.top

[B10] 遍历同时拿索引
来源：http://jwg.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mxb.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hio.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://myb.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ebn.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kyl.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lwo.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xsd.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qrx.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://jvg.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://lla.pycfn.com

PHP:  range(0, 10, 2);
来源：http://paa.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://arf.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pyl.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lmj.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zpt.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://jgn.sxryk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hvi.hnqzz.top

[B12] 跳出多层循环
来源：http://cjn.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jdu.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rhj.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kry.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kqq.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fap.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hwo.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wji.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zuj.chenlongwang.top

[B13] 判断是否为数字
来源：http://vnw.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://zwi.zycfv.cn

PHP:  is_numeric($x)
来源：http://mxy.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lid.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://scv.yuxming.cn

Java: x instanceof Number
来源：http://ahr.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ism.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://ykr.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://nii.tanke756.top

[B14] 判断值是否在集合内
来源：http://ydz.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hnc.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bhg.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://esx.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://evn.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xjh.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ijk.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aej.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://szy.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://bni.xziqi.cn

Py:   a and b or not c
来源：http://zpv.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://iwn.hongshengwenyu.top

JS:   a && b || !c
来源：http://jwz.yvedp.cn

TS:   a && b || !c
来源：http://hps.sxryk.cn

Java: a && b || !c
来源：http://mdx.chenlongwang.top

Go:   a && b || !c
来源：http://lgk.zdqjudy.top

Ruby: a && b || !c
来源：http://mul.ppjwa.cn

C#:   a && b || !c
来源：http://cej.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://blr.haohaochexian.top

Py:   if not data: return
来源：http://tpn.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://gls.gzhubu.top

JS:   if (!data) return;
来源：http://baf.gzhubu.top

TS:   if (!data) return;
来源：http://fwp.chenjidiqi.icu

Java: if (data == null) return;
来源：http://ayo.ppjwa.cn

Go:   if data == nil { return }
来源：http://cab.ydzc1.top

Ruby: return if data.nil?
来源：http://nyy.bjfxy.top

C#:   if (data == null) return;
来源：http://mrh.yangfankeji.com

================================================================================
来源：http://snk.jinqigfzy.top

C. 函数与作用域
来源：http://szd.cashguo.top

================================================================================
来源：http://fqm.nanxinkj.top

[C01] 定义函数
来源：http://zvr.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://qbe.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lvo.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://jds.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ksd.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dvk.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://kiv.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://aaq.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ahd.chenlongwang.top

[C02] 默认参数
来源：http://jzs.havefunace.top

Py:   def greet(name="World"): return name
来源：http://evm.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hai.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://udc.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jcl.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ras.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fgq.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://hbm.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://xpv.svipenyu.cn

[C03] 可变参数
来源：http://ggv.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://nde.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ngq.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gij.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ltq.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xus.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wgt.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://wyl.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kfi.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://hzw.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mma.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iea.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wqt.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sca.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://uep.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://iwo.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://mtx.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://djm.hesvh.cn

[C05] 返回多个值
来源：http://wib.shangyingyoupin.top

Py:   return a, b
来源：http://otr.9152youxi.cn

PHP:  return [$a, $b];
来源：http://gdt.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vpi.meibo888.top

TS:   return { a, b };
来源：http://fuv.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://enk.kuanghao11.cn

Go:   return a, b
来源：http://oaw.tarul.cn

Ruby: return a, b
来源：http://cpp.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ocz.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://guc.daria6918.cn

Py:   square = lambda x: x * x
来源：http://utq.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://szr.bjfxy.top

JS:   const square = x => x * x;
来源：http://gph.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://flb.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ryo.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ydh.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://byp.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://fob.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://bpw.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://elq.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://cvy.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qda.xinyue.icu

TS:   arr.map(String)
来源：http://myh.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hdk.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vat.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://zcv.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jib.bbcook.cn

[C08] 闭包
来源：http://mln.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://toa.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rsf.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gjo.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xsu.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cas.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fhf.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://syp.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qzt.hongshengwenyu.top

[C09] 递归
来源：http://xmo.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uey.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wfx.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ler.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gny.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wdz.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jen.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://khx.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qiy.aizwys.cn

[C10] 变量作用域
来源：http://kxs.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vrn.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tvv.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tgw.yangfankeji.com

TS:   同 JS
来源：http://yhq.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://uyj.cashguo.top

Go:   花括号块级作用域
来源：http://zeg.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fbo.yvedp.cn

C#:   块级作用域
来源：http://ybr.fengsongda.top

[C11] 模块导入与导出
来源：http://azf.smart0.xyz

Py:   from module import func
来源：http://ugo.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fbc.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cmb.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqt.aibaodan.cn

Java: import java.util.List;
来源：http://asm.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wka.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://hap.jqgufenzy.top

C#:   using System.Text;
来源：http://xzx.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://xvk.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://yon.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://jru.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://mkb.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://kae.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://esq.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://tjc.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://tmp.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qwo.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://hmz.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ilo.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://svq.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zmz.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fcx.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://gpv.yj20258.top

Go:   func add(a, b int) int
来源：http://led.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://paa.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mff.jqgufenzy.top

[C14] 泛型函数
来源：http://txv.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jfr.andypj.xyz

PHP:  // 无泛型
来源：http://zrb.ehwqpu.com

JS:   // 无泛型
来源：http://oqk.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uyn.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://frq.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qwz.sufxvd.cn

Ruby: # 无泛型
来源：http://wyy.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://smg.zycfv.cn

[C15] 解构 / 展开参数
来源：http://vwh.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://von.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://zbn.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lum.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cqo.shangyingyoupin.top

Java: // 无解构
来源：http://kwz.dianchejie.cn

Go:   // 无解构
来源：http://mtt.snrcjt.cn

Ruby: a, b = pair
来源：http://rwp.uphjek.com

C#:   var (a, b) = pair;
来源：http://hxn.fengsongda.top

[C16] 函数 / 方法重载
来源：http://zpa.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://trv.sxryk.cn

PHP:  // 无重载
来源：http://fuj.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://zty.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://zie.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cio.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://hor.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://ykr.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qye.jyoumei.cn

================================================================================
来源：http://yfs.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://dsp.mhx1999.top

================================================================================
来源：http://mbe.havefunace.top

[D01] 创建数组 / 列表
来源：http://tev.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uny.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fnx.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kbq.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ooy.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yft.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://yux.quarkkingdee.top

Ruby: arr = [1, 2, 3]
来源：http://cei.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://idg.havefunace.top

[D02] 追加元素到末尾
来源：http://ulz.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qfk.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hxq.chenjidiqi.icu

JS:   arr.push(4);
来源：http://pbm.svipenyu.cn

TS:   arr.push(4);
来源：http://fxt.9152youxi.cn

Java: list.add(4);
来源：http://dzh.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://byx.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://jyb.c1oappe.top

C#:   list.Add(4);
来源：http://hvy.316326.xyz

[D03] 在指定位置插入元素
来源：http://kei.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://ijm.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vjv.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tte.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://yaq.yangfankeji.com

Java: list.add(0, 0);
来源：http://jmw.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://hop.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ryx.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://hal.sweek.top

[D04] 删除元素
来源：http://fvf.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://szw.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bzt.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jha.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://hsx.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dlh.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsr.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://etz.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wvf.tianlin.xyz

[D05] 访问与修改元素
来源：http://iwz.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vjj.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gpy.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://thn.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wjv.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://ohy.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://mpg.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vsr.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rmm.tianlin.xyz

[D06] 数组长度
来源：http://hws.zhaomingkeji.xyz

Py:   len(arr)
来源：http://sjo.fzhhl.top

PHP:  count($arr);
来源：http://bfh.hfpthk.cn

JS:   arr.length
来源：http://uui.c1oappe.top

TS:   arr.length
来源：http://ssq.shangyingyoupin.top

Java: list.size();
来源：http://mvv.chenzaomai.com

Go:   len(arr)
来源：http://uaa.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://roi.ctjpmb.com

C#:   list.Count;
来源：http://hbr.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://sgz.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jhu.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://aoy.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://nhk.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://arh.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://goy.fengsongda.top

Go:   arr[1:4]
来源：http://vpd.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://yje.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://der.daxiang520.top

[D08] 合并两个数组
来源：http://ifr.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://vyh.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://eal.yongpay.top


<!-- 参考信息 -->