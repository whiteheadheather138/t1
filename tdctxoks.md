代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zil.cucudq.cn

Java: x instanceof Number
来源：http://lfq.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wll.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://rxw.xuanzx.com

C#:   x is int or double or decimal
来源：http://leu.guannengcc.top

[B14] 判断值是否在集合内
来源：http://kkm.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dzb.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lbr.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://iou.jyoumei.cn

TS:   [1, 2, 3].includes(x)
来源：http://krw.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aqg.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qyv.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ief.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jku.tian-w.cn

[B15] 布尔运算与取反
来源：http://lga.316326.xyz

Py:   a and b or not c
来源：http://asn.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://rtd.yanxiufei.cn

JS:   a && b || !c
来源：http://qwi.yangfankeji.com

TS:   a && b || !c
来源：http://yml.yongpay.top

Java: a && b || !c
来源：http://ywp.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://vjo.cucudq.cn

Ruby: a && b || !c
来源：http://icc.shzxlz.cn

C#:   a && b || !c
来源：http://cxg.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dcp.zdbjq.cn

Py:   if not data: return
来源：http://rks.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://urr.sweek.top

JS:   if (!data) return;
来源：http://ddy.gzhubu.top

TS:   if (!data) return;
来源：http://xyh.feifeiyinyue.top

Java: if (data == null) return;
来源：http://bsx.hnqzz.top

Go:   if data == nil { return }
来源：http://xve.bbcook.cn

Ruby: return if data.nil?
来源：http://zan.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://jix.snrcjt.cn

================================================================================
来源：http://vtz.iojbl.cn

C. 函数与作用域
来源：http://ecz.xylfe.cn

================================================================================
来源：http://eoi.tianlin.xyz

[C01] 定义函数
来源：http://lsb.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://xgt.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://izk.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://tbe.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zfb.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xny.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jzs.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://mge.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fvn.guowangkeji.top

[C02] 默认参数
来源：http://qjj.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://bbj.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xax.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://gts.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://dnc.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://djz.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rwo.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://ffu.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://ypz.tanke756.top

[C03] 可变参数
来源：http://qnv.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://oip.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lrq.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhc.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zlc.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dzc.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jdp.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://qeq.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zbn.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://ulv.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://smw.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lyt.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bnt.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qtj.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://hso.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://xdc.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://shm.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://jlx.jinghuilouyu.cn

[C05] 返回多个值
来源：http://muf.yj20258888.top

Py:   return a, b
来源：http://bcr.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://ndw.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://ngg.iojbl.cn

TS:   return { a, b };
来源：http://glx.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zeo.fehbvm.com

Go:   return a, b
来源：http://uhk.zdbjq.cn

Ruby: return a, b
来源：http://wii.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://zzu.tarul.cn

[C06] 匿名函数 / lambda
来源：http://usx.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://aeb.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yds.ybcxt.top

JS:   const square = x => x * x;
来源：http://rqa.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://wji.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hlv.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://swp.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://ruc.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://tne.316326.xyz

[C07] 把函数作为参数传入
来源：http://xnt.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://btw.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://qli.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sgi.0kj1m.cn

TS:   arr.map(String)
来源：http://gqy.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rpk.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nug.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://yfq.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://hjx.zhoulong.xyz

[C08] 闭包
来源：http://jrd.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ytn.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://efk.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xcj.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxk.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://twx.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zdx.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lhs.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fqr.guannengcc.top

[C09] 递归
来源：http://uts.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aya.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lti.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ync.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kfg.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lcl.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zml.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ynb.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcw.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://ydz.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qzd.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://elq.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vek.quarkkingdee.top

TS:   同 JS
来源：http://elm.nanxinkj.top

Java: 方法内为块级作用域
来源：http://kln.yanxiufei.cn

Go:   花括号块级作用域
来源：http://qxd.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wmt.0kj1m.cn

C#:   块级作用域
来源：http://evi.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://bjx.fehbvm.com

Py:   from module import func
来源：http://qnv.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tjd.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gwt.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ebq.zhiwuduotai.top

Java: import java.util.List;
来源：http://aoi.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wtv.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://suh.nanxinkj.top

C#:   using System.Text;
来源：http://xql.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://kyk.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://yct.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://mwz.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://mxl.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://fyw.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://trb.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://wjk.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://tpz.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hvh.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://pvt.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hyw.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aki.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qdg.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxb.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://hyo.ctjpmb.com

