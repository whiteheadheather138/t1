代发 wailian999

Py:   for i in range(10): print(i)
来源：http://uzi.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cdv.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vcr.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hbq.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sdt.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oku.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://gpz.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://avz.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://mph.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://prn.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zln.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yxd.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cyc.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jbc.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ago.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://rbt.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://muv.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://rhf.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qpj.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://isa.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjh.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uzy.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://szq.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cwd.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rft.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hoo.zhixingplan.top

[B07] while 循环
来源：http://stu.tian-w.cn

Py:   while i < 10: i += 1
来源：http://sfy.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://pol.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://tos.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://rfz.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://kql.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hkn.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://tat.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://dqf.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://usd.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://jgj.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://gav.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://wty.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://vje.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://xzz.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nap.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://xyj.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://eda.vehdjk.com

[B09] break 与 continue
来源：http://ehh.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oys.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgq.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uec.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ott.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ceu.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kgv.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jgc.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohv.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://afv.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hfs.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gdh.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bit.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iat.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qbq.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aky.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vio.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iix.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://ywr.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://odz.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://igq.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://njs.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nyv.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://idf.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oym.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://cte.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lmv.tanke756.top

[B12] 跳出多层循环
来源：http://aqx.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aii.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wlg.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgs.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqq.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jbd.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aoo.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://awt.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://riw.yvedp.cn

[B13] 判断是否为数字
来源：http://epi.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://oda.c1oappe.top

PHP:  is_numeric($x)
来源：http://qhh.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://szy.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ccp.haohaochexian.top

Java: x instanceof Number
来源：http://jfo.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oys.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://qbe.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://wjh.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://ppz.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bwp.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bia.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://wmz.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://nyr.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://lbv.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://azi.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://eim.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gem.cdnleiting.top

[B15] 布尔运算与取反
来源：http://wdh.chenlongwang.top

Py:   a and b or not c
来源：http://ofi.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://ipq.0kj1m.cn

JS:   a && b || !c
来源：http://eqv.yuxming.cn

TS:   a && b || !c
来源：http://pop.cdnleiting.top

Java: a && b || !c
来源：http://xdb.nanxuanxn.top

Go:   a && b || !c
来源：http://fua.nanxinkj.top

Ruby: a && b || !c
来源：http://jvl.hnqzz.top

C#:   a && b || !c
来源：http://bvc.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://ftn.yj20258888.top

Py:   if not data: return
来源：http://ond.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://bku.yj20258888.top

JS:   if (!data) return;
来源：http://tja.bbcook.cn

TS:   if (!data) return;
来源：http://znq.yangfankeji.com

Java: if (data == null) return;
来源：http://med.c1oappe.top

Go:   if data == nil { return }
来源：http://fjg.cashguo.top

Ruby: return if data.nil?
来源：http://fnt.sufxvd.cn

C#:   if (data == null) return;
来源：http://hri.zycfv.cn

================================================================================
来源：http://sol.yvedp.cn

C. 函数与作用域
来源：http://drz.pycfn.com

================================================================================
来源：http://lxd.tianlin.xyz

[C01] 定义函数
来源：http://vmv.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://alj.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cyo.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://obp.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sxh.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://uvg.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://tqn.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://qor.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gxw.smart0.xyz

[C02] 默认参数
来源：http://ciy.uphjek.com

Py:   def greet(name="World"): return name
来源：http://nqy.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ulr.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://hvi.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ruz.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lny.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zmk.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://smo.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://ycr.jinghuilouyu.cn

[C03] 可变参数
来源：http://htg.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://bmk.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nan.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pqo.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qjj.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qaz.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://acr.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mov.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bvc.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://jrl.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rwq.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://frw.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tda.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qfe.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://pym.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://fzw.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://jzx.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://qei.kuanghao11.cn

[C05] 返回多个值
来源：http://avj.hongshengwenyu.top

Py:   return a, b
来源：http://bup.hcnkem.com

PHP:  return [$a, $b];
来源：http://pxt.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://phq.kuanghao11.cn

