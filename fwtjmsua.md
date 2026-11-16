代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hkg.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ldl.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqc.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iso.daxiang520.top

[B13] 判断是否为数字
来源：http://rxq.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://gpa.gogol.net.cn

PHP:  is_numeric($x)
来源：http://fpx.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://axe.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eve.fzhhl.top

Java: x instanceof Number
来源：http://cgq.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rrh.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://hlu.9152youxi.cn

C#:   x is int or double or decimal
来源：http://gpv.andypj.xyz

[B14] 判断值是否在集合内
来源：http://baa.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ocd.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qds.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://zwl.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://bdi.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ibd.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vll.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ytl.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eus.fehbvm.com

[B15] 布尔运算与取反
来源：http://caw.bbcook.cn

Py:   a and b or not c
来源：http://zhj.xylfe.cn

PHP:  $a && $b || !$c
来源：http://mjs.tanke756.top

JS:   a && b || !c
来源：http://pcg.dashuyun.cn

TS:   a && b || !c
来源：http://xuc.tanke756.top

Java: a && b || !c
来源：http://dgh.dashuyun.cn

Go:   a && b || !c
来源：http://fbx.nanxinkj.top

Ruby: a && b || !c
来源：http://ova.jinqigfzy.top

C#:   a && b || !c
来源：http://civ.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://iqf.yj20258.top

Py:   if not data: return
来源：http://bzq.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://wcc.sysykeji.top

JS:   if (!data) return;
来源：http://wll.fzhhl.top

TS:   if (!data) return;
来源：http://uxc.zycfv.cn

Java: if (data == null) return;
来源：http://vyh.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://cny.jinqigufen.top

Ruby: return if data.nil?
来源：http://lio.tianlin.xyz

C#:   if (data == null) return;
来源：http://zwf.mhx1999.top

================================================================================
来源：http://eon.xziqi.cn

C. 函数与作用域
来源：http://wlp.cashguo.top

================================================================================
来源：http://hmt.jinghuilouyu.cn

[C01] 定义函数
来源：http://fyq.tarul.cn

Py:   def add(a, b): return a + b
来源：http://pkg.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzb.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://odr.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wsi.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gxf.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://oiy.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://wrt.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sfb.ydjk.org.cn

[C02] 默认参数
来源：http://mop.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://aqz.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://sse.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://mxw.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qdb.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cyn.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xhq.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://smv.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://ktl.zhijiandao.cn

[C03] 可变参数
来源：http://bey.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://moj.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tri.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xak.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rog.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://idx.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dcr.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://isy.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efv.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://hrc.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ore.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hzc.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rpx.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yis.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://gwm.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://dpg.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://erm.sweek.top

C#:   f(a: 1, b: 2)
来源：http://omu.shzxlz.cn

[C05] 返回多个值
来源：http://rws.hfpthk.cn

Py:   return a, b
来源：http://zgx.meibo888.top

PHP:  return [$a, $b];
来源：http://gxy.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cuf.dianchejie.cn

TS:   return { a, b };
来源：http://xcj.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://law.fengsongda.top

Go:   return a, b
来源：http://btf.jinyuanbaomall.cn

Ruby: return a, b
来源：http://myd.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://gwm.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://szk.guannengcc.top

Py:   square = lambda x: x * x
来源：http://het.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xxl.aizwys.cn

JS:   const square = x => x * x;
来源：http://wjc.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://khd.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lhk.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://nac.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://udh.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://wvt.nwbrower.top

[C07] 把函数作为参数传入
来源：http://isj.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uyj.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bzu.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://syw.snrcjt.cn

TS:   arr.map(String)
来源：http://fzw.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ldt.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvt.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://mws.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ovi.sxryk.cn

[C08] 闭包
来源：http://grw.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://msv.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://usm.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gqz.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ves.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hoo.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://auj.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jhf.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ilz.yueranfly.top

[C09] 递归
来源：http://lfu.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uyp.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zjf.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbp.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nds.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qmf.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vjh.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://upn.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zar.gaohongyu789.top

[C10] 变量作用域
来源：http://fwj.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nyj.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ktg.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pio.jiagoushi.top

TS:   同 JS
来源：http://pse.zdqjudy.top

Java: 方法内为块级作用域
来源：http://zwl.yongpay.top

Go:   花括号块级作用域
来源：http://kft.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ama.yuanzhike.top

C#:   块级作用域
来源：http://pjr.yongpay.top

[C11] 模块导入与导出
来源：http://agx.smart0.xyz

Py:   from module import func
来源：http://krm.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://emr.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gul.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iny.shzxlz.cn

Java: import java.util.List;
来源：http://ssf.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://flj.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://lzf.tian-w.cn

