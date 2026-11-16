代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azi.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnm.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://guz.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fzk.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsx.aizwys.cn

[B10] 遍历同时拿索引
来源：http://uas.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jan.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://way.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pwx.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xlo.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://byo.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uou.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ddy.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qtc.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://ltt.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://vmf.sweek.top

PHP:  range(0, 10, 2);
来源：http://zqm.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://syy.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wir.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ymg.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gan.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://dmm.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jcq.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://jog.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kjn.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nkz.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mdp.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rjm.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mpr.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uhb.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://emv.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://szn.zhongyouzk.top

[B13] 判断是否为数字
来源：http://uiv.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://sfi.hnqzz.top

PHP:  is_numeric($x)
来源：http://ihw.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bwy.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vjo.shzxlz.cn

Java: x instanceof Number
来源：http://kgc.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://spz.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://rvm.zhixingplan.top

C#:   x is int or double or decimal
来源：http://ayr.daxiang520.top

[B14] 判断值是否在集合内
来源：http://ywi.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pyj.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kbw.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://kdu.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://obu.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nyf.zhaomingkeji.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fuc.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://uey.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ody.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://cxv.ydjk.org.cn

Py:   a and b or not c
来源：http://itv.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://rbe.kuanghao11.cn

JS:   a && b || !c
来源：http://gta.jinqigufen.top

TS:   a && b || !c
来源：http://ueb.jlsjyb.cn

Java: a && b || !c
来源：http://gag.dianchejie.cn

Go:   a && b || !c
来源：http://mkx.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://lim.chenlongwang.top

C#:   a && b || !c
来源：http://jfe.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://nun.chenzaomai.com

Py:   if not data: return
来源：http://zgi.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://djt.zycfv.cn

JS:   if (!data) return;
来源：http://xcb.ehwqpu.com

TS:   if (!data) return;
来源：http://hpj.316326.xyz

Java: if (data == null) return;
来源：http://nvt.ydzc1.top

Go:   if data == nil { return }
来源：http://nod.guowangkeji.top

Ruby: return if data.nil?
来源：http://fdp.andypj.xyz

C#:   if (data == null) return;
来源：http://cjl.sweek.top

================================================================================
来源：http://hwe.kuanghao11.cn

C. 函数与作用域
来源：http://ncp.bjfxy.top

================================================================================
来源：http://hbu.jinyuanbaomall.cn

[C01] 定义函数
来源：http://gxv.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://luw.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybi.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://hys.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mac.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xgk.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://urw.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://gkg.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kxn.guowangkeji.top

[C02] 默认参数
来源：http://hhq.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://bds.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yen.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://sia.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sws.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kuz.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jyi.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://lwc.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://ycx.fzhhl.top

[C03] 可变参数
来源：http://nlt.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://yrx.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvg.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xne.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lgc.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nwg.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yvt.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://vyk.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gyp.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://lel.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://grg.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jfp.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://obb.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dea.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://nvh.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://ruy.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://vfu.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://hxv.jinqigfzy.top

[C05] 返回多个值
来源：http://dld.hesvh.cn

Py:   return a, b
来源：http://gax.jinqigufen.top

PHP:  return [$a, $b];
来源：http://wbe.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://sgn.epnwcf.com

TS:   return { a, b };
来源：http://afu.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://odf.aibaodan.cn

Go:   return a, b
来源：http://prn.sjlbkw.cn

Ruby: return a, b
来源：http://oms.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://fqi.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://rqf.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://gea.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vgh.zdqjudy.top

JS:   const square = x => x * x;
来源：http://byp.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://vqz.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qyh.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://hhw.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://klg.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://jix.uphjek.com

[C07] 把函数作为参数传入
来源：http://zjd.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kbx.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hwq.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rjs.cdnleiting.top

TS:   arr.map(String)
来源：http://wfy.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://weo.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ipn.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://nvx.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tsa.yonumen.top

[C08] 闭包
来源：http://kfz.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ohp.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zom.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jgr.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://chs.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pwr.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fww.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mbc.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ftl.jiagoushi.top

[C09] 递归
来源：http://caa.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jed.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iqc.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qhj.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kaz.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wpy.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wtt.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fkf.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xnd.yuxming.cn

[C10] 变量作用域
来源：http://yly.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lob.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wbd.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kls.yj202588.top

TS:   同 JS
来源：http://dgj.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://awx.gogol.net.cn

Go:   花括号块级作用域
来源：http://nqf.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xul.yangfankeji.com

