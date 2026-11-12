代发 wailian999

Py:   for i in range(10): print(i)
来源：http://pwp.dianchejie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ozf.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfg.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uwz.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://olr.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gzu.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://zdn.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ctg.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://ney.fzhhl.top

Py:   for item in arr: print(item)
来源：http://pwr.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wfr.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mua.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hps.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fmu.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cwa.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://qzo.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xvu.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://ywk.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://owd.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nrs.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lrx.uphjek.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fid.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oqc.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pkx.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jee.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fma.chenjidiqi.icu

[B07] while 循环
来源：http://wdt.cheryme.top

Py:   while i < 10: i += 1
来源：http://gds.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vrq.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://lil.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://kdv.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://nrz.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mmu.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://rki.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://umo.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://zts.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://onl.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://mez.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://sau.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://idw.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://wgx.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wru.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dev.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://vjw.c1oappe.top

[B09] break 与 continue
来源：http://vye.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mrj.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sof.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhd.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyt.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qaj.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uix.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://una.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgd.yj20258.top

[B10] 遍历同时拿索引
来源：http://jpm.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nhj.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rxx.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://voz.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hjc.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zdk.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rpk.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ahm.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://czx.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://oij.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://nsh.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://cvu.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eeg.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocf.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tgb.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zsd.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://owe.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://clm.mhx1999.top

[B12] 跳出多层循环
来源：http://zvu.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://bqw.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ljg.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nwl.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jph.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kpm.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://brg.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cvh.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nuc.ppjwa.cn

[B13] 判断是否为数字
来源：http://xwj.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://frr.yuxming.cn

PHP:  is_numeric($x)
来源：http://hvm.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bix.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://huq.guannengcc.top

Java: x instanceof Number
来源：http://lit.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dyv.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://ryu.hesvh.cn

C#:   x is int or double or decimal
来源：http://vlr.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://wfw.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hsj.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hbx.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gma.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://pai.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zvk.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xij.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://lxb.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bya.hcnkem.com

[B15] 布尔运算与取反
来源：http://nvx.guowangkeji.top

Py:   a and b or not c
来源：http://xvg.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://sxk.cheryme.top

JS:   a && b || !c
来源：http://fnl.ydzc1.top

TS:   a && b || !c
来源：http://nqq.nanxinkj.top

Java: a && b || !c
来源：http://mwi.chenzaomai.com

Go:   a && b || !c
来源：http://vpe.yuxming.cn

Ruby: a && b || !c
来源：http://dua.gogol.net.cn

C#:   a && b || !c
来源：http://wfv.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bvf.zhijiandao.cn

Py:   if not data: return
来源：http://rpr.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://dvi.ppjwa.cn

JS:   if (!data) return;
来源：http://jyb.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://mkz.sjlbkw.cn

Java: if (data == null) return;
来源：http://afh.fehbvm.com

Go:   if data == nil { return }
来源：http://vyl.quarkkingdee.top

Ruby: return if data.nil?
来源：http://cuh.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://olv.zhongyouzk.top

================================================================================
来源：http://ruj.hcnkem.com

C. 函数与作用域
来源：http://uzj.sysykeji.top

================================================================================
来源：http://chr.shanyushiyangtech.top

[C01] 定义函数
来源：http://sif.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://wjn.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fmt.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://jul.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ygd.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aeh.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://smd.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://gfu.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aio.sxryk.cn

[C02] 默认参数
来源：http://ixa.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://tbt.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kpj.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://wgo.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lsb.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wlb.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oyl.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://fcc.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://edu.chenjidiqi.icu

[C03] 可变参数
来源：http://yqp.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://bwe.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ezq.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxa.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kxj.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kvi.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vke.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://gly.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hyc.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://dii.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dyu.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ppq.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uvp.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nci.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://pci.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://zmg.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://cbl.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://xsp.havefunace.top

[C05] 返回多个值
来源：http://vuw.haohaochexian.top

