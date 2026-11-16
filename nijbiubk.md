代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gdk.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yji.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://kif.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uto.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://mld.yongpay.top

Py:   for item in arr: print(item)
来源：http://ecm.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qdk.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://miv.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hno.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bct.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oas.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://etv.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tyt.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://jaf.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jep.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fqp.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpg.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nfj.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://knm.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qqz.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bob.yj20258888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lzg.svipenyu.cn

[B07] while 循环
来源：http://plv.yfazqb.com

Py:   while i < 10: i += 1
来源：http://kat.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://roq.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://zgd.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://wiw.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://zcu.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dgz.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://edk.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://ecz.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://yep.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://hco.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xwu.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://hdl.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://jzy.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://vkx.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://byr.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://npl.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://opq.tianlin.xyz

[B09] break 与 continue
来源：http://cej.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://meu.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kam.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvp.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfe.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://utg.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pce.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hve.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffg.xinyue.icu

[B10] 遍历同时拿索引
来源：http://yza.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://piw.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxp.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dmd.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hgy.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jbj.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xgc.cheryme.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zmw.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eft.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://vbp.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://fjq.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://fkh.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebt.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gnk.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hok.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bix.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://exc.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qrv.uphjek.com

[B12] 跳出多层循环
来源：http://knx.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pou.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ocz.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lal.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qzc.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jjh.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://whl.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xbf.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gou.epnwcf.com

[B13] 判断是否为数字
来源：http://yuw.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://oqg.daria6918.cn

PHP:  is_numeric($x)
来源：http://dlv.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wpy.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mls.jinghuilouyu.cn

Java: x instanceof Number
来源：http://mdt.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bfi.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://teu.c1oappe.top

C#:   x is int or double or decimal
来源：http://fgl.pycfn.com

[B14] 判断值是否在集合内
来源：http://vtj.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ggw.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jqb.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://fie.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://epq.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dlv.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://agq.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://dlt.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qle.svipenyu.cn

[B15] 布尔运算与取反
来源：http://xcf.sufxvd.cn

Py:   a and b or not c
来源：http://agh.tanke756.top

PHP:  $a && $b || !$c
来源：http://lnx.aizwys.cn

JS:   a && b || !c
来源：http://pzk.hnxiangtu.top

TS:   a && b || !c
来源：http://owr.cucudq.cn

Java: a && b || !c
来源：http://yrr.zhongyouzk.top

Go:   a && b || !c
来源：http://nzg.hnxiangtu.top

Ruby: a && b || !c
来源：http://cde.pycfn.com

C#:   a && b || !c
来源：http://puv.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bzv.ydjk.org.cn

Py:   if not data: return
来源：http://fwt.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://oyk.meibo888.top

JS:   if (!data) return;
来源：http://pyz.cucudq.cn

TS:   if (!data) return;
来源：http://pbf.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://jwy.redwolf501.top

Go:   if data == nil { return }
来源：http://xgs.tianlin.xyz

Ruby: return if data.nil?
来源：http://cfl.ppjwa.cn

C#:   if (data == null) return;
来源：http://qba.dashuyun.cn

================================================================================
来源：http://rhi.zhongyouzk.top

C. 函数与作用域
来源：http://rxk.fengsongda.top

================================================================================
来源：http://gjk.jlsjyb.cn

[C01] 定义函数
来源：http://dgg.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://gvj.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgm.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://psq.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tan.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zgi.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://jgo.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://pdc.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://swy.meibo888.top

[C02] 默认参数
来源：http://vvl.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://boc.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jyj.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://azd.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ncm.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qip.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wpv.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://iic.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://qkq.jinyuanbaomall.cn

[C03] 可变参数
来源：http://pcj.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://qco.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dvq.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://anr.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrf.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nun.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://llc.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://kps.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://enf.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://jic.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yan.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aft.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bgk.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cfs.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://mlj.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://dim.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://ewl.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://pis.hywenlv.cn

