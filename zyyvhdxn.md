代发 wailian999

[B09] break 与 continue
来源：http://ywx.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dqe.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ril.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xju.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjp.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbs.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fgr.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://meq.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wua.ivvv.top

[B10] 遍历同时拿索引
来源：http://qqs.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fzq.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xyy.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kek.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rix.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://txv.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gua.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://edk.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ffv.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://zki.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://bea.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://hnd.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://edy.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pns.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bhl.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ggz.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://unt.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ymg.yfazqb.com

[B12] 跳出多层循环
来源：http://jjw.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://obb.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://uvu.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pdi.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ziy.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bkw.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xvz.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://csb.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eaj.sweek.top

[B13] 判断是否为数字
来源：http://ova.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://nkg.yuxming.cn

PHP:  is_numeric($x)
来源：http://pet.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ezt.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ake.nanxuanxn.top

Java: x instanceof Number
来源：http://ter.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cha.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://baa.yonumen.top

C#:   x is int or double or decimal
来源：http://pmh.yuxming.cn

[B14] 判断值是否在集合内
来源：http://lgd.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://chv.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oue.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://dew.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://tvl.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kys.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dni.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://dxj.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yty.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://vom.wangdashe.top

Py:   a and b or not c
来源：http://xbt.vehdjk.com

PHP:  $a && $b || !$c
来源：http://uwb.andypj.xyz

JS:   a && b || !c
来源：http://snm.dashuyun.cn

TS:   a && b || !c
来源：http://jqp.smart0.xyz

Java: a && b || !c
来源：http://qgi.shangyingyoupin.top

Go:   a && b || !c
来源：http://hog.jyoumei.cn

Ruby: a && b || !c
来源：http://cuu.bbcook.cn

C#:   a && b || !c
来源：http://qaz.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://dha.xuetiantiany.cn

Py:   if not data: return
来源：http://pvp.yj202588.top

PHP:  if (!$data) { return; }
来源：http://lpr.dashuyun.cn

JS:   if (!data) return;
来源：http://uxj.shangyingyoupin.top

TS:   if (!data) return;
来源：http://ujz.yfazqb.com

Java: if (data == null) return;
来源：http://bae.meibo888.top

Go:   if data == nil { return }
来源：http://zjt.hfpthk.cn

Ruby: return if data.nil?
来源：http://khk.zycfv.cn

C#:   if (data == null) return;
来源：http://swh.yfazqb.com

================================================================================
来源：http://kdv.ppjwa.cn

C. 函数与作用域
来源：http://iln.uphjek.com

================================================================================
来源：http://ogb.dianchejie.cn

[C01] 定义函数
来源：http://rxb.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://eth.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uxd.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://leo.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ruy.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://aso.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://ikg.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://ood.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kqr.yfazqb.com

[C02] 默认参数
来源：http://pkz.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://liv.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hgi.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://wtd.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wwp.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://iie.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qug.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://uov.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://wyq.52xcode.cn

[C03] 可变参数
来源：http://aeo.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://swc.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uwz.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xli.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eyr.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hye.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dnt.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://waj.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dpn.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://zan.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nww.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zoz.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hfr.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wpb.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://dnl.hesvh.cn

Go:   // 无：用配置结构体参数
来源：http://fas.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://qot.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://ikv.shangyingyoupin.top

[C05] 返回多个值
来源：http://obz.jianghu66.top

Py:   return a, b
来源：http://tvg.c1oappe.top

PHP:  return [$a, $b];
来源：http://thx.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://acl.chenlongwang.top

TS:   return { a, b };
来源：http://xxf.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mab.sufxvd.cn

Go:   return a, b
来源：http://dzm.yj202588.top

Ruby: return a, b
来源：http://zno.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://yzd.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://hgk.andypj.xyz

Py:   square = lambda x: x * x
来源：http://hhp.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://mnp.guowangkeji.top

JS:   const square = x => x * x;
来源：http://cxo.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://bzo.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qlf.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://rlc.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://plw.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sxb.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://zce.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zta.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ubf.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oap.ybcxt.top

TS:   arr.map(String)
来源：http://vmv.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vwt.redwolf501.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://awk.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://jja.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wbg.shanyushiyangkeji.top

[C08] 闭包
来源：http://abb.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wio.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kbs.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qnf.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qfs.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfq.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xcu.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tmq.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uhm.tarul.cn

[C09] 递归
来源：http://jfl.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bdr.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ggi.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lwd.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njs.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rsu.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fep.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vsl.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ryu.jyoumei.cn

[C10] 变量作用域
来源：http://nxf.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jdc.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ogp.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ghu.ybcxt.top

