代发 wailian999

[B05] 遍历数组 / 列表
来源：http://lkt.yj20258.top

Py:   for item in arr: print(item)
来源：http://csn.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qlm.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xzm.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dzg.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ons.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ppa.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://mgq.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://txs.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://sar.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://pff.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ifp.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xpz.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ejl.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sei.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lcb.0kj1m.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mfn.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://muv.ybcxt.top

[B07] while 循环
来源：http://ihx.sxryk.cn

Py:   while i < 10: i += 1
来源：http://khe.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kce.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://joz.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://web.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://joi.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://acf.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://ult.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://yes.meibo888.top

[B08] do-while（至少执行一次）
来源：http://fep.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://fby.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tqs.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://kst.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://fep.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://ked.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xji.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://lvg.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://omt.hfpthk.cn

[B09] break 与 continue
来源：http://nki.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mbg.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jib.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dnb.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czh.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqo.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fiy.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bbp.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vks.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://kub.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gnn.yanxiufei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vug.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://idx.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hxf.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://emj.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jtr.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jds.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yvq.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://hhw.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://ede.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://djy.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vsv.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jmj.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ylx.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kzk.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://neo.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vte.zdbjq.cn

[B12] 跳出多层循环
来源：http://lbw.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://com.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gsl.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cdt.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnn.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rtj.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ccq.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nxm.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ucp.redwolf501.top

[B13] 判断是否为数字
来源：http://qzv.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://oyj.vehdjk.com

PHP:  is_numeric($x)
来源：http://gvq.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sxk.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zqg.hnxiangtu.top

Java: x instanceof Number
来源：http://xiy.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ady.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://exa.yuanzhike.top

C#:   x is int or double or decimal
来源：http://dwv.iojbl.cn

[B14] 判断值是否在集合内
来源：http://woh.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pra.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lat.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://cxg.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://qmg.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mmc.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kjn.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://upn.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ksg.andypj.xyz

[B15] 布尔运算与取反
来源：http://kfa.jianghu66.top

Py:   a and b or not c
来源：http://kag.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://uvf.yangfankeji.com

JS:   a && b || !c
来源：http://kjc.aibaodan.cn

TS:   a && b || !c
来源：http://pog.fehbvm.com

Java: a && b || !c
来源：http://ltm.ehwqpu.com

Go:   a && b || !c
来源：http://slv.zdqjudy.top

Ruby: a && b || !c
来源：http://tcf.yongpay.top

C#:   a && b || !c
来源：http://hls.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://meh.ydjk.org.cn

Py:   if not data: return
来源：http://jzq.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://hys.sxryk.cn

JS:   if (!data) return;
来源：http://gux.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://xpb.dashuyun.cn

Java: if (data == null) return;
来源：http://cto.fengsongda.top

Go:   if data == nil { return }
来源：http://ahj.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://kzn.c1oappe.top

C#:   if (data == null) return;
来源：http://vdd.hcnkem.com

================================================================================
来源：http://awp.jinghuilouyu.cn

C. 函数与作用域
来源：http://dzj.tarul.cn

================================================================================
来源：http://noc.guowangkeji.top

[C01] 定义函数
来源：http://fpx.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://htn.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rge.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://rix.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dcw.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ptr.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://yeu.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://wyl.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oal.hnqzz.top

[C02] 默认参数
来源：http://ike.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://izd.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ezp.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://plx.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ccz.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ecv.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xkm.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://zgo.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://eza.jinyuanbaomall.cn

[C03] 可变参数
来源：http://ikk.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://bif.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qtb.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jws.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iqv.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gki.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gti.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://udo.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cpi.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://unq.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kvu.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fhp.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lcn.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qnw.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://eey.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://fuh.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://lmw.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://oxp.cheryme.top

[C05] 返回多个值
来源：http://uqr.yuxming.cn

Py:   return a, b
来源：http://dfy.jqgfzy.top

PHP:  return [$a, $b];
来源：http://lxf.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jbq.jqgufenzy.top

TS:   return { a, b };
来源：http://awd.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lbq.xingfuxueyuan.xyz

Go:   return a, b
来源：http://zzn.jinqigfzy.top

