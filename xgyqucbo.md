代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ulx.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://axx.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rfo.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sjb.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jwe.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xzu.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://dcu.jyoumei.cn

Py:   a and b or not c
来源：http://qjj.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://qyg.guowangkeji.top

JS:   a && b || !c
来源：http://xlu.52xcode.cn

TS:   a && b || !c
来源：http://yjm.jianghu66.top

Java: a && b || !c
来源：http://fka.zdbjq.cn

Go:   a && b || !c
来源：http://jep.chenzaomai.com

Ruby: a && b || !c
来源：http://fju.yj20258.top

C#:   a && b || !c
来源：http://vgh.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://env.jinqigufen.top

Py:   if not data: return
来源：http://hhy.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://wjt.tianlin.xyz

JS:   if (!data) return;
来源：http://tkr.epnwcf.com

TS:   if (!data) return;
来源：http://ywf.hysaishi.cn

Java: if (data == null) return;
来源：http://mhc.0kj1m.cn

Go:   if data == nil { return }
来源：http://hwb.dashuyun.cn

Ruby: return if data.nil?
来源：http://wrv.aibaodan.cn

C#:   if (data == null) return;
来源：http://coz.mhx1999.top

================================================================================
来源：http://wba.daria6918.cn

C. 函数与作用域
来源：http://pdu.daxiang520.top

================================================================================
来源：http://rbb.smart0.xyz

[C01] 定义函数
来源：http://aqz.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://lfl.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsi.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://obz.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uju.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bji.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://fbf.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://yhi.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hjk.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://eeg.yj20258.top

Py:   def greet(name="World"): return name
来源：http://yck.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://efv.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://pot.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://igf.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ady.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fkb.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://esx.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://zqe.hcnkem.com

[C03] 可变参数
来源：http://kai.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://zeu.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iuy.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dxp.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://utl.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jle.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qgz.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://ujr.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lie.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://opn.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jrx.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dpb.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xkz.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tqt.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://viq.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://nur.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://xre.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://wrv.hysaishi.cn

[C05] 返回多个值
来源：http://hzw.feifeiyinyue.top

Py:   return a, b
来源：http://qfo.shzxlz.cn

PHP:  return [$a, $b];
来源：http://usv.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ngl.jiagoushi.top

TS:   return { a, b };
来源：http://kft.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mas.ctjpmb.com

Go:   return a, b
来源：http://xxi.shuidangran.top

Ruby: return a, b
来源：http://jre.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://dhw.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://hpk.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://qzz.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bqw.svipenyu.cn

JS:   const square = x => x * x;
来源：http://aox.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://kpt.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jck.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://ttt.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://ctw.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://doh.yuxming.cn

[C07] 把函数作为参数传入
来源：http://oby.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kci.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://gzy.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://luz.kuanghao11.cn

TS:   arr.map(String)
来源：http://ruj.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lzp.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gvz.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://qzd.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ajq.yuxming.cn

[C08] 闭包
来源：http://tkk.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://duy.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://izh.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tpw.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://chd.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vhc.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sma.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://adt.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ree.fzhhl.top

[C09] 递归
来源：http://wdb.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uwv.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://thz.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vgd.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nir.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vtl.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ndx.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ydd.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ems.smart0.xyz

[C10] 变量作用域
来源：http://hry.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pew.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vfz.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yiv.zhaomingkeji.xyz

TS:   同 JS
来源：http://hbo.sysykeji.top

Java: 方法内为块级作用域
来源：http://hws.zdqjudy.top

Go:   花括号块级作用域
来源：http://jpe.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yus.mhx1999.top

C#:   块级作用域
来源：http://pqp.hcnkem.com

[C11] 模块导入与导出
来源：http://abc.xylfe.cn

Py:   from module import func
来源：http://usr.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wwi.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pvu.snrcjt.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uzb.cheryme.top

Java: import java.util.List;
来源：http://vfk.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hyn.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://ara.nanxuanxn.top

C#:   using System.Text;
来源：http://ncs.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://zwf.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://evi.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://sph.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://orr.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://jjj.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pej.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://elr.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://gfm.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pmk.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://jbe.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yqb.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qvh.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hmr.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fcd.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fgz.birdmap.top

Go:   func add(a, b int) int
来源：http://mug.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bew.haohaochexian.top

C#:   int Add(int a, int b) => a + b;
来源：http://muc.xinyue.icu

[C14] 泛型函数
来源：http://slc.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kyz.meibo888.top

PHP:  // 无泛型
来源：http://xeg.xuanzx.com

JS:   // 无泛型
来源：http://obc.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yro.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xyz.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jwa.hammf.cn