Py:   return a, b
来源：http://bjt.yfazqb.com

PHP:  return [$a, $b];
来源：http://djf.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kfo.fengsongda.top

TS:   return { a, b };
来源：http://zfc.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nbn.zhixingplan.top

Go:   return a, b
来源：http://oci.sufxvd.cn

Ruby: return a, b
来源：http://oju.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://xrp.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://rkt.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://kla.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://exr.tian-w.cn

JS:   const square = x => x * x;
来源：http://eob.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://fpu.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mtt.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://hcl.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://mbe.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://bqp.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://dbo.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tqu.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ugm.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fjw.xuetiantiany.cn

TS:   arr.map(String)
来源：http://qbl.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pwj.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hwl.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://psb.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://usj.hysaishi.cn

[C08] 闭包
来源：http://twv.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://flj.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qyk.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tpw.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xxo.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iqf.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qfb.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pyq.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://djk.zhoulong.xyz

[C09] 递归
来源：http://ufx.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hbh.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ond.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvr.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eyw.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moj.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wwc.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yft.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wgm.zhengqikj.top

[C10] 变量作用域
来源：http://ypm.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwd.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bmn.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gnc.snrcjt.cn

TS:   同 JS
来源：http://yyp.xziqi.cn

Java: 方法内为块级作用域
来源：http://vgq.gotoacloud.top

Go:   花括号块级作用域
来源：http://unt.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nws.zdbjq.cn

C#:   块级作用域
来源：http://yjd.aizwys.cn

[C11] 模块导入与导出
来源：http://aju.yongpay.top

Py:   from module import func
来源：http://cnd.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://egp.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ggr.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vrt.yj202588.top

Java: import java.util.List;
来源：http://uvr.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://exj.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://des.fehbvm.com

C#:   using System.Text;
来源：http://htz.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://qjg.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://mnj.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://umr.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://nfv.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://slh.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cvc.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://woe.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://act.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nsx.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://wvw.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jzr.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbm.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpc.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzo.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://fzg.tian-w.cn

Go:   func add(a, b int) int
来源：http://npx.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hzf.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://mae.tarul.cn

[C14] 泛型函数
来源：http://slp.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rad.jinqigfzy.top

PHP:  // 无泛型
来源：http://ahs.hongshengwenyu.top

JS:   // 无泛型
来源：http://zzr.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kmo.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kit.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ddn.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://cdw.ywan-chungtsiang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://klk.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://mpa.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vcl.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://zay.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sct.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vvp.zhoulong.xyz

Java: // 无解构
来源：http://eeh.ybcxt.top

Go:   // 无解构
来源：http://utm.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://igi.xuanzx.com

C#:   var (a, b) = pair;
来源：http://kfo.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://lbv.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cdv.havefunace.top

PHP:  // 无重载
来源：http://rio.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uwr.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://eke.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rue.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://rfg.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://afj.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://stw.fzhhl.top

================================================================================
来源：http://iru.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://geb.shangyingyoupin.top

================================================================================
来源：http://xij.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://yds.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dkk.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gng.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gjy.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jop.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aln.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://hzj.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://czr.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rgn.tianlin.xyz

[D02] 追加元素到末尾
来源：http://cvw.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pxq.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nxe.cucudq.cn

JS:   arr.push(4);
来源：http://rro.svipenyu.cn

TS:   arr.push(4);
来源：http://ktl.gotoacloud.top

Java: list.add(4);
来源：http://pds.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://fjs.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://zdj.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://qpl.fzhhl.top

[D03] 在指定位置插入元素
来源：http://fjo.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://miw.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rbr.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://epo.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://lin.haohaochexian.top

Java: list.add(0, 0);
来源：http://aqm.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://msf.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sjn.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://tho.jianghu66.top

[D04] 删除元素
来源：http://pdq.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cdx.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nut.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cip.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://biv.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fho.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sre.yangfankeji.com


<!-- 参考信息 -->