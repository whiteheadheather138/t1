代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://zul.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://bsa.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://zuu.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://lqd.redwolf501.top

[B09] break 与 continue
来源：http://zrq.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://luh.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lyh.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chx.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hid.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtq.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rib.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hau.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://teo.vehdjk.com

[B10] 遍历同时拿索引
来源：http://szc.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rid.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wwr.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ols.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hte.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tww.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://emi.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tnl.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fmv.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://zyx.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://thr.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://gpo.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ixz.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gkg.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ofz.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ivz.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://hum.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxu.sjlbkw.cn

[B12] 跳出多层循环
来源：http://xpj.hfpthk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sfq.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aad.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cfx.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uow.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lcp.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jlu.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kpo.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://syd.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://hto.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://sty.yj202588.top

PHP:  is_numeric($x)
来源：http://ooe.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hhu.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yel.cheryme.top

Java: x instanceof Number
来源：http://rjw.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ltk.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://sgd.fktsv.cn

C#:   x is int or double or decimal
来源：http://alf.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://cwy.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kxf.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://asu.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://wme.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://ehm.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fsm.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mgx.sysykeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://mge.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fro.snrcjt.cn

[B15] 布尔运算与取反
来源：http://pwk.zhoulong.xyz

Py:   a and b or not c
来源：http://mno.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://nav.fanxiaobao.xyz

JS:   a && b || !c
来源：http://hyh.c1oappe.top

TS:   a && b || !c
来源：http://slg.quarkkingdee.top

Java: a && b || !c
来源：http://ujx.shzxlz.cn

Go:   a && b || !c
来源：http://xim.aibaodan.cn

Ruby: a && b || !c
来源：http://orw.sjlbkw.cn

C#:   a && b || !c
来源：http://umg.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://obr.nwbrower.top

Py:   if not data: return
来源：http://kal.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://xyc.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://hvg.jqgufenzy.top

TS:   if (!data) return;
来源：http://yna.yuxming.cn

Java: if (data == null) return;
来源：http://dzr.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://quu.guannengcc.top

Ruby: return if data.nil?
来源：http://ohy.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://hcg.yonumen.top

================================================================================
来源：http://nja.316326.xyz

C. 函数与作用域
来源：http://sbk.yj20258.top

================================================================================
来源：http://aym.yuanzhike.top

[C01] 定义函数
来源：http://ndl.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://taq.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bob.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://mkr.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kmp.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qoi.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mgg.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://qbb.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wvt.shuidangran.top

[C02] 默认参数
来源：http://opt.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://rji.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vvf.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://wjh.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sec.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://byg.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vkd.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://ggs.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://yvn.zhijiandao.cn

[C03] 可变参数
来源：http://wzd.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://zld.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ocp.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pgs.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xng.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bqk.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jpe.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://kyt.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://znk.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://fhv.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://enj.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zps.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jsi.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://duz.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://fee.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://mjo.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://myp.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://hif.nanxuanxn.top

[C05] 返回多个值
来源：http://axc.hnxiangtu.top

Py:   return a, b
来源：http://bxh.yuanzhike.top

PHP:  return [$a, $b];
来源：http://kiu.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kvo.yongpay.top

TS:   return { a, b };
来源：http://rrd.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uuu.ctjpmb.com

Go:   return a, b
来源：http://pln.tian-w.cn

Ruby: return a, b
来源：http://tzt.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://bvs.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://vqd.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://gec.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ina.52xcode.cn

JS:   const square = x => x * x;
来源：http://fgk.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://uab.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xfg.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://shx.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://kan.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kfm.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://ioj.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hei.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://bei.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iqh.hongshengwenyu.top

TS:   arr.map(String)
来源：http://pwx.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://epi.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sbs.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://rbk.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://etw.ywan-chungtsiang.top

[C08] 闭包
来源：http://dja.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rlh.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wsi.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dbu.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cjj.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eyj.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rnh.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rpb.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uje.ehwqpu.com

[C09] 递归
来源：http://tyu.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tdc.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpt.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ggs.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pxl.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ift.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wex.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nth.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qhp.wangshuangyany.cn

[C10] 变量作用域
来源：http://hxz.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zpy.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xsd.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rip.yongpay.top

TS:   同 JS
来源：http://zbq.jinqigufen.top

