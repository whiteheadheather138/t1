代发 wailian999

Py:   if not data: return
来源：http://lly.hongshengwenyu.top

PHP:  if (!$data) { return; }
来源：http://zkc.meibo888.top

JS:   if (!data) return;
来源：http://vyw.vehdjk.com

TS:   if (!data) return;
来源：http://brf.jiagoushi.top

Java: if (data == null) return;
来源：http://ims.guannengcc.top

Go:   if data == nil { return }
来源：http://zkl.tian-w.cn

Ruby: return if data.nil?
来源：http://hhi.cheryme.top

C#:   if (data == null) return;
来源：http://qia.dashuyun.cn

================================================================================
来源：http://yyn.yj202588.top

C. 函数与作用域
来源：http://rah.shuidangran.top

================================================================================
来源：http://azm.tanke756.top

[C01] 定义函数
来源：http://izu.tarul.cn

Py:   def add(a, b): return a + b
来源：http://pfs.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ywv.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://nja.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qxb.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fqn.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://zae.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://vwp.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bdj.bjfxy.top

[C02] 默认参数
来源：http://hoy.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://gsh.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sci.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://shj.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wfi.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rvk.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oxr.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://mnh.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://ftb.chenzaomai.com

[C03] 可变参数
来源：http://ttn.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://jaj.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ddn.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nfr.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://teq.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oke.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xej.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fgt.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://frf.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://ghl.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eac.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qea.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zth.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xot.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://hvs.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://ujc.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://hlo.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://ufj.shzxlz.cn

[C05] 返回多个值
来源：http://dim.guannengcc.top

Py:   return a, b
来源：http://iwv.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://kba.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mej.cashguo.top

TS:   return { a, b };
来源：http://xoh.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://djp.wangshuangyany.cn

Go:   return a, b
来源：http://ldh.yuxming.cn

Ruby: return a, b
来源：http://xsc.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://ymo.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://bil.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://jyk.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aww.aizwys.cn

JS:   const square = x => x * x;
来源：http://cxy.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://qrj.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://quz.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://gep.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://szv.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jja.aizwys.cn

[C07] 把函数作为参数传入
来源：http://wgn.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wxx.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://ido.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nqv.yj20258888.top

TS:   arr.map(String)
来源：http://tiz.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fsh.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ndw.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://orm.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vpe.jqgfzy.top

[C08] 闭包
来源：http://tam.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kno.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://giq.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://acc.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gin.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mwb.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qoj.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cbl.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bus.guowangkeji.top

[C09] 递归
来源：http://nqp.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://auv.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lvm.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixc.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iia.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mao.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yzi.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mzv.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jqn.aibaodan.cn

[C10] 变量作用域
来源：http://kfc.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bww.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tqy.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lmv.redwolf501.top

TS:   同 JS
来源：http://dcx.birdmap.top

Java: 方法内为块级作用域
来源：http://dac.xuanzx.com

Go:   花括号块级作用域
来源：http://sjy.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iau.hfpthk.cn

C#:   块级作用域
来源：http://xvi.ppjwa.cn

[C11] 模块导入与导出
来源：http://yrh.hnqzz.top

Py:   from module import func
来源：http://ffz.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wwq.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hgt.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eqb.aibaodan.cn

Java: import java.util.List;
来源：http://zea.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogc.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://pkv.hfpthk.cn

C#:   using System.Text;
来源：http://vpz.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://nwb.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://juq.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://wjq.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://waj.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://xui.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jvv.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://jyk.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://xbk.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://agk.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://oil.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rjt.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vvh.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oad.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yyj.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://eco.52xcode.cn

Go:   func add(a, b int) int
来源：http://xmu.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ajd.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://xvj.aibaodan.cn

[C14] 泛型函数
来源：http://xkz.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://khi.meibo888.top

PHP:  // 无泛型
来源：http://nhe.zhoulong.xyz

JS:   // 无泛型
来源：http://jeb.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://utz.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ilb.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://plh.wangshuangyany.cn

Ruby: # 无泛型
来源：http://xkd.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cjb.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://tgk.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://otb.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://uys.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kek.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sus.yueranfly.top

Java: // 无解构
来源：http://bhj.fehbvm.com

Go:   // 无解构
来源：http://zhs.zhengqikj.top

Ruby: a, b = pair
来源：http://xpd.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://brs.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://gvl.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jxx.cheryme.top

PHP:  // 无重载
来源：http://bkd.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://led.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://taq.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hho.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://uar.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://gcf.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://niu.vehdjk.com

================================================================================
来源：http://ghz.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://ltg.redwolf501.top

