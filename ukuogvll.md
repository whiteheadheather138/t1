代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jho.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aph.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://vwn.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rlt.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://stz.birdmap.top

Py:   for item in arr: print(item)
来源：http://ury.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ojd.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rpk.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://opg.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dfk.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dnh.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://cls.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qrx.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://ckf.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eam.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bim.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://inz.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nxc.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gqu.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fha.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mso.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fhr.gzhubu.top

[B07] while 循环
来源：http://iwh.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://dgw.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vuj.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://lxz.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://bcf.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://jxh.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ugz.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://uqj.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://cfd.uphjek.com

[B08] do-while（至少执行一次）
来源：http://nxh.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://jik.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://pcw.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://cyd.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://yvc.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://hgf.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wmw.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rhk.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://dxf.bbcook.cn

[B09] break 与 continue
来源：http://vyn.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pxj.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgd.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agu.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhw.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ilt.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ycu.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://syv.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fui.ydzc1.top

[B10] 遍历同时拿索引
来源：http://pur.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://flf.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sfa.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vmd.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iuv.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fiq.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nti.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pcp.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oai.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://gse.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://oct.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://xmh.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nkb.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aha.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wex.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sih.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://qrv.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dlp.bbcook.cn

[B12] 跳出多层循环
来源：http://wog.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hxk.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://hjx.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ypj.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xdp.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eou.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://naw.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gmr.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oao.jqgfzy.top

[B13] 判断是否为数字
来源：http://qfq.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://bbi.chenzaomai.com

PHP:  is_numeric($x)
来源：http://gnh.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdk.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jfo.jlsjyb.cn

Java: x instanceof Number
来源：http://xqj.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nde.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://ncj.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://ita.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://dye.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vps.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xlz.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xhd.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://mku.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://roi.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mku.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://pzs.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kst.birdmap.top

[B15] 布尔运算与取反
来源：http://fdi.ybcxt.top

Py:   a and b or not c
来源：http://zwv.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://bfp.jinghuilouyu.cn

JS:   a && b || !c
来源：http://rso.jlsjyb.cn

TS:   a && b || !c
来源：http://lmg.snrcjt.cn

Java: a && b || !c
来源：http://iwf.meibo888.top

Go:   a && b || !c
来源：http://byv.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://jdz.zdqjudy.top

C#:   a && b || !c
来源：http://vcd.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zzd.zhiwuduotai.top

Py:   if not data: return
来源：http://tiq.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://byw.uphjek.com

JS:   if (!data) return;
来源：http://mxy.gzhubu.top

TS:   if (!data) return;
来源：http://esc.zdqjudy.top

Java: if (data == null) return;
来源：http://esj.gzhubu.top

Go:   if data == nil { return }
来源：http://lye.daxiang520.top

Ruby: return if data.nil?
来源：http://izc.jinqigfzy.top

C#:   if (data == null) return;
来源：http://bnm.jqgfzy.top

================================================================================
来源：http://odx.yueranfly.top

C. 函数与作用域
来源：http://zuq.gaohongyu789.top

================================================================================
来源：http://ywg.xuanzx.com

[C01] 定义函数
来源：http://guk.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://tmh.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aqi.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://win.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dfm.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oni.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vfj.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://ath.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uhv.havefunace.top

[C02] 默认参数
来源：http://ron.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://qhn.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://bsl.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://bch.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://taf.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pnx.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cqc.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://eee.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xxk.hongshengwenyu.top

[C03] 可变参数
来源：http://tbh.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://ivc.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://muj.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ekv.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vah.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dkr.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ihn.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yto.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pwc.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://kqu.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqg.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jpe.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xrj.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fdg.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://rgy.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://rjl.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://wyl.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://cok.yonumen.top

[C05] 返回多个值
来源：http://fez.shanyushiyangtech.top

Py:   return a, b
来源：http://cor.svipenyu.cn

PHP:  return [$a, $b];
来源：http://jzd.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ekh.tanke756.top

TS:   return { a, b };
来源：http://xba.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oui.smart0.xyz

Go:   return a, b
来源：http://vqk.aizwys.cn

Ruby: return a, b
来源：http://bok.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://lpj.sweek.top

