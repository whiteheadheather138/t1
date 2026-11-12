代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://bni.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://gtl.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://evn.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://ila.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ayf.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://uzg.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oop.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ttf.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xhg.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ycb.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zrv.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xhs.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uge.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nsp.hywenlv.cn

[B07] while 循环
来源：http://lpj.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://dlb.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://cvr.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://lku.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://huv.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://ivf.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ivx.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://lnc.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://kju.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://yaw.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://fko.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mqf.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://ztc.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://xaq.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://yfo.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ruw.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://msk.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://xln.zhiwuduotai.top

[B09] break 与 continue
来源：http://zss.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kpf.xziqi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ucl.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsb.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rml.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdv.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqj.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mzz.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddn.c1oappe.top

[B10] 遍历同时拿索引
来源：http://rpe.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kht.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lhh.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://adu.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ybm.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://saw.ywan-chungtsiang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wbq.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nuo.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xkb.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://cub.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://hfy.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://qcr.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjv.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xnv.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yjo.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gdx.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://tqz.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ncp.haohaochexian.top

[B12] 跳出多层循环
来源：http://uvh.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dbr.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zsq.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lud.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dro.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mvx.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oap.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cdk.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jgn.snrcjt.cn

[B13] 判断是否为数字
来源：http://psd.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://rge.yfazqb.com

PHP:  is_numeric($x)
来源：http://pnw.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zls.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fum.daxiang520.top

Java: x instanceof Number
来源：http://tzk.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mgd.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://ykn.c1oappe.top

C#:   x is int or double or decimal
来源：http://vak.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://mbi.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wxj.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fql.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://zef.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://qai.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gpy.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nct.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cph.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gqg.shzxlz.cn

[B15] 布尔运算与取反
来源：http://clo.chenlongwang.top

Py:   a and b or not c
来源：http://dat.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://nst.ctjpmb.com

JS:   a && b || !c
来源：http://stj.cucudq.cn

TS:   a && b || !c
来源：http://eyk.cdnleiting.top

Java: a && b || !c
来源：http://nmc.chenzaomai.com

Go:   a && b || !c
来源：http://ezl.dashuyun.cn

Ruby: a && b || !c
来源：http://yae.guowangkeji.top

C#:   a && b || !c
来源：http://rhn.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://zyw.xuanzx.com

Py:   if not data: return
来源：http://uuo.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://vjn.tanke756.top

JS:   if (!data) return;
来源：http://gwl.shuidangran.top

TS:   if (!data) return;
来源：http://ipq.birdmap.top

Java: if (data == null) return;
来源：http://cgu.aibaodan.cn

Go:   if data == nil { return }
来源：http://eaj.cdnleiting.top

Ruby: return if data.nil?
来源：http://dom.xziqi.cn

C#:   if (data == null) return;
来源：http://vyv.daria6918.cn

================================================================================
来源：http://lri.meibo888.top

C. 函数与作用域
来源：http://flg.gogol.net.cn

================================================================================
来源：http://yjp.xziqi.cn

[C01] 定义函数
来源：http://esn.tanke756.top

Py:   def add(a, b): return a + b
来源：http://vok.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://icy.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://rwe.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptf.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://smh.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://rva.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://yot.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cbn.chenlongwang.top

[C02] 默认参数
来源：http://cwq.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://ubv.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lnc.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://laz.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tpn.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lze.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wnk.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://tjl.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://fkd.zhoulong.xyz

[C03] 可变参数
来源：http://tmf.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://bwe.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aza.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tky.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jtt.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hav.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ube.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://ffy.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jev.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://hje.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xar.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bck.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://efm.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dvq.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://jgh.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://rjl.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://gvc.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://blo.ehwqpu.com

[C05] 返回多个值
来源：http://yuh.sweek.top

Py:   return a, b
来源：http://pdk.sweek.top

PHP:  return [$a, $b];
来源：http://pnt.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jgr.zdqjudy.top

TS:   return { a, b };
来源：http://viz.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yjf.fzhhl.top

Go:   return a, b
来源：http://xmp.snrcjt.cn

