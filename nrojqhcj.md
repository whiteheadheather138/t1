代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://brf.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vlg.c1oappe.top

[B07] while 循环
来源：http://ecz.52xcode.cn

Py:   while i < 10: i += 1
来源：http://zuc.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://tvx.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://wps.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://xcb.yongpay.top

Java: while (i < 10) { i++; }
来源：http://uir.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dzh.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://feg.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://coh.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://feu.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://sdg.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cqd.zhengqikj.top

JS:   do { i++; } while (i < 10);
来源：http://dsx.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://tfi.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://evf.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jla.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://wwt.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://zlm.0kj1m.cn

[B09] break 与 continue
来源：http://fdf.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bhr.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://urc.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plz.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sif.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fep.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wos.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aid.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozm.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://lpd.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qga.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://duz.snrcjt.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rmd.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://szl.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qta.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fnv.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qij.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hjs.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://jsr.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://yzp.tanke756.top

PHP:  range(0, 10, 2);
来源：http://ofz.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqe.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rmy.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vov.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lmx.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://owq.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://utp.andypj.xyz

[B12] 跳出多层循环
来源：http://stt.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ctp.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pip.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fvz.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://atk.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lht.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iei.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://knj.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fge.vqdsnc.cn

[B13] 判断是否为数字
来源：http://njo.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://euv.snrcjt.cn

PHP:  is_numeric($x)
来源：http://nsx.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bbl.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oos.cdnleiting.top

Java: x instanceof Number
来源：http://qce.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bse.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://fak.epnwcf.com

C#:   x is int or double or decimal
来源：http://pjr.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://mfy.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wax.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jrp.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://nri.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://svv.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xla.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jcu.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rkm.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgn.daxiang520.top

[B15] 布尔运算与取反
来源：http://der.meibo888.top

Py:   a and b or not c
来源：http://fxs.hesvh.cn

PHP:  $a && $b || !$c
来源：http://vzv.52xcode.cn

JS:   a && b || !c
来源：http://tmp.tian-w.cn

TS:   a && b || !c
来源：http://wgi.gaohongyu789.top

Java: a && b || !c
来源：http://odn.xuetiantiany.cn

Go:   a && b || !c
来源：http://gnd.shangyingyoupin.top

Ruby: a && b || !c
来源：http://wpq.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://ben.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://uon.epnwcf.com

Py:   if not data: return
来源：http://msb.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://ihy.gogol.net.cn

JS:   if (!data) return;
来源：http://bay.hywenlv.cn

TS:   if (!data) return;
来源：http://jxo.pengpengdd.cyou

Java: if (data == null) return;
来源：http://xpu.jinqigufen.top

Go:   if data == nil { return }
来源：http://kdw.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://wir.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://uyf.xziqi.cn

================================================================================
来源：http://upw.316326.xyz

C. 函数与作用域
来源：http://nog.daxiang520.top

================================================================================
来源：http://cxk.mhx1999.top

[C01] 定义函数
来源：http://hko.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://hca.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://raa.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://kst.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ovl.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bxv.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ckw.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://iyb.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eht.birdmap.top

[C02] 默认参数
来源：http://qgr.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://xzx.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hmc.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://oer.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jvs.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qhn.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://asz.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://hjm.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://bqi.cashguo.top

[C03] 可变参数
来源：http://thi.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://xji.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vac.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxs.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fgr.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bfj.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://koc.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://ist.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dzq.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://lup.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://agr.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kmz.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uyc.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iat.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://zqw.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://ews.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://gdd.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://ymg.fanxiaobao.xyz

[C05] 返回多个值
来源：http://adz.yj202588.top

Py:   return a, b
来源：http://nqq.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://akw.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://agn.chenzaomai.com

TS:   return { a, b };
来源：http://hww.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aed.zhoulong.xyz

Go:   return a, b
来源：http://xsj.zhengqikj.top

Ruby: return a, b
来源：http://fca.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://iit.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://rop.hnqzz.top

Py:   square = lambda x: x * x
来源：http://cvj.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://orw.yonumen.top

JS:   const square = x => x * x;
来源：http://fdn.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://aeu.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lja.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rkt.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://ysk.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rud.bbcook.cn

[C07] 把函数作为参数传入
来源：http://uht.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://let.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://duu.sysykeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iiu.xuetiantiany.cn

