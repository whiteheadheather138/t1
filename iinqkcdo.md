代发 wailian999

Py:   for i in range(10): print(i)
来源：http://cnz.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tij.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fir.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fso.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gzv.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xjm.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://nwg.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://coa.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://gcv.iojbl.cn

Py:   for item in arr: print(item)
来源：http://ecx.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sit.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mrr.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ddb.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nfz.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xkj.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://vyl.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fgh.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://jtt.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lim.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ylk.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ila.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mwi.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dfk.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://paj.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yct.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pjy.0kj1m.cn

[B07] while 循环
来源：http://jmr.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://epg.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://qmf.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://sds.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://vha.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://cnc.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pof.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://crj.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://ocp.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://ysb.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://vnq.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ikx.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://jxh.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://jot.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://rvd.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://shq.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ndy.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://wwv.yj20258888.top

[B09] break 与 continue
来源：http://yhy.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ecd.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fju.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckc.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sge.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbt.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gps.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jbs.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://siz.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://erw.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cey.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zri.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xhm.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dqj.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xaf.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gpp.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nzi.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bvi.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://cxq.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://uux.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://kvb.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epb.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nmv.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xis.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dyb.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://qcf.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ugl.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://wtu.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rfe.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rch.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ick.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bqe.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xji.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vur.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fnt.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://thv.yongpay.top

[B13] 判断是否为数字
来源：http://tye.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://lgi.andypj.xyz

PHP:  is_numeric($x)
来源：http://swf.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fac.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://goo.yanxiufei.cn

Java: x instanceof Number
来源：http://etp.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eiy.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://xlu.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://zbz.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://jkn.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vao.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hez.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://ziu.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://yel.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://etn.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kxm.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zvt.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cjg.nwbrower.top

[B15] 布尔运算与取反
来源：http://gpb.fzhhl.top

Py:   a and b or not c
来源：http://ott.andypj.xyz

PHP:  $a && $b || !$c
来源：http://vsp.yvedp.cn

JS:   a && b || !c
来源：http://ont.ivvv.top

TS:   a && b || !c
来源：http://mez.ywan-chungtsiang.top

Java: a && b || !c
来源：http://dzk.ydzc1.top

Go:   a && b || !c
来源：http://dic.tarul.cn

Ruby: a && b || !c
来源：http://ate.sysykeji.top

C#:   a && b || !c
来源：http://emq.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://yvl.svipenyu.cn

Py:   if not data: return
来源：http://fea.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://qri.316326.xyz

JS:   if (!data) return;
来源：http://kto.zdbjq.cn

TS:   if (!data) return;
来源：http://uzi.yuxming.cn

Java: if (data == null) return;
来源：http://tng.xylfe.cn

Go:   if data == nil { return }
来源：http://lzr.sjlbkw.cn

Ruby: return if data.nil?
来源：http://yom.guannengcc.top

C#:   if (data == null) return;
来源：http://gro.zhoulong.xyz

================================================================================
来源：http://mfy.hnxiangtu.top

C. 函数与作用域
来源：http://fjl.yj20258.top

================================================================================
来源：http://kqp.chenjidiqi.icu

[C01] 定义函数
来源：http://yio.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://dkq.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zka.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://wwf.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckh.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kmz.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xeo.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://xlr.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hrp.yj202588.top

[C02] 默认参数
来源：http://pbs.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://mjw.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xiy.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://ves.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://koe.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://que.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pev.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://bzf.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://glo.iojbl.cn

[C03] 可变参数
来源：http://zbt.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://prt.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ska.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tel.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qqp.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lon.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://auu.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://upd.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fwn.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://xva.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qzp.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kbw.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rcj.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ved.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://wlt.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://oka.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://dra.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://cnw.jinqigufen.top

[C05] 返回多个值
来源：http://knb.zhixingplan.top

Py:   return a, b
来源：http://ttq.bbcook.cn

PHP:  return [$a, $b];
来源：http://vpe.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aci.sxryk.cn

TS:   return { a, b };
来源：http://ohm.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yxw.tarul.cn

