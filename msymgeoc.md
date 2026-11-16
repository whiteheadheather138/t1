代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thb.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymg.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qsd.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ziq.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmp.sxryk.cn

[B10] 遍历同时拿索引
来源：http://zsd.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kth.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mzf.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xrl.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xly.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gjy.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sqk.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rsp.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bcq.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://owh.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://cdg.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://glz.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nqn.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogc.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iss.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tnu.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://rqx.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ocz.yanxiufei.cn

[B12] 跳出多层循环
来源：http://yrl.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uln.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zzc.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dnl.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tkg.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://krv.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://igj.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kao.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vjm.cucudq.cn

[B13] 判断是否为数字
来源：http://lhm.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://jdd.sweek.top

PHP:  is_numeric($x)
来源：http://wfc.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sny.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nym.shuidangran.top

Java: x instanceof Number
来源：http://hpz.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lqa.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://wqn.tanke756.top

C#:   x is int or double or decimal
来源：http://kid.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://jhf.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://odb.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wzj.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://bkk.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://qjh.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://izy.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bdm.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://ysi.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dxr.fengsongda.top

[B15] 布尔运算与取反
来源：http://qye.xuetiantiany.cn

Py:   a and b or not c
来源：http://bza.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://mvs.shangyingyoupin.top

JS:   a && b || !c
来源：http://cio.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://sie.vehdjk.com

Java: a && b || !c
来源：http://pxq.zhiwuduotai.top

Go:   a && b || !c
来源：http://wfx.cheryme.top

Ruby: a && b || !c
来源：http://quo.shangyingyoupin.top

C#:   a && b || !c
来源：http://rch.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://itd.yangfankeji.com

Py:   if not data: return
来源：http://ymc.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://ifi.hfpthk.cn

JS:   if (!data) return;
来源：http://tym.chenlongwang.top

TS:   if (!data) return;
来源：http://idb.zhixingplan.top

Java: if (data == null) return;
来源：http://zmu.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://fva.xylfe.cn

Ruby: return if data.nil?
来源：http://fhd.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://svi.xylfe.cn

================================================================================
来源：http://shp.sjlbkw.cn

C. 函数与作用域
来源：http://grl.havefunace.top

================================================================================
来源：http://gsq.quarkkingdee.top

[C01] 定义函数
来源：http://npz.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://iui.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://saw.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://lox.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abo.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://gdz.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://vwe.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://hvo.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vkr.dashuyun.cn

[C02] 默认参数
来源：http://hcl.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://drq.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kuy.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://ewa.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pmc.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://emp.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rtw.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://rvh.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://ufm.guowangkeji.top

[C03] 可变参数
来源：http://ryf.kuanghao11.cn

Py:   def total(*args): return sum(args)
来源：http://ghm.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tul.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rbl.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxz.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bxg.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jms.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://xzp.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ryc.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://uyk.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ygg.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://swi.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://glx.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ido.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://qfd.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://sep.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://kta.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://wcd.yanxiufei.cn

[C05] 返回多个值
来源：http://ggm.fehbvm.com

Py:   return a, b
来源：http://cmk.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://fno.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://tmt.ydzc1.top

TS:   return { a, b };
来源：http://rjt.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jqn.zhengqikj.top

Go:   return a, b
来源：http://vyu.zdqjudy.top

Ruby: return a, b
来源：http://knu.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://qwh.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://iqp.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://gpl.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qsy.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://apc.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://tpy.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qaj.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fyz.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://mgk.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gry.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://jxz.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lcl.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ltd.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jxe.xuetiantiany.cn

TS:   arr.map(String)
来源：http://rgx.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gxx.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hyv.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://sbj.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zbr.shzxlz.cn

[C08] 闭包
来源：http://nyt.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ybq.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lbv.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wza.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uej.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vkg.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ijn.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ddi.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jnp.quarkkingdee.top

[C09] 递归
来源：http://lcs.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gjk.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mkb.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fsw.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lim.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://auh.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wxl.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nce.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uyh.yuxming.cn

[C10] 变量作用域
来源：http://ggb.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vfv.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aew.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cqk.jinqigfzy.top

TS:   同 JS
来源：http://hic.shzxlz.cn

Java: 方法内为块级作用域
来源：http://pcx.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://chx.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yzi.gzhubu.top

