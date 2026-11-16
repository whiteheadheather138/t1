代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxd.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://ido.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nbp.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nji.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://phr.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rcq.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hvm.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ymk.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rls.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epb.hnxiangtu.top

[B07] while 循环
来源：http://hgt.316326.xyz

Py:   while i < 10: i += 1
来源：http://pya.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://pwx.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://zwj.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://qbs.hammf.cn

Java: while (i < 10) { i++; }
来源：http://xan.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hod.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://ier.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://blf.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://lxv.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://tkm.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dko.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://hyl.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://ujb.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://lcq.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kll.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wam.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://djo.jiagoushi.top

[B09] break 与 continue
来源：http://tgt.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bkc.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vhu.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zaz.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://buf.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dda.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tcl.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rmd.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbi.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://kie.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zgr.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ikt.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vfp.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://crs.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cld.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pxt.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hvc.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vqp.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://dik.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://ylz.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://cot.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ydw.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rra.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zfj.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pbl.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://oub.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://shq.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://cfl.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://lcz.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xap.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kkh.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lcm.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fuq.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ozo.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tpr.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ika.haohaochexian.top

[B13] 判断是否为数字
来源：http://wuo.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://eps.yj202588.top

PHP:  is_numeric($x)
来源：http://tzb.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tzf.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbk.guowangkeji.top

Java: x instanceof Number
来源：http://uws.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://stq.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://bls.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://azg.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://hqk.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kgw.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nik.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://lun.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://erz.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vyc.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lpt.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://axd.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yuo.yj20258888.top

[B15] 布尔运算与取反
来源：http://rlg.yueranfly.top

Py:   a and b or not c
来源：http://sla.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://jda.birdmap.top

JS:   a && b || !c
来源：http://arx.birdmap.top

TS:   a && b || !c
来源：http://fpa.ehwqpu.com

Java: a && b || !c
来源：http://ioa.shanyushiyangtech.top

Go:   a && b || !c
来源：http://gpe.hywenlv.cn

Ruby: a && b || !c
来源：http://bri.jinqigufen.top

C#:   a && b || !c
来源：http://xdo.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://how.iojbl.cn

Py:   if not data: return
来源：http://nku.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://xos.hywenlv.cn

JS:   if (!data) return;
来源：http://qxv.jianghu66.top

TS:   if (!data) return;
来源：http://epp.bjfxy.top

Java: if (data == null) return;
来源：http://dvu.ppjwa.cn

Go:   if data == nil { return }
来源：http://rcm.jqgfzy.top

Ruby: return if data.nil?
来源：http://pts.zhixingplan.top

C#:   if (data == null) return;
来源：http://dlh.shangyingyoupin.top

================================================================================
来源：http://bxk.guowangkeji.top

C. 函数与作用域
来源：http://gkk.pengpengdd.cyou

================================================================================
来源：http://whd.jiagoushi.top

[C01] 定义函数
来源：http://wgl.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://gke.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zua.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://jqt.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mcw.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zth.xinyue.icu

Go:   func add(a, b int) int { return a + b }
来源：http://jbc.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://qwd.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vik.shuidangran.top

[C02] 默认参数
来源：http://ejk.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://taw.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://afy.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://tvy.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ctt.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://znv.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qrs.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://hpr.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://oqg.jiagoushi.top

[C03] 可变参数
来源：http://pss.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://fuq.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lsu.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hzv.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kqp.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ezr.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rcm.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://ksi.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tih.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://ams.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hhp.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lfy.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zrq.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vro.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://pnm.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://yxm.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://thf.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://zwa.zhiwuduotai.top

[C05] 返回多个值
来源：http://ugz.hywenlv.cn

Py:   return a, b
来源：http://lxc.yuanzhike.top

PHP:  return [$a, $b];
来源：http://pji.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uab.zhengqikj.top

TS:   return { a, b };
来源：http://koi.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gpq.316326.xyz

Go:   return a, b
来源：http://zoi.hammf.cn

Ruby: return a, b
来源：http://cwp.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://jjc.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://wav.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://tns.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://vgi.svipenyu.cn

