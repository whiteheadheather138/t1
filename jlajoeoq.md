代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ahp.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://wzc.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xnn.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nob.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://tkg.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kzp.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://ztx.wangdashe.top

Py:   a and b or not c
来源：http://wsl.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://wtz.vqdsnc.cn

JS:   a && b || !c
来源：http://ntg.cdnleiting.top

TS:   a && b || !c
来源：http://xtp.uphjek.com

Java: a && b || !c
来源：http://pmg.hnxiangtu.top

Go:   a && b || !c
来源：http://wll.vqdsnc.cn

Ruby: a && b || !c
来源：http://hzg.jqgfzy.top

C#:   a && b || !c
来源：http://hrr.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dey.havefunace.top

Py:   if not data: return
来源：http://qkd.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://cwm.epnwcf.com

JS:   if (!data) return;
来源：http://sfp.yj20258888.top

TS:   if (!data) return;
来源：http://fsd.jqgufenzy.top

Java: if (data == null) return;
来源：http://afa.jiagoushi.top

Go:   if data == nil { return }
来源：http://bsh.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://fic.yj20258888.top

C#:   if (data == null) return;
来源：http://jdi.sweek.top

================================================================================
来源：http://kcg.jiagoushi.top

C. 函数与作用域
来源：http://wnb.jinghuilouyu.cn

================================================================================
来源：http://uja.snrcjt.cn

[C01] 定义函数
来源：http://yuk.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://ftg.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vko.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://mks.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mpg.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jva.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://pee.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://kfp.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hos.jinghuilouyu.cn

[C02] 默认参数
来源：http://lrf.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://mwh.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yyv.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://oaz.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://awa.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mqr.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wxj.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://ast.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://wle.shuidangran.top

[C03] 可变参数
来源：http://gvu.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://snn.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bvu.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jnz.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ckn.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://twt.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dtv.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://dyp.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wim.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://qfc.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xds.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://czp.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wiz.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jkl.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://drs.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://awo.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://zau.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://mos.feifeiyinyue.top

[C05] 返回多个值
来源：http://qak.9152youxi.cn

Py:   return a, b
来源：http://spi.316326.xyz

PHP:  return [$a, $b];
来源：http://vbj.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oma.ehwqpu.com

TS:   return { a, b };
来源：http://knb.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kgq.guannengcc.top

Go:   return a, b
来源：http://dwf.jinyuanbaomall.cn

Ruby: return a, b
来源：http://fcg.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://chu.ivvv.top

[C06] 匿名函数 / lambda
来源：http://nnw.birdmap.top

Py:   square = lambda x: x * x
来源：http://rtq.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://wmq.yvedp.cn

JS:   const square = x => x * x;
来源：http://wku.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://vde.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wra.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cag.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://bux.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://iqa.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://mmn.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fnp.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://xmj.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hnc.9152youxi.cn

TS:   arr.map(String)
来源：http://ctn.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oxs.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pdt.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://cxp.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qbo.gotoacloud.top

[C08] 闭包
来源：http://xkf.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wtk.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vkr.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fsb.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://unk.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vkz.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vdr.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vcb.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bpp.cucudq.cn

[C09] 递归
来源：http://hub.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eth.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wls.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dcd.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ueg.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pnv.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bux.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eqc.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ube.sweek.top

[C10] 变量作用域
来源：http://whp.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zve.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fqv.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://siv.smart0.xyz

TS:   同 JS
来源：http://ein.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://kgb.sweek.top

Go:   花括号块级作用域
来源：http://zob.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aau.shangyingyoupin.top

C#:   块级作用域
来源：http://orz.jinqigufen.top

[C11] 模块导入与导出
来源：http://okk.gzhubu.top

Py:   from module import func
来源：http://rdt.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zzx.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rrm.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fxq.yangfankeji.com

Java: import java.util.List;
来源：http://rne.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wxh.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://xwn.ydzc1.top

C#:   using System.Text;
来源：http://nsg.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://jqy.havefunace.top

Py:   (lambda: print("run"))()
来源：http://net.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://fff.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://dxu.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://azk.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lzt.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://jkl.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://nro.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fcz.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://lbm.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qjd.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivr.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rgf.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cxx.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://ves.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://eqg.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fqb.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://qpg.nanxuanxn.top

[C14] 泛型函数
来源：http://cym.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://omo.daxiang520.top

PHP:  // 无泛型
来源：http://fwd.hysaishi.cn

JS:   // 无泛型
来源：http://nhf.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aia.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bys.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hwn.epnwcf.com

Ruby: # 无泛型
来源：http://cys.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mtg.tian-w.cn