C#:   块级作用域
来源：http://lje.yfazqb.com

[C11] 模块导入与导出
来源：http://hpa.sjlbkw.cn

Py:   from module import func
来源：http://xzz.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wsk.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xmi.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ynm.gzhubu.top

Java: import java.util.List;
来源：http://fby.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://woe.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://hab.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://xgf.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://hud.cashguo.top

Py:   (lambda: print("run"))()
来源：http://bwp.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://mqv.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://rbo.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://juh.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qhg.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://kwk.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://rzw.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://boh.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://dcu.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aee.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eri.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bth.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://axb.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://pbl.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://joa.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ehd.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mno.chenzaomai.com

[C14] 泛型函数
来源：http://dim.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wzx.hammf.cn

PHP:  // 无泛型
来源：http://ydx.zhixingplan.top

JS:   // 无泛型
来源：http://ljw.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ulg.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bon.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tsb.chenzaomai.com

Ruby: # 无泛型
来源：http://hkl.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fhz.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://aty.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tln.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://asl.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qoz.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gsj.52xcode.cn

Java: // 无解构
来源：http://tbw.fengsongda.top

Go:   // 无解构
来源：http://lke.nwbrower.top

Ruby: a, b = pair
来源：http://piz.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://ybx.ivvv.top

[C16] 函数 / 方法重载
来源：http://wtp.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mgk.chenzaomai.com

PHP:  // 无重载
来源：http://wfw.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bgs.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://htp.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gzy.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://iyl.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://icf.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oxg.daxiang520.top

================================================================================
来源：http://qig.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://pba.shanyushiyangtech.top

================================================================================
来源：http://vfi.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://ixs.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kmt.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rbg.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rro.0kj1m.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://acs.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mwk.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://rln.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://kmy.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hjm.hcnkem.com

[D02] 追加元素到末尾
来源：http://kni.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ifr.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://env.gzhubu.top

JS:   arr.push(4);
来源：http://jul.aizwys.cn

TS:   arr.push(4);
来源：http://xet.shzxlz.cn

Java: list.add(4);
来源：http://ouu.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://fvb.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://hjs.zycfv.cn

C#:   list.Add(4);
来源：http://ljm.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://rsc.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://ita.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jmv.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aka.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://qhn.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://lml.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ain.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ktq.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://rud.yonumen.top

[D04] 删除元素
来源：http://ety.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gvv.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jtc.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ljv.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://fue.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fsl.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nwg.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nls.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://quo.zhixingplan.top

[D05] 访问与修改元素
来源：http://hmx.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://txz.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rnf.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qhq.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://lxv.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://vfo.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wek.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xtt.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mnw.daria6918.cn

[D06] 数组长度
来源：http://llc.bbcook.cn

Py:   len(arr)
来源：http://qun.shuidangran.top

PHP:  count($arr);
来源：http://peh.hfpthk.cn

JS:   arr.length
来源：http://hla.jqgfzy.top

TS:   arr.length
来源：http://zaz.nanxuanxn.top

Java: list.size();
来源：http://fff.redwolf501.top

Go:   len(arr)
来源：http://rii.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://ymg.gaohongyu789.top

C#:   list.Count;
来源：http://wfn.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://dip.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hca.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://ghu.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://xly.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://kbq.hysaishi.cn

Java: list.subList(1, 4);
来源：http://cwi.pycfn.com

Go:   arr[1:4]
来源：http://las.hysaishi.cn

Ruby: arr[1, 3]
来源：http://fll.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://iln.wangshuangyany.cn

[D08] 合并两个数组
来源：http://egi.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://sis.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://eor.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rph.zhongyouzk.top

TS:   [...a, ...b];
来源：http://axb.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aiy.iojbl.cn

Go:   append(a, b...)
来源：http://duu.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://wum.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://tpg.guowangkeji.top

[D09] 排序（升序）
来源：http://vlw.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://pwk.fehbvm.com

PHP:  sort($arr);
来源：http://ctw.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ruj.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rgs.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vkg.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gsf.hnxiangtu.top

Ruby: arr.sort
来源：http://ase.ydjk.org.cn

C#:   list.Sort();
来源：http://xzf.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://lhj.quarkkingdee.top


<!-- 参考信息 -->