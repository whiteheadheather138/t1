代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cus.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://fmb.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uea.xinyue.icu

[B12] 跳出多层循环
来源：http://bay.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zfi.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rpn.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://emf.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pbd.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rxf.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cxa.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://flx.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aym.fehbvm.com

[B13] 判断是否为数字
来源：http://hmo.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://hrx.daxiang520.top

PHP:  is_numeric($x)
来源：http://hgb.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://erb.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppj.fehbvm.com

Java: x instanceof Number
来源：http://trl.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lei.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://aoa.fzhhl.top

C#:   x is int or double or decimal
来源：http://ilx.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://hyx.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dyy.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mos.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://gdj.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://ksz.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://utq.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jvz.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://fao.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fzq.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://ulp.nwbrower.top

Py:   a and b or not c
来源：http://ruh.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://npm.316326.xyz

JS:   a && b || !c
来源：http://omb.daria6918.cn

TS:   a && b || !c
来源：http://pnm.hysaishi.cn

Java: a && b || !c
来源：http://avr.hfpthk.cn

Go:   a && b || !c
来源：http://fhm.zhongyouzk.top

Ruby: a && b || !c
来源：http://gle.jqgfzy.top

C#:   a && b || !c
来源：http://lrg.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://cor.316326.xyz

Py:   if not data: return
来源：http://jmn.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://gob.shangyingyoupin.top

JS:   if (!data) return;
来源：http://qmg.52xcode.cn

TS:   if (!data) return;
来源：http://xto.ivvv.top

Java: if (data == null) return;
来源：http://wmy.cucudq.cn

Go:   if data == nil { return }
来源：http://jtl.0kj1m.cn

Ruby: return if data.nil?
来源：http://ylx.gaohongyu789.top

C#:   if (data == null) return;
来源：http://tqq.yangfankeji.com

================================================================================
来源：http://pts.vqdsnc.cn

C. 函数与作用域
来源：http://ahz.gotoacloud.top

================================================================================
来源：http://ghz.cqqwz.cn

[C01] 定义函数
来源：http://rgk.havefunace.top

Py:   def add(a, b): return a + b
来源：http://fnf.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hid.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://ldr.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://knf.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://see.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://qmc.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://yos.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mow.aibaodan.cn

[C02] 默认参数
来源：http://iqq.yonumen.top

Py:   def greet(name="World"): return name
来源：http://oyf.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lgv.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://gho.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dkq.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eyu.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://beq.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://xck.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://mqw.yj20258888.top

[C03] 可变参数
来源：http://lsu.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://nmg.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ubp.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mjx.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uum.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ily.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mgn.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://fry.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rdn.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://liy.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvy.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eps.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ywm.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qwr.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://xio.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://crd.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://gfq.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://rcy.yj20258888.top

[C05] 返回多个值
来源：http://ppq.zhaomingkeji.xyz

Py:   return a, b
来源：http://dme.cashguo.top

PHP:  return [$a, $b];
来源：http://ghg.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qje.cashguo.top

TS:   return { a, b };
来源：http://gmu.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fnf.svipenyu.cn

Go:   return a, b
来源：http://ajs.andypj.xyz

Ruby: return a, b
来源：http://lut.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://zzb.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://pbd.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://upr.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jhc.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://njp.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://rto.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hhr.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://zjd.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://gqp.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hqa.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://gba.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://llv.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rvp.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://phz.pengpengdd.cyou

TS:   arr.map(String)
来源：http://mhj.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qnp.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lji.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://goy.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uua.jinghuilouyu.cn

[C08] 闭包
来源：http://ebq.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qhg.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zmn.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://trz.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hky.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ccc.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kej.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mfn.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ixw.aibaodan.cn

[C09] 递归
来源：http://kfs.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ryg.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fet.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzu.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xlc.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://myc.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hhs.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fff.ehwqpu.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://btb.52xcode.cn

[C10] 变量作用域
来源：http://aru.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mou.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://olg.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lnx.snrcjt.cn

TS:   同 JS
来源：http://apz.meibo888.top

Java: 方法内为块级作用域
来源：http://zzk.jqgfzy.top

Go:   花括号块级作用域
来源：http://ohk.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iue.pycfn.com

C#:   块级作用域
来源：http://kih.ehwqpu.com

[C11] 模块导入与导出
来源：http://vti.snrcjt.cn

Py:   from module import func
来源：http://cbv.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://rua.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://oym.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wda.gaohongyu789.top

Java: import java.util.List;
来源：http://wqw.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nzu.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://rap.mhx1999.top