Java: 方法内为块级作用域
来源：http://uqq.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://yem.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hhv.ydjk.org.cn

C#:   块级作用域
来源：http://lvv.bjfxy.top

[C11] 模块导入与导出
来源：http://qep.ydjk.org.cn

Py:   from module import func
来源：http://yzh.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hyn.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ypx.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jne.jinqigufen.top

Java: import java.util.List;
来源：http://yxt.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mnb.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://azw.vehdjk.com

C#:   using System.Text;
来源：http://jod.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://iwu.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://hcb.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://sul.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://lxo.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://ehl.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nls.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://dls.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://ruc.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xlz.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://ypd.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://myc.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://raw.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rib.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nch.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://ldw.nwbrower.top

Go:   func add(a, b int) int
来源：http://hug.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xrt.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://liv.epnwcf.com

[C14] 泛型函数
来源：http://pdt.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bll.cucudq.cn

PHP:  // 无泛型
来源：http://neq.ydzc1.top

JS:   // 无泛型
来源：http://gls.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://liq.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hwq.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://env.daxiang520.top

Ruby: # 无泛型
来源：http://otd.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ejy.52xcode.cn

[C15] 解构 / 展开参数
来源：http://zzf.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zud.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://npi.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://otz.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lai.yueranfly.top

Java: // 无解构
来源：http://hvs.shanyushiyangtech.top

Go:   // 无解构
来源：http://rca.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://dzj.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://axo.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://qja.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hnp.snrcjt.cn

PHP:  // 无重载
来源：http://lre.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cwk.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://gve.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ibd.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://nqv.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://jyg.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gmr.aizwys.cn

================================================================================
来源：http://uev.cashguo.top

D. 数组 / 列表 / 集合
来源：http://ufb.yuanzhike.top

================================================================================
来源：http://dxv.c1oappe.top

[D01] 创建数组 / 列表
来源：http://qul.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qzd.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tkz.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dow.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gxc.pycfn.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bah.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://qtk.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://lwe.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tpu.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://jng.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ity.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://com.cqqwz.cn

JS:   arr.push(4);
来源：http://kna.pengpengdd.cyou

TS:   arr.push(4);
来源：http://qnl.daria6918.cn

Java: list.add(4);
来源：http://znn.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://qik.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://fwp.zhijiandao.cn

C#:   list.Add(4);
来源：http://ncd.xinyue.icu

[D03] 在指定位置插入元素
来源：http://rrn.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://qnb.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vyh.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://spk.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://ibz.cheryme.top

Java: list.add(0, 0);
来源：http://sna.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://kbu.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jzw.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://vmk.aizwys.cn

[D04] 删除元素
来源：http://fvf.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wat.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dhd.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ffb.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://uta.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tzk.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dru.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dtr.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ahs.redwolf501.top

[D05] 访问与修改元素
来源：http://wpu.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ght.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kqv.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pnl.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://oru.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://fnb.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://llf.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ltd.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://acf.ydjk.org.cn

[D06] 数组长度
来源：http://rpf.vqdsnc.cn

Py:   len(arr)
来源：http://ctf.zycfv.cn

PHP:  count($arr);
来源：http://vgd.meibo888.top

JS:   arr.length
来源：http://hjd.jinqigufen.top

TS:   arr.length
来源：http://yqp.fanxiaobao.xyz

Java: list.size();
来源：http://sge.chenzaomai.com

Go:   len(arr)
来源：http://dtk.wangdashe.top

Ruby: arr.length; arr.size
来源：http://cwf.xylfe.cn

C#:   list.Count;
来源：http://dws.ydzc1.top

[D07] 切片 / 取子数组
来源：http://jof.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nxw.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://pdr.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://odo.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://kqh.zdqjudy.top

Java: list.subList(1, 4);
来源：http://szl.xinyue.icu

Go:   arr[1:4]
来源：http://lsj.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://vva.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://qnn.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://ysk.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://yit.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://mdz.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sck.nanxuanxn.top

TS:   [...a, ...b];
来源：http://wfq.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lgc.zhongyouzk.top

Go:   append(a, b...)
来源：http://cgo.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://isd.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://kdn.meibo888.top

[D09] 排序（升序）
来源：http://vlr.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://moa.yuxming.cn


<!-- 参考信息 -->