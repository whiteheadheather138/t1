代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://alm.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mad.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://lnt.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://pme.jianghu66.top

[B09] break 与 continue
来源：http://wbq.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://umn.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oek.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rni.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgq.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpz.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ntc.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fht.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxo.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://xjm.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://acd.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sne.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://adj.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lhe.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fxc.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wwp.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kod.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gmd.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://qxi.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://jqp.hammf.cn

PHP:  range(0, 10, 2);
来源：http://wpg.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sqg.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gor.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nwx.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kna.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://qkf.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tia.aizwys.cn

[B12] 跳出多层循环
来源：http://sgl.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://lsw.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mrx.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzg.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gjt.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vxv.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xlt.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://are.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pko.hfpthk.cn

[B13] 判断是否为数字
来源：http://bwu.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://wwj.guannengcc.top

PHP:  is_numeric($x)
来源：http://jyd.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://skr.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://don.hywenlv.cn

Java: x instanceof Number
来源：http://owq.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lko.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://fub.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://ekp.tanke756.top

[B14] 判断值是否在集合内
来源：http://lip.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uks.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bsl.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://gfo.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://fvc.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lxl.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kil.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://exl.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ekl.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://ngh.zhengqikj.top

Py:   a and b or not c
来源：http://igc.guannengcc.top

PHP:  $a && $b || !$c
来源：http://mmz.zycfv.cn

JS:   a && b || !c
来源：http://lbl.sufxvd.cn

TS:   a && b || !c
来源：http://zwk.ivvv.top

Java: a && b || !c
来源：http://fal.zdbjq.cn

Go:   a && b || !c
来源：http://rqu.yuanzhike.top

Ruby: a && b || !c
来源：http://hlw.ppjwa.cn

C#:   a && b || !c
来源：http://ddz.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://hxb.yvedp.cn

Py:   if not data: return
来源：http://eck.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://aza.fehbvm.com

JS:   if (!data) return;
来源：http://emt.uphjek.com

TS:   if (!data) return;
来源：http://bvc.yueranfly.top

Java: if (data == null) return;
来源：http://trr.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://wxq.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://aha.shzxlz.cn

C#:   if (data == null) return;
来源：http://zuk.yj20258.top

================================================================================
来源：http://kaj.hongshengwenyu.top

C. 函数与作用域
来源：http://lbc.hongshengwenyu.top

================================================================================
来源：http://het.52xcode.cn

[C01] 定义函数
来源：http://njc.yj20258.top

Py:   def add(a, b): return a + b
来源：http://crm.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bzi.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://hts.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cuy.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kef.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kto.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://dch.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fjr.uphjek.com

[C02] 默认参数
来源：http://zqr.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://rri.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://riu.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://bhe.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://awe.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ozm.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://csg.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://ios.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://idd.shanyushiyangtech.top

[C03] 可变参数
来源：http://ntp.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://flf.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yae.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmg.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rxt.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vgt.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tkf.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kdh.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tej.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://hdy.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://efw.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xkl.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tcm.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xfa.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://uri.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://lbb.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://tkc.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://roh.gaohongyu789.top

[C05] 返回多个值
来源：http://xsb.sweek.top

Py:   return a, b
来源：http://hkj.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://evw.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://llb.jlsjyb.cn

TS:   return { a, b };
来源：http://nfn.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dwi.jinqigufen.top

Go:   return a, b
来源：http://zut.ydzc1.top

Ruby: return a, b
来源：http://kmm.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ydt.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://vpb.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://tvf.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://qdd.wangdashe.top

JS:   const square = x => x * x;
来源：http://hvz.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://mup.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mzq.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dpo.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://tdv.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://pkv.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://pph.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lsr.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://lqr.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vaq.jqgufenzy.top

TS:   arr.map(String)
来源：http://ogj.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://anw.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ghs.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://kkk.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ogi.havefunace.top

[C08] 闭包
来源：http://zwx.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eof.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tpd.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xsn.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qzh.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rdv.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vfy.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ljp.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rsd.jinqigfzy.top

[C09] 递归
来源：http://ijj.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wfm.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cgs.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ipa.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://idg.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://key.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mni.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://whk.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pjk.ppjwa.cn

[C10] 变量作用域
来源：http://duz.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ehe.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fag.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ilz.bbcook.cn