[C15] 解构 / 展开参数
来源：http://fgl.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rzv.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://emu.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jzh.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vwe.hesvh.cn

Java: // 无解构
来源：http://jlm.daria6918.cn

Go:   // 无解构
来源：http://dvj.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://jfw.sysykeji.top

C#:   var (a, b) = pair;
来源：http://uob.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://zbm.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://skg.jinghuilouyu.cn

PHP:  // 无重载
来源：http://fqg.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://asx.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://iyk.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://abi.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://ykn.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://dkj.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sfg.zdqjudy.top

================================================================================
来源：http://deg.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://xpz.birdmap.top

================================================================================
来源：http://tzz.cheryme.top

[D01] 创建数组 / 列表
来源：http://ghf.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gwx.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qqt.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://keg.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://goo.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zhm.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://ckx.quarkkingdee.top

Ruby: arr = [1, 2, 3]
来源：http://zmq.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://isj.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://clx.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qsk.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vfw.zhengqikj.top

JS:   arr.push(4);
来源：http://cfh.hcnkem.com

TS:   arr.push(4);
来源：http://ycg.shzxlz.cn

Java: list.add(4);
来源：http://rpd.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://ypa.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://zbn.dashuyun.cn

C#:   list.Add(4);
来源：http://tsw.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://ekb.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://pse.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fvc.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tfn.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://aox.sufxvd.cn

Java: list.add(0, 0);
来源：http://mhb.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://rgb.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://two.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://nrg.c1oappe.top

[D04] 删除元素
来源：http://cii.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hlo.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://itc.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zgh.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://qad.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tfy.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dxr.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bgw.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nnx.zhongyouzk.top

[D05] 访问与修改元素
来源：http://tcr.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hfk.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vyd.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aqr.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ett.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://vhh.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://nih.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dco.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://syh.chenlongwang.top

[D06] 数组长度
来源：http://yet.haohaochexian.top

Py:   len(arr)
来源：http://ile.hysaishi.cn

PHP:  count($arr);
来源：http://iln.guannengcc.top

JS:   arr.length
来源：http://qgh.shanyushiyangkeji.top

TS:   arr.length
来源：http://ofp.andypj.xyz

Java: list.size();
来源：http://kyr.vqdsnc.cn

Go:   len(arr)
来源：http://lbf.hesvh.cn

Ruby: arr.length; arr.size
来源：http://rwk.bjfxy.top

C#:   list.Count;
来源：http://yfo.vehdjk.com

[D07] 切片 / 取子数组
来源：http://wyi.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tgj.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://xdh.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://ran.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://xer.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://wrd.guowangkeji.top

Go:   arr[1:4]
来源：http://xrs.hnqzz.top

Ruby: arr[1, 3]
来源：http://sph.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://bvp.bjfxy.top

[D08] 合并两个数组
来源：http://llv.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://box.yj20258.top

PHP:  array_merge($a, $b);
来源：http://snq.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://udk.sjlbkw.cn

TS:   [...a, ...b];
来源：http://vrf.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://daz.dianchejie.cn

Go:   append(a, b...)
来源：http://znr.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://daq.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://ndt.xuetiantiany.cn

[D09] 排序（升序）
来源：http://lpw.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://loo.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://tqh.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rlz.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eyr.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xtd.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vea.yuanzhike.top

Ruby: arr.sort
来源：http://mvv.zhixingplan.top

C#:   list.Sort();
来源：http://rkx.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jil.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aqc.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fgs.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dkv.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kbs.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hcg.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xey.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://byr.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tyh.epnwcf.com

[D11] 反转数组
来源：http://hcn.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tfr.pycfn.com

PHP:  array_reverse($arr);
来源：http://nnk.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lnh.cqqwz.cn

TS:   [...arr].reverse();
来源：http://qap.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://mkz.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://kne.hcnkem.com

Ruby: arr.reverse
来源：http://zdz.xinyue.icu

C#:   list.Reverse();
来源：http://mrs.jianghu66.top

[D12] 查找元素下标
来源：http://dio.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://rsp.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tlg.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ioh.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ouq.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://upx.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://wsj.nanxinkj.top

Ruby: arr.index(x)
来源：http://ydx.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://yno.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://igy.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yld.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zzt.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://ueu.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://djv.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eiu.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rum.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://mjs.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hcu.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://lox.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qtf.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cdr.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://zfi.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://nph.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tmv.yonumen.top

Go:   // 手写循环
来源：http://pxf.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://itn.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ugm.jqgfzy.top


<!-- 参考信息 -->