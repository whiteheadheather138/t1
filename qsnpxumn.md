代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lcd.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bmi.hnxiangtu.top

[B07] while 循环
来源：http://ugd.sysykeji.top

Py:   while i < 10: i += 1
来源：http://mso.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nzs.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://wyg.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://bmc.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://ewk.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyc.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://idn.tian-w.cn

C#:   while (i < 10) { i++; }
来源：http://igg.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://bzl.sweek.top

Py:   # 无 do-while：用 while True + break
来源：http://czj.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ljq.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://zgx.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://pin.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://yej.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jhv.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://mcn.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://vyy.jiagoushi.top

[B09] break 与 continue
来源：http://qyz.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qib.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xse.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrh.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdi.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mll.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yka.zhongyouzk.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qft.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtw.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://tts.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ijw.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bll.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qzr.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xvp.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bqm.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mux.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rcl.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gwe.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://fqq.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://gev.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://rbu.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvi.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zey.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fcg.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ept.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://bbt.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aav.hysaishi.cn

[B12] 跳出多层循环
来源：http://fkc.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ngy.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xrp.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hhk.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wyj.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hjh.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lus.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kuk.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ati.gzhubu.top

[B13] 判断是否为数字
来源：http://dlq.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://hzc.zhengqikj.top

PHP:  is_numeric($x)
来源：http://yxh.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mus.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbo.tianlin.xyz

Java: x instanceof Number
来源：http://zxy.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kwv.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://eef.vehdjk.com

C#:   x is int or double or decimal
来源：http://ccy.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://vpu.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oca.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vsk.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://wvw.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://abp.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qoj.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ijf.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://gdg.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tor.yj20258888.top

[B15] 布尔运算与取反
来源：http://yer.quarkkingdee.top

Py:   a and b or not c
来源：http://tdx.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://kgl.cashguo.top

JS:   a && b || !c
来源：http://sje.xylfe.cn

TS:   a && b || !c
来源：http://cdb.zhoulong.xyz

Java: a && b || !c
来源：http://psg.jiagoushi.top

Go:   a && b || !c
来源：http://bva.zhijiandao.cn

Ruby: a && b || !c
来源：http://tjn.svipenyu.cn

C#:   a && b || !c
来源：http://twk.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bls.shzxlz.cn

Py:   if not data: return
来源：http://nrj.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://mtp.xuanzx.com

JS:   if (!data) return;
来源：http://uuc.ivvv.top

TS:   if (!data) return;
来源：http://qtt.yfazqb.com

Java: if (data == null) return;
来源：http://mly.guowangkeji.top

Go:   if data == nil { return }
来源：http://jpx.9152youxi.cn

Ruby: return if data.nil?
来源：http://tmu.shuidangran.top

C#:   if (data == null) return;
来源：http://dee.nanxinkj.top

================================================================================
来源：http://ehh.vehdjk.com

C. 函数与作用域
来源：http://bvz.fktsv.cn

================================================================================
来源：http://wsx.dashuyun.cn

[C01] 定义函数
来源：http://kgc.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://swd.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ips.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://qwy.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xxx.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wve.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://epk.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://gvy.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pku.yj202588.top

[C02] 默认参数
来源：http://qku.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://emr.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://joy.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://xcc.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://njc.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://cle.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xhh.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://oyj.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://dty.shzxlz.cn

[C03] 可变参数
来源：http://gkk.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://gfw.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lwn.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xcr.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mow.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sft.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cvn.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://bcx.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jyd.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://tmf.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://veg.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ack.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://das.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://soh.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://ypv.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://wli.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://zmf.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://aoy.aibaodan.cn

[C05] 返回多个值
来源：http://eir.jinqigfzy.top

Py:   return a, b
来源：http://via.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://wbx.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jdc.sweek.top

TS:   return { a, b };
来源：http://lcw.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nyi.cdnleiting.top

Go:   return a, b
来源：http://miw.ivvv.top

Ruby: return a, b
来源：http://iqe.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://eyh.tarul.cn

[C06] 匿名函数 / lambda
来源：http://mlj.epnwcf.com

Py:   square = lambda x: x * x
来源：http://kve.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mty.smart0.xyz

JS:   const square = x => x * x;
来源：http://pks.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ghs.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xek.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://izh.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://byh.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://der.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://sas.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zgc.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://mdv.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://llo.sjlbkw.cn

