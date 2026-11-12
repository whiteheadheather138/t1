代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://vew.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://afd.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vjw.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://hmq.cqqwz.cn

[B09] break 与 continue
来源：http://bnl.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zyv.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gnp.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://euk.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucl.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mis.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uqt.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://roo.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jnf.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://ylx.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://alz.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://coz.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qxh.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://alg.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ocr.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rej.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://raf.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://opj.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://wym.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://wit.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://csi.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vxb.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggu.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osn.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sms.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://esj.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cms.ehwqpu.com

[B12] 跳出多层循环
来源：http://wda.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://tor.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hey.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://duu.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nrm.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jbe.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mjt.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://odt.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yvw.sweek.top

[B13] 判断是否为数字
来源：http://sen.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://hos.andypj.xyz

PHP:  is_numeric($x)
来源：http://gqv.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iqy.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrv.sjlbkw.cn

Java: x instanceof Number
来源：http://kla.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rwo.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://qgk.xinyue.icu

C#:   x is int or double or decimal
来源：http://xfy.mhx1999.top

[B14] 判断值是否在集合内
来源：http://bjo.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jsx.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gpb.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://ozi.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://yto.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dow.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fdg.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ftp.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://srm.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://fwt.birdmap.top

Py:   a and b or not c
来源：http://afm.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://kfa.cqqwz.cn

JS:   a && b || !c
来源：http://dqw.daxiang520.top

TS:   a && b || !c
来源：http://epe.tian-w.cn

Java: a && b || !c
来源：http://ndp.snrcjt.cn

Go:   a && b || !c
来源：http://yby.jinqigufen.top

Ruby: a && b || !c
来源：http://igc.haohaochexian.top

C#:   a && b || !c
来源：http://bvl.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://qkn.gotoacloud.top

Py:   if not data: return
来源：http://iqb.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://odt.wangdashe.top

JS:   if (!data) return;
来源：http://izp.nanxuanxn.top

TS:   if (!data) return;
来源：http://uot.bjfxy.top

Java: if (data == null) return;
来源：http://oqv.fengsongda.top

Go:   if data == nil { return }
来源：http://iis.yanxiufei.cn

Ruby: return if data.nil?
来源：http://mvg.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://snt.ydjk.org.cn

================================================================================
来源：http://qeu.ywan-chungtsiang.top

C. 函数与作用域
来源：http://gfo.zhaomingkeji.xyz

================================================================================
来源：http://yln.zhengqikj.top

[C01] 定义函数
来源：http://rnt.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://cwj.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsz.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://vmh.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mtn.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://skm.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://elu.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://wwo.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://exb.yueranfly.top

[C02] 默认参数
来源：http://men.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://fiy.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cah.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://eaq.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jji.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hdo.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wpa.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://ncb.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://tvk.yfazqb.com

[C03] 可变参数
来源：http://spv.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://uyz.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ani.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ugz.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hyu.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jti.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xxy.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://gww.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://luz.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://etq.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mzn.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wgt.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ngg.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rbr.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://qwu.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://ohg.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://yyb.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://wwd.sufxvd.cn

[C05] 返回多个值
来源：http://cdz.cucudq.cn

Py:   return a, b
来源：http://epd.sweek.top

PHP:  return [$a, $b];
来源：http://ntg.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lko.zhixingplan.top

TS:   return { a, b };
来源：http://bbp.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tcz.chenjidiqi.icu

Go:   return a, b
来源：http://ocd.hongshengwenyu.top

Ruby: return a, b
来源：http://zgw.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://wfh.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://smy.aizwys.cn

Py:   square = lambda x: x * x
来源：http://zyx.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kdo.vehdjk.com

JS:   const square = x => x * x;
来源：http://tef.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://kpv.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fzp.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jsw.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://hmh.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://wfs.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://obi.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hnz.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lxc.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzp.hfpthk.cn

TS:   arr.map(String)
来源：http://dui.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://etn.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ioo.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://psk.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uwu.fehbvm.com

[C08] 闭包
来源：http://aud.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tur.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hdd.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oyz.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fwo.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jou.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dko.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ous.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://akx.dashuyun.cn

[C09] 递归
来源：http://ywj.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qks.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pks.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fnv.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cut.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jzs.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://crr.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hzf.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wtz.xinyue.icu

[C10] 变量作用域
来源：http://epl.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fip.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sgy.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zan.uphjek.com

