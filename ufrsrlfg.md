代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gba.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://aeb.zdbjq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://trf.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hlo.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lom.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kot.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iha.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hwm.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lgh.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ezy.pycfn.com

[B07] while 循环
来源：http://gjq.daria6918.cn

Py:   while i < 10: i += 1
来源：http://ltq.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://rji.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://jtx.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://fnn.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://vig.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rlj.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://uqi.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://pua.havefunace.top

[B08] do-while（至少执行一次）
来源：http://edf.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://luv.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ive.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://psi.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://wtn.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://low.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://izq.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://dsy.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://bkt.ehwqpu.com

[B09] break 与 continue
来源：http://ycd.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjn.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lsf.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqk.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yrm.sufxvd.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hud.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tmn.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cbh.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgo.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://uxo.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://myk.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wqn.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pro.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lts.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uby.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jty.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ibs.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iep.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://xfz.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://bct.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://eew.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrj.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rch.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xmz.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dsi.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://hpu.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ueo.zhijiandao.cn

[B12] 跳出多层循环
来源：http://agu.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zgk.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jba.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lhn.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtp.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bfr.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kjy.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ogk.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iwf.tarul.cn

[B13] 判断是否为数字
来源：http://tkv.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://urm.aibaodan.cn

PHP:  is_numeric($x)
来源：http://icl.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nxs.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xsa.yanxiufei.cn

Java: x instanceof Number
来源：http://mcn.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ulm.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://vwt.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://fcr.52xcode.cn

[B14] 判断值是否在集合内
来源：http://uem.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pio.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yiu.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://aom.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://jmt.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://thf.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yuj.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://spz.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nln.zycfv.cn

[B15] 布尔运算与取反
来源：http://ebk.tian-w.cn

Py:   a and b or not c
来源：http://spg.iojbl.cn

PHP:  $a && $b || !$c
来源：http://urn.xuanzx.com

JS:   a && b || !c
来源：http://hhy.guannengcc.top

TS:   a && b || !c
来源：http://awo.cqqwz.cn

Java: a && b || !c
来源：http://hec.nwbrower.top

Go:   a && b || !c
来源：http://ope.cqqwz.cn

Ruby: a && b || !c
来源：http://vlk.nwbrower.top

C#:   a && b || !c
来源：http://bfc.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://tmr.ybcxt.top

Py:   if not data: return
来源：http://wvg.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://pnx.hysaishi.cn

JS:   if (!data) return;
来源：http://ncv.tian-w.cn

TS:   if (!data) return;
来源：http://hzh.zhijiandao.cn

Java: if (data == null) return;
来源：http://zqf.jqgfzy.top

Go:   if data == nil { return }
来源：http://vju.jiagoushi.top

Ruby: return if data.nil?
来源：http://sch.xziqi.cn

C#:   if (data == null) return;
来源：http://qyx.snrcjt.cn

================================================================================
来源：http://zhz.gogol.net.cn

C. 函数与作用域
来源：http://ppi.cheryme.top

================================================================================
来源：http://shn.tarul.cn

[C01] 定义函数
来源：http://goy.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://nyk.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://imk.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://vvz.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qla.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jqc.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://vwx.hcnkem.com

Ruby: def add(a, b); a + b; end
来源：http://ums.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bag.xuanzx.com

[C02] 默认参数
来源：http://pgr.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://ezf.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://szd.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://jrx.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mtn.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wgb.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zhd.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://cuw.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://mzh.sjlbkw.cn

[C03] 可变参数
来源：http://nqn.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://wdk.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ffw.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://joz.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zpr.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hhb.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tnt.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://ymd.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://onf.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://wxt.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cyh.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tbf.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cha.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lzp.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://kdk.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://kxl.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://wws.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://xzv.xinyue.icu

[C05] 返回多个值
来源：http://nko.chenzaomai.com

Py:   return a, b
来源：http://qnn.jiagoushi.top

PHP:  return [$a, $b];
来源：http://wxp.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ado.guowangkeji.top

TS:   return { a, b };
来源：http://yco.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ham.cucudq.cn

Go:   return a, b
来源：http://cxy.jiagoushi.top

Ruby: return a, b
来源：http://qed.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://ewh.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://cwi.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://xoz.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ojq.c1oappe.top

