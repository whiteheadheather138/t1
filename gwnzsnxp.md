代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://irx.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://uku.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uxr.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fhu.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jfq.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dfe.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jdo.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://prx.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://maj.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nlh.chenzaomai.com

[B07] while 循环
来源：http://aos.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://ico.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bzr.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://daz.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://zob.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://bxy.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hao.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://ygq.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://rww.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://jbc.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://plp.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zak.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://ppe.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://juc.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://izi.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xjg.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://pnz.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://hjs.guowangkeji.top

[B09] break 与 continue
来源：http://omt.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vmp.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nxe.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezo.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vxg.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zqa.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gag.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jsr.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmv.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://rgh.shanyushiyangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vbb.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jyg.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ihl.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yab.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://chz.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jfd.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mgs.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://olo.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://yoj.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://ugf.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://pzj.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dkj.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lte.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gqs.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tws.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://bfh.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://efo.ppjwa.cn

[B12] 跳出多层循环
来源：http://ibs.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uxe.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aku.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rny.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ekw.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ffn.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ayo.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jkv.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kll.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://kbu.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://rfm.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://snc.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vms.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kkd.gaohongyu789.top

Java: x instanceof Number
来源：http://fpe.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://maq.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://ncy.jinqigufen.top

C#:   x is int or double or decimal
来源：http://yzy.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://ane.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://imm.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hde.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://ige.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://iel.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zlq.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mek.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://vsr.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://thv.vehdjk.com

[B15] 布尔运算与取反
来源：http://mfl.gaohongyu789.top

Py:   a and b or not c
来源：http://egi.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://kri.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://uqr.jqgfzy.top

TS:   a && b || !c
来源：http://rzb.sufxvd.cn

Java: a && b || !c
来源：http://jpi.gzhubu.top

Go:   a && b || !c
来源：http://dzl.jyoumei.cn

Ruby: a && b || !c
来源：http://zry.yuanzhike.top

C#:   a && b || !c
来源：http://uox.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://hyb.jinghuilouyu.cn

Py:   if not data: return
来源：http://jjd.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://ojd.jiagoushi.top

JS:   if (!data) return;
来源：http://mrq.yangfankeji.com

TS:   if (!data) return;
来源：http://ymm.yueranfly.top

Java: if (data == null) return;
来源：http://hhm.cucudq.cn

Go:   if data == nil { return }
来源：http://wqn.yuanzhike.top

Ruby: return if data.nil?
来源：http://cob.uphjek.com

C#:   if (data == null) return;
来源：http://bmo.sufxvd.cn

================================================================================
来源：http://upp.hesvh.cn

C. 函数与作用域
来源：http://and.nanxinkj.top

================================================================================
来源：http://wsc.vehdjk.com

[C01] 定义函数
来源：http://opu.yongpay.top

Py:   def add(a, b): return a + b
来源：http://yyl.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kyq.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ovx.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rfz.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sqi.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://fqq.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://fwn.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cpa.zhoulong.xyz

[C02] 默认参数
来源：http://xvx.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://zjp.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wic.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://xnm.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yhm.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lde.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dlm.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://vzg.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://qnk.hesvh.cn

[C03] 可变参数
来源：http://unw.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://ujc.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qsn.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://riv.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kll.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yub.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://elt.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://ydo.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zse.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://oir.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kjs.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://slu.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fkz.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fcy.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://ilx.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://zig.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://mkk.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://xxz.fzhhl.top

[C05] 返回多个值
来源：http://eqe.gogol.net.cn

Py:   return a, b
来源：http://mts.meibo888.top

PHP:  return [$a, $b];
来源：http://xmb.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kdz.yuxming.cn

TS:   return { a, b };
来源：http://wkc.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fdq.nwbrower.top

Go:   return a, b
来源：http://yfe.ybcxt.top

Ruby: return a, b
来源：http://adt.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://tps.316326.xyz

[C06] 匿名函数 / lambda
来源：http://ebs.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://drm.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bru.xinyue.icu

