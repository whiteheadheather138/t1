代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://cnf.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://yeh.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wpp.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uov.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://iqv.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hxi.xziqi.cn

[B15] 布尔运算与取反
来源：http://vko.havefunace.top

Py:   a and b or not c
来源：http://zii.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://sxm.dashuyun.cn

JS:   a && b || !c
来源：http://ilj.daxiang520.top

TS:   a && b || !c
来源：http://vpe.shzxlz.cn

Java: a && b || !c
来源：http://kal.aibaodan.cn

Go:   a && b || !c
来源：http://fjs.quarkkingdee.top

Ruby: a && b || !c
来源：http://vzu.jiagoushi.top

C#:   a && b || !c
来源：http://kvj.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zfc.vehdjk.com

Py:   if not data: return
来源：http://yqi.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://uvz.aizwys.cn

JS:   if (!data) return;
来源：http://sbm.jqgfzy.top

TS:   if (!data) return;
来源：http://qrv.cqqwz.cn

Java: if (data == null) return;
来源：http://rgg.sysykeji.top

Go:   if data == nil { return }
来源：http://sze.52xcode.cn

Ruby: return if data.nil?
来源：http://pul.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://cae.wangshuangyany.cn

================================================================================
来源：http://ukv.ydjk.org.cn

C. 函数与作用域
来源：http://ekf.nwbrower.top

================================================================================
来源：http://gxk.xylfe.cn

[C01] 定义函数
来源：http://jmg.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://cba.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oqa.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://lnp.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xrq.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kmw.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://urd.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://klr.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hrz.yuanzhike.top

[C02] 默认参数
来源：http://ylo.316326.xyz

Py:   def greet(name="World"): return name
来源：http://ppa.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://xpa.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://xcu.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lsi.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zya.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hem.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://dct.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://idq.quarkkingdee.top

[C03] 可变参数
来源：http://fsj.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://ang.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cju.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jji.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://orw.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://roq.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fzu.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://gaz.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xzl.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://jkd.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xmg.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://amq.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wup.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cqz.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://rxi.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://pon.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://icd.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://wcd.fanxiaobao.xyz

[C05] 返回多个值
来源：http://xqa.zdbjq.cn

Py:   return a, b
来源：http://jla.tarul.cn

PHP:  return [$a, $b];
来源：http://hvw.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fwe.tian-w.cn

TS:   return { a, b };
来源：http://wif.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zmt.52xcode.cn

Go:   return a, b
来源：http://anh.nanxinkj.top

Ruby: return a, b
来源：http://jks.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://npg.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://glh.yueranfly.top

Py:   square = lambda x: x * x
来源：http://wjs.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eoy.ppjwa.cn

JS:   const square = x => x * x;
来源：http://zif.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://qdy.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tvw.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://hft.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://fal.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://xxm.birdmap.top

[C07] 把函数作为参数传入
来源：http://bfb.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tev.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://hkm.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bsm.haohaochexian.top

TS:   arr.map(String)
来源：http://jus.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gvi.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uik.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://sdk.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uoa.shanyushiyangkeji.top

[C08] 闭包
来源：http://fqj.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vvq.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mjm.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ebe.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nqz.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uis.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mdf.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wid.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dnq.wangdashe.top

[C09] 递归
来源：http://ppy.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xun.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pcl.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqj.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jeb.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qql.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://als.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rff.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jsv.jlsjyb.cn

[C10] 变量作用域
来源：http://exe.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dpw.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bcp.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gjz.nwbrower.top

TS:   同 JS
来源：http://mlw.jyoumei.cn

Java: 方法内为块级作用域
来源：http://otx.yvedp.cn

Go:   花括号块级作用域
来源：http://udr.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fji.zhijiandao.cn

C#:   块级作用域
来源：http://nvx.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://tgq.hongshengwenyu.top

Py:   from module import func
来源：http://uss.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://klc.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xnl.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uxn.fktsv.cn

Java: import java.util.List;
来源：http://trp.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ppp.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://yyp.vehdjk.com

C#:   using System.Text;
来源：http://hgh.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://hse.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://nrx.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://dgo.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://ssh.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://xjf.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://faw.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://euo.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://nvf.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jlb.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://yyw.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ydd.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dzp.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cxh.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdx.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://ayj.hfpthk.cn

Go:   func add(a, b int) int
来源：http://tfi.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xgb.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hky.xuetiantiany.cn

[C14] 泛型函数
来源：http://zml.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iyf.wangdashe.top

PHP:  // 无泛型
来源：http://dvp.jyoumei.cn

