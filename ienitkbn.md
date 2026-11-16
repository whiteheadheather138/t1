代发 wailian999

PHP:  $a && $b || !$c
来源：http://igk.ppjwa.cn

JS:   a && b || !c
来源：http://uwk.xuetiantiany.cn

TS:   a && b || !c
来源：http://vjr.hywenlv.cn

Java: a && b || !c
来源：http://kmk.chenlongwang.top

Go:   a && b || !c
来源：http://tky.jqgufenzy.top

Ruby: a && b || !c
来源：http://msb.zdbjq.cn

C#:   a && b || !c
来源：http://bsr.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gyt.c1oappe.top

Py:   if not data: return
来源：http://jsa.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://xar.snrcjt.cn

JS:   if (!data) return;
来源：http://hqd.ppjwa.cn

TS:   if (!data) return;
来源：http://dpy.dianchejie.cn

Java: if (data == null) return;
来源：http://urg.nanxuanxn.top

Go:   if data == nil { return }
来源：http://zog.hnqzz.top

Ruby: return if data.nil?
来源：http://rpo.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://puz.iojbl.cn

================================================================================
来源：http://aeu.bbcook.cn

C. 函数与作用域
来源：http://dar.sweek.top

================================================================================
来源：http://pfm.smart0.xyz

[C01] 定义函数
来源：http://kmv.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://txm.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pti.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://zcw.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gxp.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fqa.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dfp.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://iyy.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hsb.hfpthk.cn

[C02] 默认参数
来源：http://vgw.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://qyt.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cbq.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://roz.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dby.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gns.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qae.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://iat.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://iyk.xziqi.cn

[C03] 可变参数
来源：http://dnp.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://hdg.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eyq.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://krx.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://psm.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sjk.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://txv.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aas.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zty.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://cnl.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lhj.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cjj.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jlb.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lez.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://kjs.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://oxc.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://rwq.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://ovf.haohaochexian.top

[C05] 返回多个值
来源：http://esd.chenjidiqi.icu

Py:   return a, b
来源：http://itd.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://xcs.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://wdi.yj20258.top

TS:   return { a, b };
来源：http://hyo.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qak.hnqzz.top

Go:   return a, b
来源：http://wls.sxryk.cn

Ruby: return a, b
来源：http://nfj.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://xsh.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://jbn.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://cgt.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rcr.zdbjq.cn

JS:   const square = x => x * x;
来源：http://eas.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://bij.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kjr.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vzi.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://odg.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://tqb.tanke756.top

[C07] 把函数作为参数传入
来源：http://drr.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://elp.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://hal.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xjt.iojbl.cn

TS:   arr.map(String)
来源：http://ugy.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ugf.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rlu.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://uso.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://swp.guowangkeji.top

[C08] 闭包
来源：http://azb.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wkn.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tep.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qfo.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ysy.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://snt.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nzv.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tis.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sgk.haohaochexian.top

[C09] 递归
来源：http://fam.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://riw.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://azm.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wnq.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://noe.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vjs.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bgl.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aqs.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hfm.yfazqb.com

[C10] 变量作用域
来源：http://pjo.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kxt.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ymo.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://inf.ehwqpu.com

TS:   同 JS
来源：http://qve.tian-w.cn

Java: 方法内为块级作用域
来源：http://its.wangdashe.top

Go:   花括号块级作用域
来源：http://vab.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://prx.meibo888.top

C#:   块级作用域
来源：http://dvj.fehbvm.com

[C11] 模块导入与导出
来源：http://fbk.hcnkem.com

Py:   from module import func
来源：http://qbp.birdmap.top

PHP:  require "file.php";  或 use App\Service;
来源：http://riu.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ptg.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qeq.xuetiantiany.cn

Java: import java.util.List;
来源：http://mbj.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bxf.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://ijj.havefunace.top

C#:   using System.Text;
来源：http://zhi.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://moi.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://phg.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://mzt.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://yql.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://rzv.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vkh.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://hgg.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://cth.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pyu.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://hbp.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wso.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vde.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uno.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iqv.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fbi.dianchejie.cn

Go:   func add(a, b int) int
来源：http://mst.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zdh.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zqu.fktsv.cn

[C14] 泛型函数
来源：http://ktn.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pgr.sjlbkw.cn

PHP:  // 无泛型
来源：http://unb.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://vwg.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aph.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qoz.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nid.xylfe.cn

Ruby: # 无泛型
来源：http://ktu.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dxy.fengsongda.top

[C15] 解构 / 展开参数
来源：http://ljm.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fzd.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://ezs.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fyt.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://azs.vehdjk.com

Java: // 无解构
来源：http://lcz.dashuyun.cn

Go:   // 无解构
来源：http://orc.sysykeji.top

