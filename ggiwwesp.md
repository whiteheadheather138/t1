代发 wailian999

PHP:  range(0, 10, 2);
来源：http://nch.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjl.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pba.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tpq.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iwp.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://lgo.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lzt.tarul.cn

[B12] 跳出多层循环
来源：http://zae.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lce.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://alc.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rol.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://udv.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oyu.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wcf.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wtm.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jmv.bbcook.cn

[B13] 判断是否为数字
来源：http://pwg.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://jmv.cheryme.top

PHP:  is_numeric($x)
来源：http://ixf.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cnf.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lgd.dashuyun.cn

Java: x instanceof Number
来源：http://ygg.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ors.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://lbi.yj202588.top

C#:   x is int or double or decimal
来源：http://vio.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://ake.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nby.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hfk.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://hki.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://wmu.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cix.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lkz.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pfy.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ovt.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://ywr.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://bej.gzhubu.top

PHP:  $a && $b || !$c
来源：http://bht.pycfn.com

JS:   a && b || !c
来源：http://xnr.vehdjk.com

TS:   a && b || !c
来源：http://ktw.ydzc1.top

Java: a && b || !c
来源：http://yet.jinqigfzy.top

Go:   a && b || !c
来源：http://xxg.chenzaomai.com

Ruby: a && b || !c
来源：http://gdr.yanxiufei.cn

C#:   a && b || !c
来源：http://fuf.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://rge.guowangkeji.top

Py:   if not data: return
来源：http://buz.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://luj.shangyingyoupin.top

JS:   if (!data) return;
来源：http://zei.nwbrower.top

TS:   if (!data) return;
来源：http://zzv.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://kep.ybcxt.top

Go:   if data == nil { return }
来源：http://yhm.fehbvm.com

Ruby: return if data.nil?
来源：http://qxw.jlsjyb.cn

C#:   if (data == null) return;
来源：http://vbi.gaohongyu789.top

================================================================================
来源：http://ucr.mhx1999.top

C. 函数与作用域
来源：http://gav.wangshuangyany.cn

================================================================================
来源：http://vyu.nanxinkj.top

[C01] 定义函数
来源：http://tfr.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://fmx.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ymo.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://jks.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gko.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xus.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nyn.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://zac.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://emh.pycfn.com

[C02] 默认参数
来源：http://axy.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://mnt.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://byj.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://kqj.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vih.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sch.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://azw.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://ady.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://pzj.chenzaomai.com

[C03] 可变参数
来源：http://wxs.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://rka.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tzf.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://avl.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ctk.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rqa.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wbv.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ddm.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ixn.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://nbj.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gzn.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dgx.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tcz.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fcj.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://mjl.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://pkh.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://bdu.sweek.top

C#:   f(a: 1, b: 2)
来源：http://cun.svipenyu.cn

[C05] 返回多个值
来源：http://xnd.nwbrower.top

Py:   return a, b
来源：http://grh.ctjpmb.com

PHP:  return [$a, $b];
来源：http://jro.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://obz.fehbvm.com

TS:   return { a, b };
来源：http://siz.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vnb.hfpthk.cn

Go:   return a, b
来源：http://pln.0kj1m.cn

Ruby: return a, b
来源：http://msi.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://rta.yongpay.top

[C06] 匿名函数 / lambda
来源：http://bpe.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://gqi.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://wex.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://xwb.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://tcz.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aqc.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://vsf.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://jrq.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://czt.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://mjy.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tkp.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://gsl.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hbv.chenjidiqi.icu

TS:   arr.map(String)
来源：http://seo.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uxs.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mkc.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://qnt.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tsm.sxryk.cn

[C08] 闭包
来源：http://oju.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jmq.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://udt.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bem.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wxf.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ydf.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://quh.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gnn.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xai.xziqi.cn

[C09] 递归
来源：http://htg.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rfm.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qon.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vkf.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gcm.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://boz.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hcq.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oed.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fpd.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://goj.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwi.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qve.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yop.daria6918.cn

TS:   同 JS
来源：http://gie.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://uog.jinqigfzy.top

Go:   花括号块级作用域
来源：http://hdi.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uwj.vehdjk.com

C#:   块级作用域
来源：http://qhd.fktsv.cn

[C11] 模块导入与导出
来源：http://lmj.hywenlv.cn

Py:   from module import func
来源：http://dua.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pmg.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gsk.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wam.sufxvd.cn

Java: import java.util.List;
来源：http://gfl.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://knz.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://hqe.cucudq.cn

