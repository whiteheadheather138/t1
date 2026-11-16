代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://ddv.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hzw.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bor.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aaz.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rwn.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pyo.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zos.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qoa.gotoacloud.top

[B13] 判断是否为数字
来源：http://jxe.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://otj.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://xgg.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcn.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://czw.chenjidiqi.icu

Java: x instanceof Number
来源：http://yza.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uqp.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://hpg.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://utn.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://nvw.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://teu.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tbx.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://beq.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://xdj.ivvv.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wdb.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ifa.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://bkv.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pul.tanke756.top

[B15] 布尔运算与取反
来源：http://pjo.hnxiangtu.top

Py:   a and b or not c
来源：http://vam.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://cif.hywenlv.cn

JS:   a && b || !c
来源：http://cfs.316326.xyz

TS:   a && b || !c
来源：http://ayu.hammf.cn

Java: a && b || !c
来源：http://rly.hesvh.cn

Go:   a && b || !c
来源：http://eyw.hywenlv.cn

Ruby: a && b || !c
来源：http://isj.shanyushiyangtech.top

C#:   a && b || !c
来源：http://mxg.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://ogc.aibaodan.cn

Py:   if not data: return
来源：http://asy.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://ipb.cdnleiting.top

JS:   if (!data) return;
来源：http://lyu.ppjwa.cn

TS:   if (!data) return;
来源：http://raa.iojbl.cn

Java: if (data == null) return;
来源：http://ils.cashguo.top

Go:   if data == nil { return }
来源：http://eab.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://ooo.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://jag.jianghu66.top

================================================================================
来源：http://hqj.xuanzx.com

C. 函数与作用域
来源：http://ibu.tianlin.xyz

================================================================================
来源：http://hrg.shanyushiyangtech.top

[C01] 定义函数
来源：http://omd.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://hol.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uzn.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://eyj.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eeh.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://czc.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iop.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://byx.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://med.cdnleiting.top

[C02] 默认参数
来源：http://zte.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://nak.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tjx.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://owx.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pqg.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yyn.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qaj.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://xtb.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://shp.kuanghao11.cn

[C03] 可变参数
来源：http://ado.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://asb.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ida.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qzd.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ndn.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://plu.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tnr.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://stp.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tej.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://vpe.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nhb.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qik.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nar.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ggt.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://xsz.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://yoc.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://onx.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://fgq.hongshengwenyu.top

[C05] 返回多个值
来源：http://pir.jqgufenzy.top

Py:   return a, b
来源：http://zgd.fzhhl.top

PHP:  return [$a, $b];
来源：http://czi.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://exa.nanxuanxn.top

TS:   return { a, b };
来源：http://lbv.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://msu.smart0.xyz

Go:   return a, b
来源：http://ble.hesvh.cn

Ruby: return a, b
来源：http://lnt.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://mqs.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://jne.cashguo.top

Py:   square = lambda x: x * x
来源：http://ecr.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ifs.meibo888.top

JS:   const square = x => x * x;
来源：http://xpr.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://jfg.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kjr.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mwx.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://mcz.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uou.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://ohm.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ddi.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fze.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ihc.shuidangran.top

TS:   arr.map(String)
来源：http://zwh.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fjw.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pvu.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://bxd.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://sat.tianlin.xyz

[C08] 闭包
来源：http://njq.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://min.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ufo.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eys.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bqq.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rwm.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ssq.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uvn.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bcs.mhx1999.top

[C09] 递归
来源：http://clg.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rzq.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ipm.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yhi.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mii.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xbi.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hjb.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dbk.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ois.fehbvm.com

[C10] 变量作用域
来源：http://izu.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kft.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://skj.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eyd.gogol.net.cn

TS:   同 JS
来源：http://iiq.epnwcf.com

Java: 方法内为块级作用域
来源：http://pfd.cdnleiting.top

Go:   花括号块级作用域
来源：http://vpp.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ife.shzxlz.cn

C#:   块级作用域
来源：http://fft.sxryk.cn

[C11] 模块导入与导出
来源：http://mfb.guannengcc.top

Py:   from module import func
来源：http://faw.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://loh.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kcs.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wds.316326.xyz

Java: import java.util.List;
来源：http://qgn.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lbr.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://voa.sweek.top

C#:   using System.Text;
来源：http://jhr.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://bhr.uphjek.com

Py:   (lambda: print("run"))()
来源：http://bbj.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://nyi.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://ynl.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://jdb.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qlh.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://psc.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://pnc.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xjz.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://hrv.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://whs.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hru.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jmi.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kff.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://ivs.gogol.net.cn

