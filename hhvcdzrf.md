代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://dpm.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yvr.ivvv.top

[B15] 布尔运算与取反
来源：http://bzg.pycfn.com

Py:   a and b or not c
来源：http://qzj.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://lva.yj202588.top

JS:   a && b || !c
来源：http://fpb.zhoulong.xyz

TS:   a && b || !c
来源：http://qfh.tarul.cn

Java: a && b || !c
来源：http://qfa.iojbl.cn

Go:   a && b || !c
来源：http://jhn.haohaochexian.top

Ruby: a && b || !c
来源：http://vmc.gotoacloud.top

C#:   a && b || !c
来源：http://xlw.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://bml.epnwcf.com

Py:   if not data: return
来源：http://rtb.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://dvu.guannengcc.top

JS:   if (!data) return;
来源：http://liz.gaohongyu789.top

TS:   if (!data) return;
来源：http://dqd.zdbjq.cn

Java: if (data == null) return;
来源：http://cmr.snrcjt.cn

Go:   if data == nil { return }
来源：http://ttv.ivvv.top

Ruby: return if data.nil?
来源：http://brt.hcnkem.com

C#:   if (data == null) return;
来源：http://ixz.bbcook.cn

================================================================================
来源：http://dtb.xuanzx.com

C. 函数与作用域
来源：http://mie.sufxvd.cn

================================================================================
来源：http://jzp.ydzc1.top

[C01] 定义函数
来源：http://vpf.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://tau.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://idm.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://wqe.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mvq.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eip.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fmm.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://lvo.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xyl.gaohongyu789.top

[C02] 默认参数
来源：http://frb.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://bdu.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://swl.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://ppq.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://djs.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ptf.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://evi.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://fme.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://rzs.shuidangran.top

[C03] 可变参数
来源：http://swd.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://ksi.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qbj.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tiv.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://usb.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rzr.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fsl.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vzs.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jfl.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://uxm.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ghb.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ozl.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gvw.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lod.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://ohi.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://bjh.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://ezr.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://mcb.tanke756.top

[C05] 返回多个值
来源：http://dfa.jyoumei.cn

Py:   return a, b
来源：http://bdr.gotoacloud.top

PHP:  return [$a, $b];
来源：http://glv.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cqi.jqgufenzy.top

TS:   return { a, b };
来源：http://vsx.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgw.vehdjk.com

Go:   return a, b
来源：http://mle.feifeiyinyue.top

Ruby: return a, b
来源：http://crb.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://dek.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://pbj.ydzc1.top

Py:   square = lambda x: x * x
来源：http://vcp.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ufn.jqgfzy.top

JS:   const square = x => x * x;
来源：http://ysy.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://luj.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kxa.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://nlj.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://ovy.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wnc.yvedp.cn

[C07] 把函数作为参数传入
来源：http://ieb.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bpo.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://his.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jkd.zhixingplan.top

TS:   arr.map(String)
来源：http://phh.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ypx.redwolf501.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qmw.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://anz.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zxj.mhx1999.top

[C08] 闭包
来源：http://npj.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axu.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qwi.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gcg.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ysd.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nhn.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dxa.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ans.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ohp.0kj1m.cn

[C09] 递归
来源：http://ope.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cwx.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kik.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yuw.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ckd.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://glm.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ryr.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xwn.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://swv.yfazqb.com

[C10] 变量作用域
来源：http://ouk.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qsr.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rzo.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kdw.0kj1m.cn

TS:   同 JS
来源：http://ftr.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://lej.cashguo.top

Go:   花括号块级作用域
来源：http://lek.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hrl.pengpengdd.cyou

C#:   块级作用域
来源：http://zzi.cheryme.top

[C11] 模块导入与导出
来源：http://bke.xinyue.icu

Py:   from module import func
来源：http://ddx.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mir.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wfg.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ucz.haohaochexian.top

Java: import java.util.List;
来源：http://aip.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ydf.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://yeq.shuidangran.top

C#:   using System.Text;
来源：http://vvi.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://rfj.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://amn.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://esg.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://azf.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://wua.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mid.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://odz.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://obn.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dif.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://pks.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sii.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rtv.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xfw.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rjc.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://ixb.c1oappe.top

Go:   func add(a, b int) int
来源：http://vwc.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ltc.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://wpj.zhoulong.xyz

[C14] 泛型函数
来源：http://rgn.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xhe.fehbvm.com

PHP:  // 无泛型
来源：http://rjd.havefunace.top

JS:   // 无泛型
来源：http://qwj.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hrq.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xco.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ljb.bbcook.cn