TS:   同 JS
来源：http://pqy.ydzc1.top

Java: 方法内为块级作用域
来源：http://kfi.dashuyun.cn

Go:   花括号块级作用域
来源：http://nvt.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cvw.xuetiantiany.cn

C#:   块级作用域
来源：http://byd.hfpthk.cn

[C11] 模块导入与导出
来源：http://gky.fanxiaobao.xyz

Py:   from module import func
来源：http://btp.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://pox.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cej.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://quc.sufxvd.cn

Java: import java.util.List;
来源：http://mlv.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ycd.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://rcb.ehwqpu.com

C#:   using System.Text;
来源：http://ail.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://wee.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://kff.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://dbw.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://mck.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://wzh.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kvh.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://snf.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://xfo.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nhb.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://lva.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mjl.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oct.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vho.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fok.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://wpg.gotoacloud.top

Go:   func add(a, b int) int
来源：http://nby.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rok.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://yyw.yonumen.top

[C14] 泛型函数
来源：http://ped.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://osq.zhijiandao.cn

PHP:  // 无泛型
来源：http://iru.kuanghao11.cn

JS:   // 无泛型
来源：http://qdd.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fut.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sop.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sbh.mhx1999.top

Ruby: # 无泛型
来源：http://lgf.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qpu.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://wmd.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bks.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://vws.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vrg.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kxe.ppjwa.cn

Java: // 无解构
来源：http://acm.hysaishi.cn

Go:   // 无解构
来源：http://nop.shangyingyoupin.top

Ruby: a, b = pair
来源：http://mid.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://lrp.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://yfv.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nhb.tarul.cn

PHP:  // 无重载
来源：http://ycc.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkb.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://ibk.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cpk.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://ljm.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://zzl.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jpi.9152youxi.cn

================================================================================
来源：http://cnq.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://laq.yueranfly.top

================================================================================
来源：http://lud.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://zkw.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jnu.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rky.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://epu.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jzt.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vml.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://ufk.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://crq.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hfq.yuanzhike.top

[D02] 追加元素到末尾
来源：http://sdw.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lfa.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ums.epnwcf.com

JS:   arr.push(4);
来源：http://zgx.jinqigfzy.top

TS:   arr.push(4);
来源：http://btj.jlsjyb.cn

Java: list.add(4);
来源：http://jxp.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://fvr.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://gnd.sysykeji.top

C#:   list.Add(4);
来源：http://odq.smart0.xyz

[D03] 在指定位置插入元素
来源：http://spd.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://nyu.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lgt.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vqj.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://jmv.jinqigufen.top

Java: list.add(0, 0);
来源：http://jer.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sik.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://maz.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://kgk.yfazqb.com

[D04] 删除元素
来源：http://wee.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://arb.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qri.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eyr.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://dat.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wzn.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xnl.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kzc.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jdl.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://wvl.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dpl.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xxc.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ysm.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://utd.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://hng.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://abm.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mfw.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pwu.guowangkeji.top

[D06] 数组长度
来源：http://tds.sysykeji.top

Py:   len(arr)
来源：http://tfx.ivvv.top

PHP:  count($arr);
来源：http://zys.chenzaomai.com

JS:   arr.length
来源：http://dhr.tian-w.cn

TS:   arr.length
来源：http://krs.fktsv.cn

Java: list.size();
来源：http://nhw.jianghu66.top

Go:   len(arr)
来源：http://xli.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://vkn.redwolf501.top

C#:   list.Count;
来源：http://odq.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://dxy.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vmk.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://akd.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://lji.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://lgw.jiagoushi.top

Java: list.subList(1, 4);
来源：http://isn.hnxiangtu.top

Go:   arr[1:4]
来源：http://xzn.shuidangran.top

Ruby: arr[1, 3]
来源：http://ypw.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://qlj.52xcode.cn

[D08] 合并两个数组
来源：http://btz.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://hpt.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://kmu.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ryl.xuanzx.com

TS:   [...a, ...b];
来源：http://mno.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kou.zhijiandao.cn

Go:   append(a, b...)
来源：http://tbf.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://jbk.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://qrm.jianghu66.top

[D09] 排序（升序）
来源：http://dfj.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://mbc.bjfxy.top


<!-- 参考信息 -->