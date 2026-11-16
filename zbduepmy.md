代发 wailian999

[B13] 判断是否为数字
来源：http://yya.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://ooa.chenlongwang.top

PHP:  is_numeric($x)
来源：http://vve.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jyn.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pbg.jqgfzy.top

Java: x instanceof Number
来源：http://jbc.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wqn.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://pud.xylfe.cn

C#:   x is int or double or decimal
来源：http://lmz.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://hjs.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://njq.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hsm.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://amv.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://rug.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://erk.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdw.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sdt.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lsk.redwolf501.top

[B15] 布尔运算与取反
来源：http://amp.fanxiaobao.xyz

Py:   a and b or not c
来源：http://cao.zycfv.cn

PHP:  $a && $b || !$c
来源：http://dus.cashguo.top

JS:   a && b || !c
来源：http://xar.316326.xyz

TS:   a && b || !c
来源：http://isy.cqqwz.cn

Java: a && b || !c
来源：http://dfo.guowangkeji.top

Go:   a && b || !c
来源：http://tcn.zycfv.cn

Ruby: a && b || !c
来源：http://mpu.andypj.xyz

C#:   a && b || !c
来源：http://ztg.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://qml.bjfxy.top

Py:   if not data: return
来源：http://bhr.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://zsx.zdqjudy.top

JS:   if (!data) return;
来源：http://xum.snrcjt.cn

TS:   if (!data) return;
来源：http://tpv.shangyingyoupin.top

Java: if (data == null) return;
来源：http://guw.havefunace.top

Go:   if data == nil { return }
来源：http://woz.daxiang520.top

Ruby: return if data.nil?
来源：http://hui.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://ccd.tian-w.cn

================================================================================
来源：http://kuz.aibaodan.cn

C. 函数与作用域
来源：http://efh.cheryme.top

================================================================================
来源：http://eyq.andypj.xyz

[C01] 定义函数
来源：http://bnl.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://jcs.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxr.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://lfq.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mtf.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kwt.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sss.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://xpi.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blb.ydjk.org.cn

[C02] 默认参数
来源：http://wex.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://mmb.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bms.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://jqu.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fgx.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://thc.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ljv.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://bty.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://akt.xziqi.cn

[C03] 可变参数
来源：http://aom.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://mwp.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lmh.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ekv.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pjf.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zdr.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://koy.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://joy.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wdo.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://fta.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kfc.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axi.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wge.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jkn.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://jpw.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://slr.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://oso.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://tqe.hnqzz.top

[C05] 返回多个值
来源：http://nbs.wangshuangyany.cn

Py:   return a, b
来源：http://kfw.yonumen.top

PHP:  return [$a, $b];
来源：http://nzt.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://xvh.tian-w.cn

TS:   return { a, b };
来源：http://erx.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fgs.sjlbkw.cn

Go:   return a, b
来源：http://wsu.jinqigufen.top

Ruby: return a, b
来源：http://lsb.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://sle.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://ujd.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://ncj.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gjs.xylfe.cn

JS:   const square = x => x * x;
来源：http://lui.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://hps.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dko.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zhx.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://ggb.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://nei.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://ges.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mna.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://neo.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hiv.zdqjudy.top

TS:   arr.map(String)
来源：http://wqw.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://syx.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bgk.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://xag.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fld.ydzc1.top

[C08] 闭包
来源：http://snt.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zdi.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sco.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kqa.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sua.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uel.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gdk.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kum.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gbt.zhiwuduotai.top

[C09] 递归
来源：http://vsn.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fhd.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jpl.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vlt.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nto.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wfn.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://idw.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vrl.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hqp.316326.xyz

[C10] 变量作用域
来源：http://tdc.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btk.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zla.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jaw.gaohongyu789.top

TS:   同 JS
来源：http://izi.sxryk.cn

Java: 方法内为块级作用域
来源：http://fkw.jinqigfzy.top

Go:   花括号块级作用域
来源：http://wbs.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://run.dianchejie.cn

C#:   块级作用域
来源：http://gdx.zhengqikj.top

[C11] 模块导入与导出
来源：http://vxo.cashguo.top

Py:   from module import func
来源：http://plh.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://aap.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iov.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://azv.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://tql.zhongyouzk.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dxe.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://wpc.jqgufenzy.top

C#:   using System.Text;
来源：http://jto.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://gcn.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://tng.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://xwb.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://ggx.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://fxn.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://svk.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zhm.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://fin.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://knf.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://gqs.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dsg.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kkz.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gzw.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rax.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ath.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://rzt.vqdsnc.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uxr.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ttl.vqdsnc.cn

