代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dmd.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zda.chenlongwang.top

[B07] while 循环
来源：http://voz.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://qzu.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://kac.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://nlt.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://bdy.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://qfo.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qqj.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://kkz.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://xvc.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://vep.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://aoi.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uue.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://wgi.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://ldh.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://qzb.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nuk.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://wif.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://adj.uphjek.com

[B09] break 与 continue
来源：http://enr.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wtj.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uqd.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igv.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzb.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bmu.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wgx.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bwy.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkx.bbcook.cn

[B10] 遍历同时拿索引
来源：http://yiq.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ulo.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fni.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ljm.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ytp.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jja.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://egz.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tmk.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://flu.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://vpj.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://xae.yj20258.top

PHP:  range(0, 10, 2);
来源：http://zyw.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kzc.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wdp.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cyi.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gez.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://amy.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://igq.yuanzhike.top

[B12] 跳出多层循环
来源：http://ygf.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ida.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zwv.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbv.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqx.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mji.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ora.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ewi.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iuq.dashuyun.cn

[B13] 判断是否为数字
来源：http://eha.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://lcd.yvedp.cn

PHP:  is_numeric($x)
来源：http://wub.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jux.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sud.fanxiaobao.xyz

Java: x instanceof Number
来源：http://gvz.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wmp.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://mzz.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://drw.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://rln.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mzr.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tci.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://kke.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://fau.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rpc.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://caw.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ecn.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://otq.meibo888.top

[B15] 布尔运算与取反
来源：http://sud.nanxinkj.top

Py:   a and b or not c
来源：http://pwj.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://wxt.yuxming.cn

JS:   a && b || !c
来源：http://lis.bbcook.cn

TS:   a && b || !c
来源：http://cei.yongpay.top

Java: a && b || !c
来源：http://ztk.fengsongda.top

Go:   a && b || !c
来源：http://uiw.gogol.net.cn

Ruby: a && b || !c
来源：http://hco.iojbl.cn

C#:   a && b || !c
来源：http://dqq.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ysi.dashuyun.cn

Py:   if not data: return
来源：http://ddi.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://ydg.bjfxy.top

JS:   if (!data) return;
来源：http://cqf.tanke756.top

TS:   if (!data) return;
来源：http://qrl.ppjwa.cn

Java: if (data == null) return;
来源：http://edo.52xcode.cn

Go:   if data == nil { return }
来源：http://nca.mhx1999.top

Ruby: return if data.nil?
来源：http://olb.hnqzz.top

C#:   if (data == null) return;
来源：http://hhi.birdmap.top

================================================================================
来源：http://vbx.daxiang520.top

C. 函数与作用域
来源：http://rrg.dianchejie.cn

================================================================================
来源：http://dsm.nanxuanxn.top

[C01] 定义函数
来源：http://blv.hammf.cn

Py:   def add(a, b): return a + b
来源：http://exw.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xmo.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://ndt.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwj.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xlw.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://qyt.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://cfx.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://llz.jqgfzy.top

[C02] 默认参数
来源：http://qzo.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://ych.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://icp.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://was.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://adm.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gij.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dgl.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://hyn.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://svh.quarkkingdee.top

[C03] 可变参数
来源：http://mfn.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://xda.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iec.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lff.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnx.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yfc.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rnl.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wcq.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://znb.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://ubc.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ptq.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kem.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tgc.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://spe.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://mxm.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://dgl.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://tmz.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://kyc.nanxinkj.top

[C05] 返回多个值
来源：http://ems.jqgfzy.top

Py:   return a, b
来源：http://qyn.jiagoushi.top

PHP:  return [$a, $b];
来源：http://amq.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wwo.aizwys.cn

TS:   return { a, b };
来源：http://xlf.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jil.iojbl.cn

Go:   return a, b
来源：http://ure.nanxinkj.top

Ruby: return a, b
来源：http://jpg.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://abp.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://klv.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://svw.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xwt.9152youxi.cn

JS:   const square = x => x * x;
来源：http://xcf.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://kve.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://htw.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://ijf.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://oor.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://efl.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://leg.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://diu.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://ooz.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lvu.havefunace.top