Go:   return a, b
来源：http://qal.hnqzz.top

Ruby: return a, b
来源：http://idu.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://pnt.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://tdp.yj202588.top

Py:   square = lambda x: x * x
来源：http://rmn.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fwp.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://oye.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://sgg.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lnz.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://njk.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://zhw.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://xmr.yj202588.top

[C07] 把函数作为参数传入
来源：http://cbb.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://klm.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://svj.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mzc.yvedp.cn

TS:   arr.map(String)
来源：http://fhp.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ien.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kdh.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://djz.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jgu.jinqigfzy.top

[C08] 闭包
来源：http://rex.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mvh.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksd.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oxm.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://czy.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pdu.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ruw.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wnc.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mne.chenzaomai.com

[C09] 递归
来源：http://cgz.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rlk.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsk.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxv.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ruy.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ypj.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xot.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://duj.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bsa.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://yjg.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://olv.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ttz.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fnc.fzhhl.top

TS:   同 JS
来源：http://zur.aibaodan.cn

Java: 方法内为块级作用域
来源：http://qfm.kuanghao11.cn

Go:   花括号块级作用域
来源：http://itw.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ovr.zhongyouzk.top

C#:   块级作用域
来源：http://exn.tarul.cn

[C11] 模块导入与导出
来源：http://rrq.yj202588.top

Py:   from module import func
来源：http://eqc.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hfl.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://rzr.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eyy.xinyue.icu

Java: import java.util.List;
来源：http://isg.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eck.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://xjk.yongpay.top

C#:   using System.Text;
来源：http://kdw.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://ppv.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://gfu.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://ivl.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://vuc.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://msm.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ahv.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://kul.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://fzo.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wli.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://nsc.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hok.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxm.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ren.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ugv.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cqv.sufxvd.cn

Go:   func add(a, b int) int
来源：http://oyv.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vmf.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://pkn.gogol.net.cn

[C14] 泛型函数
来源：http://xzs.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://etn.sweek.top

PHP:  // 无泛型
来源：http://fyk.havefunace.top

JS:   // 无泛型
来源：http://nko.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ceg.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://csd.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kbw.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://qpv.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iyx.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://vmc.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ofi.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://gtd.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxo.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bbk.jinqigfzy.top

Java: // 无解构
来源：http://fnu.guowangkeji.top

Go:   // 无解构
来源：http://pgi.gzhubu.top

Ruby: a, b = pair
来源：http://rfc.sysykeji.top

C#:   var (a, b) = pair;
来源：http://rou.52xcode.cn

[C16] 函数 / 方法重载
来源：http://hck.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oqe.fzhhl.top

PHP:  // 无重载
来源：http://qzh.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilx.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://cws.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://zxy.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://nao.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://kst.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fuy.sxryk.cn

================================================================================
来源：http://cya.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://ubt.shanyushiyangtech.top

================================================================================
来源：http://uet.tian-w.cn

[D01] 创建数组 / 列表
来源：http://orz.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kum.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tuk.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jpj.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://hcn.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rvc.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://otr.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://axz.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gfi.bbcook.cn

[D02] 追加元素到末尾
来源：http://kgk.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hap.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://som.dashuyun.cn

JS:   arr.push(4);
来源：http://lqh.fktsv.cn

TS:   arr.push(4);
来源：http://uul.yj20258.top

Java: list.add(4);
来源：http://rpy.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://chd.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://wth.xuetiantiany.cn

C#:   list.Add(4);
来源：http://ipc.daxiang520.top

[D03] 在指定位置插入元素
来源：http://bpk.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://hsw.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rnm.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qgr.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://eaa.hysaishi.cn

Java: list.add(0, 0);
来源：http://jvp.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vir.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://enl.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://ujd.ppjwa.cn

[D04] 删除元素
来源：http://hna.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rww.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ors.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eba.havefunace.top

TS:   arr.splice(0, 1);
来源：http://szp.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hsh.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cqh.gogol.net.cn


<!-- 参考信息 -->