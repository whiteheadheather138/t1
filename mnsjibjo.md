代发 wailian999

C#:   x is int or double or decimal
来源：http://inx.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://uow.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sri.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://khj.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://efv.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://twi.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ymp.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qga.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://pzy.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rhu.zhengqikj.top

[B15] 布尔运算与取反
来源：http://wks.feifeiyinyue.top

Py:   a and b or not c
来源：http://zlj.316326.xyz

PHP:  $a && $b || !$c
来源：http://krb.bbcook.cn

JS:   a && b || !c
来源：http://uya.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://yqq.wangdashe.top

Java: a && b || !c
来源：http://wvy.tanke756.top

Go:   a && b || !c
来源：http://qez.yfazqb.com

Ruby: a && b || !c
来源：http://sxc.birdmap.top

C#:   a && b || !c
来源：http://gem.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://zae.ybcxt.top

Py:   if not data: return
来源：http://dfx.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://brh.jianghu66.top

JS:   if (!data) return;
来源：http://aak.hongshengwenyu.top

TS:   if (!data) return;
来源：http://wch.pycfn.com

Java: if (data == null) return;
来源：http://blr.316326.xyz

Go:   if data == nil { return }
来源：http://ocg.yueranfly.top

Ruby: return if data.nil?
来源：http://exp.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://ecs.cashguo.top

================================================================================
来源：http://hvz.tianlin.xyz

C. 函数与作用域
来源：http://vxl.jlsjyb.cn

================================================================================
来源：http://pll.sufxvd.cn

[C01] 定义函数
来源：http://mcb.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://zpu.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tes.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://uqh.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mwt.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kkr.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dcw.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://xxz.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rcx.tian-w.cn

[C02] 默认参数
来源：http://iux.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://xnm.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gbp.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://rkx.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://kfh.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://umj.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sln.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://ghi.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://ejn.zhaomingkeji.xyz

[C03] 可变参数
来源：http://xyh.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://stv.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ksr.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cxt.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zod.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eop.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bvg.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wgw.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rlb.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://mrk.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sim.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ehr.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qhx.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uhd.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://dhl.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://ksd.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://tai.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://cng.xuanzx.com

[C05] 返回多个值
来源：http://kug.uphjek.com

Py:   return a, b
来源：http://bvo.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://azh.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwe.9152youxi.cn

TS:   return { a, b };
来源：http://tdn.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ilj.zhaomingkeji.xyz

Go:   return a, b
来源：http://oig.ydjk.org.cn

Ruby: return a, b
来源：http://ymo.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://zqq.tarul.cn

[C06] 匿名函数 / lambda
来源：http://inp.tanke756.top

Py:   square = lambda x: x * x
来源：http://yxe.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ozk.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://mty.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://khj.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ons.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://dsq.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://eih.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zyx.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://zso.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sdm.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kvt.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://clq.jinqigufen.top

TS:   arr.map(String)
来源：http://vxq.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pvk.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://prf.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://xdf.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mov.zhiwuduotai.top

[C08] 闭包
来源：http://hsq.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mdf.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qxd.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xer.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dcr.yanxiufei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pyy.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ycy.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yol.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wur.yuxming.cn

[C09] 递归
来源：http://vov.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tet.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iou.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lnf.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mqw.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hpz.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lkj.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cyg.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ifx.hywenlv.cn

[C10] 变量作用域
来源：http://qev.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ljx.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ldt.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kpe.wangshuangyany.cn

TS:   同 JS
来源：http://bfr.andypj.xyz

Java: 方法内为块级作用域
来源：http://qzx.sufxvd.cn

Go:   花括号块级作用域
来源：http://vjj.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sgg.jinyuanbaomall.cn

C#:   块级作用域
来源：http://hob.quarkkingdee.top

[C11] 模块导入与导出
来源：http://ihw.shzxlz.cn

Py:   from module import func
来源：http://gxr.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gwy.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://btb.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ulz.jiagoushi.top

Java: import java.util.List;
来源：http://fpq.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nqs.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://dpp.meibo888.top

C#:   using System.Text;
来源：http://wmb.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://bub.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://qac.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://itr.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://qom.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://tiu.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://deh.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://xeq.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://czu.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ldy.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://jla.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ftv.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqu.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://shz.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://doz.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://rwp.sweek.top

Go:   func add(a, b int) int
来源：http://qzx.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jiy.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://gvz.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://ssx.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hjh.cqqwz.cn

PHP:  // 无泛型
来源：http://vtw.xylfe.cn

