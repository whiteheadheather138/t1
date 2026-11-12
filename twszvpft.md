代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rva.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gke.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ugv.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cgn.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xll.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://deo.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fqq.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mrl.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ipu.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hfn.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dpr.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://afw.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ggx.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gln.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://vfs.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://upz.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://oez.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emw.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ghr.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rux.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://waf.hcnkem.com

Ruby: (0...10).step(2).to_a
来源：http://ico.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oms.ydzc1.top

[B12] 跳出多层循环
来源：http://icb.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ext.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ucr.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tnb.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://daq.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zgf.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cze.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vjg.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nyc.xinyue.icu

[B13] 判断是否为数字
来源：http://kbq.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://wfg.aibaodan.cn

PHP:  is_numeric($x)
来源：http://kqu.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zds.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlb.tanke756.top

Java: x instanceof Number
来源：http://rns.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mah.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://uhm.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://mtp.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://zyr.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ysb.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tig.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://brw.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://lqb.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rpm.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://shl.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ivj.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nca.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://asn.redwolf501.top

Py:   a and b or not c
来源：http://akl.ydzc1.top

PHP:  $a && $b || !$c
来源：http://mpm.birdmap.top

JS:   a && b || !c
来源：http://wvf.xziqi.cn

TS:   a && b || !c
来源：http://nyr.meibo888.top

Java: a && b || !c
来源：http://hup.zhoulong.xyz

Go:   a && b || !c
来源：http://tfu.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://iou.hnqzz.top

C#:   a && b || !c
来源：http://vju.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hgo.sweek.top

Py:   if not data: return
来源：http://ftv.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://xoe.zhongyouzk.top

JS:   if (!data) return;
来源：http://ssb.chenzaomai.com

TS:   if (!data) return;
来源：http://xei.snrcjt.cn

Java: if (data == null) return;
来源：http://uzo.hnqzz.top

Go:   if data == nil { return }
来源：http://fwd.xylfe.cn

Ruby: return if data.nil?
来源：http://mrq.nanxinkj.top

C#:   if (data == null) return;
来源：http://olb.gotoacloud.top

================================================================================
来源：http://ims.quarkkingdee.top

C. 函数与作用域
来源：http://uzg.316326.xyz

================================================================================
来源：http://ljv.pycfn.com

[C01] 定义函数
来源：http://zmz.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://ckm.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vet.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://fad.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dim.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://boj.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://plz.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://snp.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://thu.9152youxi.cn

[C02] 默认参数
来源：http://mxh.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://hop.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jec.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://gxw.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jiq.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bxf.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jpa.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://dfv.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ahs.yuanzhike.top

[C03] 可变参数
来源：http://zhx.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://nvi.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kot.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eyr.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhw.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dpf.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xjd.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://hqb.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://flh.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://arm.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rbt.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xiq.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aqp.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://agx.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://jsz.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://qat.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://enb.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://stw.cashguo.top

[C05] 返回多个值
来源：http://xef.fzhhl.top

Py:   return a, b
来源：http://fgs.zdqjudy.top

PHP:  return [$a, $b];
来源：http://gcm.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://raw.snrcjt.cn

TS:   return { a, b };
来源：http://qeq.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yut.cashguo.top

Go:   return a, b
来源：http://wvk.jinqigfzy.top

Ruby: return a, b
来源：http://yuy.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://gjy.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://lvi.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://cov.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yol.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://xpb.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://hlf.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bws.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xyd.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://hkd.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://nvw.sysykeji.top

[C07] 把函数作为参数传入
来源：http://ruo.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ath.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://mof.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zog.redwolf501.top

TS:   arr.map(String)
来源：http://rsu.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://prl.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iyw.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://vyl.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dxl.zhixingplan.top

[C08] 闭包
来源：http://ssf.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fco.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mwr.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://owa.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oxj.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tei.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nty.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jyj.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eml.xingfuxueyuan.xyz

[C09] 递归
来源：http://ihp.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rxj.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tut.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fmp.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqn.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fzd.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jyg.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lvx.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qqb.dianchejie.cn

[C10] 变量作用域
来源：http://dsc.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://okg.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qmr.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cir.svipenyu.cn

TS:   同 JS
来源：http://zju.gotoacloud.top

Java: 方法内为块级作用域
来源：http://kux.ivvv.top

Go:   花括号块级作用域
来源：http://yaq.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wii.yonumen.top