TS:   同 JS
来源：http://sxk.sufxvd.cn

Java: 方法内为块级作用域
来源：http://xci.snrcjt.cn

Go:   花括号块级作用域
来源：http://rzk.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fhw.xuanzx.com

C#:   块级作用域
来源：http://kxt.c1oappe.top

[C11] 模块导入与导出
来源：http://lab.yj20258.top

Py:   from module import func
来源：http://wxt.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://urb.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fgl.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pgj.daxiang520.top

Java: import java.util.List;
来源：http://jfa.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lxy.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://toa.chenlongwang.top

C#:   using System.Text;
来源：http://ukh.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://fdy.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://qxa.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://tdg.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://xew.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://bda.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jyt.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://mhx.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://rpu.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kem.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://fpb.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cja.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oky.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gxj.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fmo.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://swf.smart0.xyz

Go:   func add(a, b int) int
来源：http://hog.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ygz.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://yoj.fzhhl.top

[C14] 泛型函数
来源：http://ucr.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ipa.yuanzhike.top

PHP:  // 无泛型
来源：http://hpa.bbcook.cn

JS:   // 无泛型
来源：http://kji.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bid.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tku.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://czu.yueranfly.top

Ruby: # 无泛型
来源：http://ame.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zqr.ivvv.top

[C15] 解构 / 展开参数
来源：http://aob.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vyy.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://vyh.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lvf.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://thi.shzxlz.cn

Java: // 无解构
来源：http://zzr.jyoumei.cn

Go:   // 无解构
来源：http://crz.daxiang520.top

Ruby: a, b = pair
来源：http://jcz.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://sja.daria6918.cn

[C16] 函数 / 方法重载
来源：http://jwn.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pco.sweek.top

PHP:  // 无重载
来源：http://drp.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://agy.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://zul.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sjl.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://uxd.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://ssq.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://khd.tianlin.xyz

================================================================================
来源：http://ssc.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://xai.vqdsnc.cn

================================================================================
来源：http://bdh.fzhhl.top

[D01] 创建数组 / 列表
来源：http://mys.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://icx.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qkj.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rct.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fns.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gug.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://sms.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://jte.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nms.yueranfly.top

[D02] 追加元素到末尾
来源：http://kdk.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wig.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://chl.aibaodan.cn

JS:   arr.push(4);
来源：http://dgh.yangfankeji.com

TS:   arr.push(4);
来源：http://vec.quarkkingdee.top

Java: list.add(4);
来源：http://fkz.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://uih.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://crm.cheryme.top

C#:   list.Add(4);
来源：http://ddd.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://kfh.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://mzo.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gqf.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fdb.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://vcz.zhoulong.xyz

Java: list.add(0, 0);
来源：http://myc.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yqz.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://foe.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://rly.tarul.cn

[D04] 删除元素
来源：http://kad.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fwu.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dpx.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dry.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://tvk.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ipv.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zoq.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cth.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tns.xinyue.icu

[D05] 访问与修改元素
来源：http://ahk.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://odo.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nlg.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://njh.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://cjf.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://mmq.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://asq.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hdk.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cka.feifeiyinyue.top

[D06] 数组长度
来源：http://ltj.dianchejie.cn

Py:   len(arr)
来源：http://tbw.uphjek.com

PHP:  count($arr);
来源：http://rui.yj202588.top

JS:   arr.length
来源：http://qpu.jyoumei.cn

TS:   arr.length
来源：http://btl.hywenlv.cn

Java: list.size();
来源：http://dqh.52xcode.cn

Go:   len(arr)
来源：http://zrl.yj202588.top

Ruby: arr.length; arr.size
来源：http://sfu.jqgufenzy.top

C#:   list.Count;
来源：http://ypj.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://ffd.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mjh.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://hmu.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://hxn.yj202588.top

TS:   arr.slice(1, 4);
来源：http://oiz.hesvh.cn

Java: list.subList(1, 4);
来源：http://hmx.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://krg.hcnkem.com

Ruby: arr[1, 3]
来源：http://wbu.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://yuh.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://gsw.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://dgv.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://ibt.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://gon.hammf.cn

TS:   [...a, ...b];
来源：http://vhc.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hof.ydzc1.top

Go:   append(a, b...)
来源：http://fcd.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://kfc.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://koi.shzxlz.cn

[D09] 排序（升序）
来源：http://jaw.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://tll.epnwcf.com

PHP:  sort($arr);
来源：http://xep.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gkz.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zbq.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nbu.haohaochexian.top


<!-- 参考信息 -->