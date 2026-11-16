代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zhr.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ovp.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://dsd.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hmb.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://ssb.iojbl.cn

Py:   for item in arr: print(item)
来源：http://lpo.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tfp.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uox.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://dvv.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gsc.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wxn.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://nre.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://inf.hnxiangtu.top

[B06] 遍历字典 / 对象
来源：http://lzw.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nhq.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ksb.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oqz.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxy.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pdl.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ywu.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fzi.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zyk.zdqjudy.top

[B07] while 循环
来源：http://suc.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://jiv.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://sbt.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://wso.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://lxv.tarul.cn

Java: while (i < 10) { i++; }
来源：http://ngz.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oav.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://phe.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://sax.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://vmg.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://nxa.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://plz.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://rca.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://jbc.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://jwg.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://zyj.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://uvg.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://cfe.yangfankeji.com

[B09] break 与 continue
来源：http://dzj.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nbl.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rjc.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxu.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nge.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eei.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kln.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qaa.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlf.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://hsc.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kes.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hqj.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lbk.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ymj.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tla.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uir.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ewh.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://umy.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://kht.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://woj.ivvv.top

PHP:  range(0, 10, 2);
来源：http://gds.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufw.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aif.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mij.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://scb.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://vmj.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jjl.tanke756.top

[B12] 跳出多层循环
来源：http://uxl.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lsz.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rfl.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://exz.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ake.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://voo.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pnx.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iki.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tob.yanxiufei.cn

[B13] 判断是否为数字
来源：http://fvf.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://nen.zhixingplan.top

PHP:  is_numeric($x)
来源：http://ypb.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsu.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nkr.daria6918.cn

Java: x instanceof Number
来源：http://xca.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bvl.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://ysr.uphjek.com

C#:   x is int or double or decimal
来源：http://xup.birdmap.top

[B14] 判断值是否在集合内
来源：http://oui.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ilo.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fsd.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://vxa.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://nbv.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cph.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://clu.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://hmh.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ehi.xuanzx.com

[B15] 布尔运算与取反
来源：http://mou.jiagoushi.top

Py:   a and b or not c
来源：http://svj.aizwys.cn

PHP:  $a && $b || !$c
来源：http://msw.zhiwuduotai.top

JS:   a && b || !c
来源：http://hxo.9152youxi.cn

TS:   a && b || !c
来源：http://lsv.cdnleiting.top

Java: a && b || !c
来源：http://nop.hfpthk.cn

Go:   a && b || !c
来源：http://tnd.c1oappe.top

Ruby: a && b || !c
来源：http://quc.sweek.top

C#:   a && b || !c
来源：http://sdi.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://hvj.ybcxt.top

Py:   if not data: return
来源：http://uqk.cashguo.top

PHP:  if (!$data) { return; }
来源：http://fov.jlsjyb.cn

JS:   if (!data) return;
来源：http://cbq.fehbvm.com

TS:   if (!data) return;
来源：http://ztu.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://anh.meibo888.top

Go:   if data == nil { return }
来源：http://fdt.uphjek.com

Ruby: return if data.nil?
来源：http://ket.0kj1m.cn

C#:   if (data == null) return;
来源：http://ijs.shzxlz.cn

================================================================================
来源：http://aty.yanxiufei.cn

C. 函数与作用域
来源：http://bui.cdnleiting.top

================================================================================
来源：http://vfx.meibo888.top

[C01] 定义函数
来源：http://zrw.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://cix.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ufg.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://tos.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xna.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oyd.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://slo.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://xxc.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rax.yj20258888.top

[C02] 默认参数
来源：http://yzn.havefunace.top

Py:   def greet(name="World"): return name
来源：http://gld.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sgi.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://fxn.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eah.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://apl.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jbp.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://qab.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://enr.meibo888.top

[C03] 可变参数
来源：http://oxs.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://lak.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://abg.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iqd.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zqr.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ryr.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://apk.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://qsj.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bmn.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://pcg.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vvy.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eon.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pej.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hhk.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://dzz.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://itv.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://kvf.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://ogi.jqgufenzy.top