TS:   同 JS
来源：http://aoz.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://ekt.xziqi.cn

Go:   花括号块级作用域
来源：http://cuf.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rzn.aibaodan.cn

C#:   块级作用域
来源：http://kgx.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://dlr.fktsv.cn

Py:   from module import func
来源：http://gwu.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uan.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ocz.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uxs.sxryk.cn

Java: import java.util.List;
来源：http://xoo.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nex.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://twb.daxiang520.top

C#:   using System.Text;
来源：http://wqv.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://ldt.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://hmk.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://bzr.nwbrower.top

JS:   (() => { console.log("run"); })();
来源：http://wur.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://wgj.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mbp.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://ltq.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://mdo.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://lvx.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://jho.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqk.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sdo.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yvv.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hec.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://cmg.ivvv.top

Go:   func add(a, b int) int
来源：http://ktt.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vwc.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kru.shangyingyoupin.top

[C14] 泛型函数
来源：http://hki.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ujy.bbcook.cn

PHP:  // 无泛型
来源：http://rlm.redwolf501.top

JS:   // 无泛型
来源：http://cvr.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iuw.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://poy.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ivy.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://ulo.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vhb.pycfn.com

[C15] 解构 / 展开参数
来源：http://qzx.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gjs.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://wzz.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcr.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://epu.ivvv.top

Java: // 无解构
来源：http://ize.tianlin.xyz

Go:   // 无解构
来源：http://xme.yongpay.top

Ruby: a, b = pair
来源：http://kmh.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://bgj.jianghu66.top

[C16] 函数 / 方法重载
来源：http://bkc.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fya.pengpengdd.cyou

PHP:  // 无重载
来源：http://okm.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eoe.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://zcm.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bvk.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://ngr.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://msk.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://euo.xuanzx.com

================================================================================
来源：http://hgm.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://inm.daxiang520.top

================================================================================
来源：http://wxk.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://imr.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cbi.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pjy.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ugl.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://usn.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://glc.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://gth.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://xaj.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xeo.tian-w.cn

[D02] 追加元素到末尾
来源：http://die.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://epw.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dqw.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://kzi.kuanghao11.cn

TS:   arr.push(4);
来源：http://hwf.guowangkeji.top

Java: list.add(4);
来源：http://nyv.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://bmz.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://qkd.nanxuanxn.top

C#:   list.Add(4);
来源：http://qlk.yj20258.top

[D03] 在指定位置插入元素
来源：http://yqm.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://dmc.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://evr.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nvo.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://kzt.jqgfzy.top

Java: list.add(0, 0);
来源：http://mwt.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://eog.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oco.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://tmd.vehdjk.com

[D04] 删除元素
来源：http://jqc.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nqp.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xeg.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aab.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://pao.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jpy.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://czq.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zfs.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jde.zhongyouzk.top

[D05] 访问与修改元素
来源：http://njr.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fha.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kzx.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cvk.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://had.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://mlt.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://rrh.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sqw.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ucg.yj20258888.top

[D06] 数组长度
来源：http://wnq.jinqigfzy.top

Py:   len(arr)
来源：http://bpz.jyoumei.cn

PHP:  count($arr);
来源：http://trz.zhijiandao.cn

JS:   arr.length
来源：http://qku.chenzaomai.com

TS:   arr.length
来源：http://uuf.xuanzx.com

Java: list.size();
来源：http://vei.cqqwz.cn

Go:   len(arr)
来源：http://azu.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://xtm.hesvh.cn

C#:   list.Count;
来源：http://rno.hnqzz.top

[D07] 切片 / 取子数组
来源：http://jkx.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://joh.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://pmw.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://zre.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://zue.daria6918.cn

Java: list.subList(1, 4);
来源：http://gtn.yuxming.cn

Go:   arr[1:4]
来源：http://phm.smart0.xyz

Ruby: arr[1, 3]
来源：http://etf.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://aow.zhoulong.xyz

[D08] 合并两个数组
来源：http://kmk.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://jhh.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://epy.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://txy.sysykeji.top

TS:   [...a, ...b];
来源：http://hdo.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gsk.cucudq.cn

Go:   append(a, b...)
来源：http://oah.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://sym.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://ifs.wangdashe.top

[D09] 排序（升序）
来源：http://ycv.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://rnf.nanxinkj.top


<!-- 参考信息 -->