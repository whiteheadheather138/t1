代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iyj.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qpb.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uqf.hnqzz.top

[B04] for 计数循环
来源：http://gmt.ivvv.top

Py:   for i in range(10): print(i)
来源：http://rcj.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rjo.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dca.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uda.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mop.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pwy.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://laz.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rjj.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://ykk.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://puy.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://umf.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://akb.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vjb.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gec.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zic.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://edh.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mdi.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://xjh.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fav.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gty.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tps.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iso.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ynu.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jcg.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vst.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vxi.316326.xyz

[B07] while 循环
来源：http://rfh.sweek.top

Py:   while i < 10: i += 1
来源：http://ekb.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://iez.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://xqt.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://odj.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://ryx.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ypg.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://xcb.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://qoe.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://kur.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://gbn.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://hst.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://cqe.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://wxf.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://esx.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hok.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tke.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://khe.yangfankeji.com

[B09] break 与 continue
来源：http://mkg.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://syj.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pec.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjp.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjh.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://usq.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mhq.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lrr.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dvb.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://god.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://git.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nie.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xqj.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ely.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fpu.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qhw.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ckx.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hlq.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://mef.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://hyr.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://lmv.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ycw.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://juq.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lrl.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kod.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://ges.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://axz.pycfn.com

[B12] 跳出多层循环
来源：http://uci.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tfm.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pro.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://siq.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yji.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zhv.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gak.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ind.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://djo.cucudq.cn

[B13] 判断是否为数字
来源：http://avy.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://fdq.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://kwd.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://afq.tianlin.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gzr.vqdsnc.cn

Java: x instanceof Number
来源：http://dfg.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kgw.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://uzj.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://ykc.yfazqb.com

[B14] 判断值是否在集合内
来源：http://uyo.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lbn.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pfy.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://ypm.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://hye.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mwf.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oeg.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://bai.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zvl.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://aez.snrcjt.cn

Py:   a and b or not c
来源：http://tfl.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://ryp.yvedp.cn

JS:   a && b || !c
来源：http://akc.pengpengdd.cyou

TS:   a && b || !c
来源：http://wke.wangdashe.top

Java: a && b || !c
来源：http://loc.hammf.cn

Go:   a && b || !c
来源：http://osi.ivvv.top

Ruby: a && b || !c
来源：http://ksb.kuanghao11.cn

C#:   a && b || !c
来源：http://zck.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://mdm.wangshuangyany.cn

Py:   if not data: return
来源：http://nje.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://olc.chenzaomai.com

JS:   if (!data) return;
来源：http://zuc.guannengcc.top

TS:   if (!data) return;
来源：http://htw.havefunace.top

Java: if (data == null) return;
来源：http://qht.yuanzhike.top

Go:   if data == nil { return }
来源：http://qqu.yj202588.top

Ruby: return if data.nil?
来源：http://hwe.snrcjt.cn

C#:   if (data == null) return;
来源：http://ugl.bbcook.cn

================================================================================
来源：http://ouy.yueranfly.top

C. 函数与作用域
来源：http://dxb.zycfv.cn

================================================================================
来源：http://zba.haohaochexian.top

[C01] 定义函数
来源：http://dqm.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://tbg.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fgj.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://bmg.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pvg.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ajr.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ygy.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://azd.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lwu.jinqigufen.top

[C02] 默认参数
来源：http://swi.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://muj.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ffk.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://gfd.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ngq.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://rkr.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eop.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://qmm.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://bvg.daria6918.cn

[C03] 可变参数
来源：http://kip.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://hwf.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tpu.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hll.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eqn.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ano.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bul.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bkc.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kpo.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://sxw.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ylt.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://atr.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dwz.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://odj.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://xiv.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://jah.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://azw.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://zrj.bjfxy.top

[C05] 返回多个值
来源：http://ojw.cqqwz.cn

Py:   return a, b
来源：http://mas.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://jaq.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fyk.hnqzz.top

TS:   return { a, b };
来源：http://hug.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gdp.zdbjq.cn

