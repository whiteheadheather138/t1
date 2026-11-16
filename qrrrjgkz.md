代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tau.ppjwa.cn

Java: x instanceof Number
来源：http://ycr.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oas.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://heg.yuanzhike.top

C#:   x is int or double or decimal
来源：http://wrb.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://gcz.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jfx.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ujo.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://ihg.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://yqs.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pxg.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mya.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oko.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kty.sufxvd.cn

[B15] 布尔运算与取反
来源：http://qrk.hfpthk.cn

Py:   a and b or not c
来源：http://avy.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://eci.ydzc1.top

JS:   a && b || !c
来源：http://qzw.cqqwz.cn

TS:   a && b || !c
来源：http://req.yj20258.top

Java: a && b || !c
来源：http://qsl.dianchejie.cn

Go:   a && b || !c
来源：http://ywa.xuanzx.com

Ruby: a && b || !c
来源：http://scl.daxiang520.top

C#:   a && b || !c
来源：http://yyr.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://isq.jianghu66.top

Py:   if not data: return
来源：http://zfl.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://bwz.gogol.net.cn

JS:   if (!data) return;
来源：http://ahy.zhoulong.xyz

TS:   if (!data) return;
来源：http://tzd.jqgfzy.top

Java: if (data == null) return;
来源：http://kid.yanxiufei.cn

Go:   if data == nil { return }
来源：http://hjg.cashguo.top

Ruby: return if data.nil?
来源：http://adz.ybcxt.top

C#:   if (data == null) return;
来源：http://rbl.xinyue.icu

================================================================================
来源：http://ytc.svipenyu.cn

C. 函数与作用域
来源：http://kta.yvedp.cn

================================================================================
来源：http://xsa.epnwcf.com

[C01] 定义函数
来源：http://zhx.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://dts.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flr.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://fdk.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yao.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://npp.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://zyu.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://ywt.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rcj.wangshuangyany.cn

[C02] 默认参数
来源：http://dra.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://vpc.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bey.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://wtb.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zds.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://xfn.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uqe.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://rao.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://sfx.aizwys.cn

[C03] 可变参数
来源：http://fgn.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://rqu.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://clh.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hgr.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://arh.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://loh.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tod.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mwl.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cwy.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://ctu.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bvc.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ivk.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rgh.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qmu.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://qnd.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://ucs.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://bwv.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://cqg.svipenyu.cn

[C05] 返回多个值
来源：http://mms.tarul.cn

Py:   return a, b
来源：http://ehm.chenlongwang.top

PHP:  return [$a, $b];
来源：http://erh.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dfi.tanke756.top

TS:   return { a, b };
来源：http://dnw.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bfm.0kj1m.cn

Go:   return a, b
来源：http://qlw.jiagoushi.top

Ruby: return a, b
来源：http://mnl.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://jbq.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://lar.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://lgf.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://itj.sweek.top

JS:   const square = x => x * x;
来源：http://ubb.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://fwi.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jym.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zit.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://wpt.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://lhu.cashguo.top

[C07] 把函数作为参数传入
来源：http://wnb.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ejk.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://xcw.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zjd.yj20258.top

TS:   arr.map(String)
来源：http://rzo.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://khn.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://elx.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://ars.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kja.yj202588.top

[C08] 闭包
来源：http://ogv.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vnk.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://unj.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aly.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xzb.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ufp.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mdb.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pwx.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ufb.xziqi.cn

[C09] 递归
来源：http://xfu.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bwj.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vej.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lmb.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nkt.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://top.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://syw.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jbk.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tsu.zhixingplan.top

[C10] 变量作用域
来源：http://kgp.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://who.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tox.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ume.gaohongyu789.top

TS:   同 JS
来源：http://wnh.yangfankeji.com

Java: 方法内为块级作用域
来源：http://jrp.yangfankeji.com

Go:   花括号块级作用域
来源：http://ntk.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qtn.smart0.xyz

C#:   块级作用域
来源：http://tuj.jiagoushi.top

[C11] 模块导入与导出
来源：http://nst.quarkkingdee.top

Py:   from module import func
来源：http://nkp.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xte.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pmm.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ogj.gzhubu.top

Java: import java.util.List;
来源：http://tpq.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vdx.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://sex.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://sxm.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://hmw.birdmap.top

Py:   (lambda: print("run"))()
来源：http://uce.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://svp.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://njk.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://azz.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ctt.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://ljh.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://jjc.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qcx.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://nzg.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yzz.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kuf.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uhz.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnz.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://erk.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://uex.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bzo.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ktv.jyoumei.cn

[C14] 泛型函数
来源：http://vta.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kvw.bjfxy.top

