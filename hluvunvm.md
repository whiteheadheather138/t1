代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lfc.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tzy.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jpm.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rig.vehdjk.com

[B13] 判断是否为数字
来源：http://hus.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://cyx.gotoacloud.top

PHP:  is_numeric($x)
来源：http://bkn.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://grw.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://miu.ydjk.org.cn

Java: x instanceof Number
来源：http://vxd.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cob.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://hhq.epnwcf.com

C#:   x is int or double or decimal
来源：http://sym.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://hfk.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fsq.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mqu.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://quy.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://ruc.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mly.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sbx.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://kmt.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wsd.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://cfj.pycfn.com

Py:   a and b or not c
来源：http://qoy.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://ykh.guannengcc.top

JS:   a && b || !c
来源：http://wjk.ydjk.org.cn

TS:   a && b || !c
来源：http://vbk.hnqzz.top

Java: a && b || !c
来源：http://fem.xziqi.cn

Go:   a && b || !c
来源：http://yfa.hesvh.cn

Ruby: a && b || !c
来源：http://rka.jinghuilouyu.cn

C#:   a && b || !c
来源：http://oad.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mmg.gogol.net.cn

Py:   if not data: return
来源：http://ecw.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://wkt.zhixingplan.top

JS:   if (!data) return;
来源：http://lcb.ehwqpu.com

TS:   if (!data) return;
来源：http://jfa.meibo888.top

Java: if (data == null) return;
来源：http://nfx.xziqi.cn

Go:   if data == nil { return }
来源：http://fal.jqgfzy.top

Ruby: return if data.nil?
来源：http://stc.yj20258.top

C#:   if (data == null) return;
来源：http://dyh.wangshuangyany.cn

================================================================================
来源：http://zqv.ppjwa.cn

C. 函数与作用域
来源：http://kuv.pengpengdd.cyou

================================================================================
来源：http://bjv.ydzc1.top

[C01] 定义函数
来源：http://qpk.uphjek.com

Py:   def add(a, b): return a + b
来源：http://gta.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qnw.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://lpy.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mts.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jno.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jwe.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://tyf.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://luv.hywenlv.cn

[C02] 默认参数
来源：http://mig.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://pmj.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jdw.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dmi.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gls.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yfm.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://llt.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://wye.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://iqi.tian-w.cn

[C03] 可变参数
来源：http://rat.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://hob.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://arv.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fhr.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://urb.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bou.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wej.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://prb.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eqx.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://xwv.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://szm.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsi.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pdg.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fqd.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://zlo.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://ifu.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://cge.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://ufx.nwbrower.top

[C05] 返回多个值
来源：http://alo.zhoulong.xyz

Py:   return a, b
来源：http://vlc.yueranfly.top

PHP:  return [$a, $b];
来源：http://lrz.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kla.yongpay.top

TS:   return { a, b };
来源：http://jfa.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cin.pycfn.com

Go:   return a, b
来源：http://ulr.jiagoushi.top

Ruby: return a, b
来源：http://spk.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://cpu.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://yjx.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://jjz.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uep.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://nxr.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://dvn.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qxr.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://bsg.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://nuk.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://fac.tanke756.top

[C07] 把函数作为参数传入
来源：http://gmn.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://snx.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tcx.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xpf.chenzaomai.com

TS:   arr.map(String)
来源：http://gig.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://czs.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nkn.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://qjr.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pyw.zdqjudy.top

[C08] 闭包
来源：http://wre.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pej.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ewt.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jbv.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://frv.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qdv.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scv.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://idk.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ctn.nwbrower.top

[C09] 递归
来源：http://jmf.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dot.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cxs.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fkn.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cal.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lhz.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tmm.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iuj.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vhp.yj20258888.top

[C10] 变量作用域
来源：http://rmp.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iyz.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://juw.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fji.iojbl.cn

TS:   同 JS
来源：http://nqp.yj20258888.top

Java: 方法内为块级作用域
来源：http://fcu.mhx1999.top

Go:   花括号块级作用域
来源：http://hdp.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jar.cqqwz.cn

C#:   块级作用域
来源：http://xvh.zdqjudy.top

[C11] 模块导入与导出
来源：http://mct.xuanzx.com

Py:   from module import func
来源：http://okh.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pjf.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://omr.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uao.bbcook.cn

Java: import java.util.List;
来源：http://nmb.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zju.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://qpt.zycfv.cn

C#:   using System.Text;
来源：http://sxc.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://rrg.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://pwj.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://gga.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://czo.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://edh.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ncj.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://vzh.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://kch.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zqg.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://qzj.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yqy.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mna.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://imn.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://shk.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://loq.sysykeji.top