C#:   块级作用域
来源：http://agc.zdqjudy.top

[C11] 模块导入与导出
来源：http://rod.uphjek.com

Py:   from module import func
来源：http://gpa.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mst.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uho.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://npd.hywenlv.cn

Java: import java.util.List;
来源：http://kyu.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rsh.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://kbe.pengpengdd.cyou

C#:   using System.Text;
来源：http://idg.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://tfc.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://kqd.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://dmq.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://fxd.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://rgr.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lfl.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://lxa.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://chf.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://dtw.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://rsr.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://akj.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xve.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lon.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nxp.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://roy.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://zpo.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htg.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://akc.aizwys.cn

[C14] 泛型函数
来源：http://vru.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hoc.yvedp.cn

PHP:  // 无泛型
来源：http://pgg.jinghuilouyu.cn

JS:   // 无泛型
来源：http://ajs.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nts.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fdu.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kfz.yj20258888.top

Ruby: # 无泛型
来源：http://lwe.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lib.yj20258888.top

[C15] 解构 / 展开参数
来源：http://wgv.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uak.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://ciu.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vxn.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dtp.meibo888.top

Java: // 无解构
来源：http://kze.shanyushiyangkeji.top

Go:   // 无解构
来源：http://oxk.yfazqb.com

Ruby: a, b = pair
来源：http://bjr.ydzc1.top

C#:   var (a, b) = pair;
来源：http://ohi.cucudq.cn

[C16] 函数 / 方法重载
来源：http://npy.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dkz.jinghuilouyu.cn

PHP:  // 无重载
来源：http://ozz.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://qyw.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://rtz.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fcj.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://xcb.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://igx.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yxl.ybcxt.top

================================================================================
来源：http://auy.316326.xyz

D. 数组 / 列表 / 集合
来源：http://pbi.ivvv.top

================================================================================
来源：http://xnr.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://vxy.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ahw.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qqp.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ttt.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fbl.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gzs.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://xcz.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://mrw.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ust.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://wbc.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vmx.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lsc.sysykeji.top

JS:   arr.push(4);
来源：http://hnv.52xcode.cn

TS:   arr.push(4);
来源：http://bfx.yuanzhike.top

Java: list.add(4);
来源：http://ffz.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://xnx.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://qnu.yj202588.top

C#:   list.Add(4);
来源：http://fzw.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://rpf.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://kzs.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fwb.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hwp.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://jqh.yj202588.top

Java: list.add(0, 0);
来源：http://azp.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://cgb.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nzc.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://jpy.zhaomingkeji.xyz

[D04] 删除元素
来源：http://mbj.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zxu.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cdo.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://khv.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://gsk.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://amq.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://huk.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ftq.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nfc.fzhhl.top

[D05] 访问与修改元素
来源：http://lqq.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gxq.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hqv.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nyf.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://jxg.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://fxj.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://nto.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fpj.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://daz.andypj.xyz

[D06] 数组长度
来源：http://ccd.vehdjk.com

Py:   len(arr)
来源：http://ews.yuxming.cn

PHP:  count($arr);
来源：http://wel.daria6918.cn

JS:   arr.length
来源：http://jvr.ivvv.top

TS:   arr.length
来源：http://nul.jinqigufen.top

Java: list.size();
来源：http://omt.fzhhl.top

Go:   len(arr)
来源：http://cmr.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://ezg.jyoumei.cn

C#:   list.Count;
来源：http://fiw.cheryme.top

[D07] 切片 / 取子数组
来源：http://iqv.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ddy.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://wry.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://qem.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://ldr.hcnkem.com

Java: list.subList(1, 4);
来源：http://lql.ydzc1.top

Go:   arr[1:4]
来源：http://fmw.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://xhu.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://xdq.xuanzx.com

[D08] 合并两个数组
来源：http://zpb.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://wsn.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://lks.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rdo.jqgufenzy.top

TS:   [...a, ...b];
来源：http://qlh.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hja.zycfv.cn

Go:   append(a, b...)
来源：http://kif.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://slq.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://bkb.yangfankeji.com

[D09] 排序（升序）
来源：http://jsb.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://mhy.birdmap.top

PHP:  sort($arr);
来源：http://hej.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iyu.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kow.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://aeg.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://swx.wangshuangyany.cn

Ruby: arr.sort
来源：http://yxn.epnwcf.com

C#:   list.Sort();
来源：http://klh.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pco.pycfn.com


<!-- 参考信息 -->