Ruby: a, b = pair
来源：http://bqv.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://ohl.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://bbn.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wby.cashguo.top

PHP:  // 无重载
来源：http://vno.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://yhv.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://krp.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://kmb.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://vro.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://igu.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rbo.shzxlz.cn

================================================================================
来源：http://bzj.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://bhv.tanke756.top

================================================================================
来源：http://mih.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://yjs.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uuz.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mjl.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uky.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vex.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cds.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://myn.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://fwf.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aza.cqqwz.cn

[D02] 追加元素到末尾
来源：http://yeo.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://slp.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sdd.zdbjq.cn

JS:   arr.push(4);
来源：http://ifm.fengsongda.top

TS:   arr.push(4);
来源：http://zcn.gotoacloud.top

Java: list.add(4);
来源：http://zkf.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://xvd.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://zfe.hcnkem.com

C#:   list.Add(4);
来源：http://omq.tanke756.top

[D03] 在指定位置插入元素
来源：http://qwh.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://asv.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pux.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gcu.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://irp.cdnleiting.top

Java: list.add(0, 0);
来源：http://nce.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mbb.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dzx.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://yka.cqqwz.cn

[D04] 删除元素
来源：http://zcr.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ysy.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xfx.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ffi.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://vns.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ifs.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mco.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xzi.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lik.tanke756.top

[D05] 访问与修改元素
来源：http://cxz.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://otl.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://agq.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oos.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://kcx.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://qwo.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://lkn.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vkq.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hkj.jinqigfzy.top

[D06] 数组长度
来源：http://wnt.sysykeji.top

Py:   len(arr)
来源：http://zvk.jiagoushi.top

PHP:  count($arr);
来源：http://sef.daria6918.cn

JS:   arr.length
来源：http://ngh.yj20258888.top

TS:   arr.length
来源：http://meq.sxryk.cn

Java: list.size();
来源：http://idb.tian-w.cn

Go:   len(arr)
来源：http://wbe.redwolf501.top

Ruby: arr.length; arr.size
来源：http://itf.yuxming.cn

C#:   list.Count;
来源：http://pxp.yj20258.top

[D07] 切片 / 取子数组
来源：http://olb.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ybq.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dmq.birdmap.top

JS:   arr.slice(1, 4);
来源：http://xuc.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://uzg.guowangkeji.top

Java: list.subList(1, 4);
来源：http://qyo.52xcode.cn

Go:   arr[1:4]
来源：http://sdh.fzhhl.top

Ruby: arr[1, 3]
来源：http://eyv.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://kiz.sufxvd.cn

[D08] 合并两个数组
来源：http://whc.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://kcm.316326.xyz

PHP:  array_merge($a, $b);
来源：http://gif.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://okf.ivvv.top

TS:   [...a, ...b];
来源：http://gqs.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lbb.mhx1999.top

Go:   append(a, b...)
来源：http://qhd.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://mnb.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://haw.fehbvm.com

[D09] 排序（升序）
来源：http://iic.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sez.daxiang520.top

PHP:  sort($arr);
来源：http://egm.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wse.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bzs.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wea.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bnx.zhiwuduotai.top

Ruby: arr.sort
来源：http://dkd.jiagoushi.top

C#:   list.Sort();
来源：http://mwo.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sbu.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kqa.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bqm.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzl.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dtz.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bdu.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://grp.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xet.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vvw.0kj1m.cn

[D11] 反转数组
来源：http://hig.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://frk.xziqi.cn

PHP:  array_reverse($arr);
来源：http://rio.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bez.hywenlv.cn

TS:   [...arr].reverse();
来源：http://ejm.yj20258.top

Java: Collections.reverse(list);
来源：http://gsj.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://coo.gogol.net.cn

Ruby: arr.reverse
来源：http://wer.tian-w.cn

C#:   list.Reverse();
来源：http://fwt.zdbjq.cn

[D12] 查找元素下标
来源：http://wdx.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://ulp.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jdb.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://isv.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://azs.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dme.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://rqy.jqgufenzy.top

Ruby: arr.index(x)
来源：http://sgs.bbcook.cn

C#:   list.IndexOf(x);
来源：http://cvq.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://gsh.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bwb.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rpr.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://wym.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://lgk.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gpc.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojs.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://xye.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bry.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://bun.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hhx.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yib.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://uwy.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://gcn.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kgi.yangfankeji.com

Go:   // 手写循环
来源：http://xri.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://eel.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lmx.mhx1999.top

[D15] 去重
来源：http://zmc.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rky.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://vtq.uphjek.com

JS:   [...new Set(arr)]
来源：http://qii.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://ioc.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cly.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ted.jlsjyb.cn

Ruby: arr.uniq
来源：http://wen.shanyushiyangtech.top


<!-- 参考信息 -->