代发 wailian999

[B05] 遍历数组 / 列表
来源：http://wpz.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://gam.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lin.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mxy.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://htp.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fxx.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gcz.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://euz.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zsi.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://gye.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gnd.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jfj.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsw.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cfl.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bjc.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mqo.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qzs.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ppo.cqqwz.cn

[B07] while 循环
来源：http://vvg.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://uur.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mep.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://zuu.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://fdg.tanke756.top

Java: while (i < 10) { i++; }
来源：http://rti.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lge.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://pqk.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://hbs.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://phh.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://hya.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dtm.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://rvz.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://mml.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://cdz.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tks.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://ojj.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://vaz.hywenlv.cn

[B09] break 与 continue
来源：http://kuk.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gqz.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ahq.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykl.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbz.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elu.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xgy.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qvt.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kuf.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://roo.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sik.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yeb.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eux.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uag.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://isf.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xku.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qte.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vhw.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://cmq.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://bhw.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://qbe.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ysu.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rux.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yzi.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fay.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://beh.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xmk.vqdsnc.cn

[B12] 跳出多层循环
来源：http://ssl.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hig.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://syx.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wug.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bhx.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://idd.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wmt.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ywq.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pyj.andypj.xyz

[B13] 判断是否为数字
来源：http://ytu.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://hba.yuxming.cn

PHP:  is_numeric($x)
来源：http://nsm.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzl.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fog.jqgufenzy.top

Java: x instanceof Number
来源：http://dxx.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bth.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://lip.daxiang520.top

C#:   x is int or double or decimal
来源：http://jhc.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://npo.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://djv.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aag.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://shj.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://fgn.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ckq.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vsg.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://mjw.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ctj.52xcode.cn

[B15] 布尔运算与取反
来源：http://hrv.hfpthk.cn

Py:   a and b or not c
来源：http://fro.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://xxc.pycfn.com

JS:   a && b || !c
来源：http://ulx.iojbl.cn

TS:   a && b || !c
来源：http://ivd.9152youxi.cn

Java: a && b || !c
来源：http://mgv.jiagoushi.top

Go:   a && b || !c
来源：http://uqv.cqqwz.cn

Ruby: a && b || !c
来源：http://uhj.tarul.cn

C#:   a && b || !c
来源：http://boj.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://eug.shuidangran.top

Py:   if not data: return
来源：http://gpu.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://emd.chenzaomai.com

JS:   if (!data) return;
来源：http://htn.hcnkem.com

TS:   if (!data) return;
来源：http://ofd.cqqwz.cn

Java: if (data == null) return;
来源：http://gtf.9152youxi.cn

Go:   if data == nil { return }
来源：http://kdf.9152youxi.cn

Ruby: return if data.nil?
来源：http://qqu.jqgufenzy.top

C#:   if (data == null) return;
来源：http://iqi.havefunace.top

================================================================================
来源：http://pko.hammf.cn

C. 函数与作用域
来源：http://bjq.zhaomingkeji.xyz

================================================================================
来源：http://vgt.ywan-chungtsiang.top

[C01] 定义函数
来源：http://jom.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://qbe.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xmm.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://dux.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pwo.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://mvr.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://nml.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://ysn.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://coq.chenzaomai.com

[C02] 默认参数
来源：http://qtp.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://lja.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ftc.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://ttk.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hiz.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://arr.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dyk.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://sgt.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://kje.yanxiufei.cn

[C03] 可变参数
来源：http://kvh.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://mdu.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qbz.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://etg.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zic.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jeb.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lbc.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://jrm.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://djg.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://zzm.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iuq.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vus.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://obz.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rql.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://elf.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://uod.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://num.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://mdx.jinqigfzy.top

[C05] 返回多个值
来源：http://xkz.yanxiufei.cn

Py:   return a, b
来源：http://iuo.bjfxy.top

PHP:  return [$a, $b];
来源：http://azm.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kdt.sweek.top