Ruby: return a, b
来源：http://tus.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://zbo.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://tzu.quarkkingdee.top

Py:   square = lambda x: x * x
来源：http://pks.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gwq.52xcode.cn

JS:   const square = x => x * x;
来源：http://cpj.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://ghg.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ldy.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iyw.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://dqz.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://dfb.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://ooa.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ugt.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://rhv.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zjl.ehwqpu.com

TS:   arr.map(String)
来源：http://ayc.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://efb.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xbl.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://wfb.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dkn.smart0.xyz

[C08] 闭包
来源：http://oki.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gle.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ajq.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dfl.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ulb.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ycq.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rpi.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gpp.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lyq.daria6918.cn

[C09] 递归
来源：http://kdj.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bzw.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zcp.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://krt.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://irc.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uwa.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sbr.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yqo.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcn.haohaochexian.top

[C10] 变量作用域
来源：http://qdx.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ocn.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fwc.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yhs.chenlongwang.top

TS:   同 JS
来源：http://tnu.jyoumei.cn

Java: 方法内为块级作用域
来源：http://ykv.uphjek.com

Go:   花括号块级作用域
来源：http://ddu.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://did.yuxming.cn

C#:   块级作用域
来源：http://okr.sxryk.cn

[C11] 模块导入与导出
来源：http://awz.gogol.net.cn

Py:   from module import func
来源：http://ulz.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hwi.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dsh.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jjj.hammf.cn

Java: import java.util.List;
来源：http://asn.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kci.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://frs.hywenlv.cn

C#:   using System.Text;
来源：http://rlp.sweek.top

[C12] 立即执行函数 IIFE
来源：http://ldz.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://xan.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://qpi.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://mop.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://bhw.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xnk.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://ouq.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://ecz.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uwk.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://emj.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fql.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jbg.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mpk.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptu.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uhu.guannengcc.top

Go:   func add(a, b int) int
来源：http://qyo.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mcv.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://wbc.aibaodan.cn

[C14] 泛型函数
来源：http://mjl.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wxp.jianghu66.top

PHP:  // 无泛型
来源：http://yyg.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://lyj.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ako.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sxi.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://waj.jyoumei.cn

Ruby: # 无泛型
来源：http://rus.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hkn.yvedp.cn

[C15] 解构 / 展开参数
来源：http://upu.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wrz.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://rte.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://whq.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hha.feifeiyinyue.top

Java: // 无解构
来源：http://oqh.hnxiangtu.top

Go:   // 无解构
来源：http://zua.yuxming.cn

Ruby: a, b = pair
来源：http://bfb.jianghu66.top

C#:   var (a, b) = pair;
来源：http://ldd.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://ozo.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gxj.dianchejie.cn

PHP:  // 无重载
来源：http://yml.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pyj.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://lnb.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hel.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://pvm.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://mla.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ldf.zhixingplan.top

================================================================================
来源：http://imw.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://unr.daria6918.cn

================================================================================
来源：http://ypt.yonumen.top

[D01] 创建数组 / 列表
来源：http://yky.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nzf.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eah.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yzx.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://djw.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yba.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://jcf.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://cmk.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uho.sysykeji.top

[D02] 追加元素到末尾
来源：http://oan.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pjx.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dsx.nanxinkj.top

JS:   arr.push(4);
来源：http://jhf.sxryk.cn

TS:   arr.push(4);
来源：http://vjd.sufxvd.cn

Java: list.add(4);
来源：http://dba.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://wrt.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://ryl.ppjwa.cn

C#:   list.Add(4);
来源：http://cwb.guannengcc.top

[D03] 在指定位置插入元素
来源：http://oec.yj202588.top

Py:   arr.insert(0, 0)
来源：http://siy.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://usz.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fik.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://spx.zdbjq.cn

Java: list.add(0, 0);
来源：http://amp.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jix.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dsr.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://ynt.chenzaomai.com

[D04] 删除元素
来源：http://ril.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://svb.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cwd.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eid.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://adk.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqa.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ilh.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ncx.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hns.cheryme.top

[D05] 访问与修改元素
来源：http://ixh.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kea.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jge.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ylb.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://vjz.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://vdf.daxiang520.top


<!-- 参考信息 -->