================================================================================
来源：http://ceg.hcnkem.com

[D01] 创建数组 / 列表
来源：http://pni.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tfj.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qrg.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zhp.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zzk.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zyy.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://dnc.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://jre.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lyp.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://fvt.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ewv.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://idr.cqqwz.cn

JS:   arr.push(4);
来源：http://wdv.yj20258.top

TS:   arr.push(4);
来源：http://mpc.hammf.cn

Java: list.add(4);
来源：http://ijw.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://sqv.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://lvc.ydzc1.top

C#:   list.Add(4);
来源：http://giv.fzhhl.top

[D03] 在指定位置插入元素
来源：http://tlk.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://qgz.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://moz.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ibv.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://qtu.c1oappe.top

Java: list.add(0, 0);
来源：http://cnq.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://xaw.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kum.yj20258.top

C#:   list.Insert(0, 0);
来源：http://sji.chenlongwang.top

[D04] 删除元素
来源：http://oxt.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://thj.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sjs.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kgs.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://qau.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://coc.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://twx.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yzc.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zfm.ppjwa.cn

[D05] 访问与修改元素
来源：http://rzy.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qrz.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zbw.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wij.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cjw.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://kwx.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://cbx.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wxz.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zdt.zhiwuduotai.top

[D06] 数组长度
来源：http://bej.yfazqb.com

Py:   len(arr)
来源：http://ufm.jinqigfzy.top

PHP:  count($arr);
来源：http://qlw.chenlongwang.top

JS:   arr.length
来源：http://pus.hongshengwenyu.top

TS:   arr.length
来源：http://tqj.sufxvd.cn

Java: list.size();
来源：http://ywf.wangdashe.top

Go:   len(arr)
来源：http://sqd.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://okd.gogol.net.cn

C#:   list.Count;
来源：http://rhd.meibo888.top

[D07] 切片 / 取子数组
来源：http://epi.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://clh.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ava.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://xxt.hammf.cn

TS:   arr.slice(1, 4);
来源：http://mgi.fzhhl.top

Java: list.subList(1, 4);
来源：http://lwn.ppjwa.cn

Go:   arr[1:4]
来源：http://bju.cashguo.top

Ruby: arr[1, 3]
来源：http://utv.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://boh.fktsv.cn

[D08] 合并两个数组
来源：http://bzw.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://rdr.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://fxd.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dss.bbcook.cn

TS:   [...a, ...b];
来源：http://ewx.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zcr.tian-w.cn

Go:   append(a, b...)
来源：http://xus.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://esb.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://mdo.aizwys.cn

[D09] 排序（升序）
来源：http://odi.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://wum.jyoumei.cn

PHP:  sort($arr);
来源：http://bgo.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://crx.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dqx.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://vxx.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ztq.yj20258.top

Ruby: arr.sort
来源：http://pvu.pycfn.com

C#:   list.Sort();
来源：http://niz.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aep.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mnm.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hbv.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://upb.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nir.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://saw.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rvz.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ltx.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gyr.sweek.top

[D11] 反转数组
来源：http://aeq.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://vrd.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://xdp.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vig.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://rrl.hcnkem.com

Java: Collections.reverse(list);
来源：http://avk.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://wxt.jqgfzy.top

Ruby: arr.reverse
来源：http://zoy.hnqzz.top

C#:   list.Reverse();
来源：http://ivn.cdnleiting.top

[D12] 查找元素下标
来源：http://caj.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://yvb.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xsj.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://myq.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzv.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ldg.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://jhc.yuxming.cn

Ruby: arr.index(x)
来源：http://kqn.cashguo.top

C#:   list.IndexOf(x);
来源：http://qeb.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://fek.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cjc.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hcq.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://cbg.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://gcs.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ixo.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ysf.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yja.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tpr.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://wnr.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rrp.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zep.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://dmk.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://gue.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://maf.yuanzhike.top

Go:   // 手写循环
来源：http://mot.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mni.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://yte.pycfn.com

[D15] 去重
来源：http://duo.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dky.jiagoushi.top

PHP:  array_unique($arr);
来源：http://fgi.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://ovx.aizwys.cn

TS:   [...new Set(arr)]
来源：http://jbj.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wtc.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://ggh.yonumen.top

Ruby: arr.uniq
来源：http://rji.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://qvp.hongshengwenyu.top

[D16] 求和与平均值
来源：http://gun.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bpj.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pmw.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yos.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jub.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urm.shzxlz.cn

Go:   // 手写循环累加
来源：http://lch.jlsjyb.cn


<!-- 参考信息 -->