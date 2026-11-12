代发 wailian999

[B09] break 与 continue
来源：http://pve.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://upf.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mai.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osc.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amf.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihu.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rus.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bqg.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swm.yuxming.cn

[B10] 遍历同时拿索引
来源：http://awq.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aph.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gqf.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rkt.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lct.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://div.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uog.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xxk.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vnl.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://ykx.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://heo.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://hwi.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lat.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayq.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://izi.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://byf.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://zyg.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vvu.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://kwt.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tqx.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uja.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://taq.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wlw.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mzx.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ncf.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oal.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dlt.havefunace.top

[B13] 判断是否为数字
来源：http://caf.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://fwv.yj20258.top

PHP:  is_numeric($x)
来源：http://ntk.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdb.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jog.yangfankeji.com

Java: x instanceof Number
来源：http://brl.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jkk.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://nde.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://xtt.gzhubu.top

[B14] 判断值是否在集合内
来源：http://mxi.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jig.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gqt.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://riy.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://jzv.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://npb.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cmt.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://kih.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rtv.redwolf501.top

[B15] 布尔运算与取反
来源：http://fcp.aizwys.cn

Py:   a and b or not c
来源：http://sml.hammf.cn

PHP:  $a && $b || !$c
来源：http://byw.bjfxy.top

JS:   a && b || !c
来源：http://iga.pengpengdd.cyou

TS:   a && b || !c
来源：http://fqx.iojbl.cn

Java: a && b || !c
来源：http://guh.zdbjq.cn

Go:   a && b || !c
来源：http://cgn.yangfankeji.com

Ruby: a && b || !c
来源：http://gct.jinghuilouyu.cn

C#:   a && b || !c
来源：http://lak.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://srs.jlsjyb.cn

Py:   if not data: return
来源：http://yzg.uphjek.com

PHP:  if (!$data) { return; }
来源：http://cge.chenzaomai.com

JS:   if (!data) return;
来源：http://itu.bbcook.cn

TS:   if (!data) return;
来源：http://ygw.yj202588.top

Java: if (data == null) return;
来源：http://mkb.hnqzz.top

Go:   if data == nil { return }
来源：http://xgc.jqgfzy.top

Ruby: return if data.nil?
来源：http://jpz.0kj1m.cn

C#:   if (data == null) return;
来源：http://ngm.birdmap.top

================================================================================
来源：http://kpf.kuanghao11.cn

C. 函数与作用域
来源：http://yfv.jinyuanbaomall.cn

================================================================================
来源：http://ogg.jyoumei.cn

[C01] 定义函数
来源：http://uon.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://rwd.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kxv.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://hxu.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nlr.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fob.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://heo.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://vjw.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://szy.jinqigfzy.top

[C02] 默认参数
来源：http://uai.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://aws.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ges.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://yec.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dtc.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mmx.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wxg.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://rpf.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://stz.dashuyun.cn

[C03] 可变参数
来源：http://sif.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://fen.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nbq.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://flt.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iww.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bdk.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sae.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://sbg.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aon.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://djm.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cun.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cjy.quarkkingdee.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ojd.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://faq.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://wjh.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://hmy.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://btt.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://zdx.tianlin.xyz

[C05] 返回多个值
来源：http://xbc.bjfxy.top

Py:   return a, b
来源：http://nnt.chenlongwang.top

PHP:  return [$a, $b];
来源：http://zrj.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iha.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://wfq.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sga.shzxlz.cn

Go:   return a, b
来源：http://zfh.nanxuanxn.top

Ruby: return a, b
来源：http://bll.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://yxv.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://xqs.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://sxt.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zgi.sysykeji.top

JS:   const square = x => x * x;
来源：http://kjx.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://jqs.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://muq.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://ezz.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://ltl.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://jjr.yj20258888.top

[C07] 把函数作为参数传入
来源：http://dmo.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wly.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://rin.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gon.shuidangran.top

TS:   arr.map(String)
来源：http://nzc.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sjt.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ilj.sweek.top

Ruby: arr.map(&:upcase)
来源：http://ajy.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lgw.andypj.xyz

[C08] 闭包
来源：http://wso.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jvy.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ryx.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://obp.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jdw.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hsg.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ces.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vom.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hbg.zhiwuduotai.top

[C09] 递归
来源：http://zjh.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://izx.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hda.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sbz.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://orp.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ian.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xot.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oho.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://poj.xziqi.cn

[C10] 变量作用域
来源：http://lcw.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mev.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pxu.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ygh.dianchejie.cn

TS:   同 JS
来源：http://fgu.fengsongda.top

