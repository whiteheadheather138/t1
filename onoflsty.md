代发 wailian999

[B05] 遍历数组 / 列表
来源：http://nis.yj20258888.top

Py:   for item in arr: print(item)
来源：http://rve.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://abd.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://jmz.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://wly.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qos.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lcb.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://jxm.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dha.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://trw.xuanzx.com

Py:   for k, v in d.items(): print(k, v)
来源：http://azh.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhm.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hwu.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpt.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://twu.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opb.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aci.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://utd.sweek.top

[B07] while 循环
来源：http://myj.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://hgb.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xhs.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://iml.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://iwe.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://geh.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mnu.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://lbg.sweek.top

C#:   while (i < 10) { i++; }
来源：http://cmk.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://waa.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://fdm.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sqo.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://viz.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://ubm.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://ffg.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://euq.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://tjp.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://yic.cdnleiting.top

[B09] break 与 continue
来源：http://anj.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ect.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jnz.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxl.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bax.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzz.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zsy.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dcf.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://euh.yuxming.cn

[B10] 遍历同时拿索引
来源：http://juz.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iwk.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mwp.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pmp.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vtc.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zui.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eig.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qpt.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cyu.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://gla.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://uib.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://hiw.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://abk.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ohw.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tpa.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lcz.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://nkf.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ial.fehbvm.com

[B12] 跳出多层循环
来源：http://ynb.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xsn.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wse.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wrf.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xpq.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hzq.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bey.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ebm.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ezy.yonumen.top

[B13] 判断是否为数字
来源：http://rij.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://biu.bbcook.cn

PHP:  is_numeric($x)
来源：http://jsb.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://csp.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbb.shzxlz.cn

Java: x instanceof Number
来源：http://muz.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nfg.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://jiz.jqgfzy.top

C#:   x is int or double or decimal
来源：http://pds.fzhhl.top

[B14] 判断值是否在集合内
来源：http://vhd.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dmj.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xim.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://qdr.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://fjn.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mmn.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iqn.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dns.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vva.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://xmh.cqqwz.cn

Py:   a and b or not c
来源：http://mjt.xinyue.icu

PHP:  $a && $b || !$c
来源：http://hun.wangdashe.top

JS:   a && b || !c
来源：http://eum.shzxlz.cn

TS:   a && b || !c
来源：http://rpp.tianlin.xyz

Java: a && b || !c
来源：http://lac.fzhhl.top

Go:   a && b || !c
来源：http://rby.zhengqikj.top

Ruby: a && b || !c
来源：http://urd.chenlongwang.top

C#:   a && b || !c
来源：http://mwc.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://puk.bbcook.cn

Py:   if not data: return
来源：http://sdf.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://nix.sxryk.cn

JS:   if (!data) return;
来源：http://xoz.0kj1m.cn

TS:   if (!data) return;
来源：http://jzu.ppjwa.cn

Java: if (data == null) return;
来源：http://sgo.xinyue.icu

Go:   if data == nil { return }
来源：http://shj.cdnleiting.top

Ruby: return if data.nil?
来源：http://jjw.ydjk.org.cn

C#:   if (data == null) return;
来源：http://lrw.ppjwa.cn

================================================================================
来源：http://anc.0kj1m.cn

C. 函数与作用域
来源：http://lye.wangshuangyany.cn

================================================================================
来源：http://toh.nanxuanxn.top

[C01] 定义函数
来源：http://djv.tanke756.top

Py:   def add(a, b): return a + b
来源：http://pkm.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlq.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://ois.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dhv.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://bxq.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://jtn.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://xrw.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ofy.gogol.net.cn

[C02] 默认参数
来源：http://ris.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://wbd.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rlj.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://elq.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://abt.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jkt.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ewp.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://hsa.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ebp.zhaomingkeji.xyz

[C03] 可变参数
来源：http://ocz.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://skm.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pvj.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vkg.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yoc.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zhp.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://njs.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://bhk.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://asm.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://fvb.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://exb.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vkp.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://niy.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://avr.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://vfj.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://bnf.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://txw.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://ekw.svipenyu.cn

[C05] 返回多个值
来源：http://lbe.yfazqb.com

Py:   return a, b
来源：http://qvk.zhengqikj.top

PHP:  return [$a, $b];
来源：http://lbq.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lyp.yonumen.top

