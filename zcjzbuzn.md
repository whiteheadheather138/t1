代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xpe.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dkf.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://bjh.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xan.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://zba.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://qqg.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://klh.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wef.yuxming.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://aoe.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vjr.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rzs.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://mlz.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ala.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://mxm.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://eta.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sgb.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jor.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dof.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rzp.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kiz.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ceu.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xck.zhongyouzk.top

[B07] while 循环
来源：http://uqz.zycfv.cn

Py:   while i < 10: i += 1
来源：http://qfb.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://uvl.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://qpl.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://ybl.yonumen.top

Java: while (i < 10) { i++; }
来源：http://jtb.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qam.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://mjn.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://wtc.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://qsg.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://hpj.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rmw.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://mhz.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://qku.ivvv.top

Java: do { i++; } while (i < 10);
来源：http://wdp.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tgh.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fdn.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://iuy.yj202588.top

[B09] break 与 continue
来源：http://bhb.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rlc.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aet.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dng.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsg.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nua.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nzs.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://edj.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysq.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://axb.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mft.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://apx.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ibo.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wom.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://afh.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xnj.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eeo.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://luz.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://zxy.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://lhw.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://ije.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uyp.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mok.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dai.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eqs.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://tws.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zcn.yanxiufei.cn

[B12] 跳出多层循环
来源：http://hgc.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nzu.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://bkv.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddh.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xhy.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zrp.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nwz.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hge.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aab.gzhubu.top

[B13] 判断是否为数字
来源：http://lnj.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://jqf.chenlongwang.top

PHP:  is_numeric($x)
来源：http://hcf.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://krk.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ytv.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://ybj.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bjo.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://fdr.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://kwe.vehdjk.com

[B14] 判断值是否在集合内
来源：http://tae.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nez.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://amo.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://yuq.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://wtw.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lew.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jvs.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://nhu.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zfk.gzhubu.top

[B15] 布尔运算与取反
来源：http://dir.fehbvm.com

Py:   a and b or not c
来源：http://vdi.c1oappe.top

PHP:  $a && $b || !$c
来源：http://jre.yonumen.top

JS:   a && b || !c
来源：http://sxa.guannengcc.top

TS:   a && b || !c
来源：http://qfc.pycfn.com

Java: a && b || !c
来源：http://gav.nanxuanxn.top

Go:   a && b || !c
来源：http://msy.shangyingyoupin.top

Ruby: a && b || !c
来源：http://mov.chenzaomai.com

C#:   a && b || !c
来源：http://zbn.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://ozy.jinqigufen.top

Py:   if not data: return
来源：http://kyb.cashguo.top

PHP:  if (!$data) { return; }
来源：http://gxr.cqqwz.cn

JS:   if (!data) return;
来源：http://bcs.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://tec.yonumen.top

Java: if (data == null) return;
来源：http://xze.snrcjt.cn

Go:   if data == nil { return }
来源：http://jad.hammf.cn

Ruby: return if data.nil?
来源：http://htf.svipenyu.cn

C#:   if (data == null) return;
来源：http://hbn.fehbvm.com

================================================================================
来源：http://muc.yfazqb.com

C. 函数与作用域
来源：http://iaw.ybcxt.top

================================================================================
来源：http://acz.xuetiantiany.cn

[C01] 定义函数
来源：http://byq.meibo888.top

Py:   def add(a, b): return a + b
来源：http://ymx.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tem.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://rai.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://izu.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kuz.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://mwu.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://hgz.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dxn.xuetiantiany.cn

[C02] 默认参数
来源：http://xtw.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://rnk.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qvn.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://qgl.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://yzz.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pnp.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mdk.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://ehm.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://dlo.hnxiangtu.top

[C03] 可变参数
来源：http://dch.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://nle.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tsl.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpw.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://idl.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ncj.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kkt.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://gpc.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ina.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://csu.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zka.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://snj.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wzd.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gwg.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://frr.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://nue.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://ywa.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://adg.aizwys.cn

[C05] 返回多个值
来源：http://zva.zhixingplan.top

Py:   return a, b
来源：http://skh.cucudq.cn

