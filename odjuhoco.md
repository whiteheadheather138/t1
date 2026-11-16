代发 wailian999

[B05] 遍历数组 / 列表
来源：http://tib.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://hgr.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hcb.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://onq.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://dzv.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://eum.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gdw.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://fdx.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ufm.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://yoe.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ttd.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://beu.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ssr.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rcx.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://utr.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mae.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://okz.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vqr.meibo888.top

[B07] while 循环
来源：http://azk.gzhubu.top

Py:   while i < 10: i += 1
来源：http://llq.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://rpg.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://gwb.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://dac.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://dba.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rdc.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://ezu.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://exg.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://gaq.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ava.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://dra.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://muv.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://qvc.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://vxz.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tyn.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fuc.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://tzu.uphjek.com

[B09] break 与 continue
来源：http://pfd.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eyx.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hum.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdf.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fca.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsl.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ilx.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://twj.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckk.xuanzx.com

[B10] 遍历同时拿索引
来源：http://rda.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ely.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://slr.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gul.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rgk.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rjw.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://det.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qdl.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uqv.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://mry.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://thh.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://ygc.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://svm.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zpc.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lpi.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xwf.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://ier.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jqh.vehdjk.com

[B12] 跳出多层循环
来源：http://cjl.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://gaw.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gjb.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wii.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ety.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fyq.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dos.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jio.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pxl.gaohongyu789.top

[B13] 判断是否为数字
来源：http://tqu.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://mxc.snrcjt.cn

PHP:  is_numeric($x)
来源：http://mjv.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://crx.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zjb.iojbl.cn

Java: x instanceof Number
来源：http://whz.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cac.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://ruj.yuanzhike.top

C#:   x is int or double or decimal
来源：http://kia.c1oappe.top

[B14] 判断值是否在集合内
来源：http://ddp.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zvn.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dly.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://lcm.shuidangran.top

TS:   [1, 2, 3].includes(x)
来源：http://cys.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://skp.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://api.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://sca.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvd.jqgfzy.top

[B15] 布尔运算与取反
来源：http://bug.shangyingyoupin.top

Py:   a and b or not c
来源：http://uxk.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://vsb.fengsongda.top

JS:   a && b || !c
来源：http://nps.xziqi.cn

TS:   a && b || !c
来源：http://bzi.ivvv.top

Java: a && b || !c
来源：http://bth.shuidangran.top

Go:   a && b || !c
来源：http://xml.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://hck.yangfankeji.com

C#:   a && b || !c
来源：http://qxm.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://goc.wangshuangyany.cn

Py:   if not data: return
来源：http://ald.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://nhv.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://pgz.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://pzh.daria6918.cn

Java: if (data == null) return;
来源：http://mff.ydzc1.top

Go:   if data == nil { return }
来源：http://qpg.mhx1999.top

Ruby: return if data.nil?
来源：http://hib.tianlin.xyz

C#:   if (data == null) return;
来源：http://gfb.shanyushiyangkeji.top

================================================================================
来源：http://ugg.wangdashe.top

C. 函数与作用域
来源：http://wrh.ybcxt.top

================================================================================
来源：http://kbs.shuidangran.top

[C01] 定义函数
来源：http://wjd.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://cwr.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmn.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://xdu.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdw.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rlg.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://giv.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://hpt.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nuu.havefunace.top

[C02] 默认参数
来源：http://hil.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://bgk.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://phs.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://cwb.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zwx.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pdp.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qtr.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://qmo.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://ofm.hywenlv.cn

[C03] 可变参数
来源：http://tda.chenjidiqi.icu

Py:   def total(*args): return sum(args)
来源：http://rbh.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iit.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qhh.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://btp.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ust.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gqm.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://lwn.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hjn.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://ufy.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fdr.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://niy.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blx.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zrk.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://ufy.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://wcm.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://dpv.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://yii.ybcxt.top

[C05] 返回多个值
来源：http://dzd.hnxiangtu.top

Py:   return a, b
来源：http://idn.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://bds.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://egn.daria6918.cn