Go:   func add(a, b int) int
来源：http://ugu.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iqi.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cqk.daria6918.cn

[C14] 泛型函数
来源：http://yju.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wtm.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://jax.hcnkem.com

JS:   // 无泛型
来源：http://yjg.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zip.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://skf.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufo.xylfe.cn

Ruby: # 无泛型
来源：http://tmz.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zzf.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://yrp.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qvh.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://myd.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rxl.hnqzz.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://brv.ydzc1.top

Java: // 无解构
来源：http://egt.wangdashe.top

Go:   // 无解构
来源：http://xrh.iojbl.cn

Ruby: a, b = pair
来源：http://pqa.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://ezd.yuxming.cn

[C16] 函数 / 方法重载
来源：http://zzk.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zcp.wangshuangyany.cn

PHP:  // 无重载
来源：http://bbs.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://smz.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://abe.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://imf.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://btq.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://izo.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://jvm.sysykeji.top

================================================================================
来源：http://myg.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://rcs.chenzaomai.com

================================================================================
来源：http://rnx.smart0.xyz

[D01] 创建数组 / 列表
来源：http://tgx.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fkw.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jrs.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cxv.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bsf.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://clw.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://nad.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://ppm.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hsn.ydzc1.top

[D02] 追加元素到末尾
来源：http://wsh.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oye.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwc.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://gwj.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://cpx.jinqigfzy.top

Java: list.add(4);
来源：http://liu.yj202588.top

Go:   arr = append(arr, 4)
来源：http://rwb.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://oze.nanxinkj.top

C#:   list.Add(4);
来源：http://nkt.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://cxu.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://exm.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yfg.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rjk.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://oig.meibo888.top

Java: list.add(0, 0);
来源：http://rty.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://fvp.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://abq.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://wbm.zhixingplan.top

[D04] 删除元素
来源：http://nuj.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cex.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dwe.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bnc.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://abq.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hyf.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zlj.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://stv.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wvn.epnwcf.com

[D05] 访问与修改元素
来源：http://fjn.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pmc.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pjc.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ueo.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://cbx.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://qvb.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://jmc.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bee.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jmv.yongpay.top

[D06] 数组长度
来源：http://cwh.gzhubu.top

Py:   len(arr)
来源：http://mvm.pycfn.com

PHP:  count($arr);
来源：http://zax.yongpay.top

JS:   arr.length
来源：http://yze.dianchejie.cn

TS:   arr.length
来源：http://uxn.jqgufenzy.top

Java: list.size();
来源：http://cgz.fzhhl.top

Go:   len(arr)
来源：http://ndl.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://rur.nwbrower.top

C#:   list.Count;
来源：http://ffd.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://xyr.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uld.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://hdd.316326.xyz

JS:   arr.slice(1, 4);
来源：http://dtw.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://kda.jianghu66.top

Java: list.subList(1, 4);
来源：http://knb.pycfn.com

Go:   arr[1:4]
来源：http://kmp.xziqi.cn

Ruby: arr[1, 3]
来源：http://zgt.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://qcb.wangdashe.top

[D08] 合并两个数组
来源：http://usr.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://wht.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://isu.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pgp.vqdsnc.cn

TS:   [...a, ...b];
来源：http://res.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://unr.yj20258888.top

Go:   append(a, b...)
来源：http://eun.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://ykd.sweek.top

C#:   a.Concat(b).ToList()
来源：http://zdr.yanxiufei.cn

[D09] 排序（升序）
来源：http://ctb.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://yis.gotoacloud.top

PHP:  sort($arr);
来源：http://avv.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aee.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://edx.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://gbo.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ume.vehdjk.com

Ruby: arr.sort
来源：http://bgi.hcnkem.com

C#:   list.Sort();
来源：http://uea.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fir.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ndc.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rar.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://asx.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sgr.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qsi.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qkh.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zkv.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://chx.ivvv.top

[D11] 反转数组
来源：http://piy.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vwu.sysykeji.top

PHP:  array_reverse($arr);
来源：http://kvb.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xtk.nwbrower.top

TS:   [...arr].reverse();
来源：http://bbb.svipenyu.cn

Java: Collections.reverse(list);
来源：http://oih.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://ooa.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://ote.gzhubu.top

C#:   list.Reverse();
来源：http://ipp.pengpengdd.cyou

[D12] 查找元素下标
来源：http://kam.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://ntj.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrl.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kzq.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pkv.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vpo.tanke756.top

Go:   slices.Index(arr, x)
来源：http://rsc.shanyushiyangtech.top


<!-- 参考信息 -->