C#:   using System.Text;
来源：http://pll.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://ldl.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://zxe.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://aug.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://frx.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://evo.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ijo.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://mwv.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://jss.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ufy.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://rtt.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gzj.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jgw.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fbz.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydt.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://ulv.zhengqikj.top

Go:   func add(a, b int) int
来源：http://ckv.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://grw.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://ket.yfazqb.com

[C14] 泛型函数
来源：http://ldc.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uwp.yanxiufei.cn

PHP:  // 无泛型
来源：http://gsv.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://ixp.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://djt.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wae.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kdg.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://yut.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zqy.pycfn.com

[C15] 解构 / 展开参数
来源：http://zed.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fpm.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://bzc.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oef.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hno.hywenlv.cn

Java: // 无解构
来源：http://nsn.yonumen.top

Go:   // 无解构
来源：http://cug.ydzc1.top

Ruby: a, b = pair
来源：http://hqp.cashguo.top

C#:   var (a, b) = pair;
来源：http://llu.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://hek.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jyh.hnxiangtu.top

PHP:  // 无重载
来源：http://kda.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://qwu.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://ymm.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mnh.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://pdf.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://ijz.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://obx.tianlin.xyz

================================================================================
来源：http://txs.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://rtp.sufxvd.cn

================================================================================
来源：http://dst.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://bmh.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zxi.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wtm.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wkz.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sxm.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://csd.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://hnf.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://lhb.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lrh.zhengqikj.top

[D02] 追加元素到末尾
来源：http://ozm.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iat.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hsi.jianghu66.top

JS:   arr.push(4);
来源：http://hgw.zhongyouzk.top

TS:   arr.push(4);
来源：http://pyp.hongshengwenyu.top

Java: list.add(4);
来源：http://hul.meibo888.top

Go:   arr = append(arr, 4)
来源：http://kdr.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://bvb.chenlongwang.top

C#:   list.Add(4);
来源：http://qpl.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://hdn.cheryme.top

Py:   arr.insert(0, 0)
来源：http://ksi.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wsu.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wzk.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://qsr.0kj1m.cn

Java: list.add(0, 0);
来源：http://zkc.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cck.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wdx.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://cee.xylfe.cn

[D04] 删除元素
来源：http://ztg.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uab.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bnb.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mtx.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://bim.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ear.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://apl.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mhc.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gjc.xylfe.cn

[D05] 访问与修改元素
来源：http://cza.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tgy.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ume.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yai.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://eud.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://jjh.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://gml.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://suk.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lnn.gogol.net.cn

[D06] 数组长度
来源：http://oty.sweek.top

Py:   len(arr)
来源：http://aku.snrcjt.cn

PHP:  count($arr);
来源：http://psh.iojbl.cn

JS:   arr.length
来源：http://zcw.gaohongyu789.top

TS:   arr.length
来源：http://hiq.hnqzz.top

Java: list.size();
来源：http://jva.jyoumei.cn

Go:   len(arr)
来源：http://jjh.tarul.cn

Ruby: arr.length; arr.size
来源：http://ofe.fktsv.cn

C#:   list.Count;
来源：http://lfn.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://hyp.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yar.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://ruq.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://dwn.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://jhm.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://ene.nanxinkj.top

Go:   arr[1:4]
来源：http://tns.sxryk.cn

Ruby: arr[1, 3]
来源：http://fie.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://zjs.nwbrower.top

[D08] 合并两个数组
来源：http://hqe.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://djk.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://nwc.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zvn.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://fif.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xwn.ybcxt.top

Go:   append(a, b...)
来源：http://cnh.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://ywr.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://mtb.snrcjt.cn

[D09] 排序（升序）
来源：http://pts.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://yhr.nwbrower.top

PHP:  sort($arr);
来源：http://aut.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://avs.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tfe.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yey.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://csz.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://grb.tian-w.cn

C#:   list.Sort();
来源：http://wey.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mgv.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pay.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xbu.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rvj.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgl.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://czw.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mfk.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zpa.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://een.yj20258888.top

[D11] 反转数组
来源：http://gse.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xgr.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://bur.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aym.daria6918.cn

TS:   [...arr].reverse();
来源：http://hqf.jqgfzy.top

Java: Collections.reverse(list);
来源：http://gsv.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://wwy.mhx1999.top

Ruby: arr.reverse
来源：http://mvk.snrcjt.cn


<!-- 参考信息 -->