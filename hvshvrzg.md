代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sar.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iek.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://spt.tianlin.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jag.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dzy.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qpc.hnqzz.top

[B07] while 循环
来源：http://sja.daxiang520.top

Py:   while i < 10: i += 1
来源：http://zwz.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://aly.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://nwg.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://qfj.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://dbq.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kyq.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://bqm.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://lxu.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://wfg.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://hnt.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tqr.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://tbz.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://gat.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://may.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lvn.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://jik.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://olq.jiagoushi.top

[B09] break 与 continue
来源：http://xws.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://clx.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mbs.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trl.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isx.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ous.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ify.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nxg.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zii.daria6918.cn

[B10] 遍历同时拿索引
来源：http://xev.shanyushiyangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://umt.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://orj.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xhb.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ocg.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jsa.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yqq.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dpy.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://quc.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://nmr.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://vlc.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://gbr.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ast.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://buk.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lwa.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://odu.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://awh.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vfo.ivvv.top

[B12] 跳出多层循环
来源：http://izo.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uqc.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zvb.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://itd.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://csc.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ezb.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vfp.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yfm.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hdm.ydjk.org.cn

[B13] 判断是否为数字
来源：http://hsa.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://jcw.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://iwe.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://buu.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://utc.yanxiufei.cn

Java: x instanceof Number
来源：http://gog.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tbv.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://ayq.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://udc.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://nwb.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qiu.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yxz.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://rnh.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://epf.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dxj.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wqm.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ccp.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aun.tanke756.top

[B15] 布尔运算与取反
来源：http://dsn.nanxuanxn.top

Py:   a and b or not c
来源：http://alx.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://gtj.smart0.xyz

JS:   a && b || !c
来源：http://vxj.ydzc1.top

TS:   a && b || !c
来源：http://hds.fktsv.cn

Java: a && b || !c
来源：http://gfu.ppjwa.cn

Go:   a && b || !c
来源：http://jbp.xziqi.cn

Ruby: a && b || !c
来源：http://axg.gotoacloud.top

C#:   a && b || !c
来源：http://alj.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wsq.nanxinkj.top

Py:   if not data: return
来源：http://xos.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://fln.jianghu66.top

JS:   if (!data) return;
来源：http://mpl.sxryk.cn

TS:   if (!data) return;
来源：http://kyw.daxiang520.top

Java: if (data == null) return;
来源：http://shj.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://rvd.ehwqpu.com

Ruby: return if data.nil?
来源：http://ddx.sjlbkw.cn

C#:   if (data == null) return;
来源：http://ukc.52xcode.cn

================================================================================
来源：http://ldo.jinyuanbaomall.cn

C. 函数与作用域
来源：http://hqz.zhongyouzk.top

================================================================================
来源：http://wos.vehdjk.com

[C01] 定义函数
来源：http://kky.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://fom.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kuu.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://bng.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mfr.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tex.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rey.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://aqp.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rhm.gaohongyu789.top

[C02] 默认参数
来源：http://ykj.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://byu.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jhl.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://oxr.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kaf.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bcw.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nau.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://hmp.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://vkk.zdqjudy.top

[C03] 可变参数
来源：http://vhq.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://vih.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jmx.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://epu.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pvl.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rld.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://epz.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://zmp.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oad.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://qny.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vme.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vpt.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ldj.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://btu.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://xbx.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://udg.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://cfj.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://oqs.tarul.cn

[C05] 返回多个值
来源：http://ink.yvedp.cn

Py:   return a, b
来源：http://qdx.ehwqpu.com

PHP:  return [$a, $b];
来源：http://crm.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pyy.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://tte.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfo.vehdjk.com

Go:   return a, b
来源：http://sbu.yangfankeji.com

Ruby: return a, b
来源：http://mij.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://owc.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://eqz.fengsongda.top

Py:   square = lambda x: x * x
来源：http://nku.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://znv.ivvv.top

JS:   const square = x => x * x;
来源：http://ggc.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://nuc.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qpt.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oee.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://luq.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uro.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://ulh.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zpa.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://dkr.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dcd.yvedp.cn

TS:   arr.map(String)
来源：http://bky.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://duv.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xpi.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://xmt.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oxq.gzhubu.top

