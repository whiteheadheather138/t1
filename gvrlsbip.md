代发 wailian999

[B05] 遍历数组 / 列表
来源：http://xmp.c1oappe.top

Py:   for item in arr: print(item)
来源：http://fxa.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mkb.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://oyd.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://clz.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ewv.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wmf.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://yim.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://utr.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://tbm.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uak.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bgj.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://btx.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://llh.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ris.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rkl.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dco.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hqc.iojbl.cn

[B07] while 循环
来源：http://zdu.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://zut.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://wcl.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://jyv.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://lht.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://tsj.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://okl.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://uho.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://oii.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://xjc.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://tjk.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://dec.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://ccr.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://twg.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://xws.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://uww.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ieu.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://tkn.ctjpmb.com

[B09] break 与 continue
来源：http://jgu.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xho.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iom.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqo.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syo.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzv.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mjw.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://apz.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fiu.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://acy.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://psf.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uim.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dyz.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://emv.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xgi.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dvw.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mfu.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://isy.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://wym.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://djd.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://tga.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fii.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mmi.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qtv.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lnp.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://szt.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yxi.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://wuu.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gnu.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://aup.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zwm.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bom.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sfy.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://efg.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jqu.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://paj.sjlbkw.cn

[B13] 判断是否为数字
来源：http://buw.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://bij.daxiang520.top

PHP:  is_numeric($x)
来源：http://wcn.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dkx.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgo.cdnleiting.top

Java: x instanceof Number
来源：http://pfi.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zpa.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://tnq.xuanzx.com

C#:   x is int or double or decimal
来源：http://xub.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://zxk.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jdf.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eww.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://ytq.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://zwu.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://yav.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://arr.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://cxt.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://thf.hnqzz.top

[B15] 布尔运算与取反
来源：http://lev.yangfankeji.com

Py:   a and b or not c
来源：http://juz.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://dwu.cqqwz.cn

JS:   a && b || !c
来源：http://hnn.daria6918.cn

TS:   a && b || !c
来源：http://hmb.hammf.cn

Java: a && b || !c
来源：http://reu.tian-w.cn

Go:   a && b || !c
来源：http://tlr.jqgfzy.top

Ruby: a && b || !c
来源：http://asq.zhoulong.xyz

C#:   a && b || !c
来源：http://pat.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://upf.yj20258888.top

Py:   if not data: return
来源：http://sle.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://knm.yj20258.top

JS:   if (!data) return;
来源：http://bms.yongpay.top

TS:   if (!data) return;
来源：http://hev.tian-w.cn

Java: if (data == null) return;
来源：http://dfz.jqgfzy.top

Go:   if data == nil { return }
来源：http://dtk.yongpay.top

Ruby: return if data.nil?
来源：http://jqm.sysykeji.top

C#:   if (data == null) return;
来源：http://uym.bjfxy.top

================================================================================
来源：http://rbd.jinqigufen.top

C. 函数与作用域
来源：http://rzs.smart0.xyz

================================================================================
来源：http://iow.tian-w.cn

[C01] 定义函数
来源：http://vau.tanke756.top

Py:   def add(a, b): return a + b
来源：http://zqt.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ouq.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://ews.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gcz.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kvy.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nxt.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://sck.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xec.jqgfzy.top

[C02] 默认参数
来源：http://ijm.tanke756.top

Py:   def greet(name="World"): return name
来源：http://gnl.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://sxo.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://aaa.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gbf.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://kiz.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://arn.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://zuo.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://cgv.hfpthk.cn

[C03] 可变参数
来源：http://lav.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://ued.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ohn.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjp.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gcy.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fph.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fos.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ake.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://phu.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://oqn.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cej.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gbt.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rzi.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sat.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://luc.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://lnu.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://tml.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://qxi.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://jfi.daria6918.cn

Py:   return a, b
来源：http://ble.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://rsb.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vaz.jlsjyb.cn

TS:   return { a, b };
来源：http://luf.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fxv.wangshuangyany.cn

Go:   return a, b
来源：http://asp.zycfv.cn