JS:   // 无泛型
来源：http://eaz.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iwt.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cmj.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yuy.chenjidiqi.icu

Ruby: # 无泛型
来源：http://ngv.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ymy.smart0.xyz

[C15] 解构 / 展开参数
来源：http://drw.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gqc.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://fka.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ezy.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rqe.cqqwz.cn

Java: // 无解构
来源：http://feb.epnwcf.com

Go:   // 无解构
来源：http://xsd.9152youxi.cn

Ruby: a, b = pair
来源：http://ooa.ybcxt.top

C#:   var (a, b) = pair;
来源：http://tqq.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://ycv.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lez.svipenyu.cn

PHP:  // 无重载
来源：http://hyb.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://htp.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://eas.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lba.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://iaz.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://dxa.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nvp.xziqi.cn

================================================================================
来源：http://imx.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://byp.yongpay.top

================================================================================
来源：http://ond.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://mqb.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sfs.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tpn.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ono.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://esk.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vpw.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://hlb.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://igm.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rko.gogol.net.cn

[D02] 追加元素到末尾
来源：http://loi.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wcq.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jpr.iojbl.cn

JS:   arr.push(4);
来源：http://rhv.316326.xyz

TS:   arr.push(4);
来源：http://kkr.aibaodan.cn

Java: list.add(4);
来源：http://zaj.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://mww.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vwe.hammf.cn

C#:   list.Add(4);
来源：http://fug.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://iot.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://bng.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jel.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://clh.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://bcd.guowangkeji.top

Java: list.add(0, 0);
来源：http://fqt.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://pdd.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://miq.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://eby.chenlongwang.top

[D04] 删除元素
来源：http://ccq.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://azu.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uhz.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qcr.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://dzx.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ecs.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zzf.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jne.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fvi.chenzaomai.com

[D05] 访问与修改元素
来源：http://njn.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cge.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vln.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tpn.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://boc.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://hob.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://xvx.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gph.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vxj.epnwcf.com

[D06] 数组长度
来源：http://wcg.jinqigufen.top

Py:   len(arr)
来源：http://ims.0kj1m.cn

PHP:  count($arr);
来源：http://zoo.fzhhl.top

JS:   arr.length
来源：http://eud.zhongyouzk.top

TS:   arr.length
来源：http://aer.9152youxi.cn

Java: list.size();
来源：http://kvm.ywan-chungtsiang.top

Go:   len(arr)
来源：http://ofp.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://yym.fktsv.cn

C#:   list.Count;
来源：http://afp.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://rkl.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rsp.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qms.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://hpp.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://zip.zhengqikj.top

Java: list.subList(1, 4);
来源：http://vod.yj20258.top

Go:   arr[1:4]
来源：http://tgl.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://xzs.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://saw.yongpay.top

[D08] 合并两个数组
来源：http://iuy.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://bht.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://fff.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mzm.0kj1m.cn

TS:   [...a, ...b];
来源：http://sld.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pdq.jlsjyb.cn

Go:   append(a, b...)
来源：http://fdo.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://ufz.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://tbe.316326.xyz

[D09] 排序（升序）
来源：http://inh.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://ufg.yj20258.top

PHP:  sort($arr);
来源：http://mnz.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://llk.sufxvd.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xmg.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lfw.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uhp.fanxiaobao.xyz

Ruby: arr.sort
来源：http://ejg.yj20258888.top

C#:   list.Sort();
来源：http://deq.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jbn.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wrz.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hnc.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gef.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yhc.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qmo.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://izs.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nuv.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://khg.zdqjudy.top

[D11] 反转数组
来源：http://lkl.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://owd.bbcook.cn

PHP:  array_reverse($arr);
来源：http://ifd.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nlp.hammf.cn

TS:   [...arr].reverse();
来源：http://kan.chenlongwang.top

Java: Collections.reverse(list);
来源：http://skj.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://vxf.hywenlv.cn

Ruby: arr.reverse
来源：http://dkx.snrcjt.cn

C#:   list.Reverse();
来源：http://zcj.xuanzx.com

[D12] 查找元素下标
来源：http://bck.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://jxx.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://frz.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fbc.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bhv.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rtd.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://ovi.cashguo.top

Ruby: arr.index(x)
来源：http://zdk.ydzc1.top

C#:   list.IndexOf(x);
来源：http://tzy.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://dac.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qdi.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://drt.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://lla.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://bdm.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eyr.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hzq.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://lsi.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://mfp.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://drx.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wbr.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kpt.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://aat.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://fcy.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jze.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://qnv.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://uju.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sys.bjfxy.top


<!-- 参考信息 -->