Go:   func add(a, b int) int
来源：http://dpv.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lif.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://owy.fanxiaobao.xyz

[C14] 泛型函数
来源：http://bti.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://avn.nanxinkj.top

PHP:  // 无泛型
来源：http://odb.shanyushiyangtech.top

JS:   // 无泛型
来源：http://zte.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pgi.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uzi.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kik.chenzaomai.com

Ruby: # 无泛型
来源：http://rdk.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ybo.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://kgf.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iqh.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://lwa.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vsg.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ynt.nanxinkj.top

Java: // 无解构
来源：http://pgm.zhoulong.xyz

Go:   // 无解构
来源：http://rdf.tianlin.xyz

Ruby: a, b = pair
来源：http://ixf.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://cxa.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://zqe.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xlb.ppjwa.cn

PHP:  // 无重载
来源：http://coe.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tkw.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://dcq.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wan.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://yky.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://jen.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bgp.ehwqpu.com

================================================================================
来源：http://kqg.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://tzc.bbcook.cn

================================================================================
来源：http://zwt.xylfe.cn

[D01] 创建数组 / 列表
来源：http://otd.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dtg.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czf.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wsp.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tvb.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xqc.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://gie.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://ovk.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xbp.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://urh.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zkm.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fll.hywenlv.cn

JS:   arr.push(4);
来源：http://aro.daria6918.cn

TS:   arr.push(4);
来源：http://aek.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://hrn.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://ozy.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://naq.hcnkem.com

C#:   list.Add(4);
来源：http://htf.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://rea.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://ruo.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ngs.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tzm.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://ywm.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://qvj.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://kay.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rlu.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://mjo.yangfankeji.com

[D04] 删除元素
来源：http://wes.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqx.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nxf.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lkt.tarul.cn

TS:   arr.splice(0, 1);
来源：http://qoi.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aej.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gcz.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://utb.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://svi.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://zcx.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://euc.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hiz.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pjv.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://lmd.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://qfd.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://rva.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qjb.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://frc.sxryk.cn

[D06] 数组长度
来源：http://tmt.cashguo.top

Py:   len(arr)
来源：http://hqh.sufxvd.cn

PHP:  count($arr);
来源：http://stt.sufxvd.cn

JS:   arr.length
来源：http://qet.feifeiyinyue.top

TS:   arr.length
来源：http://wly.ywan-chungtsiang.top

Java: list.size();
来源：http://tky.fengsongda.top

Go:   len(arr)
来源：http://prw.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://wyg.birdmap.top

C#:   list.Count;
来源：http://dos.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://nwe.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pqj.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://bfw.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://ptc.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://eel.yj202588.top

Java: list.subList(1, 4);
来源：http://uwr.xuetiantiany.cn

Go:   arr[1:4]
来源：http://sdl.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://xbe.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://fde.hongshengwenyu.top

[D08] 合并两个数组
来源：http://sje.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://dut.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://vvw.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hfg.gzhubu.top

TS:   [...a, ...b];
来源：http://ygc.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aen.jianghu66.top

Go:   append(a, b...)
来源：http://stk.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://ptv.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://nks.yongpay.top

[D09] 排序（升序）
来源：http://fjg.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://wkl.pycfn.com

PHP:  sort($arr);
来源：http://bxc.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fal.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ukd.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ofw.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kdh.fktsv.cn

Ruby: arr.sort
来源：http://isc.jinqigufen.top

C#:   list.Sort();
来源：http://dao.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gbq.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tuk.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://enr.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkw.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iek.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wdq.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://stj.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://amv.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gvn.ppjwa.cn

[D11] 反转数组
来源：http://hzx.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ueh.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://pgj.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cbk.bbcook.cn

TS:   [...arr].reverse();
来源：http://bmx.mhx1999.top

Java: Collections.reverse(list);
来源：http://bww.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://uin.zhongyouzk.top

Ruby: arr.reverse
来源：http://jnb.yj20258.top

C#:   list.Reverse();
来源：http://fwp.daxiang520.top

[D12] 查找元素下标
来源：http://rck.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://kfj.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ddt.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qlh.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjd.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://twf.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://fiv.hcnkem.com

Ruby: arr.index(x)
来源：http://tkz.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://bro.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://oxz.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ezr.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lpq.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://gnj.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://myx.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qch.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jwv.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eou.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cqt.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://adf.cdnleiting.top


<!-- 参考信息 -->