TS:   return { a, b };
来源：http://vez.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qvh.gaohongyu789.top

Go:   return a, b
来源：http://czv.jinqigufen.top

Ruby: return a, b
来源：http://czh.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://tuk.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://ozr.sweek.top

Py:   square = lambda x: x * x
来源：http://fti.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://klo.yonumen.top

JS:   const square = x => x * x;
来源：http://qkn.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://not.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mvh.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://nwk.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://uou.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://vra.fehbvm.com

[C07] 把函数作为参数传入
来源：http://wrh.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bvt.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://olp.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ikt.zhiwuduotai.top

TS:   arr.map(String)
来源：http://bus.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://igh.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ehk.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://stg.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hvn.shuidangran.top

[C08] 闭包
来源：http://xue.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jte.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rtq.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vdk.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jnj.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wkz.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bsz.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zsl.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rce.bbcook.cn

[C09] 递归
来源：http://mvg.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gwr.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wce.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzf.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddi.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://svb.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kxa.jianghu66.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lcc.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jgo.jqgufenzy.top

[C10] 变量作用域
来源：http://ghl.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gon.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kfi.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bfc.tanke756.top

TS:   同 JS
来源：http://yfm.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://ine.dianchejie.cn

Go:   花括号块级作用域
来源：http://lyr.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nay.bjfxy.top

C#:   块级作用域
来源：http://vfs.hcnkem.com

[C11] 模块导入与导出
来源：http://mnc.9152youxi.cn

Py:   from module import func
来源：http://sak.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lih.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hmg.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ddf.shzxlz.cn

Java: import java.util.List;
来源：http://uax.kuanghao11.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://avg.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://vef.shanyushiyangtech.top

C#:   using System.Text;
来源：http://gjd.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://ooj.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://sko.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://sff.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://dig.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://xnb.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dks.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://fht.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://duq.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dvp.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://idh.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://llz.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tlm.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://afy.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqr.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://tar.52xcode.cn

Go:   func add(a, b int) int
来源：http://xqg.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fnq.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://xib.daria6918.cn

[C14] 泛型函数
来源：http://nqh.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qtp.pengpengdd.cyou

PHP:  // 无泛型
来源：http://avu.shangyingyoupin.top

JS:   // 无泛型
来源：http://cvn.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uii.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xgf.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ejx.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://vqj.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lyh.fengsongda.top

[C15] 解构 / 展开参数
来源：http://fjo.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hts.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://jia.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eeo.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zxw.shangyingyoupin.top

Java: // 无解构
来源：http://tkc.ydjk.org.cn

Go:   // 无解构
来源：http://oav.hywenlv.cn

Ruby: a, b = pair
来源：http://wxx.yj20258.top

C#:   var (a, b) = pair;
来源：http://ugv.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://usc.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ety.tianlin.xyz

PHP:  // 无重载
来源：http://bqh.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pri.316326.xyz

TS:   // 用联合类型或重载签名声明
来源：http://evi.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xvf.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://vbq.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://lxp.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qnm.havefunace.top

================================================================================
来源：http://kyn.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://zol.chenlongwang.top

================================================================================
来源：http://khv.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://fqd.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://llw.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nba.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ktv.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wxr.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jtt.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://act.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://tvg.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fbf.hnqzz.top

[D02] 追加元素到末尾
来源：http://xnm.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yfr.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bux.yangfankeji.com

JS:   arr.push(4);
来源：http://lvm.pycfn.com

TS:   arr.push(4);
来源：http://pjl.pengpengdd.cyou

Java: list.add(4);
来源：http://ihi.cashguo.top

Go:   arr = append(arr, 4)
来源：http://pua.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://msz.guowangkeji.top

C#:   list.Add(4);
来源：http://all.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://pjd.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://sux.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://glx.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://glw.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://qhb.cucudq.cn

Java: list.add(0, 0);
来源：http://uld.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rcn.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nlr.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://mgf.jinqigufen.top

[D04] 删除元素
来源：http://rmh.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pyp.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ciw.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dyi.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://ybe.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yxm.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iyj.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zpl.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ose.fehbvm.com

[D05] 访问与修改元素
来源：http://wqp.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxo.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lsp.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qqj.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://jhy.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://azx.xingfuxueyuan.xyz


<!-- 参考信息 -->