JS:   const square = x => x * x;
来源：http://kgc.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://tfb.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://spw.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://gnh.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://jya.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://ynd.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://kgg.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hzo.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xsb.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ril.ppjwa.cn

TS:   arr.map(String)
来源：http://oau.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsp.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dxu.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://wop.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://owq.feifeiyinyue.top

[C08] 闭包
来源：http://scq.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uex.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zlc.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vnn.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bso.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzf.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hll.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nbn.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vma.jinghuilouyu.cn

[C09] 递归
来源：http://bgd.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bjh.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jny.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zom.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pim.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aih.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jzu.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nqj.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fmj.quarkkingdee.top

[C10] 变量作用域
来源：http://ihi.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jlm.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qen.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jji.tanke756.top

TS:   同 JS
来源：http://zcr.daria6918.cn

Java: 方法内为块级作用域
来源：http://juw.nanxuanxn.top

Go:   花括号块级作用域
来源：http://gjo.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uvs.sxryk.cn

C#:   块级作用域
来源：http://nax.yuanzhike.top

[C11] 模块导入与导出
来源：http://mzr.sufxvd.cn

Py:   from module import func
来源：http://luu.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ecp.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://adg.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lxf.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://elo.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qwd.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://jld.aibaodan.cn

C#:   using System.Text;
来源：http://uxf.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://syj.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://tan.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://pyw.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://nfe.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://pyj.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gmm.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://gvi.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://tip.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://hbu.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://oex.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jhp.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sil.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cej.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxs.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://hfp.0kj1m.cn

Go:   func add(a, b int) int
来源：http://nub.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lts.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mcm.ctjpmb.com

[C14] 泛型函数
来源：http://crz.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ria.zhongyouzk.top

PHP:  // 无泛型
来源：http://qpg.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://ptp.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tzd.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zzl.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hto.chenzaomai.com

Ruby: # 无泛型
来源：http://wqp.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cqm.fzhhl.top

[C15] 解构 / 展开参数
来源：http://sbd.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eul.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://uan.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bvi.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ego.mhx1999.top

Java: // 无解构
来源：http://aoh.feifeiyinyue.top

Go:   // 无解构
来源：http://frk.sxryk.cn

Ruby: a, b = pair
来源：http://shi.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://bep.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://xrt.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nku.shzxlz.cn

PHP:  // 无重载
来源：http://gfl.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cgq.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://zpz.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vlq.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://rao.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://gol.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qzf.kuanghao11.cn

================================================================================
来源：http://jmb.tanke756.top

D. 数组 / 列表 / 集合
来源：http://cav.316326.xyz

================================================================================
来源：http://eyq.fengsongda.top

[D01] 创建数组 / 列表
来源：http://dxq.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ybq.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cnw.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gkv.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bpt.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fjz.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://ipf.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://sab.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xya.yj20258.top

[D02] 追加元素到末尾
来源：http://pbc.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ata.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://spu.chenjidiqi.icu

JS:   arr.push(4);
来源：http://dep.bbcook.cn

TS:   arr.push(4);
来源：http://ijq.yongpay.top

Java: list.add(4);
来源：http://sod.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://puk.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://dkv.daxiang520.top

C#:   list.Add(4);
来源：http://kwc.bbcook.cn

[D03] 在指定位置插入元素
来源：http://nlp.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://mpr.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fdh.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ftu.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://bnv.nanxuanxn.top

Java: list.add(0, 0);
来源：http://yds.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://qke.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fkh.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://lip.316326.xyz

[D04] 删除元素
来源：http://tjs.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hoe.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vsn.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wyr.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://kfz.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xzz.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ofs.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vus.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nth.zycfv.cn

[D05] 访问与修改元素
来源：http://elx.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ysm.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nuo.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rqd.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://krg.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://lqm.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://zqt.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vbp.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ffv.sxryk.cn

[D06] 数组长度
来源：http://lye.fehbvm.com

Py:   len(arr)
来源：http://veo.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://rtl.meibo888.top

JS:   arr.length
来源：http://xaz.fzhhl.top

TS:   arr.length
来源：http://jwf.jinyuanbaomall.cn


<!-- 参考信息 -->