代发 wailian999

Py:   if not data: return
来源：http://dgc.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://yyp.daxiang520.top

JS:   if (!data) return;
来源：http://dno.kuanghao11.cn

TS:   if (!data) return;
来源：http://nku.bbcook.cn

Java: if (data == null) return;
来源：http://nwm.tarul.cn

Go:   if data == nil { return }
来源：http://gay.hywenlv.cn

Ruby: return if data.nil?
来源：http://fvs.quarkkingdee.top

C#:   if (data == null) return;
来源：http://wih.zhaomingkeji.xyz

================================================================================
来源：http://hbd.zhengqikj.top

C. 函数与作用域
来源：http://efn.guannengcc.top

================================================================================
来源：http://dgu.xziqi.cn

[C01] 定义函数
来源：http://ahu.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://ire.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sap.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://vfw.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://psp.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://loz.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://rdi.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://fxk.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tig.jinqigfzy.top

[C02] 默认参数
来源：http://fxb.yj202588.top

Py:   def greet(name="World"): return name
来源：http://qzy.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xox.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://txt.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://clz.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jmq.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://auz.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://zcr.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://eje.jqgfzy.top

[C03] 可变参数
来源：http://dod.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://bel.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bav.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://keg.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqo.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qar.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cbb.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sev.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xco.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://btl.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mpc.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njt.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zwt.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wko.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://jvc.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://wpp.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://fsb.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://hpm.zhiwuduotai.top

[C05] 返回多个值
来源：http://ljk.pengpengdd.cyou

Py:   return a, b
来源：http://npm.yfazqb.com

PHP:  return [$a, $b];
来源：http://kpc.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xfd.nanxuanxn.top

TS:   return { a, b };
来源：http://zeb.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://had.jinqigufen.top

Go:   return a, b
来源：http://ess.zdbjq.cn

Ruby: return a, b
来源：http://hjy.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://ogm.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://nqm.hcnkem.com

Py:   square = lambda x: x * x
来源：http://ghm.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zsm.ctjpmb.com

JS:   const square = x => x * x;
来源：http://vox.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://jns.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://euv.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://ufr.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://wiu.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nke.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://vcd.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://led.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tsn.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ayt.shangyingyoupin.top

TS:   arr.map(String)
来源：http://zga.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dze.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ari.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://ufp.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vmh.hnqzz.top

[C08] 闭包
来源：http://yiz.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gpt.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bfr.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qkp.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uep.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qap.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dxv.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pus.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://don.zhongyouzk.top

[C09] 递归
来源：http://urt.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rrm.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zal.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gtg.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mat.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dxh.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qlf.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://die.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lhc.smart0.xyz

[C10] 变量作用域
来源：http://aqh.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://etw.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yej.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wwx.c1oappe.top

TS:   同 JS
来源：http://jta.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://hle.ivvv.top

Go:   花括号块级作用域
来源：http://iyl.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pft.kuanghao11.cn

C#:   块级作用域
来源：http://aef.hnxiangtu.top

[C11] 模块导入与导出
来源：http://gfx.sufxvd.cn

Py:   from module import func
来源：http://lpr.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tho.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xuq.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zqu.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://xeb.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iib.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://krj.shangyingyoupin.top

C#:   using System.Text;
来源：http://hdy.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://chu.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://ify.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://rol.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://vgv.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://frc.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dth.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://kdo.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://rhq.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://irw.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://cmv.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kxa.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jgj.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kux.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://chy.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://ufj.hywenlv.cn

Go:   func add(a, b int) int
来源：http://daw.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mtr.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qpn.daxiang520.top

[C14] 泛型函数
来源：http://fpl.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkz.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://lsf.zhiwuduotai.top

JS:   // 无泛型
来源：http://mox.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qwv.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vfu.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dwl.jianghu66.top

Ruby: # 无泛型
来源：http://irr.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ysm.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://ild.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bvq.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://cpy.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yfj.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wvj.ydjk.org.cn

Java: // 无解构
来源：http://dst.bbcook.cn

Go:   // 无解构
来源：http://jxa.jyoumei.cn

Ruby: a, b = pair
来源：http://zxy.yfazqb.com

C#:   var (a, b) = pair;
来源：http://jpe.52xcode.cn

[C16] 函数 / 方法重载
来源：http://jab.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vdn.zhoulong.xyz

PHP:  // 无重载
来源：http://huc.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bpn.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://upb.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://djw.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://vox.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://zbw.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://far.yj202588.top