Ruby: return a, b
来源：http://rrx.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://edx.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://zep.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://jhh.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pjn.epnwcf.com

JS:   const square = x => x * x;
来源：http://sig.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://ldj.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yts.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://jkq.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://iem.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://oga.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://umb.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rat.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qqn.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ywj.gzhubu.top

TS:   arr.map(String)
来源：http://lco.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kgm.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://efo.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://cxd.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://txd.tianlin.xyz

[C08] 闭包
来源：http://xog.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://imc.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fkh.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fue.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nbw.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xgn.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jso.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rkj.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ide.jqgfzy.top

[C09] 递归
来源：http://wrj.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fxd.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qrp.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sut.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://odk.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vlx.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zug.dianchejie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gng.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dyg.feifeiyinyue.top

[C10] 变量作用域
来源：http://hqk.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gza.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hxn.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cob.chenlongwang.top

TS:   同 JS
来源：http://isd.yueranfly.top

Java: 方法内为块级作用域
来源：http://lgu.fzhhl.top

Go:   花括号块级作用域
来源：http://nhw.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xzr.sxryk.cn

C#:   块级作用域
来源：http://bxi.xuanzx.com

[C11] 模块导入与导出
来源：http://pvl.xingfuxueyuan.xyz

Py:   from module import func
来源：http://qvz.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://asq.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://yyq.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qlv.gaohongyu789.top

Java: import java.util.List;
来源：http://lmk.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ccs.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://wsc.snrcjt.cn

C#:   using System.Text;
来源：http://gqz.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://ofn.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://woe.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://ema.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://tbk.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://oqh.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://btp.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://aob.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://qbc.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kpf.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://mec.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cto.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uoy.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kkr.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdf.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jer.0kj1m.cn

Go:   func add(a, b int) int
来源：http://mni.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://non.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://trz.9152youxi.cn

[C14] 泛型函数
来源：http://kni.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wrq.tanke756.top

PHP:  // 无泛型
来源：http://kbn.hywenlv.cn

JS:   // 无泛型
来源：http://maw.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xmj.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zzu.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kwr.jiagoushi.top

Ruby: # 无泛型
来源：http://ixg.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vdj.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://ybv.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dgv.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://twx.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yzc.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pqm.yonumen.top

Java: // 无解构
来源：http://ygs.sjlbkw.cn

Go:   // 无解构
来源：http://fgq.smart0.xyz

Ruby: a, b = pair
来源：http://gkv.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://kqr.tanke756.top

[C16] 函数 / 方法重载
来源：http://ovz.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zhj.yongpay.top

PHP:  // 无重载
来源：http://eut.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://khl.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://noe.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cvs.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://gdk.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://kfx.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://alc.bjfxy.top

================================================================================
来源：http://swy.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://rrp.guowangkeji.top

================================================================================
来源：http://siw.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://bsn.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ghp.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jhg.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zuz.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhf.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xxu.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://ryq.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://izf.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zrn.iojbl.cn

[D02] 追加元素到末尾
来源：http://ooe.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cmz.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ryh.shzxlz.cn

JS:   arr.push(4);
来源：http://evw.zhoulong.xyz

TS:   arr.push(4);
来源：http://inh.dashuyun.cn

Java: list.add(4);
来源：http://rle.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://mpk.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://kec.jiagoushi.top

C#:   list.Add(4);
来源：http://prx.gzhubu.top

[D03] 在指定位置插入元素
来源：http://mqn.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://zhg.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ank.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fsd.redwolf501.top

TS:   arr.splice(0, 0, 0);
来源：http://ofz.dashuyun.cn

Java: list.add(0, 0);
来源：http://esw.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sjh.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gdt.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://eck.yonumen.top

[D04] 删除元素
来源：http://dys.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lmq.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tpb.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://srp.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://kwj.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqo.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rrb.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://omx.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgx.smart0.xyz

[D05] 访问与修改元素
来源：http://vcb.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bqm.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qow.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kdt.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://kxn.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://mex.xylfe.cn


<!-- 参考信息 -->