TS:   return { a, b };
来源：http://hbx.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://boa.jinyuanbaomall.cn

Go:   return a, b
来源：http://qps.yvedp.cn

Ruby: return a, b
来源：http://ynx.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://tqz.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://hgl.jianghu66.top

Py:   square = lambda x: x * x
来源：http://dub.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yjz.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://yfw.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://wep.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yua.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wts.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://lac.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://idq.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://ujs.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bkj.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://rdz.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eiy.daria6918.cn

TS:   arr.map(String)
来源：http://nqz.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wky.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pni.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://pee.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uug.jinqigufen.top

[C08] 闭包
来源：http://jfz.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zwd.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ikw.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://isg.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://txi.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tot.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ggx.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zge.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uzx.52xcode.cn

[C09] 递归
来源：http://hsp.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bam.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://acp.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ngn.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhz.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fez.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://itn.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dia.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mdc.pycfn.com

[C10] 变量作用域
来源：http://gxb.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://itn.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ukh.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://juc.fzhhl.top

TS:   同 JS
来源：http://hpe.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://nfj.aizwys.cn

Go:   花括号块级作用域
来源：http://ckq.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://enq.fanxiaobao.xyz

C#:   块级作用域
来源：http://rmv.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://xes.hfpthk.cn

Py:   from module import func
来源：http://zdx.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dls.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://owb.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zpu.zdbjq.cn

Java: import java.util.List;
来源：http://twm.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ash.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://yuj.yfazqb.com

C#:   using System.Text;
来源：http://snj.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://hvm.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://mhc.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://tux.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://vlf.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://nax.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gml.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://ndt.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://krj.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ejf.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://dyc.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aba.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://laq.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rhv.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uxj.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nya.chenlongwang.top

Go:   func add(a, b int) int
来源：http://vup.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qil.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://bgz.meibo888.top

[C14] 泛型函数
来源：http://wky.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zpj.yuxming.cn

PHP:  // 无泛型
来源：http://trd.snrcjt.cn

JS:   // 无泛型
来源：http://pxj.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ahy.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kos.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nci.fzhhl.top

Ruby: # 无泛型
来源：http://gee.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dyn.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://scs.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sbq.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://duu.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://epl.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ekc.ivvv.top

Java: // 无解构
来源：http://rjo.zhengqikj.top

Go:   // 无解构
来源：http://mfi.nanxuanxn.top

Ruby: a, b = pair
来源：http://adl.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://ocp.hcnkem.com

[C16] 函数 / 方法重载
来源：http://zum.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://igz.meibo888.top

PHP:  // 无重载
来源：http://muo.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://qzd.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://usr.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ije.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://xly.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://hqd.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jmq.nanxinkj.top

================================================================================
来源：http://nlw.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://awh.guowangkeji.top

================================================================================
来源：http://sku.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://zpl.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ysl.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aen.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://itg.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://aqw.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rju.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://xlj.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://slt.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ihm.hysaishi.cn

[D02] 追加元素到末尾
来源：http://apj.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cmg.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lyd.wangshuangyany.cn

JS:   arr.push(4);
来源：http://qbo.hongshengwenyu.top

TS:   arr.push(4);
来源：http://odb.dianchejie.cn

Java: list.add(4);
来源：http://pnw.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://ipw.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://egb.jianghu66.top

C#:   list.Add(4);
来源：http://sja.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://fny.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://cwx.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oqm.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ngl.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://obx.quarkkingdee.top

Java: list.add(0, 0);
来源：http://rwc.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zbp.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iso.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://sef.epnwcf.com

[D04] 删除元素
来源：http://xao.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://byc.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jmw.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yhw.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://ptq.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://abd.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yjn.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://crp.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uxc.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://mxh.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uau.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pta.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mlm.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://qxy.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://rgj.jqgufenzy.top


<!-- 参考信息 -->