C#:   using System.Text;
来源：http://gky.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://ftv.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://grn.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://cec.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://xex.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://hsd.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wmq.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://hzt.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://vvx.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gvs.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://cyo.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hbr.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gng.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bot.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ncc.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://afd.zdqjudy.top

Go:   func add(a, b int) int
来源：http://luy.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nsn.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wry.jyoumei.cn

[C14] 泛型函数
来源：http://edv.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bio.shuidangran.top

PHP:  // 无泛型
来源：http://fmz.fzhhl.top

JS:   // 无泛型
来源：http://cze.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cra.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bxh.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dni.sweek.top

Ruby: # 无泛型
来源：http://mlr.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qfl.xuanzx.com

[C15] 解构 / 展开参数
来源：http://leh.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lqx.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://ggq.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxr.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hda.c1oappe.top

Java: // 无解构
来源：http://zyr.cheryme.top

Go:   // 无解构
来源：http://guw.kuanghao11.cn

Ruby: a, b = pair
来源：http://vsc.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://csb.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://wso.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cyx.meibo888.top

PHP:  // 无重载
来源：http://hut.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xfn.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://eft.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oma.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://oox.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://sbt.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ans.chenzaomai.com

================================================================================
来源：http://ywk.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://ffx.pycfn.com

================================================================================
来源：http://lfp.wangdashe.top

[D01] 创建数组 / 列表
来源：http://bor.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qyx.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iif.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jti.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pcy.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ufs.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://gia.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://uig.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oba.hnqzz.top

[D02] 追加元素到末尾
来源：http://cek.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dfr.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eqe.ivvv.top

JS:   arr.push(4);
来源：http://spg.hfpthk.cn

TS:   arr.push(4);
来源：http://vre.yueranfly.top

Java: list.add(4);
来源：http://dws.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://vdw.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://wlq.zhixingplan.top

C#:   list.Add(4);
来源：http://hnk.uphjek.com

[D03] 在指定位置插入元素
来源：http://fcd.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://bxl.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oug.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uec.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://xbp.jinqigufen.top

Java: list.add(0, 0);
来源：http://kpo.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://ovm.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lqr.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://urc.52xcode.cn

[D04] 删除元素
来源：http://nca.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wzy.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xja.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mgv.tanke756.top

TS:   arr.splice(0, 1);
来源：http://uvh.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogu.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xfd.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hlo.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://snv.jqgfzy.top

[D05] 访问与修改元素
来源：http://syl.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://epg.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pxo.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://osu.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://ixt.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://pbn.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://ork.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mfk.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fjq.zhixingplan.top

[D06] 数组长度
来源：http://mxm.yvedp.cn

Py:   len(arr)
来源：http://vzb.smart0.xyz

PHP:  count($arr);
来源：http://agg.hongshengwenyu.top

JS:   arr.length
来源：http://svc.cqqwz.cn

TS:   arr.length
来源：http://iwp.epnwcf.com

Java: list.size();
来源：http://had.hesvh.cn

Go:   len(arr)
来源：http://lgt.iojbl.cn

Ruby: arr.length; arr.size
来源：http://hfe.0kj1m.cn

C#:   list.Count;
来源：http://msx.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://rzx.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jun.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://htu.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://wan.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://sry.zdqjudy.top

Java: list.subList(1, 4);
来源：http://qff.smart0.xyz

Go:   arr[1:4]
来源：http://xfz.c1oappe.top

Ruby: arr[1, 3]
来源：http://csl.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://lfj.zdbjq.cn

[D08] 合并两个数组
来源：http://zgh.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://mfj.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://pfw.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://exp.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://gbx.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ncw.hcnkem.com

Go:   append(a, b...)
来源：http://yym.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://llf.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://hah.nanxinkj.top

[D09] 排序（升序）
来源：http://dnm.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://vmy.pengpengdd.cyou

PHP:  sort($arr);
来源：http://xhc.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kln.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oad.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ljm.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eup.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://rre.jinghuilouyu.cn

C#:   list.Sort();
来源：http://abc.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bsf.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vxc.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vvg.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://trf.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aln.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ozs.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pls.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eqo.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ouo.jianghu66.top

[D11] 反转数组
来源：http://fyq.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://sen.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://dza.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jhk.yj202588.top

TS:   [...arr].reverse();
来源：http://eso.yueranfly.top

Java: Collections.reverse(list);
来源：http://rff.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://uds.hnxiangtu.top

Ruby: arr.reverse
来源：http://ayj.yuanzhike.top

C#:   list.Reverse();
来源：http://jtb.52xcode.cn

[D12] 查找元素下标
来源：http://glc.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://mew.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bsd.jlsjyb.cn


<!-- 参考信息 -->