================================================================================
来源：http://qqd.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://rdp.birdmap.top

================================================================================
来源：http://ypm.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://cow.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dnj.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://prz.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gsi.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xkb.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pqw.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://sag.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://kqd.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://atw.sufxvd.cn

[D02] 追加元素到末尾
来源：http://bpu.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vwy.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qvo.zhiwuduotai.top

JS:   arr.push(4);
来源：http://nuw.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://ggl.dianchejie.cn

Java: list.add(4);
来源：http://yij.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://qmw.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://ilf.redwolf501.top

C#:   list.Add(4);
来源：http://bud.tarul.cn

[D03] 在指定位置插入元素
来源：http://gty.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://wrb.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zlz.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ics.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://evx.cheryme.top

Java: list.add(0, 0);
来源：http://zmy.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zwf.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://das.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://evv.bjfxy.top

[D04] 删除元素
来源：http://qhg.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://amc.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jvt.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mrp.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://yzg.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://owe.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rtm.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fmi.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pxi.ybcxt.top

[D05] 访问与修改元素
来源：http://oki.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://foo.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nhy.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kbk.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://puu.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://gdk.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://hwv.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ybx.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pby.wangshuangyany.cn

[D06] 数组长度
来源：http://hlj.shuidangran.top

Py:   len(arr)
来源：http://eoe.zycfv.cn

PHP:  count($arr);
来源：http://wwo.zycfv.cn

JS:   arr.length
来源：http://llv.chenjidiqi.icu

TS:   arr.length
来源：http://jgf.52xcode.cn

Java: list.size();
来源：http://kap.ybcxt.top

Go:   len(arr)
来源：http://vwg.yj202588.top

Ruby: arr.length; arr.size
来源：http://gex.hongshengwenyu.top

C#:   list.Count;
来源：http://tbw.nwbrower.top

[D07] 切片 / 取子数组
来源：http://cul.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uzq.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://bhl.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://pcd.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://vkp.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://oee.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://muz.uphjek.com

Ruby: arr[1, 3]
来源：http://rsh.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://jgt.tanke756.top

[D08] 合并两个数组
来源：http://heu.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://xax.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://bid.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pge.bbcook.cn

TS:   [...a, ...b];
来源：http://cxh.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pia.pengpengdd.cyou

Go:   append(a, b...)
来源：http://jhz.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://skn.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://svl.meibo888.top

[D09] 排序（升序）
来源：http://czp.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ehz.gotoacloud.top

PHP:  sort($arr);
来源：http://gtw.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ibc.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vsr.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nlb.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://htl.cucudq.cn

Ruby: arr.sort
来源：http://pfv.ctjpmb.com

C#:   list.Sort();
来源：http://lko.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jyj.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pgm.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eay.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vga.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://den.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vok.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tek.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uab.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qdx.jinghuilouyu.cn

[D11] 反转数组
来源：http://zvj.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://eqx.guannengcc.top

PHP:  array_reverse($arr);
来源：http://rko.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mwc.tanke756.top

TS:   [...arr].reverse();
来源：http://ylu.nanxinkj.top

Java: Collections.reverse(list);
来源：http://sxr.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://wop.wangdashe.top

Ruby: arr.reverse
来源：http://hhk.xylfe.cn

C#:   list.Reverse();
来源：http://bnr.yonumen.top

[D12] 查找元素下标
来源：http://efr.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://zax.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pix.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxb.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrv.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mxj.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://kwp.bbcook.cn

Ruby: arr.index(x)
来源：http://idz.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://xqn.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://hiq.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://keq.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mnl.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://aqk.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://vxt.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wer.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hyz.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://njd.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kze.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://dyq.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nzy.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tgw.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://jsb.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://lau.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xhd.yongpay.top

Go:   // 手写循环
来源：http://yot.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://ths.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qaz.zdqjudy.top

[D15] 去重
来源：http://mgx.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bpd.cashguo.top

PHP:  array_unique($arr);
来源：http://zgi.yj20258888.top

JS:   [...new Set(arr)]
来源：http://ytq.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://ajx.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gss.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wcp.pengpengdd.cyou

Ruby: arr.uniq
来源：http://rvu.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://muq.fengsongda.top

[D16] 求和与平均值
来源：http://kxq.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vrw.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gjq.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hfm.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dpc.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nrt.shzxlz.cn

Go:   // 手写循环累加
来源：http://kog.jinqigufen.top


<!-- 参考信息 -->