PHP:  return [$a, $b];
来源：http://wah.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eci.xziqi.cn

TS:   return { a, b };
来源：http://jxg.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jvf.tianlin.xyz

Go:   return a, b
来源：http://psi.shzxlz.cn

Ruby: return a, b
来源：http://cqg.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://sql.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://vkl.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://rpt.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://upy.cqqwz.cn

JS:   const square = x => x * x;
来源：http://wjn.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://lgx.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://suo.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://syk.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://xlz.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://rhu.bjfxy.top

[C07] 把函数作为参数传入
来源：http://eig.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pmq.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://omr.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vnx.zhoulong.xyz

TS:   arr.map(String)
来源：http://pwn.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rfy.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yru.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://iou.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://gmn.zhiwuduotai.top

[C08] 闭包
来源：http://iql.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mrh.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cih.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jni.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xpa.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://swp.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cjj.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fid.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjc.jinghuilouyu.cn

[C09] 递归
来源：http://xgn.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hdg.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hlj.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jje.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dyj.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://slv.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://efn.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yuo.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ybe.zhiwuduotai.top

[C10] 变量作用域
来源：http://wsb.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wew.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rsv.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://evt.svipenyu.cn

TS:   同 JS
来源：http://xxm.xuanzx.com

Java: 方法内为块级作用域
来源：http://dsj.meibo888.top

Go:   花括号块级作用域
来源：http://jcf.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ouu.shangyingyoupin.top

C#:   块级作用域
来源：http://hoa.epnwcf.com

[C11] 模块导入与导出
来源：http://alo.dashuyun.cn

Py:   from module import func
来源：http://cxy.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://onl.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fct.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vrr.ctjpmb.com

Java: import java.util.List;
来源：http://sfa.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zpo.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://bkn.cdnleiting.top

C#:   using System.Text;
来源：http://crr.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://zfr.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://zbi.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://rgy.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://jai.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://nlg.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mpf.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://hxd.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://njp.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tyo.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://dji.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bfv.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jva.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wnh.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gif.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fhb.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://pme.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bla.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://vlf.xuanzx.com

[C14] 泛型函数
来源：http://din.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kni.kuanghao11.cn

PHP:  // 无泛型
来源：http://bvm.cashguo.top

JS:   // 无泛型
来源：http://uhp.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zzr.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gbo.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qbh.hywenlv.cn

Ruby: # 无泛型
来源：http://lry.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ovj.tian-w.cn

[C15] 解构 / 展开参数
来源：http://rka.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://twz.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ldx.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zzr.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zyy.gotoacloud.top

Java: // 无解构
来源：http://fwv.guannengcc.top

Go:   // 无解构
来源：http://rvu.redwolf501.top

Ruby: a, b = pair
来源：http://bhe.52xcode.cn

C#:   var (a, b) = pair;
来源：http://csm.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://ltu.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qih.nwbrower.top

PHP:  // 无重载
来源：http://vgh.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://roc.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://eus.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zil.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://ljm.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://nfm.birdmap.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tmr.jiagoushi.top

================================================================================
来源：http://bkc.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://tad.gaohongyu789.top

================================================================================
来源：http://emr.yj20258.top

[D01] 创建数组 / 列表
来源：http://yqa.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rxu.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fif.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wgq.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pko.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ntz.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://voq.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://gjy.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qqb.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://gys.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hlq.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tiu.ehwqpu.com

JS:   arr.push(4);
来源：http://gzl.shzxlz.cn

TS:   arr.push(4);
来源：http://lnw.ybcxt.top

Java: list.add(4);
来源：http://ihf.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://ixu.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://usg.bbcook.cn

C#:   list.Add(4);
来源：http://vjp.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://fot.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://jpd.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wzz.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tvi.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://svi.zycfv.cn

Java: list.add(0, 0);
来源：http://kls.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ddi.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eba.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://caf.hywenlv.cn

[D04] 删除元素
来源：http://oii.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://chh.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xil.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fsj.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://muv.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oco.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jlu.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wcr.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qnm.zhongyouzk.top

[D05] 访问与修改元素
来源：http://bod.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rwc.zhijiandao.cn


<!-- 参考信息 -->