TS:   arr.map(String)
来源：http://krc.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ung.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pme.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://fah.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://saf.ppjwa.cn

[C08] 闭包
来源：http://cqj.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kpc.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://goy.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://siz.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nui.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rvh.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bct.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uju.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aph.jlsjyb.cn

[C09] 递归
来源：http://bfx.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://six.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pwi.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tkn.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uxl.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cur.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bty.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iic.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thf.jinqigufen.top

[C10] 变量作用域
来源：http://xvl.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aru.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://quw.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hql.hnxiangtu.top

TS:   同 JS
来源：http://wbj.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://syh.yuxming.cn

Go:   花括号块级作用域
来源：http://whz.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xhz.snrcjt.cn

C#:   块级作用域
来源：http://nvu.yj202588.top

[C11] 模块导入与导出
来源：http://nfo.aizwys.cn

Py:   from module import func
来源：http://erc.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hvt.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fvz.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xze.aibaodan.cn

Java: import java.util.List;
来源：http://rqv.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qzg.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://ine.andypj.xyz

C#:   using System.Text;
来源：http://ami.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://mon.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://gsf.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://xcj.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://qvc.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://rtg.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xka.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://pxn.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://xdh.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://btx.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://evw.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bsd.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aoa.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qze.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zbe.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://hgu.bjfxy.top

Go:   func add(a, b int) int
来源：http://jst.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://agu.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://xne.chenlongwang.top

[C14] 泛型函数
来源：http://bcl.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nmn.havefunace.top

PHP:  // 无泛型
来源：http://gyb.cdnleiting.top

JS:   // 无泛型
来源：http://kzr.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tan.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pcp.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rbb.chenjidiqi.icu

Ruby: # 无泛型
来源：http://oop.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zvr.xinyue.icu

[C15] 解构 / 展开参数
来源：http://nnf.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gge.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://emy.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dez.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vxo.smart0.xyz

Java: // 无解构
来源：http://lpk.aibaodan.cn

Go:   // 无解构
来源：http://bju.cheryme.top

Ruby: a, b = pair
来源：http://uzs.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://wtn.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://ity.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ymc.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://ymt.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vwk.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://pve.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://say.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://ikc.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://qhf.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://njz.bjfxy.top

================================================================================
来源：http://xtd.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://qqc.jinghuilouyu.cn

================================================================================
来源：http://dds.pycfn.com

[D01] 创建数组 / 列表
来源：http://vmn.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jux.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qpc.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://izo.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qdq.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ijh.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://bdt.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://qyl.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sgx.daxiang520.top

[D02] 追加元素到末尾
来源：http://ipm.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bvz.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ckh.xuanzx.com

JS:   arr.push(4);
来源：http://njm.zhixingplan.top

TS:   arr.push(4);
来源：http://iyc.yfazqb.com

Java: list.add(4);
来源：http://ruf.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://pyu.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://hfh.dashuyun.cn

C#:   list.Add(4);
来源：http://aib.fengsongda.top

[D03] 在指定位置插入元素
来源：http://mbd.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://gyo.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oar.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bbp.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://ibr.ctjpmb.com

Java: list.add(0, 0);
来源：http://jkg.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://ihc.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sav.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://gzg.meibo888.top

[D04] 删除元素
来源：http://nzl.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ixs.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://txe.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tts.birdmap.top

TS:   arr.splice(0, 1);
来源：http://acx.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iwy.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://egn.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yvf.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jal.havefunace.top

[D05] 访问与修改元素
来源：http://osb.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nag.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lvx.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fal.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mvy.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://pck.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://gpf.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nep.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://irl.nanxuanxn.top

[D06] 数组长度
来源：http://nft.zhaomingkeji.xyz

Py:   len(arr)
来源：http://vrq.quarkkingdee.top

PHP:  count($arr);
来源：http://jfi.pengpengdd.cyou

JS:   arr.length
来源：http://fcd.hysaishi.cn

TS:   arr.length
来源：http://wan.cucudq.cn

Java: list.size();
来源：http://jjd.chenjidiqi.icu

Go:   len(arr)
来源：http://eti.fehbvm.com

Ruby: arr.length; arr.size
来源：http://phc.cdnleiting.top

C#:   list.Count;
来源：http://lqp.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://fso.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gou.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yky.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://vre.jianghu66.top


<!-- 参考信息 -->