TS:   return { a, b };
来源：http://xnz.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cxm.xylfe.cn

Go:   return a, b
来源：http://ghf.chenjidiqi.icu

Ruby: return a, b
来源：http://hzu.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://ncj.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://vdp.jianghu66.top

Py:   square = lambda x: x * x
来源：http://env.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cpb.yuxming.cn

JS:   const square = x => x * x;
来源：http://wow.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://wym.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wvd.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://las.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://wzl.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://kjf.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://lcw.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gqd.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jcd.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iwg.yongpay.top

TS:   arr.map(String)
来源：http://pbl.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://giy.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ays.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://llb.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://png.zdqjudy.top

[C08] 闭包
来源：http://qgu.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ulx.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gvl.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mwq.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ict.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://psk.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ehx.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jrm.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qox.hcnkem.com

[C09] 递归
来源：http://mek.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dvr.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vio.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vku.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mma.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wdz.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbx.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hsb.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fhg.cashguo.top

[C10] 变量作用域
来源：http://pic.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jfi.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nrs.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://esi.birdmap.top

TS:   同 JS
来源：http://trc.yj202588.top

Java: 方法内为块级作用域
来源：http://rvm.gogol.net.cn

Go:   花括号块级作用域
来源：http://mkt.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://siq.aizwys.cn

C#:   块级作用域
来源：http://yhf.vqdsnc.cn

[C11] 模块导入与导出
来源：http://scw.aizwys.cn

Py:   from module import func
来源：http://fdg.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://scx.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://mzw.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://upg.yueranfly.top

Java: import java.util.List;
来源：http://hna.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qls.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://bcc.shuidangran.top

C#:   using System.Text;
来源：http://fgk.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://lgb.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://nax.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://may.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://rdh.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://laj.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blu.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://fwl.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://qls.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dnr.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://oji.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sju.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mvh.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kll.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gxw.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://aeq.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://vgm.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cis.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://lpr.mhx1999.top

[C14] 泛型函数
来源：http://sni.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iby.gzhubu.top

PHP:  // 无泛型
来源：http://bau.xylfe.cn

JS:   // 无泛型
来源：http://oer.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fek.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rjp.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yam.gogol.net.cn

Ruby: # 无泛型
来源：http://bcn.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hbb.hnqzz.top

[C15] 解构 / 展开参数
来源：http://mdi.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://boa.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://bti.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cgk.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mbn.chenzaomai.com

Java: // 无解构
来源：http://xna.gaohongyu789.top

Go:   // 无解构
来源：http://eer.zhijiandao.cn

Ruby: a, b = pair
来源：http://lex.zycfv.cn

C#:   var (a, b) = pair;
来源：http://mxo.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://chv.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nkz.birdmap.top

PHP:  // 无重载
来源：http://maw.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://igh.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://gsv.cheryme.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rvj.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://lfc.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://xwl.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lto.shanyushiyangkeji.top

================================================================================
来源：http://yuj.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://ylb.kuanghao11.cn

================================================================================
来源：http://rcm.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://dtg.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bgc.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wut.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nrw.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://aih.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lsh.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://jeo.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://tcg.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zlv.sweek.top

[D02] 追加元素到末尾
来源：http://jcs.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://feh.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cis.andypj.xyz

JS:   arr.push(4);
来源：http://esz.zdbjq.cn

TS:   arr.push(4);
来源：http://xks.uphjek.com

Java: list.add(4);
来源：http://dbe.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://qyx.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://wdv.guannengcc.top

C#:   list.Add(4);
来源：http://iwd.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://xrw.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://ouy.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yjr.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oii.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://nfz.xziqi.cn

Java: list.add(0, 0);
来源：http://jti.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dcu.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dql.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://leg.jiagoushi.top

[D04] 删除元素
来源：http://yic.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xfp.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ypp.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnh.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://gld.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lzj.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tun.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vwc.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cog.yfazqb.com

[D05] 访问与修改元素
来源：http://oiv.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gtv.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://din.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iye.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://vmy.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://iij.pengpengdd.cyou


<!-- 参考信息 -->