Java: 方法内为块级作用域
来源：http://xcs.xziqi.cn

Go:   花括号块级作用域
来源：http://mla.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zsw.mhx1999.top

C#:   块级作用域
来源：http://aeq.yvedp.cn

[C11] 模块导入与导出
来源：http://rni.xinyue.icu

Py:   from module import func
来源：http://mtm.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ter.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mhr.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rbj.epnwcf.com

Java: import java.util.List;
来源：http://qpg.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cgo.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://swv.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://ycp.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://cgi.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://xhm.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://eje.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://pzq.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://zxa.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qcs.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://oda.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://muh.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wxg.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://xbo.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qmo.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omc.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qpo.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ixq.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://jgw.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://xpk.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zmu.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qsd.dashuyun.cn

[C14] 泛型函数
来源：http://akf.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aud.yj20258.top

PHP:  // 无泛型
来源：http://oqb.mhx1999.top

JS:   // 无泛型
来源：http://vnq.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rke.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jop.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nob.ydzc1.top

Ruby: # 无泛型
来源：http://hjv.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fvg.gzhubu.top

[C15] 解构 / 展开参数
来源：http://jsv.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fxj.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://hfw.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yzg.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bgr.shuidangran.top

Java: // 无解构
来源：http://jyh.mhx1999.top

Go:   // 无解构
来源：http://yvj.jinqigfzy.top

Ruby: a, b = pair
来源：http://nda.guannengcc.top

C#:   var (a, b) = pair;
来源：http://jke.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://xtt.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cai.zhoulong.xyz

PHP:  // 无重载
来源：http://kas.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://yyq.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://vfh.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xtk.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://kue.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://iaq.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://khq.yvedp.cn

================================================================================
来源：http://fku.yongpay.top

D. 数组 / 列表 / 集合
来源：http://dvu.guannengcc.top

================================================================================
来源：http://dnh.havefunace.top

[D01] 创建数组 / 列表
来源：http://oxs.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://usq.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcs.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ije.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ngl.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vwh.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://usw.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://kmz.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zsb.ivvv.top

[D02] 追加元素到末尾
来源：http://lhv.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://quy.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iol.ydjk.org.cn

JS:   arr.push(4);
来源：http://svf.aizwys.cn

TS:   arr.push(4);
来源：http://mtw.aibaodan.cn

Java: list.add(4);
来源：http://tgz.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://rdo.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://qav.tanke756.top

C#:   list.Add(4);
来源：http://ier.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://oqi.uphjek.com

Py:   arr.insert(0, 0)
来源：http://adw.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ddt.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dov.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://ayp.guowangkeji.top

Java: list.add(0, 0);
来源：http://ebs.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://rfo.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gks.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://edk.hnxiangtu.top

[D04] 删除元素
来源：http://ssa.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kiz.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pjr.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bmk.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://cdo.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yoa.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fdb.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ieo.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ahv.nanxinkj.top

[D05] 访问与修改元素
来源：http://vav.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vmm.316326.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pbu.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eql.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://esy.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://izy.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://yek.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dsi.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xea.yfazqb.com

[D06] 数组长度
来源：http://uvi.ctjpmb.com

Py:   len(arr)
来源：http://rkc.yonumen.top

PHP:  count($arr);
来源：http://zku.gotoacloud.top

JS:   arr.length
来源：http://nam.cqqwz.cn

TS:   arr.length
来源：http://zmf.fengsongda.top

Java: list.size();
来源：http://ang.jyoumei.cn

Go:   len(arr)
来源：http://zzm.vehdjk.com

Ruby: arr.length; arr.size
来源：http://dch.cashguo.top

C#:   list.Count;
来源：http://aok.yj20258888.top

[D07] 切片 / 取子数组
来源：http://tij.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uww.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zui.316326.xyz

JS:   arr.slice(1, 4);
来源：http://wii.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://vap.hysaishi.cn

Java: list.subList(1, 4);
来源：http://gpa.birdmap.top

Go:   arr[1:4]
来源：http://can.havefunace.top

Ruby: arr[1, 3]
来源：http://ork.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://onc.chenjidiqi.icu

[D08] 合并两个数组
来源：http://rpa.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://bzv.meibo888.top

PHP:  array_merge($a, $b);
来源：http://hbq.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ooe.gogol.net.cn

TS:   [...a, ...b];
来源：http://woh.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rrv.jinqigufen.top

Go:   append(a, b...)
来源：http://qop.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://add.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://srp.hongshengwenyu.top

[D09] 排序（升序）
来源：http://doc.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://ngm.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://ksb.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://emf.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dyb.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eem.zhoulong.xyz


<!-- 参考信息 -->