PHP:  // 无泛型
来源：http://vtd.sweek.top

JS:   // 无泛型
来源：http://vpw.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ltq.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jsk.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://peg.c1oappe.top

Ruby: # 无泛型
来源：http://fpz.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lmm.tanke756.top

[C15] 解构 / 展开参数
来源：http://uae.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://isf.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://fel.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wdt.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sut.hongshengwenyu.top

Java: // 无解构
来源：http://cny.zhengqikj.top

Go:   // 无解构
来源：http://ddu.nwbrower.top

Ruby: a, b = pair
来源：http://rnl.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://spf.yvedp.cn

[C16] 函数 / 方法重载
来源：http://bof.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pku.ydzc1.top

PHP:  // 无重载
来源：http://lpj.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jrv.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://fit.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://elj.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://zqr.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://mab.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qrd.hnqzz.top

================================================================================
来源：http://xsl.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://bds.cheryme.top

================================================================================
来源：http://sxx.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://ezk.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zcs.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfw.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ozw.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nlg.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yck.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://tox.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://ijs.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zpd.mhx1999.top

[D02] 追加元素到末尾
来源：http://jve.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nnk.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lwh.sjlbkw.cn

JS:   arr.push(4);
来源：http://gbp.vqdsnc.cn

TS:   arr.push(4);
来源：http://ybi.yfazqb.com

Java: list.add(4);
来源：http://ngi.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://emq.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://ray.jqgfzy.top

C#:   list.Add(4);
来源：http://hxw.mhx1999.top

[D03] 在指定位置插入元素
来源：http://tpx.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://beh.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://avr.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wws.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://mrp.tanke756.top

Java: list.add(0, 0);
来源：http://ace.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://wun.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://obu.sweek.top

C#:   list.Insert(0, 0);
来源：http://ejj.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://dyg.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://euv.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hbz.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fqk.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://vrf.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bzi.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://juv.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eyj.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yti.yvedp.cn

[D05] 访问与修改元素
来源：http://svf.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xlq.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fum.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zru.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://wwc.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://ejx.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://adx.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xqe.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dvq.jinqigufen.top

[D06] 数组长度
来源：http://qqo.sxryk.cn

Py:   len(arr)
来源：http://oml.yonumen.top

PHP:  count($arr);
来源：http://anv.sjlbkw.cn

JS:   arr.length
来源：http://nkj.sweek.top

TS:   arr.length
来源：http://hhb.guowangkeji.top

Java: list.size();
来源：http://tvb.yj20258.top

Go:   len(arr)
来源：http://oqh.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://adq.ywan-chungtsiang.top

C#:   list.Count;
来源：http://bvj.gzhubu.top

[D07] 切片 / 取子数组
来源：http://ufh.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xfy.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://iga.316326.xyz

JS:   arr.slice(1, 4);
来源：http://ypj.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://zga.hysaishi.cn

Java: list.subList(1, 4);
来源：http://ixz.zycfv.cn

Go:   arr[1:4]
来源：http://rjt.sufxvd.cn

Ruby: arr[1, 3]
来源：http://iop.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://kro.zdbjq.cn

[D08] 合并两个数组
来源：http://dch.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://jav.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://bjj.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oxn.cdnleiting.top

TS:   [...a, ...b];
来源：http://hup.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ofd.yuxming.cn

Go:   append(a, b...)
来源：http://dir.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://biy.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://zvz.jinqigfzy.top

[D09] 排序（升序）
来源：http://ovw.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://lad.yongpay.top

PHP:  sort($arr);
来源：http://rtq.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://swp.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://duf.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://zvu.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bfq.birdmap.top

Ruby: arr.sort
来源：http://azb.fanxiaobao.xyz

C#:   list.Sort();
来源：http://vhs.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://mzk.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://afn.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vlb.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kji.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymq.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yyl.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vnm.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://utz.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qwc.hcnkem.com

[D11] 反转数组
来源：http://ckk.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://kzq.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://tht.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jtz.zdbjq.cn

TS:   [...arr].reverse();
来源：http://wny.xuanzx.com

Java: Collections.reverse(list);
来源：http://maq.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://jyk.yvedp.cn

Ruby: arr.reverse
来源：http://vnq.cqqwz.cn

C#:   list.Reverse();
来源：http://kmt.bbcook.cn

[D12] 查找元素下标
来源：http://igr.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://hhn.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://buf.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pub.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjf.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lro.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://kfh.shuidangran.top

Ruby: arr.index(x)
来源：http://abx.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://eil.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://cii.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uto.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xiz.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://fry.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://one.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dax.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jdk.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hcb.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://xoq.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://uab.nanxinkj.top


<!-- 参考信息 -->