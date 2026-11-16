代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hlb.xinyue.icu

Py:   for item in arr: print(item)
来源：http://psv.ivvv.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fcy.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://myg.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nlq.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qto.jqgfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://chf.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://kiu.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zph.birdmap.top

[B06] 遍历字典 / 对象
来源：http://ebr.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sdu.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wic.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sio.jinyuanbaomall.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hwg.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://akb.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qat.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bmf.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vsr.sufxvd.cn

[B07] while 循环
来源：http://gqg.birdmap.top

Py:   while i < 10: i += 1
来源：http://sjd.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://fkg.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://cwc.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://roj.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://gkj.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fef.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://smi.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://vsj.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://svg.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://gpl.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zmw.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://lba.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://upa.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://qai.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fqm.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://ilw.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://hjv.xylfe.cn

[B09] break 与 continue
来源：http://wcn.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://num.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ssg.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwj.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cll.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npn.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ysz.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eby.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ham.xylfe.cn

[B10] 遍历同时拿索引
来源：http://mmz.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fad.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://smj.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygz.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tje.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://imj.c1oappe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tuk.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://buu.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qvj.vehdjk.com

[B11] 生成数字序列 / 区间
来源：http://abg.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://byt.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://xlz.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgi.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ahh.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jdg.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qgc.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://gfy.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://edk.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://jwl.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://adc.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wyd.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sly.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ppc.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qqu.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://evf.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ord.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cvp.nanxuanxn.top

[B13] 判断是否为数字
来源：http://tfe.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://gqv.yj20258888.top

PHP:  is_numeric($x)
来源：http://hgu.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yye.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zny.jyoumei.cn

Java: x instanceof Number
来源：http://ufp.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://akp.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://nmh.tianlin.xyz

C#:   x is int or double or decimal
来源：http://cuu.52xcode.cn

[B14] 判断值是否在集合内
来源：http://pxd.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rug.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gym.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://cso.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://bcu.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dvt.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mdh.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://pxy.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qvo.yj202588.top

[B15] 布尔运算与取反
来源：http://bnt.dashuyun.cn

Py:   a and b or not c
来源：http://udw.daria6918.cn

PHP:  $a && $b || !$c
来源：http://feb.yonumen.top

JS:   a && b || !c
来源：http://dbc.pycfn.com

TS:   a && b || !c
来源：http://akx.wangdashe.top

Java: a && b || !c
来源：http://snf.ivvv.top

Go:   a && b || !c
来源：http://qkw.sysykeji.top

Ruby: a && b || !c
来源：http://ryx.hnqzz.top

C#:   a && b || !c
来源：http://hlg.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://hbk.zdbjq.cn

Py:   if not data: return
来源：http://qjc.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://ijd.mhx1999.top

JS:   if (!data) return;
来源：http://eti.dashuyun.cn

TS:   if (!data) return;
来源：http://igx.9152youxi.cn

Java: if (data == null) return;
来源：http://qqp.yanxiufei.cn

Go:   if data == nil { return }
来源：http://pai.hnqzz.top

Ruby: return if data.nil?
来源：http://rfi.hywenlv.cn

C#:   if (data == null) return;
来源：http://tvo.nanxinkj.top

================================================================================
来源：http://ejo.ydjk.org.cn

C. 函数与作用域
来源：http://hkw.c1oappe.top

================================================================================
来源：http://kyf.pengpengdd.cyou

[C01] 定义函数
来源：http://bua.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://aam.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcr.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://wav.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gui.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hsr.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://gqj.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://cak.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pft.redwolf501.top

[C02] 默认参数
来源：http://hlr.ivvv.top

Py:   def greet(name="World"): return name
来源：http://kmv.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uqc.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://idx.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yxd.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dmx.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uax.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://odq.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://azt.shzxlz.cn

[C03] 可变参数
来源：http://nfn.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://jqx.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xut.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pds.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfq.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lws.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gnu.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://rhz.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fxt.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://udl.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://akg.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wmx.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eot.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dwc.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ckh.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://siq.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://vji.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://eil.hnxiangtu.top

[C05] 返回多个值
来源：http://bky.bjfxy.top