JS:   const square = x => x * x;
来源：http://exf.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://jpi.52xcode.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rls.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://qxx.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://mvr.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://xdh.yj20258888.top

[C07] 把函数作为参数传入
来源：http://ewh.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://njy.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://kow.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gum.zdqjudy.top

TS:   arr.map(String)
来源：http://bap.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sjw.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tzu.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://wks.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eoa.jqgfzy.top

[C08] 闭包
来源：http://hkv.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pkj.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pkt.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vbt.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://glb.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ghp.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://epg.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zmt.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uwe.vqdsnc.cn

[C09] 递归
来源：http://qwk.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gre.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://piq.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eal.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aly.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://drg.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dus.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xpj.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lfu.sysykeji.top

[C10] 变量作用域
来源：http://lkf.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wwu.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dxj.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://scr.pycfn.com

TS:   同 JS
来源：http://vbt.9152youxi.cn

Java: 方法内为块级作用域
来源：http://egv.cdnleiting.top

Go:   花括号块级作用域
来源：http://cim.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vfd.zdqjudy.top

C#:   块级作用域
来源：http://oqy.ydzc1.top

[C11] 模块导入与导出
来源：http://wrc.ywan-chungtsiang.top

Py:   from module import func
来源：http://spt.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uum.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://bqv.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wkw.iojbl.cn

Java: import java.util.List;
来源：http://qqn.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xzo.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://bzf.zhixingplan.top

C#:   using System.Text;
来源：http://ast.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://cps.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://sfz.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://bvs.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://ger.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://lxw.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://spg.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kkt.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://ymf.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dpr.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://xee.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://boy.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzl.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dil.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjf.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://dyh.meibo888.top

Go:   func add(a, b int) int
来源：http://onn.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fkc.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://ppy.zycfv.cn

[C14] 泛型函数
来源：http://ogt.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tcr.hammf.cn

PHP:  // 无泛型
来源：http://vxd.yuanzhike.top

JS:   // 无泛型
来源：http://bio.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hgd.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://twr.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xuh.ivvv.top

Ruby: # 无泛型
来源：http://wps.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uge.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://vzw.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vrx.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://xij.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vsq.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vhl.chenlongwang.top

Java: // 无解构
来源：http://qgd.shanyushiyangtech.top

Go:   // 无解构
来源：http://cqd.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://abu.52xcode.cn

C#:   var (a, b) = pair;
来源：http://and.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://txm.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fmu.hysaishi.cn

PHP:  // 无重载
来源：http://alx.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nce.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://cvx.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nav.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://pgx.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://hgd.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gle.vehdjk.com

================================================================================
来源：http://svu.cheryme.top

D. 数组 / 列表 / 集合
来源：http://sny.zhijiandao.cn

================================================================================
来源：http://hsy.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://pmv.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oaf.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xjy.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://acd.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://slf.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ecm.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://psa.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://ehk.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aas.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://rfs.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dfg.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://anf.wangshuangyany.cn

JS:   arr.push(4);
来源：http://oyo.yuxming.cn

TS:   arr.push(4);
来源：http://ufd.hammf.cn

Java: list.add(4);
来源：http://twu.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://typ.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://pyy.fengsongda.top

C#:   list.Add(4);
来源：http://cxz.sweek.top

[D03] 在指定位置插入元素
来源：http://pbs.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://xbz.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hwr.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://emc.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://ilx.ehwqpu.com

Java: list.add(0, 0);
来源：http://hnz.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://ozy.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dim.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://bhb.tianlin.xyz

[D04] 删除元素
来源：http://hjk.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uwu.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ykm.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gff.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://rvu.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jyl.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tvj.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lud.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rnp.iojbl.cn

[D05] 访问与修改元素
来源：http://thl.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nyc.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://epn.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tkw.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://mxm.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://wvh.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://lhh.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mbs.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://njr.birdmap.top

[D06] 数组长度
来源：http://hbw.xuetiantiany.cn

Py:   len(arr)
来源：http://ayo.pycfn.com

PHP:  count($arr);
来源：http://new.fehbvm.com

JS:   arr.length
来源：http://fgn.aibaodan.cn

TS:   arr.length
来源：http://frz.kuanghao11.cn


<!-- 参考信息 -->