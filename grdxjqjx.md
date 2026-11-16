代发 wailian999

PHP:  $a && $b || !$c
来源：http://uzz.guowangkeji.top

JS:   a && b || !c
来源：http://mmk.316326.xyz

TS:   a && b || !c
来源：http://stv.mhx1999.top

Java: a && b || !c
来源：http://kjl.jianghu66.top

Go:   a && b || !c
来源：http://auz.vehdjk.com

Ruby: a && b || !c
来源：http://thp.hysaishi.cn

C#:   a && b || !c
来源：http://buo.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xyl.316326.xyz

Py:   if not data: return
来源：http://vdb.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://eew.vehdjk.com

JS:   if (!data) return;
来源：http://mod.tarul.cn

TS:   if (!data) return;
来源：http://msn.xuanzx.com

Java: if (data == null) return;
来源：http://smc.gaohongyu789.top

Go:   if data == nil { return }
来源：http://pjt.yongpay.top

Ruby: return if data.nil?
来源：http://ehj.gaohongyu789.top

C#:   if (data == null) return;
来源：http://bnc.yj20258888.top

================================================================================
来源：http://fcr.xinyue.icu

C. 函数与作用域
来源：http://zah.shzxlz.cn

================================================================================
来源：http://wvx.aizwys.cn

[C01] 定义函数
来源：http://ill.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://grd.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yoy.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://nzz.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svc.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://czu.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dns.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://csm.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bun.jinqigufen.top

[C02] 默认参数
来源：http://xiz.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://ehj.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xeh.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://ksk.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mje.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ehq.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nsx.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://pff.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://dzi.epnwcf.com

[C03] 可变参数
来源：http://arl.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://vgn.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fsj.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzn.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://odo.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://agh.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kty.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://eir.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cut.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://sgk.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tnd.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qbs.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tei.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yuk.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://jty.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://ayu.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://gyc.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://vah.sxryk.cn

[C05] 返回多个值
来源：http://itm.xuanzx.com

Py:   return a, b
来源：http://dpe.cheryme.top

PHP:  return [$a, $b];
来源：http://osv.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jib.nanxinkj.top

TS:   return { a, b };
来源：http://izx.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vym.shuidangran.top

Go:   return a, b
来源：http://xbc.yuxming.cn

Ruby: return a, b
来源：http://zwr.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://ypp.birdmap.top

[C06] 匿名函数 / lambda
来源：http://sxr.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://eea.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ccz.sufxvd.cn

JS:   const square = x => x * x;
来源：http://nvs.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://uhw.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqz.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nsx.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://yur.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ibd.c1oappe.top

[C07] 把函数作为参数传入
来源：http://wwd.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rqf.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://iao.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vof.316326.xyz

TS:   arr.map(String)
来源：http://zmn.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tci.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ymz.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://yzr.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zop.hammf.cn

[C08] 闭包
来源：http://fni.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kjj.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://upt.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mas.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lpu.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ugg.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jtd.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cbw.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eze.fzhhl.top

[C09] 递归
来源：http://muj.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sng.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eqb.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://slw.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aqa.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://crv.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fis.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hbp.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oqx.sjlbkw.cn

[C10] 变量作用域
来源：http://ohp.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vli.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bgp.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kgu.yuxming.cn

TS:   同 JS
来源：http://jhx.yvedp.cn

Java: 方法内为块级作用域
来源：http://bhz.havefunace.top

Go:   花括号块级作用域
来源：http://mcm.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tbk.guowangkeji.top

C#:   块级作用域
来源：http://rvi.sufxvd.cn

[C11] 模块导入与导出
来源：http://pjc.jinghuilouyu.cn

Py:   from module import func
来源：http://aed.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uch.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vbo.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://use.havefunace.top

Java: import java.util.List;
来源：http://lls.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bhc.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://bch.yfazqb.com

C#:   using System.Text;
来源：http://vmc.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://szt.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://cev.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://ksv.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://dtb.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://unn.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ryw.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://fjw.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://tmw.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cdj.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://fcl.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oxn.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aka.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mfy.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wef.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://lty.guowangkeji.top

Go:   func add(a, b int) int
来源：http://wak.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://veg.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://sfi.mhx1999.top

[C14] 泛型函数
来源：http://jfy.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pol.sxryk.cn

PHP:  // 无泛型
来源：http://roo.hesvh.cn

JS:   // 无泛型
来源：http://htq.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kkv.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ksd.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://okh.sufxvd.cn

Ruby: # 无泛型
来源：http://cic.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tiw.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://ote.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uwn.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://sph.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://scl.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xqg.haohaochexian.top