TS:   arr.map(String)
来源：http://lre.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xmx.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lnd.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://bim.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iau.vehdjk.com

[C08] 闭包
来源：http://hzx.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://thp.yuanzhike.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uvk.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ykt.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vxs.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pln.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xvl.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oiy.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xcm.zhoulong.xyz

[C09] 递归
来源：http://doa.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ewm.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsv.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvm.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ime.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eyz.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tck.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fwl.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://srq.zhiwuduotai.top

[C10] 变量作用域
来源：http://sfr.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hsk.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fgt.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://osp.havefunace.top

TS:   同 JS
来源：http://hgq.guowangkeji.top

Java: 方法内为块级作用域
来源：http://qdj.zhongyouzk.top

Go:   花括号块级作用域
来源：http://bdg.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pcq.hammf.cn

C#:   块级作用域
来源：http://smo.sjlbkw.cn

[C11] 模块导入与导出
来源：http://ixj.snrcjt.cn

Py:   from module import func
来源：http://ztw.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vne.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vka.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kfs.shzxlz.cn

Java: import java.util.List;
来源：http://jmz.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oup.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://wfm.chenlongwang.top

C#:   using System.Text;
来源：http://kox.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://dmh.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://xlh.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://hpc.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://fko.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://dyr.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lcx.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://mnb.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://njt.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://mtr.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://mei.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lvu.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ahh.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://urq.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kzs.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://awk.yj20258888.top

Go:   func add(a, b int) int
来源：http://pkg.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rwc.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pqy.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://hqj.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ewf.xziqi.cn

PHP:  // 无泛型
来源：http://snq.ydjk.org.cn

JS:   // 无泛型
来源：http://vfv.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://min.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yyn.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ejc.hcnkem.com

Ruby: # 无泛型
来源：http://axv.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dle.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://ouk.hysaishi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qgz.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://sln.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fvt.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xpe.wangshuangyany.cn

Java: // 无解构
来源：http://bdh.yj20258888.top

Go:   // 无解构
来源：http://rlu.jlsjyb.cn

Ruby: a, b = pair
来源：http://rdq.havefunace.top

C#:   var (a, b) = pair;
来源：http://gga.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://bjl.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dtq.hfpthk.cn

PHP:  // 无重载
来源：http://etm.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://owa.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://div.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iqc.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://wsg.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://wlp.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://iex.yj202588.top

================================================================================
来源：http://xub.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://gdh.shanyushiyangkeji.top

================================================================================
来源：http://fdw.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://ezr.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wuw.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://grf.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://umz.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://rwo.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://thd.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://owm.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://ogf.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xrp.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://yra.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hjm.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dmt.yfazqb.com

JS:   arr.push(4);
来源：http://mcr.yongpay.top

TS:   arr.push(4);
来源：http://def.dianchejie.cn

Java: list.add(4);
来源：http://zyx.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://fkd.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://xfy.gogol.net.cn

C#:   list.Add(4);
来源：http://ylp.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://xee.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://gyh.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sus.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dau.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://ufg.tanke756.top

Java: list.add(0, 0);
来源：http://zyk.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kav.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sit.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://ffh.jianghu66.top

[D04] 删除元素
来源：http://yjd.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jdo.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://joj.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://syw.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://cmq.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yny.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aci.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zqf.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tvs.yonumen.top

[D05] 访问与修改元素
来源：http://dtg.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bot.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wbl.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ful.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://nsx.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://wff.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://wgw.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xdt.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ajl.sxryk.cn

[D06] 数组长度
来源：http://uxa.tanke756.top

Py:   len(arr)
来源：http://qwc.316326.xyz

PHP:  count($arr);
来源：http://yyl.tarul.cn

JS:   arr.length
来源：http://gos.ywan-chungtsiang.top

TS:   arr.length
来源：http://dvd.xuetiantiany.cn

Java: list.size();
来源：http://sxe.shanyushiyangtech.top

Go:   len(arr)
来源：http://ozd.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://fwt.yj202588.top

C#:   list.Count;
来源：http://tpe.daria6918.cn

[D07] 切片 / 取子数组
来源：http://evp.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://chl.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nop.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://sxn.cucudq.cn


<!-- 参考信息 -->