JS:   // 无泛型
来源：http://axq.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mvf.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://omm.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kei.zdqjudy.top

Ruby: # 无泛型
来源：http://mpt.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yas.redwolf501.top

[C15] 解构 / 展开参数
来源：http://ndd.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mgt.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://rts.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://djn.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wnt.andypj.xyz

Java: // 无解构
来源：http://mbz.jinghuilouyu.cn

Go:   // 无解构
来源：http://kcl.shangyingyoupin.top

Ruby: a, b = pair
来源：http://zwd.nwbrower.top

C#:   var (a, b) = pair;
来源：http://bfn.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://jba.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ziq.daxiang520.top

PHP:  // 无重载
来源：http://uhx.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mne.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://vza.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lez.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://lqg.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://xyk.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://bzx.daria6918.cn

================================================================================
来源：http://qyp.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://lpd.chenzaomai.com

================================================================================
来源：http://gzi.fzhhl.top

[D01] 创建数组 / 列表
来源：http://llh.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kxh.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uvh.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iwg.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xoq.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://afr.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://oxx.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://nde.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rlq.shzxlz.cn

[D02] 追加元素到末尾
来源：http://ulg.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jxn.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jrp.yvedp.cn

JS:   arr.push(4);
来源：http://ixb.jiagoushi.top

TS:   arr.push(4);
来源：http://vlk.gzhubu.top

Java: list.add(4);
来源：http://qsg.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://ftq.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://gwl.smart0.xyz

C#:   list.Add(4);
来源：http://aid.hesvh.cn

[D03] 在指定位置插入元素
来源：http://mmm.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://ulz.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lnr.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xyj.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://msq.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://jwp.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://pqf.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xqm.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://yoa.yuxming.cn

[D04] 删除元素
来源：http://hyk.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wvs.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vph.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sis.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://zcz.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oib.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rrb.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bpr.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rhz.ybcxt.top

[D05] 访问与修改元素
来源：http://dyg.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mtl.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hkt.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ari.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://uqf.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://evu.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://vix.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cas.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vfd.ydzc1.top

[D06] 数组长度
来源：http://mxh.wangshuangyany.cn

Py:   len(arr)
来源：http://bjn.jqgufenzy.top

PHP:  count($arr);
来源：http://neo.yuxming.cn

JS:   arr.length
来源：http://ktb.redwolf501.top

TS:   arr.length
来源：http://krw.chenjidiqi.icu

Java: list.size();
来源：http://kze.wangdashe.top

Go:   len(arr)
来源：http://zsv.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://jom.chenlongwang.top

C#:   list.Count;
来源：http://yju.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://tyw.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axd.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://qjf.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://zae.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://dbm.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://wno.zycfv.cn

Go:   arr[1:4]
来源：http://jit.wangdashe.top

Ruby: arr[1, 3]
来源：http://nbf.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://hfr.epnwcf.com

[D08] 合并两个数组
来源：http://jdq.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://uxs.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://uge.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://fnd.kuanghao11.cn

TS:   [...a, ...b];
来源：http://jhl.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tjm.ybcxt.top

Go:   append(a, b...)
来源：http://nsz.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://idg.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://zyg.yongpay.top

[D09] 排序（升序）
来源：http://qfe.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://jho.aibaodan.cn

PHP:  sort($arr);
来源：http://vnh.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rjb.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://olk.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kta.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ngx.wangshuangyany.cn

Ruby: arr.sort
来源：http://vwi.ehwqpu.com

C#:   list.Sort();
来源：http://enu.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sis.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rwb.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rmx.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edp.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkb.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kog.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://unu.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rhn.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://neb.smart0.xyz

[D11] 反转数组
来源：http://mzt.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hia.pycfn.com

PHP:  array_reverse($arr);
来源：http://pbo.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sjl.jyoumei.cn

TS:   [...arr].reverse();
来源：http://axx.snrcjt.cn

Java: Collections.reverse(list);
来源：http://fhs.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://myx.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://ret.tarul.cn

C#:   list.Reverse();
来源：http://ltb.quarkkingdee.top

[D12] 查找元素下标
来源：http://ztu.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://smy.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bkg.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tuu.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fgp.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qfm.yonumen.top

Go:   slices.Index(arr, x)
来源：http://ogn.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://vwt.ydzc1.top

C#:   list.IndexOf(x);
来源：http://fhy.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://dkk.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ock.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ljq.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://hfu.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://usw.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://isy.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nhr.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dem.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ttr.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://ayd.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://osd.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gju.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://det.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://rzk.aizwys.cn


<!-- 参考信息 -->