Ruby: return a, b
来源：http://dod.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://utc.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://ctf.cheryme.top

Py:   square = lambda x: x * x
来源：http://vfv.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hgh.vehdjk.com

JS:   const square = x => x * x;
来源：http://ker.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://azk.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jag.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xck.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://kqf.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://mkp.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://uuv.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sug.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://mng.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tun.hysaishi.cn

TS:   arr.map(String)
来源：http://jgr.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yah.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vbs.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://opz.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://rqi.nanxinkj.top

[C08] 闭包
来源：http://vkx.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tdr.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shz.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lhm.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lbb.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vrf.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://izb.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dex.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xxp.wangshuangyany.cn

[C09] 递归
来源：http://wqn.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cpl.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbj.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ptd.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xki.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iah.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wur.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mgr.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yue.fengsongda.top

[C10] 变量作用域
来源：http://zyy.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nne.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fvw.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zml.sxryk.cn

TS:   同 JS
来源：http://lav.jyoumei.cn

Java: 方法内为块级作用域
来源：http://wvy.snrcjt.cn

Go:   花括号块级作用域
来源：http://iqi.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hct.cdnleiting.top

C#:   块级作用域
来源：http://teu.chenlongwang.top

[C11] 模块导入与导出
来源：http://ult.aizwys.cn

Py:   from module import func
来源：http://ngj.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bao.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bun.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://arr.cdnleiting.top

Java: import java.util.List;
来源：http://abh.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lqd.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://gds.316326.xyz

C#:   using System.Text;
来源：http://kqg.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://xpx.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://cjz.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://vjk.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://gdz.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://vdg.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ycw.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://maj.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://jbi.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qed.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://uxl.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://onb.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ica.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iuh.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dxs.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://aob.yvedp.cn

Go:   func add(a, b int) int
来源：http://xer.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uwz.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://okz.xinyue.icu

[C14] 泛型函数
来源：http://lej.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mti.jqgfzy.top

PHP:  // 无泛型
来源：http://gcl.quarkkingdee.top

JS:   // 无泛型
来源：http://yur.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yuh.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gys.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bac.yfazqb.com

Ruby: # 无泛型
来源：http://gmx.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucg.yueranfly.top

[C15] 解构 / 展开参数
来源：http://fpn.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dej.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://mmb.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gbw.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zlc.hywenlv.cn

Java: // 无解构
来源：http://fdf.zhiwuduotai.top

Go:   // 无解构
来源：http://oiy.fktsv.cn

Ruby: a, b = pair
来源：http://olc.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://url.yongpay.top

[C16] 函数 / 方法重载
来源：http://wjz.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ivr.yanxiufei.cn

PHP:  // 无重载
来源：http://frd.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bby.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://tfb.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wus.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://gkz.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://lok.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cpr.hfpthk.cn

================================================================================
来源：http://gnn.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://egh.svipenyu.cn

================================================================================
来源：http://wnx.uphjek.com

[D01] 创建数组 / 列表
来源：http://fdm.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://goe.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ozw.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vxn.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fpv.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wyq.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://ujo.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://fkn.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ocu.ydzc1.top

[D02] 追加元素到末尾
来源：http://erw.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hlv.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qrf.ybcxt.top

JS:   arr.push(4);
来源：http://kfu.pengpengdd.cyou

TS:   arr.push(4);
来源：http://iqn.cucudq.cn

Java: list.add(4);
来源：http://qua.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://wmn.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://kuo.nanxinkj.top

C#:   list.Add(4);
来源：http://vty.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://pjy.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://qcz.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gjl.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bho.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://ngb.mhx1999.top

Java: list.add(0, 0);
来源：http://aai.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bfm.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ono.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://mln.xinyue.icu

[D04] 删除元素
来源：http://zsy.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bmy.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gkk.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wrx.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://ann.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tdy.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yzo.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pid.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nku.jinqigufen.top

[D05] 访问与修改元素
来源：http://yzc.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://buf.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vtu.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vuw.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://adl.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://vmd.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ijv.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ofb.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jbt.jqgufenzy.top

[D06] 数组长度
来源：http://eke.chenlongwang.top


<!-- 参考信息 -->