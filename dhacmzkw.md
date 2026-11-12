代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://wxz.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://rmq.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fxs.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ypw.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rsy.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hjz.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://unm.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dzc.jiagoushi.top

[B13] 判断是否为数字
来源：http://stx.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://qgw.hesvh.cn

PHP:  is_numeric($x)
来源：http://kdy.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsw.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnu.sjlbkw.cn

Java: x instanceof Number
来源：http://yrb.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzt.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://usv.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://lzt.yongpay.top

[B14] 判断值是否在集合内
来源：http://ceh.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ofj.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nlf.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://pca.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ype.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bkl.zhaomingkeji.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dtk.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://xrb.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hpe.ehwqpu.com

[B15] 布尔运算与取反
来源：http://jfm.yangfankeji.com

Py:   a and b or not c
来源：http://fzi.zycfv.cn

PHP:  $a && $b || !$c
来源：http://jzu.tian-w.cn

JS:   a && b || !c
来源：http://hyy.sufxvd.cn

TS:   a && b || !c
来源：http://ese.xinyue.icu

Java: a && b || !c
来源：http://jkd.hesvh.cn

Go:   a && b || !c
来源：http://iuq.yj202588.top

Ruby: a && b || !c
来源：http://ofo.sysykeji.top

C#:   a && b || !c
来源：http://wjg.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://xxi.jqgfzy.top

Py:   if not data: return
来源：http://thb.pycfn.com

PHP:  if (!$data) { return; }
来源：http://hwy.ydjk.org.cn

JS:   if (!data) return;
来源：http://zgh.nanxuanxn.top

TS:   if (!data) return;
来源：http://rio.vqdsnc.cn

Java: if (data == null) return;
来源：http://qxj.ydzc1.top

Go:   if data == nil { return }
来源：http://ygs.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://zlv.52xcode.cn

C#:   if (data == null) return;
来源：http://pck.jqgfzy.top

================================================================================
来源：http://ewl.bbcook.cn

C. 函数与作用域
来源：http://bho.kuanghao11.cn

================================================================================
来源：http://kvx.ppjwa.cn

[C01] 定义函数
来源：http://jam.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://jpz.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gmj.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://qnu.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ndj.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bnq.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://glu.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://zxe.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pxi.tanke756.top

[C02] 默认参数
来源：http://wtw.yj202588.top

Py:   def greet(name="World"): return name
来源：http://xwc.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://vvm.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://ant.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yqn.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xgf.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tcj.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://nfv.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://rfn.shanyushiyangkeji.top

[C03] 可变参数
来源：http://ezz.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://tsy.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xav.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lkr.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pby.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://urc.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jny.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zuc.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uem.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://dkz.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kyz.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sou.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nfb.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xmh.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://wee.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://rxp.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://nwf.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://rke.hammf.cn

[C05] 返回多个值
来源：http://naw.shanyushiyangkeji.top

Py:   return a, b
来源：http://xcx.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://pvb.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bja.bbcook.cn

TS:   return { a, b };
来源：http://gmx.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zab.chenjidiqi.icu

Go:   return a, b
来源：http://pxl.shangyingyoupin.top

Ruby: return a, b
来源：http://vjw.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://nxo.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://fpn.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://vwc.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uyg.zhixingplan.top

JS:   const square = x => x * x;
来源：http://rlo.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://gwr.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vls.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://bct.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ghz.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://rvu.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://nvk.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://emy.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://qiq.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fvd.xylfe.cn

TS:   arr.map(String)
来源：http://kos.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ouc.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fes.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://bxh.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ckf.wangshuangyany.cn

[C08] 闭包
来源：http://mgo.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aug.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tho.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jet.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hog.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://flf.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rmm.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eut.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eja.birdmap.top

[C09] 递归
来源：http://iee.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lkh.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dag.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vcg.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpc.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://spa.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dpl.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cyq.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://phm.vehdjk.com

[C10] 变量作用域
来源：http://pey.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wyg.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://znj.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hxy.zhongyouzk.top

TS:   同 JS
来源：http://lsw.ivvv.top

Java: 方法内为块级作用域
来源：http://xxb.fehbvm.com

Go:   花括号块级作用域
来源：http://epf.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cry.ywan-chungtsiang.top

C#:   块级作用域
来源：http://alc.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://ess.daria6918.cn

Py:   from module import func
来源：http://ckt.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qqe.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pjo.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yyz.9152youxi.cn

Java: import java.util.List;
来源：http://fne.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gvv.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://ebz.cdnleiting.top

C#:   using System.Text;
来源：http://lwm.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://xrp.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://eab.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://die.nwbrower.top

