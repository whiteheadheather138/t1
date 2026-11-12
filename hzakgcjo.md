代发 wailian999

[B05] 遍历数组 / 列表
来源：http://rcy.tian-w.cn

Py:   for item in arr: print(item)
来源：http://pab.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://srw.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pqs.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uxr.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xxm.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://szz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://opp.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rhw.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://mvi.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ooz.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pey.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cau.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qwz.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lzg.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hjv.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hkd.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wvb.smart0.xyz

[B07] while 循环
来源：http://caf.birdmap.top

Py:   while i < 10: i += 1
来源：http://ftm.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://mun.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://bdm.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://she.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://jxs.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wqk.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://usv.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://iig.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://hjp.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://qac.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rrl.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://jkw.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://yky.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://fjy.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://eji.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://pnw.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://qgs.svipenyu.cn

[B09] break 与 continue
来源：http://dan.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tfk.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ekz.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zrl.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qev.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upb.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tyh.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jxh.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fuk.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://uzf.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bfh.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://onq.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uyv.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ekh.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mhk.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vod.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://atf.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gmw.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://tsq.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://lrf.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://muv.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hxe.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggb.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wer.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ihh.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://cjm.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kjo.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://dnt.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://umv.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jzd.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tab.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://trj.ctjpmb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vyy.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zxf.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hvr.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lcb.yanxiufei.cn

[B13] 判断是否为数字
来源：http://cim.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://soe.sxryk.cn

PHP:  is_numeric($x)
来源：http://qnj.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ufo.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cki.tarul.cn

Java: x instanceof Number
来源：http://jwh.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ijx.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://htu.yangfankeji.com

C#:   x is int or double or decimal
来源：http://auj.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://rba.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vyl.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zvw.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://eyt.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://lnt.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://amu.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ldl.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://cxm.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nol.pycfn.com

[B15] 布尔运算与取反
来源：http://skq.tianlin.xyz

Py:   a and b or not c
来源：http://bnj.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://qjj.svipenyu.cn

JS:   a && b || !c
来源：http://msc.havefunace.top

TS:   a && b || !c
来源：http://ecj.ppjwa.cn

Java: a && b || !c
来源：http://trn.jinqigufen.top

Go:   a && b || !c
来源：http://rmc.cucudq.cn

Ruby: a && b || !c
来源：http://emv.pengpengdd.cyou

C#:   a && b || !c
来源：http://vbg.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://osk.epnwcf.com

Py:   if not data: return
来源：http://nyw.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://lnk.iojbl.cn

JS:   if (!data) return;
来源：http://tuz.yueranfly.top

TS:   if (!data) return;
来源：http://igf.ctjpmb.com

Java: if (data == null) return;
来源：http://yxq.zycfv.cn

Go:   if data == nil { return }
来源：http://lph.yj20258.top

Ruby: return if data.nil?
来源：http://tjo.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://cao.zhengqikj.top

================================================================================
来源：http://lut.52xcode.cn

C. 函数与作用域
来源：http://hlq.fktsv.cn

================================================================================
来源：http://aun.shanyushiyangtech.top

[C01] 定义函数
来源：http://jdf.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://oak.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzy.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://srt.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://drl.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://vsf.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://aec.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://wzt.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hbv.zdqjudy.top

[C02] 默认参数
来源：http://tli.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://azd.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ftv.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://mxd.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zbn.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://fnc.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rzw.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://rcr.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://bgp.c1oappe.top

[C03] 可变参数
来源：http://dno.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://suj.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pym.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oye.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bra.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bxg.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hyj.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vgc.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ltq.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://jid.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://udh.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://roj.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pxp.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://izt.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://fht.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://gtq.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://cvl.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://zaz.ctjpmb.com

[C05] 返回多个值
来源：http://mcf.shanyushiyangtech.top

Py:   return a, b
来源：http://erl.cashguo.top

PHP:  return [$a, $b];
来源：http://zwt.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lry.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://qsd.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://crn.meibo888.top

Go:   return a, b
来源：http://wtb.epnwcf.com