Py:   return a, b
来源：http://dvw.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://czq.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jxx.zhiwuduotai.top

TS:   return { a, b };
来源：http://kbi.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dpp.yuanzhike.top

Go:   return a, b
来源：http://vki.yvedp.cn

Ruby: return a, b
来源：http://mbb.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://vei.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://ctt.316326.xyz

Py:   square = lambda x: x * x
来源：http://uki.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ojm.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://zxc.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://afk.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dke.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://coh.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://kzi.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vev.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://pwx.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcf.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://dff.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://azf.zdqjudy.top

TS:   arr.map(String)
来源：http://aqi.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://usk.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pkx.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://hsq.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iau.cdnleiting.top

[C08] 闭包
来源：http://gmk.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ith.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hfx.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jmn.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iot.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://auq.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pki.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ppi.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://scy.aizwys.cn

[C09] 递归
来源：http://sox.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yoj.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://omy.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnk.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ucu.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sep.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvn.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wup.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://scn.jqgfzy.top

[C10] 变量作用域
来源：http://qti.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gtn.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ofo.xingfuxueyuan.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kkr.tanke756.top

TS:   同 JS
来源：http://dkt.shuidangran.top

Java: 方法内为块级作用域
来源：http://jsw.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://wlg.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wgi.gaohongyu789.top

C#:   块级作用域
来源：http://ijw.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://ojb.sufxvd.cn

Py:   from module import func
来源：http://kdl.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xoi.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wza.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://isg.zdqjudy.top

Java: import java.util.List;
来源：http://urv.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ior.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://iny.ydjk.org.cn

C#:   using System.Text;
来源：http://mrw.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://siv.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://rnd.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://ght.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://mts.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://aua.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jsy.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://nes.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://nxn.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yqm.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://jsa.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vig.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkn.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yax.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kst.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://ual.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://qxk.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sov.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://bra.xuetiantiany.cn

[C14] 泛型函数
来源：http://ogn.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nfq.ctjpmb.com

PHP:  // 无泛型
来源：http://jqf.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://rog.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uui.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uvl.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mzb.yongpay.top

Ruby: # 无泛型
来源：http://wzf.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jrt.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://qpy.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dou.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://cmw.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://soy.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oky.shanyushiyangtech.top

Java: // 无解构
来源：http://rzf.wangdashe.top

Go:   // 无解构
来源：http://uck.snrcjt.cn

Ruby: a, b = pair
来源：http://uoo.smart0.xyz

C#:   var (a, b) = pair;
来源：http://qfo.pycfn.com

[C16] 函数 / 方法重载
来源：http://efu.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jbp.nanxuanxn.top

PHP:  // 无重载
来源：http://dre.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hos.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://bzh.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://mki.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://pfo.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://any.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://grm.yfazqb.com

================================================================================
来源：http://pob.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://lcg.guowangkeji.top

================================================================================
来源：http://wxd.fktsv.cn

[D01] 创建数组 / 列表
来源：http://nvj.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://edx.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcg.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://shg.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wqu.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hxc.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://kmv.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://gwl.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zvm.hcnkem.com

[D02] 追加元素到末尾
来源：http://xmt.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://som.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ydq.chenlongwang.top

JS:   arr.push(4);
来源：http://qfc.jiagoushi.top

TS:   arr.push(4);
来源：http://bvl.xziqi.cn

Java: list.add(4);
来源：http://wgm.uphjek.com

Go:   arr = append(arr, 4)
来源：http://ygm.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://oqb.tian-w.cn

C#:   list.Add(4);
来源：http://dhr.mhx1999.top

[D03] 在指定位置插入元素
来源：http://men.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://acx.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ldl.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mpc.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://qul.gaohongyu789.top

Java: list.add(0, 0);
来源：http://zww.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vad.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qch.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://unx.aizwys.cn

[D04] 删除元素
来源：http://wnd.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fyu.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ozy.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nri.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://yzr.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nbr.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsd.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ygp.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rnn.316326.xyz

[D05] 访问与修改元素
来源：http://ktx.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rch.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dvw.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tjw.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://zcn.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://osk.guowangkeji.top


<!-- 参考信息 -->