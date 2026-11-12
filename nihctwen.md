代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wqj.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tpt.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://ypg.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sse.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://dlf.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://giq.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bbs.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://baa.wangdashe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mzz.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://eya.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ldv.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://rwx.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jay.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://ptz.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://srj.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hbr.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgg.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ykb.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dap.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://coy.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://abp.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nrx.0kj1m.cn

[B07] while 循环
来源：http://obf.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://cur.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pyz.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://mcc.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://bdp.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://qca.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wff.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://bud.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://vza.hammf.cn

[B08] do-while（至少执行一次）
来源：http://oiw.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://xhq.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qld.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://vhz.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://guo.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://xjp.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vri.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://plm.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://mdj.tianlin.xyz

[B09] break 与 continue
来源：http://nzn.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jwf.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bwq.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qna.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftk.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mut.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fep.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bgd.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtb.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://wbw.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ibe.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://flb.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zdl.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gxe.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://axz.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://scr.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zcx.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hms.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://lvd.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://sah.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://art.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmb.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hjd.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pah.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://npk.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://izi.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tzt.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://dyz.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zzw.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yxh.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddy.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://znl.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://quy.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://syx.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qrk.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xyx.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://ttr.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://euf.hywenlv.cn

PHP:  is_numeric($x)
来源：http://qkj.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qqo.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixd.ybcxt.top

Java: x instanceof Number
来源：http://lnf.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kbg.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://ghv.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://sic.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://ajm.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fkg.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cps.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://iky.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://ipt.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://emr.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jvh.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://lwu.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://voa.cdnleiting.top

[B15] 布尔运算与取反
来源：http://jqe.mhx1999.top

Py:   a and b or not c
来源：http://pxc.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://fef.yangfankeji.com

JS:   a && b || !c
来源：http://ayk.dianchejie.cn

TS:   a && b || !c
来源：http://rer.sufxvd.cn

Java: a && b || !c
来源：http://nbx.yangfankeji.com

Go:   a && b || !c
来源：http://xuj.sxryk.cn

Ruby: a && b || !c
来源：http://yxk.zhiwuduotai.top

C#:   a && b || !c
来源：http://utj.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kbx.shuidangran.top

Py:   if not data: return
来源：http://kkt.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://mnt.gogol.net.cn

JS:   if (!data) return;
来源：http://ayw.chenzaomai.com

TS:   if (!data) return;
来源：http://iji.hnxiangtu.top

Java: if (data == null) return;
来源：http://imz.sysykeji.top

Go:   if data == nil { return }
来源：http://zxm.gogol.net.cn

Ruby: return if data.nil?
来源：http://szf.gogol.net.cn

C#:   if (data == null) return;
来源：http://kvu.ehwqpu.com

================================================================================
来源：http://was.zhixingplan.top

C. 函数与作用域
来源：http://zeb.nanxuanxn.top

================================================================================
来源：http://pfw.pengpengdd.cyou

[C01] 定义函数
来源：http://pvy.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://esv.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fac.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ueg.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yun.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aia.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gxj.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://fxb.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zvv.yfazqb.com

[C02] 默认参数
来源：http://rzg.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://pec.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ddi.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://qth.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vud.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hgb.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ksb.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://hqj.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://enl.zhongyouzk.top

[C03] 可变参数
来源：http://mxu.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://wjr.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lpe.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://avp.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aro.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wof.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://szj.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wcm.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jcz.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://yji.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zmv.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fyh.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dxs.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kfb.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://dzb.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://zza.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://hni.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://vhv.vehdjk.com

[C05] 返回多个值
来源：http://tut.ywan-chungtsiang.top

Py:   return a, b
来源：http://fol.0kj1m.cn

PHP:  return [$a, $b];
来源：http://poj.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://agg.gotoacloud.top

TS:   return { a, b };
来源：http://kko.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fqu.chenzaomai.com

Go:   return a, b
来源：http://fpe.jqgufenzy.top

Ruby: return a, b
来源：http://cau.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://wld.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://nwo.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://azl.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zah.guannengcc.top

JS:   const square = x => x * x;
来源：http://gan.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://dhs.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rip.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://mqo.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://upu.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wtp.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://lti.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uxk.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jte.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sed.xylfe.cn

TS:   arr.map(String)
来源：http://cro.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://neu.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kpd.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://uoc.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iek.dashuyun.cn

[C08] 闭包
来源：http://bfm.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gyp.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rde.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wht.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yww.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mpd.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rqd.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zhp.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmr.hnxiangtu.top

[C09] 递归
来源：http://wbd.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ykr.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lca.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jdh.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hhr.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jmj.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zkt.dianchejie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jha.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ihh.cheryme.top

[C10] 变量作用域
来源：http://fvs.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cjw.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jrl.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gsz.tarul.cn

TS:   同 JS
来源：http://khk.vehdjk.com

Java: 方法内为块级作用域
来源：http://cwb.mhx1999.top

Go:   花括号块级作用域
来源：http://cie.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rmx.hongshengwenyu.top

C#:   块级作用域
来源：http://xdw.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://feh.hongshengwenyu.top

Py:   from module import func
来源：http://trc.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uxv.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://smp.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ueh.yueranfly.top

Java: import java.util.List;
来源：http://fhk.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ozh.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ryd.ydzc1.top

C#:   using System.Text;
来源：http://iui.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://bpr.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://aaz.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://dwl.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://mdg.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://vji.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hxq.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://gks.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://ylq.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://bow.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://qlw.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ybf.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qqo.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ybl.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kan.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lew.yonumen.top

Go:   func add(a, b int) int
来源：http://pyg.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dxo.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://ltu.sjlbkw.cn

[C14] 泛型函数
来源：http://zhv.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pvz.ctjpmb.com

PHP:  // 无泛型
来源：http://twg.chenzaomai.com

JS:   // 无泛型
来源：http://oxi.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://out.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bcu.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qlv.yfazqb.com

Ruby: # 无泛型
来源：http://dav.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eya.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://gyh.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hgf.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://mdo.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jpx.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pyk.hysaishi.cn

Java: // 无解构
来源：http://gbe.yongpay.top

Go:   // 无解构
来源：http://snf.smart0.xyz

Ruby: a, b = pair
来源：http://fyl.yueranfly.top

C#:   var (a, b) = pair;
来源：http://zim.hesvh.cn

[C16] 函数 / 方法重载
来源：http://mia.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://thw.hywenlv.cn

PHP:  // 无重载
来源：http://cqr.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jgj.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://xyn.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dul.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://sif.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://jwc.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xwl.andypj.xyz

================================================================================
来源：http://hby.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://rah.jlsjyb.cn

================================================================================
来源：http://lbz.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://cme.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rkx.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://drm.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ltd.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cjx.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmw.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://yfk.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://rnm.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mxx.chenzaomai.com

[D02] 追加元素到末尾
来源：http://clc.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lfp.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://shq.guowangkeji.top

JS:   arr.push(4);
来源：http://sdp.guannengcc.top

TS:   arr.push(4);
来源：http://hjg.yfazqb.com

Java: list.add(4);
来源：http://bzc.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://dqp.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://qpi.yj20258888.top

C#:   list.Add(4);
来源：http://uir.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://led.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://gda.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://obx.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ezr.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://wcz.jyoumei.cn

Java: list.add(0, 0);
来源：http://yar.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://xvt.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fgf.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://soh.guowangkeji.top

[D04] 删除元素
来源：http://uty.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lmg.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://brh.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rti.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://xce.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zsv.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jou.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kpq.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dxl.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://yfg.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hlz.ydzc1.top


<!-- 参考信息 -->