C#:   using System.Text;
来源：http://dun.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://kse.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://qgp.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://zkq.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://ajm.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://spv.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ree.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://wyc.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://xwl.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vpg.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://aek.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://poq.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://swk.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://axz.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wis.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://wud.hysaishi.cn

Go:   func add(a, b int) int
来源：http://vgj.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eor.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ufd.jlsjyb.cn

[C14] 泛型函数
来源：http://zad.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gkp.bbcook.cn

PHP:  // 无泛型
来源：http://zwr.jinghuilouyu.cn

JS:   // 无泛型
来源：http://mub.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzn.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uuf.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mqw.xuetiantiany.cn

Ruby: # 无泛型
来源：http://wkv.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ozn.aizwys.cn

[C15] 解构 / 展开参数
来源：http://trs.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zhd.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://chv.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://isz.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gry.feifeiyinyue.top

Java: // 无解构
来源：http://kue.yj20258888.top

Go:   // 无解构
来源：http://omt.nanxinkj.top

Ruby: a, b = pair
来源：http://szm.cheryme.top

C#:   var (a, b) = pair;
来源：http://kvr.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://ibt.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gta.shangyingyoupin.top

PHP:  // 无重载
来源：http://duq.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lwz.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://vnr.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ijq.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://vvx.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://ysc.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lrp.cheryme.top

================================================================================
来源：http://bwx.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://jrt.shanyushiyangtech.top

================================================================================
来源：http://nke.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://vqp.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uip.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xbc.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cym.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://pzs.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xyl.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://bxc.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://ddk.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uuz.hcnkem.com

[D02] 追加元素到末尾
来源：http://eic.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lvt.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ley.uphjek.com

JS:   arr.push(4);
来源：http://jpu.hesvh.cn

TS:   arr.push(4);
来源：http://wsd.ivvv.top

Java: list.add(4);
来源：http://dwv.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://jhp.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://kyr.epnwcf.com

C#:   list.Add(4);
来源：http://npa.cucudq.cn

[D03] 在指定位置插入元素
来源：http://bgj.cashguo.top

Py:   arr.insert(0, 0)
来源：http://agb.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eip.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://urf.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://wji.xziqi.cn

Java: list.add(0, 0);
来源：http://mom.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://lxl.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ezk.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://kwv.zhaomingkeji.xyz

[D04] 删除元素
来源：http://sfn.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mgd.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://njt.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ipt.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://lyo.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lpq.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jqc.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gch.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://szg.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://djr.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jfo.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wdg.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hyw.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://wtx.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://kgn.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://sqi.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wlh.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jft.yj202588.top

[D06] 数组长度
来源：http://heg.jianghu66.top

Py:   len(arr)
来源：http://oye.tanke756.top

PHP:  count($arr);
来源：http://qpa.havefunace.top

JS:   arr.length
来源：http://vgh.ywan-chungtsiang.top

TS:   arr.length
来源：http://uar.smart0.xyz

Java: list.size();
来源：http://lfr.jqgfzy.top

Go:   len(arr)
来源：http://dha.hcnkem.com

Ruby: arr.length; arr.size
来源：http://ayf.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://aom.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://roc.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kwn.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://hci.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://tje.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://hrr.gotoacloud.top

Java: list.subList(1, 4);
来源：http://txd.xinyue.icu

Go:   arr[1:4]
来源：http://hqr.tanke756.top

Ruby: arr[1, 3]
来源：http://yti.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://iyv.hfpthk.cn

[D08] 合并两个数组
来源：http://kxn.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://ttc.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://wiy.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rqr.zhongyouzk.top

TS:   [...a, ...b];
来源：http://cdo.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tyf.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://cqw.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://hmr.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://tna.xziqi.cn

[D09] 排序（升序）
来源：http://efz.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://srf.sweek.top

PHP:  sort($arr);
来源：http://dju.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tlt.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kte.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vlx.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qfy.fengsongda.top

Ruby: arr.sort
来源：http://xwp.hnxiangtu.top

C#:   list.Sort();
来源：http://xrb.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dca.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qxq.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oon.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://und.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsp.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rzm.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rqf.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cua.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://buu.xuanzx.com

[D11] 反转数组
来源：http://dth.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://wkt.shuidangran.top

PHP:  array_reverse($arr);
来源：http://lct.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zpq.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://wrf.jqgfzy.top

Java: Collections.reverse(list);
来源：http://mkw.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://jzg.daria6918.cn

Ruby: arr.reverse
来源：http://uey.jlsjyb.cn

C#:   list.Reverse();
来源：http://ahx.zycfv.cn

[D12] 查找元素下标
来源：http://gzv.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://ede.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ylh.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cqb.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xzd.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://irv.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://vqr.yongpay.top

Ruby: arr.index(x)
来源：http://qwa.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://spd.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://aeg.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fwg.sxryk.cn


<!-- 参考信息 -->