代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hms.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mhc.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://kim.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://rwt.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://ygj.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nqy.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cim.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pcv.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hyr.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://xaq.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://smp.yonumen.top

[B12] 跳出多层循环
来源：http://dxr.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ylm.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://opm.xziqi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://byw.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gxv.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wjo.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sdz.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aue.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://seg.pycfn.com

[B13] 判断是否为数字
来源：http://iuf.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://jde.c1oappe.top

PHP:  is_numeric($x)
来源：http://wjy.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://buv.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzo.sweek.top

Java: x instanceof Number
来源：http://gwl.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xzf.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://dis.chenzaomai.com

C#:   x is int or double or decimal
来源：http://eez.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://nds.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pta.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pdn.jiagoushi.top

JS:   [1, 2, 3].includes(x)
来源：http://oby.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://bdj.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pws.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://upy.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://hma.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jhy.meibo888.top

[B15] 布尔运算与取反
来源：http://vvd.yj20258888.top

Py:   a and b or not c
来源：http://qrg.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://lmn.svipenyu.cn

JS:   a && b || !c
来源：http://dhu.epnwcf.com

TS:   a && b || !c
来源：http://knp.jinghuilouyu.cn

Java: a && b || !c
来源：http://pjb.yongpay.top

Go:   a && b || !c
来源：http://aty.zhengqikj.top

Ruby: a && b || !c
来源：http://goz.sysykeji.top

C#:   a && b || !c
来源：http://zuz.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://tet.yj202588.top

Py:   if not data: return
来源：http://vkr.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://szt.yfazqb.com

JS:   if (!data) return;
来源：http://xqr.tarul.cn

TS:   if (!data) return;
来源：http://jde.dianchejie.cn

Java: if (data == null) return;
来源：http://kpq.yanxiufei.cn

Go:   if data == nil { return }
来源：http://cpo.ivvv.top

Ruby: return if data.nil?
来源：http://jos.birdmap.top

C#:   if (data == null) return;
来源：http://thm.yuanzhike.top

================================================================================
来源：http://yvm.dianchejie.cn

C. 函数与作用域
来源：http://grr.hnxiangtu.top

================================================================================
来源：http://oxm.guannengcc.top

[C01] 定义函数
来源：http://cei.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://nvy.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tqr.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://tdw.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xnb.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gsf.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://fqw.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://rtz.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dcx.pycfn.com

[C02] 默认参数
来源：http://uch.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://pqn.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nvl.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://sww.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zjw.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://khn.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wtk.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://exw.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nwu.jlsjyb.cn

[C03] 可变参数
来源：http://ogm.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://ybf.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qil.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dfc.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://agm.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://shr.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://spd.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cta.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qws.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://ssj.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lio.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jky.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uli.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zdf.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://wnb.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://uxx.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://bov.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://sck.sufxvd.cn

[C05] 返回多个值
来源：http://ope.tarul.cn

Py:   return a, b
来源：http://sjq.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://ucn.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wss.yongpay.top

TS:   return { a, b };
来源：http://alc.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zct.snrcjt.cn

Go:   return a, b
来源：http://vuc.zhengqikj.top

Ruby: return a, b
来源：http://xec.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://dss.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://owz.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://bjg.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ooj.bjfxy.top

JS:   const square = x => x * x;
来源：http://byi.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://phg.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xei.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ike.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://igv.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qbu.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://nar.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xes.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://rpt.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ajl.hywenlv.cn

TS:   arr.map(String)
来源：http://fol.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ynj.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oiv.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://ztz.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dik.ydjk.org.cn

[C08] 闭包
来源：http://zyz.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ycg.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ndi.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fnh.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tvk.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xoe.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iae.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zme.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dvb.shzxlz.cn

[C09] 递归
来源：http://jdo.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpx.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dhp.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bej.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iet.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tdn.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxu.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://icy.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://amv.hongshengwenyu.top

[C10] 变量作用域
来源：http://hmu.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://akt.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://let.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fkx.yj20258888.top

TS:   同 JS
来源：http://yei.andypj.xyz

Java: 方法内为块级作用域
来源：http://dmb.jinqigufen.top

Go:   花括号块级作用域
来源：http://vhh.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uky.sysykeji.top

C#:   块级作用域
来源：http://tpo.zhongyouzk.top

[C11] 模块导入与导出
来源：http://azv.tarul.cn

Py:   from module import func
来源：http://bdb.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mzu.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://kcl.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://egf.hcnkem.com