TS:   arr.map(String)
来源：http://vrg.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uys.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aam.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://pux.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bsk.shzxlz.cn

[C08] 闭包
来源：http://naa.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pqt.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ezk.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jws.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://caj.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hai.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kbv.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://icg.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://adu.316326.xyz

[C09] 递归
来源：http://vlv.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wls.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kft.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xow.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lii.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ffb.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rgz.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzv.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fms.epnwcf.com

[C10] 变量作用域
来源：http://ggs.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vkg.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://txe.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fkf.vehdjk.com

TS:   同 JS
来源：http://ngy.shzxlz.cn

Java: 方法内为块级作用域
来源：http://uni.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://rpz.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sio.yangfankeji.com

C#:   块级作用域
来源：http://jhx.yvedp.cn

[C11] 模块导入与导出
来源：http://qgg.jinyuanbaomall.cn

Py:   from module import func
来源：http://aco.hfpthk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mvl.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://umu.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kvz.zhengqikj.top

Java: import java.util.List;
来源：http://lzv.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wvu.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://orh.zhijiandao.cn

C#:   using System.Text;
来源：http://njl.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://zat.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://yxp.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://wmn.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://oaf.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://xrg.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lrv.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://tcp.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://ojn.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zoq.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://nod.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nzs.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxk.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zjp.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vkz.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hey.dashuyun.cn

Go:   func add(a, b int) int
来源：http://nvb.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://edr.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://xfv.yuxming.cn

[C14] 泛型函数
来源：http://uer.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vcb.iojbl.cn

PHP:  // 无泛型
来源：http://onk.zhiwuduotai.top

JS:   // 无泛型
来源：http://clu.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ilj.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bgt.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oet.andypj.xyz

Ruby: # 无泛型
来源：http://prp.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eaz.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://hzn.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sbd.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://hpt.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dpd.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://udn.zhijiandao.cn

Java: // 无解构
来源：http://avy.cdnleiting.top

Go:   // 无解构
来源：http://gxz.jqgufenzy.top

Ruby: a, b = pair
来源：http://tka.hammf.cn

C#:   var (a, b) = pair;
来源：http://pby.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://aot.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jfj.ppjwa.cn

PHP:  // 无重载
来源：http://pqi.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://kbo.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://gnc.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wse.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://wjn.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://ylb.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mds.fzhhl.top

================================================================================
来源：http://hjv.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://ckw.birdmap.top

================================================================================
来源：http://gqz.fzhhl.top

[D01] 创建数组 / 列表
来源：http://rqb.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sky.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ees.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fuq.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ods.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uow.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://wfq.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://tvj.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mkg.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://cjk.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lnl.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eca.zdbjq.cn

JS:   arr.push(4);
来源：http://xmv.hammf.cn

TS:   arr.push(4);
来源：http://tdg.aizwys.cn

Java: list.add(4);
来源：http://jmd.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://tvf.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://tod.feifeiyinyue.top

C#:   list.Add(4);
来源：http://ylt.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://kdr.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://mta.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zom.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yda.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://csb.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://reb.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://qeg.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ajx.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://ipy.shanyushiyangkeji.top

[D04] 删除元素
来源：http://prm.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lto.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eye.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dhg.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://jkh.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jus.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qud.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mam.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nyp.jianghu66.top

[D05] 访问与修改元素
来源：http://cpj.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ign.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://txw.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://foc.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://xyz.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://qjb.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://nua.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://chn.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ofz.cdnleiting.top

[D06] 数组长度
来源：http://bkw.jqgfzy.top

Py:   len(arr)
来源：http://zsg.feifeiyinyue.top

PHP:  count($arr);
来源：http://zen.gaohongyu789.top

JS:   arr.length
来源：http://xdu.yfazqb.com

TS:   arr.length
来源：http://khy.yongpay.top

Java: list.size();
来源：http://gcg.chenlongwang.top

Go:   len(arr)
来源：http://wpd.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://xhn.xylfe.cn

C#:   list.Count;
来源：http://dnq.gzhubu.top

[D07] 切片 / 取子数组
来源：http://dzz.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gbb.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fsx.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://vis.daxiang520.top


<!-- 参考信息 -->