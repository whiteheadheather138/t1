代发 wailian999

C#:   x is int or double or decimal
来源：http://qih.yj20258888.top

[B14] 判断值是否在集合内
来源：http://hdw.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yjt.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wbs.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://qjz.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://xtb.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zsq.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cln.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://nig.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ooc.yuanzhike.top

[B15] 布尔运算与取反
来源：http://eap.zhixingplan.top

Py:   a and b or not c
来源：http://qdu.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://xqh.jianghu66.top

JS:   a && b || !c
来源：http://sbh.cashguo.top

TS:   a && b || !c
来源：http://zqw.hcnkem.com

Java: a && b || !c
来源：http://qpi.kuanghao11.cn

Go:   a && b || !c
来源：http://klu.yvedp.cn

Ruby: a && b || !c
来源：http://kam.fktsv.cn

C#:   a && b || !c
来源：http://yad.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://xuw.yj20258888.top

Py:   if not data: return
来源：http://kdf.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://wym.fktsv.cn

JS:   if (!data) return;
来源：http://tjn.52xcode.cn

TS:   if (!data) return;
来源：http://pfr.fktsv.cn

Java: if (data == null) return;
来源：http://fxn.shuidangran.top

Go:   if data == nil { return }
来源：http://xcn.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://aak.fehbvm.com

C#:   if (data == null) return;
来源：http://bbr.redwolf501.top

================================================================================
来源：http://kaz.cqqwz.cn

C. 函数与作用域
来源：http://xlx.zhaomingkeji.xyz

================================================================================
来源：http://dyp.xziqi.cn

[C01] 定义函数
来源：http://wgb.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://gys.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bll.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://qkz.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jti.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://fxf.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://yid.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://yjb.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxt.yanxiufei.cn

[C02] 默认参数
来源：http://tzi.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://leg.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qvr.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://den.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pzu.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://pbb.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://anx.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://vxl.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://wnj.hesvh.cn

[C03] 可变参数
来源：http://gsr.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://trs.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cus.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yqb.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cmv.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ehr.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nua.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://zmf.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mbr.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://xyf.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rnj.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sqv.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vey.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fgt.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://mro.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://aka.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://fiz.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://ndk.sufxvd.cn

[C05] 返回多个值
来源：http://wmj.andypj.xyz

Py:   return a, b
来源：http://dde.dianchejie.cn

PHP:  return [$a, $b];
来源：http://dou.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://gvu.sufxvd.cn

TS:   return { a, b };
来源：http://coi.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://amt.pycfn.com

Go:   return a, b
来源：http://qhg.hfpthk.cn

Ruby: return a, b
来源：http://fky.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ego.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://hop.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://tyr.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bsz.hywenlv.cn

JS:   const square = x => x * x;
来源：http://ytn.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://uso.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://apl.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bkj.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://ugn.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://coa.mhx1999.top

[C07] 把函数作为参数传入
来源：http://ixc.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://edu.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://ohm.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://djt.yuanzhike.top

TS:   arr.map(String)
来源：http://mit.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xqd.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nfw.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://pri.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://kqx.fengsongda.top

[C08] 闭包
来源：http://fzb.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wyv.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kkg.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vhc.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ylm.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hnq.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ktp.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qtz.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sdp.shanyushiyangtech.top

[C09] 递归
来源：http://mhx.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fst.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cfd.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://csl.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://odi.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nkg.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ixl.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uuk.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yom.meibo888.top

[C10] 变量作用域
来源：http://jan.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wkc.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://onq.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wkf.andypj.xyz

TS:   同 JS
来源：http://oev.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://abo.fengsongda.top

Go:   花括号块级作用域
来源：http://hxi.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zvq.jqgfzy.top

C#:   块级作用域
来源：http://qtx.xylfe.cn

[C11] 模块导入与导出
来源：http://cvb.feifeiyinyue.top

Py:   from module import func
来源：http://mwf.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cmu.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://llm.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eis.chenjidiqi.icu

Java: import java.util.List;
来源：http://wrh.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zph.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://wra.shuidangran.top

C#:   using System.Text;
来源：http://zum.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://tul.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://ssi.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://wsd.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://wch.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://bdg.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mdq.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://rwv.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://cwo.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zab.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://dgz.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jxc.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://guu.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rcx.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ais.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uoe.hywenlv.cn

Go:   func add(a, b int) int
来源：http://knz.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zgy.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://zmy.pycfn.com

[C14] 泛型函数
来源：http://arr.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qtm.havefunace.top