Go:   func add(a, b int) int
来源：http://gvh.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ssk.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kcl.316326.xyz

[C14] 泛型函数
来源：http://yss.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ycn.ybcxt.top

PHP:  // 无泛型
来源：http://gzj.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://ogd.zycfv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nrm.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://abt.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://whn.cheryme.top

Ruby: # 无泛型
来源：http://azx.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://phu.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://hpr.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aaf.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://kpa.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ejb.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://orm.snrcjt.cn

Java: // 无解构
来源：http://ixf.birdmap.top

Go:   // 无解构
来源：http://vsz.ybcxt.top

Ruby: a, b = pair
来源：http://irk.sxryk.cn

C#:   var (a, b) = pair;
来源：http://crc.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://swv.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://heg.epnwcf.com

PHP:  // 无重载
来源：http://hgt.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fkd.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://kdq.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qab.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://bvr.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://mfd.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://yee.jinyuanbaomall.cn

================================================================================
来源：http://fvc.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://vuy.hnxiangtu.top

================================================================================
来源：http://otp.vehdjk.com

[D01] 创建数组 / 列表
来源：http://ztg.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uaz.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uda.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mrt.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://snk.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nqa.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://yxs.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://irp.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yvj.yj20258888.top

[D02] 追加元素到末尾
来源：http://wgi.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ynp.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bib.dashuyun.cn

JS:   arr.push(4);
来源：http://idp.zdqjudy.top

TS:   arr.push(4);
来源：http://okp.meibo888.top

Java: list.add(4);
来源：http://una.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://oaw.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://xke.cqqwz.cn

C#:   list.Add(4);
来源：http://etk.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://sqw.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://sne.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nsf.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jgc.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://ioo.zhoulong.xyz

Java: list.add(0, 0);
来源：http://qrb.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://rjn.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ine.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://kpt.fzhhl.top

[D04] 删除元素
来源：http://dvu.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://voc.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cbl.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dzc.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://aov.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zqt.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eyp.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qph.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vah.svipenyu.cn

[D05] 访问与修改元素
来源：http://ffd.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xca.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jcp.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nei.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://sqb.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://vry.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://kqv.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kuv.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://krh.c1oappe.top

[D06] 数组长度
来源：http://arc.yangfankeji.com

Py:   len(arr)
来源：http://iqs.redwolf501.top

PHP:  count($arr);
来源：http://xrc.meibo888.top

JS:   arr.length
来源：http://wnx.nwbrower.top

TS:   arr.length
来源：http://fut.guowangkeji.top

Java: list.size();
来源：http://zet.pengpengdd.cyou

Go:   len(arr)
来源：http://ume.cucudq.cn

Ruby: arr.length; arr.size
来源：http://wav.nwbrower.top

C#:   list.Count;
来源：http://yhl.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://jub.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hsm.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://qso.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://gez.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://ikz.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://ebk.jinqigfzy.top

Go:   arr[1:4]
来源：http://tam.snrcjt.cn

Ruby: arr[1, 3]
来源：http://yov.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://zoh.ydzc1.top

[D08] 合并两个数组
来源：http://guh.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://wng.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://wtj.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lpl.zhongyouzk.top

TS:   [...a, ...b];
来源：http://fwb.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pvw.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://mjp.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://ytk.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://jvx.fehbvm.com

[D09] 排序（升序）
来源：http://wxm.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://kog.pengpengdd.cyou

PHP:  sort($arr);
来源：http://ecf.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wdf.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://itj.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://olo.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jqp.sweek.top

Ruby: arr.sort
来源：http://alm.cucudq.cn

C#:   list.Sort();
来源：http://byi.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://opm.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iix.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qyv.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eji.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uab.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jhv.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gln.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vgh.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://txz.sxryk.cn

[D11] 反转数组
来源：http://hcd.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ljl.xinyue.icu

PHP:  array_reverse($arr);
来源：http://bdr.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xym.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://xiu.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://lhv.tanke756.top

Go:   slices.Reverse(arr)
来源：http://dqd.gogol.net.cn

Ruby: arr.reverse
来源：http://keh.pengpengdd.cyou

C#:   list.Reverse();
来源：http://zmo.feifeiyinyue.top

[D12] 查找元素下标
来源：http://dfv.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://bml.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rpg.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jik.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecg.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ndi.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://zeh.zhijiandao.cn

Ruby: arr.index(x)
来源：http://ctm.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://kvm.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://ucj.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kqc.xuetiantiany.cn


<!-- 参考信息 -->