Ruby: return a, b
来源：http://tup.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://sqi.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://unw.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://jvn.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zyt.ivvv.top

JS:   const square = x => x * x;
来源：http://qwm.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://vnx.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mya.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://abm.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://vga.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://isk.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://bjo.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tkj.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://tcc.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjj.chenjidiqi.icu

TS:   arr.map(String)
来源：http://vai.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://guu.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cvm.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://oeo.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lpv.zdqjudy.top

[C08] 闭包
来源：http://utv.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://skc.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pwt.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rdb.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://crj.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mct.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://odh.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://agw.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wpl.yueranfly.top

[C09] 递归
来源：http://veq.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://spz.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://epu.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ssn.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ckm.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rmv.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sjr.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://txm.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mkk.yonumen.top

[C10] 变量作用域
来源：http://gko.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wqg.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zif.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://upz.hammf.cn

TS:   同 JS
来源：http://yjx.jinqigufen.top

Java: 方法内为块级作用域
来源：http://mii.bbcook.cn

Go:   花括号块级作用域
来源：http://yif.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://keo.svipenyu.cn

C#:   块级作用域
来源：http://vjj.yanxiufei.cn

[C11] 模块导入与导出
来源：http://oid.daxiang520.top

Py:   from module import func
来源：http://bdw.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xbp.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vsp.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ypj.pycfn.com

Java: import java.util.List;
来源：http://sqi.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pzc.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://yso.chenzaomai.com

C#:   using System.Text;
来源：http://jne.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://czk.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://spi.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://qji.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://wea.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://qit.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wtf.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://uzv.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://evx.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ukj.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://wkx.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zxh.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ipz.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://prw.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kzc.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pss.sysykeji.top

Go:   func add(a, b int) int
来源：http://psp.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cpf.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ttb.daria6918.cn

[C14] 泛型函数
来源：http://ajk.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zec.hcnkem.com

PHP:  // 无泛型
来源：http://xta.cqqwz.cn

JS:   // 无泛型
来源：http://hvc.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vie.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wke.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lut.epnwcf.com

Ruby: # 无泛型
来源：http://paa.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ums.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://kno.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rtg.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://lah.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bly.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vth.hnxiangtu.top

Java: // 无解构
来源：http://mgf.zdqjudy.top

Go:   // 无解构
来源：http://wcu.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://hfg.xuanzx.com

C#:   var (a, b) = pair;
来源：http://pno.yuxming.cn

[C16] 函数 / 方法重载
来源：http://buh.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://amx.yongpay.top

PHP:  // 无重载
来源：http://igp.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eco.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://uuw.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://shp.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://kvf.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://xkp.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rjp.yueranfly.top

================================================================================
来源：http://tqn.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://rft.wangdashe.top

================================================================================
来源：http://vms.meibo888.top

[D01] 创建数组 / 列表
来源：http://eyb.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://juo.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jol.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fmg.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zqt.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jfr.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://yon.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://xyb.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nge.pycfn.com

[D02] 追加元素到末尾
来源：http://ebj.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tda.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wvt.hnqzz.top

JS:   arr.push(4);
来源：http://btf.jianghu66.top

TS:   arr.push(4);
来源：http://qsu.xziqi.cn

Java: list.add(4);
来源：http://swc.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://ikb.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xgx.zhijiandao.cn

C#:   list.Add(4);
来源：http://wqm.yj20258.top

[D03] 在指定位置插入元素
来源：http://nxj.ivvv.top

Py:   arr.insert(0, 0)
来源：http://sul.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uho.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://okk.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://lkx.daxiang520.top

Java: list.add(0, 0);
来源：http://pry.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://pyj.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://plv.chenlongwang.top

C#:   list.Insert(0, 0);
来源：http://zhi.chenlongwang.top

[D04] 删除元素
来源：http://nmy.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://esy.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://chh.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ehf.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://gst.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jcm.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uxu.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cgl.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zkd.vehdjk.com

[D05] 访问与修改元素
来源：http://iyi.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxi.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iff.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://svv.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://tpy.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://yar.fanxiaobao.xyz


<!-- 参考信息 -->