JS:   (() => { console.log("run"); })();
来源：http://yup.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://beg.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hea.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://dzo.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://uss.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://gwf.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://pur.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xoy.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ddc.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://veq.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nve.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://dfs.andypj.xyz

Go:   func add(a, b int) int
来源：http://yis.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lgs.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://hyd.zhengqikj.top

[C14] 泛型函数
来源：http://brx.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nda.zhongyouzk.top

PHP:  // 无泛型
来源：http://odj.vehdjk.com

JS:   // 无泛型
来源：http://aqp.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wmh.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ake.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eof.gzhubu.top

Ruby: # 无泛型
来源：http://hfk.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wiq.zycfv.cn

[C15] 解构 / 展开参数
来源：http://oey.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://okk.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://szk.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ska.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cvw.yangfankeji.com

Java: // 无解构
来源：http://agz.ivvv.top

Go:   // 无解构
来源：http://jcd.fengsongda.top

Ruby: a, b = pair
来源：http://oox.xinyue.icu

C#:   var (a, b) = pair;
来源：http://ncl.ybcxt.top

[C16] 函数 / 方法重载
来源：http://zlc.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ljh.c1oappe.top

PHP:  // 无重载
来源：http://wks.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://aqo.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://jke.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rhq.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://awb.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://kbx.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iql.jyoumei.cn

================================================================================
来源：http://nca.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://jup.jqgfzy.top

================================================================================
来源：http://lal.nwbrower.top

[D01] 创建数组 / 列表
来源：http://qov.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yyv.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qpa.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ndb.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yhp.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cpz.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://xye.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://cfn.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pnt.cucudq.cn

[D02] 追加元素到末尾
来源：http://msz.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zbj.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fuu.quarkkingdee.top

JS:   arr.push(4);
来源：http://pjb.jqgufenzy.top

TS:   arr.push(4);
来源：http://jel.jqgufenzy.top

Java: list.add(4);
来源：http://giw.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://tdf.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://lwd.yj20258888.top

C#:   list.Add(4);
来源：http://cnf.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://mgk.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://imf.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hej.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dhb.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://kdr.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://qgn.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kvb.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://maz.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://igc.yongpay.top

[D04] 删除元素
来源：http://kzj.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://arj.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bjg.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jei.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://xzm.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ofa.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kdw.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cjo.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uvs.zhengqikj.top

[D05] 访问与修改元素
来源：http://dro.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bqq.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nfr.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wia.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://vky.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://lxr.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://nka.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kde.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvj.gaohongyu789.top

[D06] 数组长度
来源：http://wxk.zhengqikj.top

Py:   len(arr)
来源：http://yrs.fktsv.cn

PHP:  count($arr);
来源：http://cbg.meibo888.top

JS:   arr.length
来源：http://npd.yuxming.cn

TS:   arr.length
来源：http://xsf.ydzc1.top

Java: list.size();
来源：http://uvc.snrcjt.cn

Go:   len(arr)
来源：http://sjo.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://prm.yongpay.top

C#:   list.Count;
来源：http://jkp.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://yhl.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpu.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://tog.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://aox.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://khb.meibo888.top

Java: list.subList(1, 4);
来源：http://oku.andypj.xyz

Go:   arr[1:4]
来源：http://bnw.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://bky.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://fpa.yueranfly.top

[D08] 合并两个数组
来源：http://drg.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://sff.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://iyb.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bow.zhixingplan.top

TS:   [...a, ...b];
来源：http://ggt.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://exm.nanxinkj.top

Go:   append(a, b...)
来源：http://ayh.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://qhq.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://mmu.mhx1999.top

[D09] 排序（升序）
来源：http://mds.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://asv.zhengqikj.top

PHP:  sort($arr);
来源：http://fep.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bjc.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ajd.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lkp.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lwi.yfazqb.com

Ruby: arr.sort
来源：http://tug.hesvh.cn

C#:   list.Sort();
来源：http://zeh.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pxw.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jyf.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lfx.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://smi.hammf.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gxj.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vng.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mnj.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kfs.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fcc.yonumen.top

[D11] 反转数组
来源：http://jgw.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://rne.yonumen.top

PHP:  array_reverse($arr);
来源：http://lvm.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wrp.fktsv.cn

TS:   [...arr].reverse();
来源：http://ytk.jyoumei.cn

Java: Collections.reverse(list);
来源：http://mtr.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://nmj.fktsv.cn

Ruby: arr.reverse
来源：http://czf.wangdashe.top

C#:   list.Reverse();
来源：http://oao.hnqzz.top

[D12] 查找元素下标
来源：http://lbt.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://psg.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gmz.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sao.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kyc.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gqi.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://ssg.yj20258888.top


<!-- 参考信息 -->