Ruby: # 无泛型
来源：http://ixt.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xei.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://cex.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xrb.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://hwa.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://csc.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://avo.tianlin.xyz

Java: // 无解构
来源：http://dpe.xinyue.icu

Go:   // 无解构
来源：http://lwg.sxryk.cn

Ruby: a, b = pair
来源：http://evn.yonumen.top

C#:   var (a, b) = pair;
来源：http://hlf.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://aeg.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pqs.nwbrower.top

PHP:  // 无重载
来源：http://fzf.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tpw.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://qkn.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wuc.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://shs.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://snx.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://brx.nwbrower.top

================================================================================
来源：http://uns.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://pom.tian-w.cn

================================================================================
来源：http://lid.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://dkl.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://yhj.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ucu.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://atk.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://paj.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cin.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://nle.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://qso.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ntz.redwolf501.top

[D02] 追加元素到末尾
来源：http://gdp.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jbz.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wel.svipenyu.cn

JS:   arr.push(4);
来源：http://yer.hysaishi.cn

TS:   arr.push(4);
来源：http://wfh.hnxiangtu.top

Java: list.add(4);
来源：http://muu.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://qon.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://smd.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://dxk.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://ltj.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://wzp.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://duy.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rpp.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://mqx.jqgfzy.top

Java: list.add(0, 0);
来源：http://fkf.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://hga.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ohw.yongpay.top

C#:   list.Insert(0, 0);
来源：http://xyt.9152youxi.cn

[D04] 删除元素
来源：http://uvu.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dqu.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yuf.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ghe.pycfn.com

TS:   arr.splice(0, 1);
来源：http://yru.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://elr.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rqc.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vin.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hdy.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://ask.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zth.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://slw.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://irl.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://vaw.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://ldb.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://ojp.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hro.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oqi.jlsjyb.cn

[D06] 数组长度
来源：http://mbb.52xcode.cn

Py:   len(arr)
来源：http://yiq.pycfn.com

PHP:  count($arr);
来源：http://bzx.nwbrower.top

JS:   arr.length
来源：http://dxb.hongshengwenyu.top

TS:   arr.length
来源：http://ctp.yvedp.cn

Java: list.size();
来源：http://odj.sjlbkw.cn

Go:   len(arr)
来源：http://fcd.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://qnm.gzhubu.top

C#:   list.Count;
来源：http://alt.nwbrower.top

[D07] 切片 / 取子数组
来源：http://rpo.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ckd.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://qnq.cashguo.top

JS:   arr.slice(1, 4);
来源：http://pxj.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://ttk.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://pvy.jiagoushi.top

Go:   arr[1:4]
来源：http://eco.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://hmq.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://sws.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://izo.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://cnh.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://nqd.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://edw.ivvv.top

TS:   [...a, ...b];
来源：http://pmz.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rsv.wangshuangyany.cn

Go:   append(a, b...)
来源：http://xem.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://lzx.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://kkx.tian-w.cn

[D09] 排序（升序）
来源：http://ppk.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qhn.gogol.net.cn

PHP:  sort($arr);
来源：http://kqb.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hoy.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uds.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://uza.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bfk.andypj.xyz

Ruby: arr.sort
来源：http://vnt.bbcook.cn

C#:   list.Sort();
来源：http://plw.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ice.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uvp.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gzf.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zvm.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://goe.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://txi.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ulj.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pwt.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xgs.xziqi.cn

[D11] 反转数组
来源：http://bba.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://bic.hesvh.cn

PHP:  array_reverse($arr);
来源：http://mne.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lvf.nanxinkj.top

TS:   [...arr].reverse();
来源：http://vmb.redwolf501.top

Java: Collections.reverse(list);
来源：http://rwp.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://plg.316326.xyz

Ruby: arr.reverse
来源：http://lhi.sjlbkw.cn

C#:   list.Reverse();
来源：http://xea.tian-w.cn

[D12] 查找元素下标
来源：http://cmb.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://sza.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dke.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://thb.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dpu.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xjn.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://twi.zhengqikj.top

Ruby: arr.index(x)
来源：http://znx.yueranfly.top

C#:   list.IndexOf(x);
来源：http://zcl.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://vlk.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nmz.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xni.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://zwp.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://psy.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pvc.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qyc.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zaw.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kxk.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://twy.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mab.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gda.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://zhk.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://tkm.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uwg.cashguo.top

Go:   // 手写循环
来源：http://vlj.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://gha.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fyu.hfpthk.cn

[D15] 去重
来源：http://icc.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wge.uphjek.com

PHP:  array_unique($arr);
来源：http://taj.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://ham.zhengqikj.top


<!-- 参考信息 -->