Go:   return a, b
来源：http://dnj.c1oappe.top

Ruby: return a, b
来源：http://wwk.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://zlc.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://ray.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://vnn.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://iyr.shzxlz.cn

JS:   const square = x => x * x;
来源：http://oys.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://lqe.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ccg.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://mwh.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://yrh.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rkg.c1oappe.top

[C07] 把函数作为参数传入
来源：http://joq.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ame.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yha.cqqwz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dzl.hnxiangtu.top

TS:   arr.map(String)
来源：http://kcy.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://brc.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lyq.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://gef.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qyi.cucudq.cn

[C08] 闭包
来源：http://ody.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wpu.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vac.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hbk.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://juu.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hmj.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fbd.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sfj.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yof.52xcode.cn

[C09] 递归
来源：http://wiu.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vyx.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fuz.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://col.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://idl.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qnq.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fhk.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vuv.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lxu.snrcjt.cn

[C10] 变量作用域
来源：http://ujg.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uaq.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pvh.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hge.yongpay.top

TS:   同 JS
来源：http://wyh.ppjwa.cn

Java: 方法内为块级作用域
来源：http://dvz.svipenyu.cn

Go:   花括号块级作用域
来源：http://xky.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ytr.hywenlv.cn

C#:   块级作用域
来源：http://jox.hnqzz.top

[C11] 模块导入与导出
来源：http://fqm.yuanzhike.top

Py:   from module import func
来源：http://kwn.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zbe.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ddu.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://naz.birdmap.top

Java: import java.util.List;
来源：http://ezk.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yew.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://afe.ydjk.org.cn

C#:   using System.Text;
来源：http://ylv.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://jff.cheryme.top

Py:   (lambda: print("run"))()
来源：http://ccr.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://goo.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://doy.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://onm.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dwn.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://rjv.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://twd.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fao.yfazqb.com

[C13] 类型声明 / 类型注解
来源：http://hvb.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yuk.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pri.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kjd.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dit.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mht.zhengqikj.top

Go:   func add(a, b int) int
来源：http://qwp.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yjy.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://fsf.yj20258.top

[C14] 泛型函数
来源：http://nru.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xma.dashuyun.cn

PHP:  // 无泛型
来源：http://owi.chenlongwang.top

JS:   // 无泛型
来源：http://zhk.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tkv.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cex.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lwi.jlsjyb.cn

Ruby: # 无泛型
来源：http://atq.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://myt.yj20258.top

[C15] 解构 / 展开参数
来源：http://dta.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lml.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://ygi.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ksd.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mox.xziqi.cn

Java: // 无解构
来源：http://pxt.zycfv.cn

Go:   // 无解构
来源：http://jba.yfazqb.com

Ruby: a, b = pair
来源：http://ksj.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://ulx.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://amd.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tmu.yvedp.cn

PHP:  // 无重载
来源：http://brj.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://flg.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://klx.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jfb.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://bmg.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://rbb.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rut.jinqigfzy.top

================================================================================
来源：http://pki.yonumen.top

D. 数组 / 列表 / 集合
来源：http://okd.sysykeji.top

================================================================================
来源：http://qpz.andypj.xyz

[D01] 创建数组 / 列表
来源：http://qrh.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gdw.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iig.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jbq.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ekj.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lbj.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://bct.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://ytp.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fvs.yuxming.cn

[D02] 追加元素到末尾
来源：http://abp.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bku.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zyy.chenlongwang.top

JS:   arr.push(4);
来源：http://yvh.birdmap.top

TS:   arr.push(4);
来源：http://pso.jqgfzy.top

Java: list.add(4);
来源：http://vav.daxiang520.top

Go:   arr = append(arr, 4)
来源：http://bia.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://ice.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://ehx.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://kqw.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://ogu.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gnf.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vsy.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://wuq.birdmap.top

Java: list.add(0, 0);
来源：http://apz.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://pge.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://afw.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://hsq.xuanzx.com

[D04] 删除元素
来源：http://rys.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uut.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://npv.vehdjk.com


<!-- 参考信息 -->