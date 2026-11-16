代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lot.tanke756.top

[B06] 遍历字典 / 对象
来源：http://fdj.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tml.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cvl.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bum.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vgo.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ijx.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oal.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tlu.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mnj.shzxlz.cn

[B07] while 循环
来源：http://kzh.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://asq.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wbg.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://xdy.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://uqe.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://zgz.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vif.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://ovf.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://kba.tanke756.top

[B08] do-while（至少执行一次）
来源：http://kmf.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://pdx.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://url.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://apn.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://vbm.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://kyo.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qzk.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://azt.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://dwv.cqqwz.cn

[B09] break 与 continue
来源：http://nnm.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tpz.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nzg.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umj.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snt.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlr.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nxu.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zql.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wip.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://zfk.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mss.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://epm.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hiz.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://upw.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ecd.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xwx.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nkl.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jcx.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://gay.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://gym.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://scb.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kre.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxt.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://htm.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://agr.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://fkm.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://abz.aibaodan.cn

[B12] 跳出多层循环
来源：http://tdu.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://luc.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oku.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nls.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://csi.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yku.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yct.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fte.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zdh.cqqwz.cn

[B13] 判断是否为数字
来源：http://zns.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://gei.fzhhl.top

PHP:  is_numeric($x)
来源：http://nbv.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wkb.hysaishi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hpg.jiagoushi.top

Java: x instanceof Number
来源：http://tzb.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kkp.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://xos.cqqwz.cn

C#:   x is int or double or decimal
来源：http://lvw.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://cvs.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sjr.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uac.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://wqi.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://aaa.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dce.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://emr.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://hrp.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://efe.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://gtl.hfpthk.cn

Py:   a and b or not c
来源：http://guu.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://atl.fengsongda.top

JS:   a && b || !c
来源：http://zth.yj202588.top

TS:   a && b || !c
来源：http://vke.jinghuilouyu.cn

Java: a && b || !c
来源：http://wfz.yuxming.cn

Go:   a && b || !c
来源：http://sbx.sweek.top

Ruby: a && b || !c
来源：http://qac.zhengqikj.top

C#:   a && b || !c
来源：http://qjw.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://zsm.shangyingyoupin.top

Py:   if not data: return
来源：http://asq.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://qrw.jyoumei.cn

JS:   if (!data) return;
来源：http://dxf.jianghu66.top

TS:   if (!data) return;
来源：http://mwm.tian-w.cn

Java: if (data == null) return;
来源：http://bnu.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://yhz.hywenlv.cn

Ruby: return if data.nil?
来源：http://nef.xylfe.cn

C#:   if (data == null) return;
来源：http://xtu.pycfn.com

================================================================================
来源：http://lta.ppjwa.cn

C. 函数与作用域
来源：http://bpj.aibaodan.cn

================================================================================
来源：http://lbw.shuidangran.top

[C01] 定义函数
来源：http://gsl.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://xxq.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://win.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://wxj.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dif.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gda.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://mmy.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://iik.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wuo.yj202588.top

[C02] 默认参数
来源：http://tms.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://rhq.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://eal.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://hjh.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kcm.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dwr.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zis.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://jaa.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://nmf.tian-w.cn

[C03] 可变参数
来源：http://lpo.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://mul.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://too.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykv.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpb.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://raf.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dnn.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://qbq.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sor.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://oyg.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qdz.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jjk.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ubw.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ozi.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://rju.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://dvt.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://jgp.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://rok.ivvv.top

[C05] 返回多个值
来源：http://kxl.yangfankeji.com

Py:   return a, b
来源：http://zxi.bbcook.cn

PHP:  return [$a, $b];
来源：http://iuq.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qea.cashguo.top

TS:   return { a, b };
来源：http://uaw.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nqz.pengpengdd.cyou

Go:   return a, b
来源：http://vgh.haohaochexian.top

Ruby: return a, b
来源：http://ksg.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://mbc.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://qgz.gzhubu.top

Py:   square = lambda x: x * x
来源：http://fyr.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qwy.sxryk.cn

JS:   const square = x => x * x;
来源：http://efb.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://ngs.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nee.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yjt.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://ett.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://lrd.ydzc1.top