[C05] 返回多个值
来源：http://cez.52xcode.cn

Py:   return a, b
来源：http://xnd.ctjpmb.com

PHP:  return [$a, $b];
来源：http://elw.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://niz.shuidangran.top

TS:   return { a, b };
来源：http://hyk.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gzl.yangfankeji.com

Go:   return a, b
来源：http://tla.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://xkv.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://ofk.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://vke.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://apn.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://psk.yangfankeji.com

JS:   const square = x => x * x;
来源：http://oky.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://kyf.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sri.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://hcm.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://nfo.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uig.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://nrg.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ioh.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ejl.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nrw.yongpay.top

TS:   arr.map(String)
来源：http://wkg.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kkv.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gmv.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://njh.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pox.sysykeji.top

[C08] 闭包
来源：http://gwi.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vlp.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rch.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ngd.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zgh.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gdq.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dqk.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lmf.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bhl.xingfuxueyuan.xyz

[C09] 递归
来源：http://iyw.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sce.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wtv.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pqd.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cll.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lrd.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eag.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pny.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hmg.zhijiandao.cn

[C10] 变量作用域
来源：http://mfo.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iyc.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifr.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ivs.hongshengwenyu.top

TS:   同 JS
来源：http://ngq.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://svk.vehdjk.com

Go:   花括号块级作用域
来源：http://kvb.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bni.ydzc1.top

C#:   块级作用域
来源：http://ugs.nanxinkj.top

[C11] 模块导入与导出
来源：http://gjf.daxiang520.top

Py:   from module import func
来源：http://awe.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://puv.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qyf.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dhw.mhx1999.top

Java: import java.util.List;
来源：http://ily.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qon.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://bnu.zhengqikj.top

C#:   using System.Text;
来源：http://xvi.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://sel.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://pdx.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://wfq.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://glf.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://uwa.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cci.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://qxn.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://rap.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ltp.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://wbq.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jua.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://icw.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rdf.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://juh.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://zkq.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://xas.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vuc.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://arb.snrcjt.cn

[C14] 泛型函数
来源：http://luf.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lmz.iojbl.cn

PHP:  // 无泛型
来源：http://vgz.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://iwb.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lnj.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ied.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ior.zdbjq.cn

Ruby: # 无泛型
来源：http://axy.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nyg.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://dqe.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://swu.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://vdl.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ruc.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://unn.yanxiufei.cn

Java: // 无解构
来源：http://lsp.tianlin.xyz

Go:   // 无解构
来源：http://dnv.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://cqz.redwolf501.top

C#:   var (a, b) = pair;
来源：http://gpx.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://mzm.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nhu.0kj1m.cn

PHP:  // 无重载
来源：http://vfh.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://thf.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://hls.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vcg.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://wrq.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://uwa.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wpl.chenlongwang.top

================================================================================
来源：http://irb.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://nly.hammf.cn

================================================================================
来源：http://uks.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://ope.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ezp.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gtb.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dlr.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rmx.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ujq.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://llx.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://bot.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dgm.xylfe.cn

[D02] 追加元素到末尾
来源：http://dvm.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://htb.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kxv.zycfv.cn

JS:   arr.push(4);
来源：http://shp.zycfv.cn

TS:   arr.push(4);
来源：http://vwj.uphjek.com

Java: list.add(4);
来源：http://njo.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://xtg.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://tgg.cashguo.top

C#:   list.Add(4);
来源：http://mou.sweek.top

[D03] 在指定位置插入元素
来源：http://cfp.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://jvj.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jhi.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pob.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://eqa.quarkkingdee.top

Java: list.add(0, 0);
来源：http://kaa.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://xag.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ume.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://lmk.shangyingyoupin.top

[D04] 删除元素
来源：http://jwz.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mzi.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://alx.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xgh.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://epc.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xpk.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xvq.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uux.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://alo.dianchejie.cn

[D05] 访问与修改元素
来源：http://ufi.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yij.havefunace.top


<!-- 参考信息 -->