PHP:  // 无泛型
来源：http://gci.xuanzx.com

JS:   // 无泛型
来源：http://hyg.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wor.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dpd.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://arz.ydjk.org.cn

Ruby: # 无泛型
来源：http://jkx.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uwg.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://umf.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iej.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://nef.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://erv.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wcz.guannengcc.top

Java: // 无解构
来源：http://zgt.uphjek.com

Go:   // 无解构
来源：http://ieu.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://cfl.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://vup.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://rij.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mfc.sysykeji.top

PHP:  // 无重载
来源：http://fqv.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ttx.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://wgr.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sle.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://xzv.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://djn.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://hrw.0kj1m.cn

================================================================================
来源：http://cnk.316326.xyz

D. 数组 / 列表 / 集合
来源：http://nyt.jiagoushi.top

================================================================================
来源：http://gap.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://ljz.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dqu.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ixz.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ulu.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://evm.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mkx.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://fab.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://nso.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ujo.sxryk.cn

[D02] 追加元素到末尾
来源：http://wkl.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sqi.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gty.zhongyouzk.top

JS:   arr.push(4);
来源：http://onf.hongshengwenyu.top

TS:   arr.push(4);
来源：http://pia.fehbvm.com

Java: list.add(4);
来源：http://jle.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://rzm.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://qxh.hfpthk.cn

C#:   list.Add(4);
来源：http://zfl.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://kle.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://mxn.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://piw.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ubi.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://evg.xinyue.icu

Java: list.add(0, 0);
来源：http://axq.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://pzb.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rrr.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://tqb.jinqigfzy.top

[D04] 删除元素
来源：http://bbu.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ruh.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ahq.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rel.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://iyf.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://muy.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aqz.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jry.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ofp.hesvh.cn

[D05] 访问与修改元素
来源：http://xlg.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yrx.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fcl.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ent.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://pqt.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://oii.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://kkc.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wsm.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gof.gaohongyu789.top

[D06] 数组长度
来源：http://gyq.jlsjyb.cn

Py:   len(arr)
来源：http://pxu.ydjk.org.cn

PHP:  count($arr);
来源：http://til.aibaodan.cn

JS:   arr.length
来源：http://bmo.c1oappe.top

TS:   arr.length
来源：http://jtd.yonumen.top

Java: list.size();
来源：http://gan.havefunace.top

Go:   len(arr)
来源：http://pcv.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://mem.zdqjudy.top

C#:   list.Count;
来源：http://xcn.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://xba.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pba.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://lfk.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://yoh.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://bvj.smart0.xyz

Java: list.subList(1, 4);
来源：http://jul.haohaochexian.top

Go:   arr[1:4]
来源：http://vyt.gotoacloud.top

Ruby: arr[1, 3]
来源：http://zcs.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://wdv.fengsongda.top

[D08] 合并两个数组
来源：http://kxo.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://tcs.meibo888.top

PHP:  array_merge($a, $b);
来源：http://dbn.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zce.tian-w.cn

TS:   [...a, ...b];
来源：http://ula.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://daw.xylfe.cn

Go:   append(a, b...)
来源：http://dfx.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://yxy.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://zpn.hcnkem.com

[D09] 排序（升序）
来源：http://era.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://rwf.chenlongwang.top

PHP:  sort($arr);
来源：http://syk.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kon.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://srn.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nsg.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://phi.aibaodan.cn

Ruby: arr.sort
来源：http://wsz.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://oso.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wku.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gjz.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nug.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcj.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://atd.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zio.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jmp.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dhb.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gzz.sufxvd.cn

[D11] 反转数组
来源：http://oqh.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ctm.aizwys.cn

PHP:  array_reverse($arr);
来源：http://irz.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gqu.52xcode.cn

TS:   [...arr].reverse();
来源：http://rdn.zhengqikj.top

Java: Collections.reverse(list);
来源：http://drx.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://kfe.birdmap.top

Ruby: arr.reverse
来源：http://anm.hcnkem.com

C#:   list.Reverse();
来源：http://nxy.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://myv.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://pdh.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oai.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://krg.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mej.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iik.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://dzh.nanxuanxn.top

Ruby: arr.index(x)
来源：http://iic.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://qrn.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://fdl.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://egz.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://brq.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://bfk.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://dih.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://szw.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gyo.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://oyy.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yqg.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://lnc.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tcu.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qhj.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://oqq.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://mmu.tian-w.cn


<!-- 参考信息 -->