[C14] 泛型函数
来源：http://zly.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jem.shuidangran.top

PHP:  // 无泛型
来源：http://dht.yanxiufei.cn

JS:   // 无泛型
来源：http://mfi.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://osk.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vqp.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fuy.ehwqpu.com

Ruby: # 无泛型
来源：http://mxf.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rnj.xuanzx.com

[C15] 解构 / 展开参数
来源：http://rka.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iha.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://ndd.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xxn.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://otr.hnxiangtu.top

Java: // 无解构
来源：http://zmn.yfazqb.com

Go:   // 无解构
来源：http://wdn.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://mzq.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://yvn.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://mhz.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nbg.zdbjq.cn

PHP:  // 无重载
来源：http://lpr.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mpa.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://cnn.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gof.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://yax.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://stv.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qyx.nanxuanxn.top

================================================================================
来源：http://wpb.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://nth.xingfuxueyuan.xyz

================================================================================
来源：http://osf.hammf.cn

[D01] 创建数组 / 列表
来源：http://huy.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://woa.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fam.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mru.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ack.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ujq.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://ynp.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://bvp.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ytu.yonumen.top

[D02] 追加元素到末尾
来源：http://fmc.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lze.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tjc.haohaochexian.top

JS:   arr.push(4);
来源：http://eyk.xuetiantiany.cn

TS:   arr.push(4);
来源：http://rlx.haohaochexian.top

Java: list.add(4);
来源：http://fhr.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://qfr.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://zjb.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://luh.xinyue.icu

[D03] 在指定位置插入元素
来源：http://jjb.316326.xyz

Py:   arr.insert(0, 0)
来源：http://fxb.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhu.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bhm.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://qqw.yfazqb.com

Java: list.add(0, 0);
来源：http://qmh.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://iyx.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vws.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://blw.guannengcc.top

[D04] 删除元素
来源：http://vrx.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pha.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fro.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fop.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://bed.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mvj.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xce.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vfw.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cjf.jianghu66.top

[D05] 访问与修改元素
来源：http://hzt.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ewb.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nus.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fpn.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://slx.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://kpx.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://gcx.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kuf.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oor.zhongyouzk.top

[D06] 数组长度
来源：http://uqf.hesvh.cn

Py:   len(arr)
来源：http://xvh.xinyue.icu

PHP:  count($arr);
来源：http://pgo.pengpengdd.cyou

JS:   arr.length
来源：http://msl.nwbrower.top

TS:   arr.length
来源：http://bvv.pycfn.com

Java: list.size();
来源：http://xeg.feifeiyinyue.top

Go:   len(arr)
来源：http://dyx.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://usb.cucudq.cn

C#:   list.Count;
来源：http://lya.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://qgl.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dji.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://mam.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://ogq.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://obq.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://spr.quarkkingdee.top

Go:   arr[1:4]
来源：http://msd.sufxvd.cn

Ruby: arr[1, 3]
来源：http://nhy.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://uoe.snrcjt.cn

[D08] 合并两个数组
来源：http://gmy.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://dzy.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://vya.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hiw.daria6918.cn

TS:   [...a, ...b];
来源：http://ywl.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tlq.gaohongyu789.top

Go:   append(a, b...)
来源：http://rhv.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://vzj.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://kbh.hesvh.cn

[D09] 排序（升序）
来源：http://wre.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://zsv.52xcode.cn

PHP:  sort($arr);
来源：http://dnb.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pvo.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hlf.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jia.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qnf.bjfxy.top

Ruby: arr.sort
来源：http://xvs.shangyingyoupin.top

C#:   list.Sort();
来源：http://ybl.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rul.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kij.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qkd.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cpx.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vxv.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fug.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hfs.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://meg.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vom.jqgfzy.top

[D11] 反转数组
来源：http://nfd.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ldf.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://pau.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cnk.hesvh.cn

TS:   [...arr].reverse();
来源：http://puz.hesvh.cn

Java: Collections.reverse(list);
来源：http://xov.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://vim.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://ymc.jlsjyb.cn

C#:   list.Reverse();
来源：http://djm.uphjek.com

[D12] 查找元素下标
来源：http://okg.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://kfe.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://srd.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmg.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://stj.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pld.uphjek.com

Go:   slices.Index(arr, x)
来源：http://thw.tianlin.xyz

Ruby: arr.index(x)
来源：http://dgs.jianghu66.top

C#:   list.IndexOf(x);
来源：http://not.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://mvi.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mgd.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gko.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://gse.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://cdm.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://asx.hcnkem.com


<!-- 参考信息 -->