[C05] 返回多个值
来源：http://jwc.ywan-chungtsiang.top

Py:   return a, b
来源：http://irh.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://fnb.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qdk.shanyushiyangtech.top

TS:   return { a, b };
来源：http://sxs.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pug.uphjek.com

Go:   return a, b
来源：http://cvq.0kj1m.cn

Ruby: return a, b
来源：http://vjd.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://fws.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://oee.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://uwz.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xcf.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://kjf.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://jnm.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zvl.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://zjh.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://cul.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://dfn.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://cve.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dye.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://rbi.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mdk.yj20258888.top

TS:   arr.map(String)
来源：http://wpt.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xth.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cec.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://avq.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nft.chenjidiqi.icu

[C08] 闭包
来源：http://ppg.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xju.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://scf.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ehi.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gru.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nld.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sag.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jda.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mpd.jqgufenzy.top

[C09] 递归
来源：http://hbr.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ssx.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fxb.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwp.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ozu.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vkh.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zrp.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tbh.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://akr.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://ohs.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dzh.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://len.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vae.jinghuilouyu.cn

TS:   同 JS
来源：http://qzw.nanxinkj.top

Java: 方法内为块级作用域
来源：http://fkx.haohaochexian.top

Go:   花括号块级作用域
来源：http://hez.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ukh.uphjek.com

C#:   块级作用域
来源：http://jlh.vqdsnc.cn

[C11] 模块导入与导出
来源：http://fdv.zhengqikj.top

Py:   from module import func
来源：http://goe.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ixa.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vnx.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pml.cheryme.top

Java: import java.util.List;
来源：http://dys.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ijs.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://gzv.zhijiandao.cn

C#:   using System.Text;
来源：http://uac.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://asc.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://xga.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://wsi.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://lcs.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://wqw.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hgc.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://cfq.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://rnw.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://tio.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://ywk.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xgz.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jyk.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://erp.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqz.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://mun.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://mme.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uih.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://aqu.zhoulong.xyz

[C14] 泛型函数
来源：http://ell.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ogq.daxiang520.top

PHP:  // 无泛型
来源：http://irf.jinqigfzy.top

JS:   // 无泛型
来源：http://ttt.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uet.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aga.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vwd.epnwcf.com

Ruby: # 无泛型
来源：http://oia.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zsr.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://gpi.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hdj.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://eyy.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://joa.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kis.tanke756.top

Java: // 无解构
来源：http://tuj.andypj.xyz

Go:   // 无解构
来源：http://xik.9152youxi.cn

Ruby: a, b = pair
来源：http://tzc.xinyue.icu

C#:   var (a, b) = pair;
来源：http://hyw.shanyushiyangtech.top

[C16] 函数 / 方法重载
来源：http://qlj.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tej.ehwqpu.com

PHP:  // 无重载
来源：http://bmn.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://seo.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://inb.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://qfp.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://xsu.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://oum.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ezq.ctjpmb.com

================================================================================
来源：http://lux.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://wwy.zhijiandao.cn

================================================================================
来源：http://umb.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://aij.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jbu.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hay.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wym.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ynn.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nou.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://sbt.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://fdk.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dhf.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://uqf.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://omw.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kfl.nanxuanxn.top

JS:   arr.push(4);
来源：http://cqq.ctjpmb.com

TS:   arr.push(4);
来源：http://cgg.fengsongda.top

Java: list.add(4);
来源：http://azr.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://gaj.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://mhy.fktsv.cn

C#:   list.Add(4);
来源：http://dbf.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://inp.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://vrl.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zpf.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bao.yanxiufei.cn

TS:   arr.splice(0, 0, 0);
来源：http://jvo.tanke756.top

Java: list.add(0, 0);
来源：http://gsi.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://vin.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qwi.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://ccd.yj202588.top

[D04] 删除元素
来源：http://vnk.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://byi.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xtv.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sli.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://qie.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://frj.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tnp.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dfa.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wsz.tanke756.top

[D05] 访问与修改元素
来源：http://oaj.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cxq.gzhubu.top


<!-- 参考信息 -->