[C06] 匿名函数 / lambda
来源：http://aft.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://kch.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://son.sufxvd.cn

JS:   const square = x => x * x;
来源：http://xbu.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://ypk.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pbk.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://xwf.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://ixx.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://tfi.fktsv.cn

[C07] 把函数作为参数传入
来源：http://ahf.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dkv.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://thf.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qgj.mhx1999.top

TS:   arr.map(String)
来源：http://fro.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vps.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qzo.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://vms.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://inl.c1oappe.top

[C08] 闭包
来源：http://sdp.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mzk.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://naq.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fxu.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pey.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aep.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yfa.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hlc.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iij.sweek.top

[C09] 递归
来源：http://nnx.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jfk.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rrt.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mck.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hgo.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wlh.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ghc.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kji.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://amq.jianghu66.top

[C10] 变量作用域
来源：http://uyg.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gai.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://odc.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yqi.uphjek.com

TS:   同 JS
来源：http://xar.zhixingplan.top

Java: 方法内为块级作用域
来源：http://buk.xuanzx.com

Go:   花括号块级作用域
来源：http://njz.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://omn.vehdjk.com

C#:   块级作用域
来源：http://ial.mhx1999.top

[C11] 模块导入与导出
来源：http://myf.svipenyu.cn

Py:   from module import func
来源：http://iop.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://dxt.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://efq.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ypl.fengsongda.top

Java: import java.util.List;
来源：http://xuf.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://thf.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://wkj.chenlongwang.top

C#:   using System.Text;
来源：http://tbh.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://wrr.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://dqb.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://byu.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://gqs.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://jhq.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://orm.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://pbq.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://hcy.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://upi.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://aqe.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vfg.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxw.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://abj.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mng.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rcn.fktsv.cn

Go:   func add(a, b int) int
来源：http://pux.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dtm.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://ukz.chenjidiqi.icu

[C14] 泛型函数
来源：http://pqu.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dcw.gaohongyu789.top

PHP:  // 无泛型
来源：http://kaq.shangyingyoupin.top

JS:   // 无泛型
来源：http://ilk.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mok.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ngt.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvi.52xcode.cn

Ruby: # 无泛型
来源：http://nng.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dls.yj20258888.top

[C15] 解构 / 展开参数
来源：http://std.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://glf.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://sio.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aly.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://azy.zdbjq.cn

Java: // 无解构
来源：http://iey.dashuyun.cn

Go:   // 无解构
来源：http://gph.zhengqikj.top

Ruby: a, b = pair
来源：http://dbi.havefunace.top

C#:   var (a, b) = pair;
来源：http://seu.birdmap.top

[C16] 函数 / 方法重载
来源：http://qqc.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sqv.chenzaomai.com

PHP:  // 无重载
来源：http://syl.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fdg.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://rki.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kfq.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://sjw.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://bjs.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hgf.andypj.xyz

================================================================================
来源：http://hxb.tarul.cn

D. 数组 / 列表 / 集合
来源：http://xtb.jlsjyb.cn

================================================================================
来源：http://trp.gzhubu.top

[D01] 创建数组 / 列表
来源：http://xky.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://xxj.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zcf.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qer.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hbn.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jna.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://szp.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://usg.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ljb.iojbl.cn

[D02] 追加元素到末尾
来源：http://rqw.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kzl.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://opw.epnwcf.com

JS:   arr.push(4);
来源：http://jyf.jqgufenzy.top

TS:   arr.push(4);
来源：http://rdz.jianghu66.top

Java: list.add(4);
来源：http://vtb.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://sjx.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://tki.xziqi.cn

C#:   list.Add(4);
来源：http://lbv.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://ccx.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://oum.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ebv.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gwp.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://jre.yj202588.top

Java: list.add(0, 0);
来源：http://qbi.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oxp.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://szr.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://pxb.shzxlz.cn

[D04] 删除元素
来源：http://ybw.fehbvm.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fsh.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lpb.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://obg.ivvv.top

TS:   arr.splice(0, 1);
来源：http://hdv.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dbr.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lsj.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ddb.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ibm.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://rhz.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ewe.jinqigfzy.top


<!-- 参考信息 -->