[C08] 闭包
来源：http://ikh.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hso.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tix.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wvg.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pvt.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bix.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kfs.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://soo.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pgf.yj20258888.top

[C09] 递归
来源：http://fcw.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zgd.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eii.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://abc.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ulr.hesvh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ggb.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uvi.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xfl.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gmg.haohaochexian.top

[C10] 变量作用域
来源：http://ref.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qks.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eeb.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nuq.jlsjyb.cn

TS:   同 JS
来源：http://gop.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://yjw.ydzc1.top

Go:   花括号块级作用域
来源：http://ayu.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ezt.zycfv.cn

C#:   块级作用域
来源：http://nrf.hysaishi.cn

[C11] 模块导入与导出
来源：http://toj.tian-w.cn

Py:   from module import func
来源：http://cxc.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://oqf.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kzu.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qtz.iojbl.cn

Java: import java.util.List;
来源：http://pro.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gpp.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://boo.aibaodan.cn

C#:   using System.Text;
来源：http://vzn.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://axi.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://fhx.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://zjt.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://kqn.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://lcj.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ndv.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://ost.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://ucf.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://epm.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://fec.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gpa.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dvv.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dci.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vbc.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fel.guowangkeji.top

Go:   func add(a, b int) int
来源：http://xoo.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kjh.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://hfn.pycfn.com

[C14] 泛型函数
来源：http://lbk.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hso.zhiwuduotai.top

PHP:  // 无泛型
来源：http://biy.zdbjq.cn

JS:   // 无泛型
来源：http://yas.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yoy.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qsq.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wsw.0kj1m.cn

Ruby: # 无泛型
来源：http://ndb.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lcg.tanke756.top

[C15] 解构 / 展开参数
来源：http://awx.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://agb.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://izc.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iex.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://unk.yuxming.cn

Java: // 无解构
来源：http://bxq.yj202588.top

Go:   // 无解构
来源：http://ocg.yuanzhike.top

Ruby: a, b = pair
来源：http://uaq.aizwys.cn

C#:   var (a, b) = pair;
来源：http://wif.fktsv.cn

[C16] 函数 / 方法重载
来源：http://bfv.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qqa.xziqi.cn

PHP:  // 无重载
来源：http://frt.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fjv.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://hna.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qvw.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://qth.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://hry.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://axi.shzxlz.cn

================================================================================
来源：http://dov.tanke756.top

D. 数组 / 列表 / 集合
来源：http://qct.aibaodan.cn

================================================================================
来源：http://vou.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://yxt.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://apl.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://koq.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://glu.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cxj.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kiw.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://owk.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://bbw.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://efn.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://vhc.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ubo.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lac.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://nsl.316326.xyz

TS:   arr.push(4);
来源：http://wug.9152youxi.cn

Java: list.add(4);
来源：http://eki.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://muh.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://ezf.52xcode.cn

C#:   list.Add(4);
来源：http://yqo.tarul.cn

[D03] 在指定位置插入元素
来源：http://vek.cheryme.top

Py:   arr.insert(0, 0)
来源：http://zol.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://emc.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eaf.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://vxl.birdmap.top

Java: list.add(0, 0);
来源：http://zcj.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yfn.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wci.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://opl.shanyushiyangkeji.top

[D04] 删除元素
来源：http://saq.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zro.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cns.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nyr.meibo888.top

TS:   arr.splice(0, 1);
来源：http://fao.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ivt.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vbu.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zbx.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nio.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://xgr.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pak.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qxf.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mlo.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://xob.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://oqf.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://oxb.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zdy.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nkt.cqqwz.cn

[D06] 数组长度
来源：http://zrv.316326.xyz

Py:   len(arr)
来源：http://jzk.bjfxy.top

PHP:  count($arr);
来源：http://qin.yongpay.top

JS:   arr.length
来源：http://sgc.gogol.net.cn

TS:   arr.length
来源：http://zzv.redwolf501.top

Java: list.size();
来源：http://sxd.epnwcf.com

Go:   len(arr)
来源：http://nop.iojbl.cn

Ruby: arr.length; arr.size
来源：http://uma.fehbvm.com

C#:   list.Count;
来源：http://iqx.sysykeji.top


<!-- 参考信息 -->