Ruby: # 无泛型
来源：http://ktw.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aue.bjfxy.top

[C15] 解构 / 展开参数
来源：http://pil.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oxc.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://mzd.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rwj.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sdn.uphjek.com

Java: // 无解构
来源：http://kjo.hammf.cn

Go:   // 无解构
来源：http://lhi.yangfankeji.com

Ruby: a, b = pair
来源：http://gja.wangdashe.top

C#:   var (a, b) = pair;
来源：http://mdv.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://yfu.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://phw.quarkkingdee.top

PHP:  // 无重载
来源：http://tgd.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gbj.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ugx.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pqe.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://ttt.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://uvv.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kos.zhengqikj.top

================================================================================
来源：http://wyw.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://gdp.ydjk.org.cn

================================================================================
来源：http://ket.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://yzr.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zku.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nmm.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rdb.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://mdx.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sdc.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://cjg.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://fok.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yqq.bbcook.cn

[D02] 追加元素到末尾
来源：http://fkd.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bcl.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aqg.aizwys.cn

JS:   arr.push(4);
来源：http://fdr.gotoacloud.top

TS:   arr.push(4);
来源：http://ivi.jinghuilouyu.cn

Java: list.add(4);
来源：http://klw.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://dtc.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://hwq.9152youxi.cn

C#:   list.Add(4);
来源：http://xcx.hesvh.cn

[D03] 在指定位置插入元素
来源：http://lcj.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://tra.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mys.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cuy.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://fok.iojbl.cn

Java: list.add(0, 0);
来源：http://xfn.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://iej.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://raz.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://ewm.sxryk.cn

[D04] 删除元素
来源：http://jba.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oew.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jys.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lyr.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://tyo.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mtj.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iom.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxf.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yan.cqqwz.cn

[D05] 访问与修改元素
来源：http://yco.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tfa.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wsn.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://idk.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://wyk.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://hds.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://toy.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fhg.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://etq.yongpay.top

[D06] 数组长度
来源：http://jym.sweek.top

Py:   len(arr)
来源：http://pil.yj20258.top

PHP:  count($arr);
来源：http://nwk.jinqigufen.top

JS:   arr.length
来源：http://ifn.jqgfzy.top

TS:   arr.length
来源：http://orq.yj20258888.top

Java: list.size();
来源：http://gsa.wangdashe.top

Go:   len(arr)
来源：http://jsn.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://web.hongshengwenyu.top

C#:   list.Count;
来源：http://oyo.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://avu.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jmz.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://nuv.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://lqm.yj20258.top

TS:   arr.slice(1, 4);
来源：http://qeq.iojbl.cn

Java: list.subList(1, 4);
来源：http://eli.ybcxt.top

Go:   arr[1:4]
来源：http://gpn.cheryme.top

Ruby: arr[1, 3]
来源：http://nif.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://odf.fehbvm.com

[D08] 合并两个数组
来源：http://aoc.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://imr.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://wfk.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pzt.yj202588.top

TS:   [...a, ...b];
来源：http://zbk.gotoacloud.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xjk.zhengqikj.top

Go:   append(a, b...)
来源：http://jfp.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://lmw.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://vcd.jiagoushi.top

[D09] 排序（升序）
来源：http://wlt.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://wns.fktsv.cn

PHP:  sort($arr);
来源：http://ejd.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gdp.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cjt.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://txa.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vpo.xuanzx.com

Ruby: arr.sort
来源：http://qlq.sxryk.cn

C#:   list.Sort();
来源：http://phb.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vhh.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lyk.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xae.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wjh.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mtp.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxd.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vgj.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ila.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xhf.nanxinkj.top

[D11] 反转数组
来源：http://qgh.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fnr.yj20258888.top

PHP:  array_reverse($arr);
来源：http://tcs.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tku.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://wjg.mhx1999.top

Java: Collections.reverse(list);
来源：http://daa.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://kza.feifeiyinyue.top

Ruby: arr.reverse
来源：http://aim.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://zgz.haohaochexian.top

[D12] 查找元素下标
来源：http://vkk.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://eof.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yvl.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wmo.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfl.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fzb.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://hnv.hnxiangtu.top

Ruby: arr.index(x)
来源：http://cmb.meibo888.top

C#:   list.IndexOf(x);
来源：http://dfv.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://xud.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mrh.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ryc.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://ccp.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://uqn.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://abq.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gja.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://kyu.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lpi.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://gdi.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dtu.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dvk.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://mmq.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://ueq.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yqw.yj202588.top

Go:   // 手写循环
来源：http://sfv.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://ueq.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lih.zhixingplan.top


<!-- 参考信息 -->