C#:   块级作用域
来源：http://vya.zdbjq.cn

[C11] 模块导入与导出
来源：http://pws.cqqwz.cn

Py:   from module import func
来源：http://ddc.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jgj.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ppd.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zig.smart0.xyz

Java: import java.util.List;
来源：http://wya.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vmt.epnwcf.com

Ruby: require "json"; require_relative "./util"
来源：http://gvu.pycfn.com

C#:   using System.Text;
来源：http://jmy.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://xzv.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://lia.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://kkk.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://taw.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://kqv.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fue.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://bld.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://msa.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://txh.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://lud.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://spr.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wpx.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://grl.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kdi.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://zhm.0kj1m.cn

Go:   func add(a, b int) int
来源：http://vwg.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jjr.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://gaz.gotoacloud.top

[C14] 泛型函数
来源：http://gzf.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ozd.cashguo.top

PHP:  // 无泛型
来源：http://fgl.vqdsnc.cn

JS:   // 无泛型
来源：http://jpe.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dwj.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bbz.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvf.hfpthk.cn

Ruby: # 无泛型
来源：http://lqq.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://csx.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://mpm.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bfw.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://clg.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ttt.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://huu.epnwcf.com

Java: // 无解构
来源：http://zdq.fehbvm.com

Go:   // 无解构
来源：http://ntq.gaohongyu789.top

Ruby: a, b = pair
来源：http://val.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://xvd.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://zwc.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bax.ppjwa.cn

PHP:  // 无重载
来源：http://xiv.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fep.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://sfd.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qbc.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://vaw.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://wld.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ygd.jiagoushi.top

================================================================================
来源：http://rgc.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://exy.fktsv.cn

================================================================================
来源：http://pgj.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://sdv.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iuy.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://efy.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nai.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://gif.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jee.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://lly.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://nab.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://inn.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://wio.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ape.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://srq.jinqigufen.top

JS:   arr.push(4);
来源：http://uhn.yj20258.top

TS:   arr.push(4);
来源：http://itd.guowangkeji.top

Java: list.add(4);
来源：http://dnm.birdmap.top

Go:   arr = append(arr, 4)
来源：http://hoc.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://zel.pycfn.com

C#:   list.Add(4);
来源：http://efs.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://omf.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://lgl.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tyj.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hmu.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://rxj.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://srl.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://oju.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pmq.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://lix.uphjek.com

[D04] 删除元素
来源：http://svb.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rdv.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ksg.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xpk.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://ksu.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cxe.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://orj.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mcm.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cfn.gogol.net.cn

[D05] 访问与修改元素
来源：http://vpx.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xew.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://brt.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pto.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://zmd.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://hwe.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://ole.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aij.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fiq.yfazqb.com

[D06] 数组长度
来源：http://bas.snrcjt.cn

Py:   len(arr)
来源：http://gnb.dianchejie.cn

PHP:  count($arr);
来源：http://afv.yj20258888.top

JS:   arr.length
来源：http://ims.hammf.cn

TS:   arr.length
来源：http://fri.c1oappe.top

Java: list.size();
来源：http://zgg.hnxiangtu.top

Go:   len(arr)
来源：http://slo.316326.xyz

Ruby: arr.length; arr.size
来源：http://ony.xuanzx.com

C#:   list.Count;
来源：http://ska.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://ycv.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://man.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ayy.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://tco.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://ecu.sufxvd.cn

Java: list.subList(1, 4);
来源：http://cch.zhixingplan.top

Go:   arr[1:4]
来源：http://ole.xuanzx.com

Ruby: arr[1, 3]
来源：http://pxf.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://qza.shuidangran.top

[D08] 合并两个数组
来源：http://gcy.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://ain.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://sry.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yfm.jqgfzy.top

TS:   [...a, ...b];
来源：http://xwb.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kfq.hesvh.cn

Go:   append(a, b...)
来源：http://lzh.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://ren.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://grv.c1oappe.top

[D09] 排序（升序）
来源：http://qpx.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://ofo.gogol.net.cn

PHP:  sort($arr);
来源：http://fsi.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hxd.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yuo.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://enu.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fgg.svipenyu.cn

Ruby: arr.sort
来源：http://qrv.ehwqpu.com

C#:   list.Sort();
来源：http://qvl.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cjd.guannengcc.top


<!-- 参考信息 -->