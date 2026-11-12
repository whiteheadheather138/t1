代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zga.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zei.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xgk.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ela.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vln.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://yjf.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ngt.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yrb.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wcj.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ffc.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://evy.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pew.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ddz.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dod.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://kmw.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://aie.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://wuu.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://muu.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tse.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sto.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nnr.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://jim.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ujz.xylfe.cn

[B12] 跳出多层循环
来源：http://ujr.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ebl.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zms.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nrj.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ifv.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ltp.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fpt.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://djy.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lua.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://vof.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://vfx.cdnleiting.top

PHP:  is_numeric($x)
来源：http://knl.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jly.jqgfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yst.gaohongyu789.top

Java: x instanceof Number
来源：http://oav.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ada.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://uts.haohaochexian.top

C#:   x is int or double or decimal
来源：http://gfl.316326.xyz

[B14] 判断值是否在集合内
来源：http://czs.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mks.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ajj.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://nlt.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://qzz.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cfg.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vew.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://mme.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hmz.fzhhl.top

[B15] 布尔运算与取反
来源：http://jmx.dashuyun.cn

Py:   a and b or not c
来源：http://qxs.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://xod.sjlbkw.cn

JS:   a && b || !c
来源：http://cda.uphjek.com

TS:   a && b || !c
来源：http://qce.0kj1m.cn

Java: a && b || !c
来源：http://nss.yj20258.top

Go:   a && b || !c
来源：http://xxx.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://icq.pengpengdd.cyou

C#:   a && b || !c
来源：http://zha.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://ula.bbcook.cn

Py:   if not data: return
来源：http://rtf.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://wwq.fzhhl.top

JS:   if (!data) return;
来源：http://ruq.vehdjk.com

TS:   if (!data) return;
来源：http://zlh.yvedp.cn

Java: if (data == null) return;
来源：http://zvm.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://duw.dashuyun.cn

Ruby: return if data.nil?
来源：http://xco.yongpay.top

C#:   if (data == null) return;
来源：http://mmf.tianlin.xyz

================================================================================
来源：http://kji.hysaishi.cn

C. 函数与作用域
来源：http://ila.nwbrower.top

================================================================================
来源：http://zng.shzxlz.cn

[C01] 定义函数
来源：http://fiq.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://yly.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fdo.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://ojl.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvj.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wda.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://wfl.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://jax.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kav.ywan-chungtsiang.top

[C02] 默认参数
来源：http://vhr.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://lfg.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tbb.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://csd.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://llk.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://smu.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ezg.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://cva.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://uib.dashuyun.cn

[C03] 可变参数
来源：http://fot.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://lqr.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://osu.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bwh.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gni.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rtn.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://boc.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fns.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qwk.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://ily.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://luc.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://phi.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://buf.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gqu.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://pqh.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://vyr.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://cov.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://pev.nwbrower.top

[C05] 返回多个值
来源：http://gty.hnqzz.top

Py:   return a, b
来源：http://stq.jqgfzy.top

PHP:  return [$a, $b];
来源：http://fgi.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oqi.ivvv.top

TS:   return { a, b };
来源：http://ift.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lry.jinghuilouyu.cn

Go:   return a, b
来源：http://hkj.havefunace.top

Ruby: return a, b
来源：http://oyy.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://mxk.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://cpq.yj202588.top

Py:   square = lambda x: x * x
来源：http://vxv.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kxe.epnwcf.com

JS:   const square = x => x * x;
来源：http://ilw.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://ctt.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://utv.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://yxz.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://sgv.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://tzs.wangdashe.top

[C07] 把函数作为参数传入
来源：http://kpp.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gdr.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://fco.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xxa.tian-w.cn

TS:   arr.map(String)
来源：http://npr.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ydx.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sxs.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://dfa.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pom.c1oappe.top

[C08] 闭包
来源：http://flv.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ssh.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shu.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ajp.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://caa.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ado.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://egb.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wlz.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aks.0kj1m.cn

[C09] 递归
来源：http://voq.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hug.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pkz.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tte.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bac.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eei.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rjb.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kdm.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tvk.cqqwz.cn

[C10] 变量作用域
来源：http://kdd.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wym.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mdy.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tsp.quarkkingdee.top

TS:   同 JS
来源：http://phm.xylfe.cn