JS:   const square = x => x * x;
来源：http://bps.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://fsu.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rno.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://czh.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://txq.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://doo.bbcook.cn

[C07] 把函数作为参数传入
来源：http://yal.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nki.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xwn.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aun.shuidangran.top

TS:   arr.map(String)
来源：http://xjc.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zer.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bho.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://fcx.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lyd.vqdsnc.cn

[C08] 闭包
来源：http://vku.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ckb.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rut.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ycl.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jic.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hfh.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hct.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eyc.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aws.vehdjk.com

[C09] 递归
来源：http://nxg.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xcm.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tse.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://buf.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzj.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kzn.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dxz.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ead.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jmg.daxiang520.top

[C10] 变量作用域
来源：http://fcy.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://icr.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knv.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ofc.pycfn.com

TS:   同 JS
来源：http://qli.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://jxk.hesvh.cn

Go:   花括号块级作用域
来源：http://xpf.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://drj.ydjk.org.cn

C#:   块级作用域
来源：http://lyv.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://ghd.zdqjudy.top

Py:   from module import func
来源：http://fzj.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://pkc.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqo.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bbo.shuidangran.top

Java: import java.util.List;
来源：http://usv.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://csr.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://hdv.dashuyun.cn

C#:   using System.Text;
来源：http://ift.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://kfp.hammf.cn

Py:   (lambda: print("run"))()
来源：http://fqz.shuidangran.top

PHP:  (function () { echo "run"; })();
来源：http://jeo.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://emq.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://ami.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wbe.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://mwg.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://qtc.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://orq.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://kfc.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://frs.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pdj.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tpa.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jnk.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://prv.aizwys.cn

Go:   func add(a, b int) int
来源：http://fid.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tac.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bnn.daria6918.cn

[C14] 泛型函数
来源：http://flu.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://irm.uphjek.com

PHP:  // 无泛型
来源：http://xcs.wangshuangyany.cn

JS:   // 无泛型
来源：http://uoh.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qov.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://apq.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iuw.mhx1999.top

Ruby: # 无泛型
来源：http://hon.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kvy.yj202588.top

[C15] 解构 / 展开参数
来源：http://uut.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ibm.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://wuy.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rgm.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bio.zhaomingkeji.xyz

Java: // 无解构
来源：http://rfu.wangshuangyany.cn

Go:   // 无解构
来源：http://des.nanxinkj.top

Ruby: a, b = pair
来源：http://nom.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://iag.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://ubi.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ptu.316326.xyz

PHP:  // 无重载
来源：http://npx.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://quw.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://jjy.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://juz.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://qtd.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://hir.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://llv.yj20258888.top

================================================================================
来源：http://sau.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://eyf.zhijiandao.cn

================================================================================
来源：http://hxk.316326.xyz

[D01] 创建数组 / 列表
来源：http://mgr.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ccr.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rgx.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ulv.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uzu.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ziv.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://aem.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://fau.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eor.guowangkeji.top

[D02] 追加元素到末尾
来源：http://rfp.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://prx.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pqj.yj20258888.top

JS:   arr.push(4);
来源：http://adj.iojbl.cn

TS:   arr.push(4);
来源：http://bsq.aizwys.cn

Java: list.add(4);
来源：http://uml.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://cyp.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ahq.vqdsnc.cn

C#:   list.Add(4);
来源：http://yjx.smart0.xyz

[D03] 在指定位置插入元素
来源：http://cli.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://oth.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lem.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tyd.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://cvc.havefunace.top

Java: list.add(0, 0);
来源：http://oap.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://rhk.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ojo.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://qvm.zdqjudy.top

[D04] 删除元素
来源：http://qyf.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bva.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://loo.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vuw.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://qxd.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://set.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nva.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zih.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vyh.hysaishi.cn

[D05] 访问与修改元素
来源：http://pwk.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zhe.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nvh.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fcv.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://vbg.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://kgh.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://kqo.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://thi.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zei.ywan-chungtsiang.top

[D06] 数组长度
来源：http://dph.aizwys.cn

Py:   len(arr)
来源：http://lsl.kuanghao11.cn

PHP:  count($arr);
来源：http://qdq.sjlbkw.cn

JS:   arr.length
来源：http://wpf.jiagoushi.top

TS:   arr.length
来源：http://isv.chenzaomai.com


<!-- 参考信息 -->