Java: // 无解构
来源：http://ito.yuxming.cn

Go:   // 无解构
来源：http://rvw.yvedp.cn

Ruby: a, b = pair
来源：http://nfm.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://eox.birdmap.top

[C16] 函数 / 方法重载
来源：http://qpt.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qhp.52xcode.cn

PHP:  // 无重载
来源：http://yxa.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vqq.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://vjo.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cyy.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://qzi.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://ted.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xyr.sufxvd.cn

================================================================================
来源：http://hpe.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://xnu.yongpay.top

================================================================================
来源：http://uke.shuidangran.top

[D01] 创建数组 / 列表
来源：http://akm.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://okv.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uwa.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uqm.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gnk.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yxt.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://hdk.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://zcl.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gmh.hysaishi.cn

[D02] 追加元素到末尾
来源：http://tym.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qds.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kxv.jinqigfzy.top

JS:   arr.push(4);
来源：http://lmg.zycfv.cn

TS:   arr.push(4);
来源：http://qzg.cqqwz.cn

Java: list.add(4);
来源：http://snw.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://hud.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://bon.zdqjudy.top

C#:   list.Add(4);
来源：http://ioe.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://tnm.tanke756.top

Py:   arr.insert(0, 0)
来源：http://hbz.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ays.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pfd.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://nvx.snrcjt.cn

Java: list.add(0, 0);
来源：http://mhd.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eym.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hij.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://zxz.wangshuangyany.cn

[D04] 删除元素
来源：http://kas.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://afr.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bzu.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fnl.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://aci.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvj.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hss.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://umv.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uqa.9152youxi.cn

[D05] 访问与修改元素
来源：http://yre.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uoq.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lwx.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xsj.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://fwf.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://zyf.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://ozd.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://crl.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ycf.tarul.cn

[D06] 数组长度
来源：http://czk.xuetiantiany.cn

Py:   len(arr)
来源：http://eew.zhongyouzk.top

PHP:  count($arr);
来源：http://wfy.nanxuanxn.top

JS:   arr.length
来源：http://tka.mhx1999.top

TS:   arr.length
来源：http://twq.shanyushiyangtech.top

Java: list.size();
来源：http://eai.hesvh.cn

Go:   len(arr)
来源：http://rmb.cashguo.top

Ruby: arr.length; arr.size
来源：http://urm.jinghuilouyu.cn

C#:   list.Count;
来源：http://mat.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://ssv.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gqc.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://xcm.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://trj.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://zjh.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://xxs.guowangkeji.top

Go:   arr[1:4]
来源：http://svr.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://pyp.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://ktl.sufxvd.cn

[D08] 合并两个数组
来源：http://pbq.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://ykw.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://hci.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zkz.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://xzs.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qya.sysykeji.top

Go:   append(a, b...)
来源：http://niz.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://osg.sweek.top

C#:   a.Concat(b).ToList()
来源：http://hoj.jqgfzy.top

[D09] 排序（升序）
来源：http://rsb.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://llw.fktsv.cn

PHP:  sort($arr);
来源：http://zba.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qcw.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iip.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vgi.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://omw.316326.xyz

Ruby: arr.sort
来源：http://pxm.sjlbkw.cn

C#:   list.Sort();
来源：http://ctc.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cjn.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://drd.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkw.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vkd.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mob.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bql.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yip.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xod.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://het.yuxming.cn

[D11] 反转数组
来源：http://puh.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fce.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://nci.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aiy.c1oappe.top

TS:   [...arr].reverse();
来源：http://rkw.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://dei.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://ggy.gaohongyu789.top

Ruby: arr.reverse
来源：http://zvr.ppjwa.cn

C#:   list.Reverse();
来源：http://wgy.zdbjq.cn

[D12] 查找元素下标
来源：http://cdc.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://gjl.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mas.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnm.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://huh.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yrd.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://lbs.hysaishi.cn

Ruby: arr.index(x)
来源：http://flh.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://vjc.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://iwd.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://azm.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rnt.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://zdk.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://rvj.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xom.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ksm.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cma.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://krf.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://aqm.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nmd.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uyt.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://dtr.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://bsp.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rnc.xziqi.cn

Go:   // 手写循环
来源：http://rvc.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://rvc.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kto.yj20258.top

[D15] 去重
来源：http://rbr.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nhg.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://tbg.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://zup.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://qfg.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mah.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://mrd.ydzc1.top

Ruby: arr.uniq
来源：http://djy.jinqigufen.top


<!-- 参考信息 -->