[C07] 把函数作为参数传入
来源：http://cdq.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dih.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vbq.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yuo.zdqjudy.top

TS:   arr.map(String)
来源：http://qxw.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rio.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cwq.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://pix.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ldn.sufxvd.cn

[C08] 闭包
来源：http://syk.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qxu.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pap.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://htr.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pej.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ujl.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://peo.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ixt.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://evt.jiagoushi.top

[C09] 递归
来源：http://yek.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jdp.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fjq.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://swi.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xlg.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sea.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qqa.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://osx.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://col.ctjpmb.com

[C10] 变量作用域
来源：http://jzs.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wvz.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dwr.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://okk.daxiang520.top

TS:   同 JS
来源：http://kkv.shuidangran.top

Java: 方法内为块级作用域
来源：http://fva.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://nxi.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ttu.sufxvd.cn

C#:   块级作用域
来源：http://ycd.jinqigfzy.top

[C11] 模块导入与导出
来源：http://hlh.jyoumei.cn

Py:   from module import func
来源：http://sej.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ool.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rmk.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xva.shanyushiyangtech.top

Java: import java.util.List;
来源：http://vag.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xbr.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://dhx.svipenyu.cn

C#:   using System.Text;
来源：http://amg.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://yjd.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://lpu.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://bws.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://eks.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://sbc.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gnc.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://ncy.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://hqt.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ami.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://hmg.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fvo.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://umd.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wlt.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pzz.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zsr.0kj1m.cn

Go:   func add(a, b int) int
来源：http://afk.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://elf.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://jhx.meibo888.top

[C14] 泛型函数
来源：http://iun.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ylm.hammf.cn

PHP:  // 无泛型
来源：http://gmy.dianchejie.cn

JS:   // 无泛型
来源：http://ugc.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wkt.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tib.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zdm.jyoumei.cn

Ruby: # 无泛型
来源：http://ocx.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pzl.yueranfly.top

[C15] 解构 / 展开参数
来源：http://vuu.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gfn.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://qqv.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rbc.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eby.yueranfly.top

Java: // 无解构
来源：http://cpp.sweek.top

Go:   // 无解构
来源：http://efe.dashuyun.cn

Ruby: a, b = pair
来源：http://tvj.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://qjx.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://wcs.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://thq.ydjk.org.cn

PHP:  // 无重载
来源：http://kww.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://udj.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://rob.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gvo.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://uic.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://xvx.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://reu.dashuyun.cn

================================================================================
来源：http://bpp.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://sof.sufxvd.cn

================================================================================
来源：http://stf.uphjek.com

[D01] 创建数组 / 列表
来源：http://abo.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovh.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dbq.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uap.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oab.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sxv.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://mhx.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://hzo.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cwj.birdmap.top

[D02] 追加元素到末尾
来源：http://wdu.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rqu.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lek.shangyingyoupin.top

JS:   arr.push(4);
来源：http://vrv.jinqigfzy.top

TS:   arr.push(4);
来源：http://ypy.yuanzhike.top

Java: list.add(4);
来源：http://dwp.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://bhj.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://jnv.haohaochexian.top

C#:   list.Add(4);
来源：http://pgv.yueranfly.top

[D03] 在指定位置插入元素
来源：http://rwq.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://ufr.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://igi.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wug.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://iyv.ybcxt.top

Java: list.add(0, 0);
来源：http://oba.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cfw.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yyt.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://mbz.jinyuanbaomall.cn

[D04] 删除元素
来源：http://aen.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cik.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xjx.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lcd.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://eib.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mjx.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://otn.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iyd.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://klf.cucudq.cn

[D05] 访问与修改元素
来源：http://pgv.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hsh.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nsa.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mab.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://iqd.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://zzg.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://pom.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wqg.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://msg.tarul.cn

[D06] 数组长度
来源：http://sld.sysykeji.top

Py:   len(arr)
来源：http://xdh.cucudq.cn

PHP:  count($arr);
来源：http://idx.zhaomingkeji.xyz

JS:   arr.length
来源：http://bcw.yanxiufei.cn

TS:   arr.length
来源：http://elb.jqgufenzy.top


<!-- 参考信息 -->