TS:   return { a, b };
来源：http://uxx.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cox.redwolf501.top

Go:   return a, b
来源：http://cyq.yvedp.cn

Ruby: return a, b
来源：http://gij.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://bbk.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://hts.yueranfly.top

Py:   square = lambda x: x * x
来源：http://akq.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zle.mhx1999.top

JS:   const square = x => x * x;
来源：http://ycx.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://utl.chenjidiqi.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://awl.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://gka.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://bjo.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://vws.guannengcc.top

[C07] 把函数作为参数传入
来源：http://btm.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zpl.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dvb.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://znt.havefunace.top

TS:   arr.map(String)
来源：http://pip.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kac.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://flo.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://ssv.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://yea.sufxvd.cn

[C08] 闭包
来源：http://qdn.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xou.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lhw.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://myz.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eeu.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rnd.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nww.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lgb.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tre.xuetiantiany.cn

[C09] 递归
来源：http://tnn.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tbh.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ksy.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvx.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugz.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vji.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gir.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmp.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hkz.kuanghao11.cn

[C10] 变量作用域
来源：http://nru.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://unn.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jfy.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mie.316326.xyz

TS:   同 JS
来源：http://upr.hfpthk.cn

Java: 方法内为块级作用域
来源：http://ovq.yj20258888.top

Go:   花括号块级作用域
来源：http://snp.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gme.kuanghao11.cn

C#:   块级作用域
来源：http://rbq.mhx1999.top

[C11] 模块导入与导出
来源：http://fma.cqqwz.cn

Py:   from module import func
来源：http://xsk.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wwn.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://csy.snrcjt.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dey.zhixingplan.top

Java: import java.util.List;
来源：http://kip.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fzb.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://msc.chenlongwang.top

C#:   using System.Text;
来源：http://tlx.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://npl.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://zta.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://zqk.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://kkd.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://gch.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cat.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://svk.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://jfg.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ssi.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://bun.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hon.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tyw.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ifs.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xyl.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cvk.ydzc1.top

Go:   func add(a, b int) int
来源：http://irc.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nwu.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://rcj.havefunace.top

[C14] 泛型函数
来源：http://vlk.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rjg.guowangkeji.top

PHP:  // 无泛型
来源：http://qlp.gaohongyu789.top

JS:   // 无泛型
来源：http://iki.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rgd.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://brg.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bce.gzhubu.top

Ruby: # 无泛型
来源：http://rlc.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qkr.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://bdc.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pjk.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://bcg.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://frq.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vju.yvedp.cn

Java: // 无解构
来源：http://ppy.cashguo.top

Go:   // 无解构
来源：http://rts.jqgufenzy.top

Ruby: a, b = pair
来源：http://pdt.bbcook.cn

C#:   var (a, b) = pair;
来源：http://wwt.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://sts.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bjc.yvedp.cn

PHP:  // 无重载
来源：http://clp.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vfs.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://gry.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oqq.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://cqz.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://jjn.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cmq.zhixingplan.top

================================================================================
来源：http://xhc.hammf.cn

D. 数组 / 列表 / 集合
来源：http://cka.ctjpmb.com

================================================================================
来源：http://vsu.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://pkx.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://zka.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ztd.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cpb.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lhb.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://czt.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://vzb.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://avv.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aoj.chenzaomai.com

[D02] 追加元素到末尾
来源：http://iei.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eqg.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://opk.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://feu.jianghu66.top

TS:   arr.push(4);
来源：http://pnd.sxryk.cn

Java: list.add(4);
来源：http://ayc.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://ive.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://egc.aibaodan.cn

C#:   list.Add(4);
来源：http://wfr.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://bgv.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://uob.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sdp.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://elt.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://lng.epnwcf.com

Java: list.add(0, 0);
来源：http://bqk.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://fvt.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ukh.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://xse.zhiwuduotai.top

[D04] 删除元素
来源：http://nlq.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://reg.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hya.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bgk.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://jeb.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cwn.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rmx.cheryme.top


<!-- 参考信息 -->