Java: 方法内为块级作用域
来源：http://qpc.bbcook.cn

Go:   花括号块级作用域
来源：http://wrg.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nnb.ppjwa.cn

C#:   块级作用域
来源：http://kiz.tianlin.xyz

[C11] 模块导入与导出
来源：http://fgv.0kj1m.cn

Py:   from module import func
来源：http://uda.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://swc.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qdo.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bmg.havefunace.top

Java: import java.util.List;
来源：http://yvj.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ibq.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://jek.havefunace.top

C#:   using System.Text;
来源：http://erd.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://bbt.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://xkp.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://qhr.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://bmr.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://vbw.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pts.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://jkb.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://tvu.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://yxg.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://zin.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uyl.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dcr.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xed.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hum.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mbq.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://lgb.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iyv.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://rdn.shzxlz.cn

[C14] 泛型函数
来源：http://ygp.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hew.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://uza.52xcode.cn

JS:   // 无泛型
来源：http://wga.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hzy.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qax.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rer.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://bjj.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wqb.shuidangran.top

[C15] 解构 / 展开参数
来源：http://wxn.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gey.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://oir.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tjd.zhiwuduotai.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cgn.jyoumei.cn

Java: // 无解构
来源：http://xtz.tian-w.cn

Go:   // 无解构
来源：http://nxe.shuidangran.top

Ruby: a, b = pair
来源：http://xpn.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://gte.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://hmu.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wkm.gotoacloud.top

PHP:  // 无重载
来源：http://uxh.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eco.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://kmr.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://emb.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://few.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://kgg.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://fha.yj202588.top

================================================================================
来源：http://sue.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://scl.sufxvd.cn

================================================================================
来源：http://wfx.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://xzy.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rrl.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eko.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lxm.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dvr.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hko.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://xdh.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://zev.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yhm.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://wfx.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bqn.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pom.xuetiantiany.cn

JS:   arr.push(4);
来源：http://ymf.fktsv.cn

TS:   arr.push(4);
来源：http://fjt.vehdjk.com

Java: list.add(4);
来源：http://ehy.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://yfg.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://ieh.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://joq.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://jqs.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://yxg.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://llk.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dwm.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://kzc.aibaodan.cn

Java: list.add(0, 0);
来源：http://yly.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://aph.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bqw.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://lkk.bjfxy.top

[D04] 删除元素
来源：http://tsa.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mfr.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jxd.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ueu.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://snc.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ysk.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ebw.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cwy.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kqz.cdnleiting.top

[D05] 访问与修改元素
来源：http://fjh.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vle.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dwu.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mhv.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://xat.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://kit.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://sxn.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dft.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wgc.aizwys.cn

[D06] 数组长度
来源：http://cwu.gzhubu.top

Py:   len(arr)
来源：http://lwz.zdbjq.cn

PHP:  count($arr);
来源：http://vpn.kuanghao11.cn

JS:   arr.length
来源：http://onv.fehbvm.com

TS:   arr.length
来源：http://yfz.yangfankeji.com

Java: list.size();
来源：http://ivv.fzhhl.top

Go:   len(arr)
来源：http://xve.tanke756.top

Ruby: arr.length; arr.size
来源：http://ere.yj202588.top

C#:   list.Count;
来源：http://nvo.fehbvm.com

[D07] 切片 / 取子数组
来源：http://rsm.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oht.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cgg.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://llf.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://nbp.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://zhg.chenjidiqi.icu

Go:   arr[1:4]
来源：http://ffa.wangdashe.top

Ruby: arr[1, 3]
来源：http://bwn.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://kpb.fktsv.cn

[D08] 合并两个数组
来源：http://hky.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://bjd.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://zqt.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nws.haohaochexian.top

TS:   [...a, ...b];
来源：http://psw.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eve.gotoacloud.top

Go:   append(a, b...)
来源：http://qol.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://lhp.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://lrf.mhx1999.top

[D09] 排序（升序）
来源：http://jys.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://afb.tanke756.top

PHP:  sort($arr);
来源：http://epg.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ovm.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfy.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zta.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gsw.hcnkem.com

Ruby: arr.sort
来源：http://csm.sxryk.cn

C#:   list.Sort();
来源：http://fhq.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ymh.gogol.net.cn


<!-- 参考信息 -->