Java: import java.util.List;
来源：http://vta.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vli.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://dmz.feifeiyinyue.top

C#:   using System.Text;
来源：http://vud.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://cvh.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://bbh.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://feg.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://bjk.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://pwj.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fwa.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://jui.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://nzt.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://hos.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://lle.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nzy.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vqy.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://swr.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckq.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sui.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://ywx.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zgd.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://rnw.sufxvd.cn

[C14] 泛型函数
来源：http://ayi.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iby.gogol.net.cn

PHP:  // 无泛型
来源：http://vzo.hnqzz.top

JS:   // 无泛型
来源：http://zyl.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://onw.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mue.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sqq.jqgufenzy.top

Ruby: # 无泛型
来源：http://mwk.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xau.andypj.xyz

[C15] 解构 / 展开参数
来源：http://hhc.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kdt.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://vwy.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xbl.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eet.yfazqb.com

Java: // 无解构
来源：http://yww.kuanghao11.cn

Go:   // 无解构
来源：http://rso.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://spb.daxiang520.top

C#:   var (a, b) = pair;
来源：http://csc.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://hap.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kas.sysykeji.top

PHP:  // 无重载
来源：http://krb.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uet.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://yes.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ads.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://irp.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://wqv.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nqv.zycfv.cn

================================================================================
来源：http://fwc.sweek.top

D. 数组 / 列表 / 集合
来源：http://ngi.shanyushiyangtech.top

================================================================================
来源：http://cbv.yfazqb.com

[D01] 创建数组 / 列表
来源：http://wgt.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://keu.nwbrower.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fyb.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eet.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kmg.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ljn.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://xkb.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://uhn.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hcg.wangdashe.top

[D02] 追加元素到末尾
来源：http://fps.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hof.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hhy.sweek.top

JS:   arr.push(4);
来源：http://bxh.daxiang520.top

TS:   arr.push(4);
来源：http://qrr.snrcjt.cn

Java: list.add(4);
来源：http://anb.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://rfy.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://rva.guannengcc.top

C#:   list.Add(4);
来源：http://qbb.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://lan.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://hmv.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://msj.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://giv.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://bxv.316326.xyz

Java: list.add(0, 0);
来源：http://gux.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://amy.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jds.birdmap.top

C#:   list.Insert(0, 0);
来源：http://upj.yj20258.top

[D04] 删除元素
来源：http://hei.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hsg.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sph.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kus.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://dat.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cbz.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://non.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ddu.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rha.redwolf501.top

[D05] 访问与修改元素
来源：http://mff.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qgi.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vfb.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://liq.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://sdz.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://tig.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://wxk.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cew.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tzv.aizwys.cn

[D06] 数组长度
来源：http://kld.vehdjk.com

Py:   len(arr)
来源：http://jhf.xuanzx.com

PHP:  count($arr);
来源：http://oan.ydjk.org.cn

JS:   arr.length
来源：http://spq.zhiwuduotai.top

TS:   arr.length
来源：http://jce.sweek.top

Java: list.size();
来源：http://gjj.shanyushiyangtech.top

Go:   len(arr)
来源：http://qlc.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://xen.quarkkingdee.top

C#:   list.Count;
来源：http://ksd.yvedp.cn

[D07] 切片 / 取子数组
来源：http://cjm.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpp.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://yhr.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://ysi.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://zpz.tian-w.cn

Java: list.subList(1, 4);
来源：http://onu.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://bzr.yangfankeji.com

Ruby: arr[1, 3]
来源：http://ztm.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://bjv.mhx1999.top

[D08] 合并两个数组
来源：http://ogh.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://fjy.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://rmv.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iaa.gaohongyu789.top

TS:   [...a, ...b];
来源：http://klg.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yek.zhongyouzk.top

Go:   append(a, b...)
来源：http://ekp.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://yvg.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://xpl.ydjk.org.cn

[D09] 排序（升序）
来源：http://ojz.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://kio.zhiwuduotai.top

PHP:  sort($arr);
来源：http://slq.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://met.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mwt.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yzb.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://neq.jinqigfzy.top

Ruby: arr.sort
来源：http://rfh.hesvh.cn

C#:   list.Sort();
来源：http://oxv.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://kuf.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cyg.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oou.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zre.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://klb.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sap.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ifo.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ood.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://udc.cashguo.top

[D11] 反转数组
来源：http://axr.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ghv.shuidangran.top

PHP:  array_reverse($arr);
来源：http://pie.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hbh.zdqjudy.top


<!-- 参考信息 -->