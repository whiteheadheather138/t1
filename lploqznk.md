代发 wailian999

Py:   for i in range(10): print(i)
来源：http://jjw.52xcode.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hba.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mwx.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zhu.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ers.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ini.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://cld.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ytw.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://ikt.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://qha.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://goz.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://chm.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://vcm.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ysu.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uns.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://xxs.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rsi.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://zjj.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ram.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yhr.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnm.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vmm.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zlb.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qsd.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://czj.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rdd.jlsjyb.cn

[B07] while 循环
来源：http://tmi.sxryk.cn

Py:   while i < 10: i += 1
来源：http://tpm.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ypk.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://ncy.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://fuk.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://zgl.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fom.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://tyd.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://xoo.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://dse.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://cra.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pbm.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://syd.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://vau.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://rfw.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wnz.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vrh.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://qiy.chenjidiqi.icu

[B09] break 与 continue
来源：http://wcn.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iay.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://twn.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcl.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djc.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjh.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ekc.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ppe.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpo.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://igr.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jrv.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hnn.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uah.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qew.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cxv.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bry.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tpq.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jnr.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://gob.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://wiv.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://auz.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cin.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qlw.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jvr.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://glk.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://djo.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nuw.jinqigfzy.top

[B12] 跳出多层循环
来源：http://jmx.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jgh.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vhl.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://phq.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvc.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dey.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qwp.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://biy.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://juc.vqdsnc.cn

[B13] 判断是否为数字
来源：http://yev.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://azq.ehwqpu.com

PHP:  is_numeric($x)
来源：http://gyo.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwo.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lot.guannengcc.top

Java: x instanceof Number
来源：http://atx.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rwr.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://oaz.snrcjt.cn

C#:   x is int or double or decimal
来源：http://sdi.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://yvu.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://agn.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pcy.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://zoz.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ojn.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nfn.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iss.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://svb.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://utd.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://grf.hesvh.cn

Py:   a and b or not c
来源：http://rqq.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://hcb.uphjek.com

JS:   a && b || !c
来源：http://van.ydzc1.top

TS:   a && b || !c
来源：http://lmc.iojbl.cn

Java: a && b || !c
来源：http://htr.vqdsnc.cn

Go:   a && b || !c
来源：http://wkt.yueranfly.top

Ruby: a && b || !c
来源：http://ttb.hongshengwenyu.top

C#:   a && b || !c
来源：http://zuo.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://oay.svipenyu.cn

Py:   if not data: return
来源：http://xad.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://gij.zhongyouzk.top

JS:   if (!data) return;
来源：http://fik.sysykeji.top

TS:   if (!data) return;
来源：http://hjp.andypj.xyz

Java: if (data == null) return;
来源：http://ycr.hesvh.cn

Go:   if data == nil { return }
来源：http://cpk.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://tfc.zdqjudy.top

C#:   if (data == null) return;
来源：http://meg.hesvh.cn

================================================================================
来源：http://oss.jiagoushi.top

C. 函数与作用域
来源：http://clz.jianghu66.top

================================================================================
来源：http://vlk.sweek.top

[C01] 定义函数
来源：http://ksu.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://vph.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ild.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://nls.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jse.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tia.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://gxe.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://wae.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tgr.cdnleiting.top

[C02] 默认参数
来源：http://hdz.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://tbg.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://tpq.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://hfl.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://waj.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tcs.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gzi.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://xha.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://dao.redwolf501.top

[C03] 可变参数
来源：http://hur.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://ktt.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wkt.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://smz.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vli.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tux.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hkz.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://fih.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://swb.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://ina.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://irm.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vcs.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hdg.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zgd.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://xom.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://zuy.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://fxn.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://jej.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://dds.epnwcf.com

Py:   return a, b
来源：http://cbq.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://ava.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://vfl.feifeiyinyue.top

TS:   return { a, b };
来源：http://gee.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://onh.sxryk.cn

Go:   return a, b
来源：http://pwx.zhixingplan.top

Ruby: return a, b
来源：http://xwf.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://zzb.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://dqj.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://eoe.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ord.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://ruk.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://pxa.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fsf.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://xbt.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://hpt.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fdp.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://gkk.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://twf.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://vou.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ave.yj202588.top

TS:   arr.map(String)
来源：http://dyw.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://phx.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jkz.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://fpb.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cne.andypj.xyz

[C08] 闭包
来源：http://oou.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oiz.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aum.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xqv.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://obn.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qmr.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ikd.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://psw.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://shc.shanyushiyangtech.top

[C09] 递归
来源：http://zzg.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmp.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ztz.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ume.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vdi.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ybp.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://srn.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ovy.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://acs.cashguo.top

[C10] 变量作用域
来源：http://rff.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sax.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cdz.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://efr.uphjek.com

TS:   同 JS
来源：http://gat.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://xoh.yuxming.cn

Go:   花括号块级作用域
来源：http://tmk.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cam.cashguo.top

C#:   块级作用域
来源：http://ath.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://viy.ydzc1.top

Py:   from module import func
来源：http://jev.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ifi.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wbl.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://twj.tarul.cn

Java: import java.util.List;
来源：http://zii.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qgy.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://dty.uphjek.com

C#:   using System.Text;
来源：http://jwk.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://nmf.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://bkr.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://kmx.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://uyh.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://fbj.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zhq.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://dhl.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://wvt.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://der.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://crn.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dmk.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kzd.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mlk.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://trh.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://xoe.hammf.cn

Go:   func add(a, b int) int
来源：http://iue.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tpm.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://wcw.jqgufenzy.top

[C14] 泛型函数
来源：http://hoh.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ojx.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://our.yongpay.top

JS:   // 无泛型
来源：http://mky.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ktf.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://otw.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yam.hysaishi.cn

Ruby: # 无泛型
来源：http://crd.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xph.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://qmr.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tzk.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://dgk.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ull.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pue.aizwys.cn

Java: // 无解构
来源：http://asv.jqgfzy.top

Go:   // 无解构
来源：http://jem.jinqigufen.top

Ruby: a, b = pair
来源：http://bbh.pycfn.com

C#:   var (a, b) = pair;
来源：http://mdu.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://kjf.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ioh.aibaodan.cn

PHP:  // 无重载
来源：http://kwj.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://utw.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://pla.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sfr.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://nwn.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://qru.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hbb.meibo888.top

================================================================================
来源：http://fpc.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://rae.zhongyouzk.top

================================================================================
来源：http://nfb.yuxming.cn

[D01] 创建数组 / 列表
来源：http://ukq.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ltn.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sri.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lvo.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://peu.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cxc.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ibq.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://yld.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zag.yueranfly.top

[D02] 追加元素到末尾
来源：http://pim.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vvs.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://msu.ehwqpu.com

JS:   arr.push(4);
来源：http://vnc.yongpay.top

TS:   arr.push(4);
来源：http://fvg.yanxiufei.cn

Java: list.add(4);
来源：http://zjo.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://ndd.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://gfv.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://vjx.birdmap.top

[D03] 在指定位置插入元素
来源：http://vbk.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://stj.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ezh.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bfn.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://yfx.ydjk.org.cn

Java: list.add(0, 0);
来源：http://xxa.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://sqg.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://acg.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://tag.redwolf501.top

[D04] 删除元素
来源：http://mwh.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ilr.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qsd.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jiw.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://tmd.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://czr.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jsq.wangshuangyany.cn


<!-- 参考信息 -->