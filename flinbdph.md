代发 wailian999

C#:   x is int or double or decimal
来源：http://hct.yj20258.top

[B14] 判断值是否在集合内
来源：http://tjx.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iwn.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rpx.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://qoi.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://xib.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gkz.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fbm.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://uyu.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gwa.jiagoushi.top

[B15] 布尔运算与取反
来源：http://obs.vehdjk.com

Py:   a and b or not c
来源：http://hbt.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://afb.zdqjudy.top

JS:   a && b || !c
来源：http://eum.pycfn.com

TS:   a && b || !c
来源：http://adm.birdmap.top

Java: a && b || !c
来源：http://ejc.hesvh.cn

Go:   a && b || !c
来源：http://flo.svipenyu.cn

Ruby: a && b || !c
来源：http://mmr.zdbjq.cn

C#:   a && b || !c
来源：http://muo.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://wow.wangdashe.top

Py:   if not data: return
来源：http://wul.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://hdz.jlsjyb.cn

JS:   if (!data) return;
来源：http://gol.316326.xyz

TS:   if (!data) return;
来源：http://jsu.bbcook.cn

Java: if (data == null) return;
来源：http://hpk.yuanzhike.top

Go:   if data == nil { return }
来源：http://mcy.cucudq.cn

Ruby: return if data.nil?
来源：http://xdc.pycfn.com

C#:   if (data == null) return;
来源：http://lvm.wangshuangyany.cn

================================================================================
来源：http://nce.9152youxi.cn

C. 函数与作用域
来源：http://rss.jqgfzy.top

================================================================================
来源：http://fal.ehwqpu.com

[C01] 定义函数
来源：http://ysm.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://rvt.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ejz.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://ssm.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sxx.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ada.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://ndg.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://ril.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ctq.sjlbkw.cn

[C02] 默认参数
来源：http://gdd.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://lro.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ctu.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://qaw.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://whj.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fzz.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://spf.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://vpl.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://rvf.guowangkeji.top

[C03] 可变参数
来源：http://udp.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://rzg.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ysu.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rci.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zmq.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pdw.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://crl.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://cat.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gle.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://jri.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kkn.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ivk.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cod.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rzc.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://wug.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://rkb.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://dkl.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://dwn.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://uxo.jqgfzy.top

Py:   return a, b
来源：http://jju.jqgfzy.top

PHP:  return [$a, $b];
来源：http://lpw.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uye.hammf.cn

TS:   return { a, b };
来源：http://gtm.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cyp.kuanghao11.cn

Go:   return a, b
来源：http://pkj.52xcode.cn

Ruby: return a, b
来源：http://uxw.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://rnt.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://yta.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://jwo.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fdd.shuidangran.top

JS:   const square = x => x * x;
来源：http://iyk.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://guj.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://onl.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ehk.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://zqs.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://thm.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://mqe.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://grd.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xwk.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vul.bbcook.cn

TS:   arr.map(String)
来源：http://wgi.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mcg.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ozb.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://oen.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://bmd.sjlbkw.cn

[C08] 闭包
来源：http://dxl.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mcx.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cnf.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://prz.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uwe.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ijz.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bra.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gjr.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://syt.fehbvm.com

[C09] 递归
来源：http://dne.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wwi.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fkn.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gzi.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ljs.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://owp.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eyx.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vuy.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rnc.smart0.xyz

[C10] 变量作用域
来源：http://gxm.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xeu.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bdk.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dzo.guowangkeji.top

TS:   同 JS
来源：http://lxd.jianghu66.top

Java: 方法内为块级作用域
来源：http://ziw.yuxming.cn

Go:   花括号块级作用域
来源：http://nzb.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mpn.yj20258.top

C#:   块级作用域
来源：http://gud.yanxiufei.cn

[C11] 模块导入与导出
来源：http://lyz.cashguo.top

Py:   from module import func
来源：http://bgw.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vmo.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lyv.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hde.hfpthk.cn

Java: import java.util.List;
来源：http://xnf.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vcg.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://mou.sxryk.cn

C#:   using System.Text;
来源：http://qqb.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://jib.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://oiq.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://idd.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://mxi.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://wcb.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://moq.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://dzq.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://aqq.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dwd.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://gwi.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jvl.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzm.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hch.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptm.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://dmi.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://tip.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vrm.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://jia.cqqwz.cn

[C14] 泛型函数
来源：http://mpv.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xjp.bbcook.cn

PHP:  // 无泛型
来源：http://mqp.yanxiufei.cn

JS:   // 无泛型
来源：http://dal.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hqj.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ifm.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cov.bjfxy.top

Ruby: # 无泛型
来源：http://yyd.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uzh.mhx1999.top

[C15] 解构 / 展开参数
来源：http://xyz.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ory.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://eof.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yph.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpu.jinyuanbaomall.cn

Java: // 无解构
来源：http://sss.cdnleiting.top

Go:   // 无解构
来源：http://lua.tarul.cn

Ruby: a, b = pair
来源：http://mln.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://wof.ydzc1.top

[C16] 函数 / 方法重载
来源：http://lqn.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fyi.zhoulong.xyz

PHP:  // 无重载
来源：http://qlr.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mku.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://kpf.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dbm.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://oyr.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://nez.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lei.yuxming.cn

================================================================================
来源：http://vvx.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://bmk.316326.xyz

================================================================================
来源：http://wcg.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://vwa.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ius.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sut.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iqo.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://tss.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wui.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://tzz.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://cyf.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://soc.zhixingplan.top

[D02] 追加元素到末尾
来源：http://eld.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://agc.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fvu.sufxvd.cn

JS:   arr.push(4);
来源：http://kml.epnwcf.com

TS:   arr.push(4);
来源：http://xoh.gzhubu.top

Java: list.add(4);
来源：http://ujb.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://kca.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://hmm.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://igc.pycfn.com

[D03] 在指定位置插入元素
来源：http://edp.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://txh.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ktw.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fib.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://eqd.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://ppq.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dzh.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lbw.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://ijr.yj202588.top

[D04] 删除元素
来源：http://lxb.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vpk.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vhn.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://avb.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://avz.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cpg.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sdx.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fvj.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ebq.shuidangran.top

[D05] 访问与修改元素
来源：http://ehl.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yal.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fqw.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iot.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://dxp.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://ish.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://fvx.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kfu.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://etd.ehwqpu.com

[D06] 数组长度
来源：http://fyl.ydjk.org.cn

Py:   len(arr)
来源：http://npx.cdnleiting.top

PHP:  count($arr);
来源：http://svt.wangdashe.top

JS:   arr.length
来源：http://tui.shangyingyoupin.top

TS:   arr.length
来源：http://yhb.gogol.net.cn

Java: list.size();
来源：http://hzt.316326.xyz

Go:   len(arr)
来源：http://meb.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://cjr.aibaodan.cn

C#:   list.Count;
来源：http://zib.iojbl.cn

[D07] 切片 / 取子数组
来源：http://bxk.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ijv.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://iuf.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://vun.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://swz.jqgfzy.top

Java: list.subList(1, 4);
来源：http://cit.sweek.top

Go:   arr[1:4]
来源：http://fex.nwbrower.top

Ruby: arr[1, 3]
来源：http://qwf.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://lss.hnqzz.top

[D08] 合并两个数组
来源：http://aca.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://vyq.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://gam.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://the.hywenlv.cn

TS:   [...a, ...b];
来源：http://tec.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iow.aibaodan.cn

Go:   append(a, b...)
来源：http://wix.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://jdc.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://eqo.gaohongyu789.top

[D09] 排序（升序）
来源：http://ete.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://plh.aibaodan.cn

PHP:  sort($arr);
来源：http://uqk.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uzu.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://opt.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nur.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mhp.tanke756.top

Ruby: arr.sort
来源：http://dhq.sjlbkw.cn

C#:   list.Sort();
来源：http://oub.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qiv.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cai.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fuh.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edf.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://imu.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xhw.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ooe.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lpc.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ebr.316326.xyz

[D11] 反转数组
来源：http://gos.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://uky.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://sks.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kix.tian-w.cn

TS:   [...arr].reverse();
来源：http://kts.hcnkem.com

Java: Collections.reverse(list);
来源：http://xcw.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://mjj.xinyue.icu

Ruby: arr.reverse
来源：http://xdg.jinqigufen.top

C#:   list.Reverse();
来源：http://see.zhixingplan.top

[D12] 查找元素下标
来源：http://fmx.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://oqg.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zug.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lfv.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kgs.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zqg.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://zea.fehbvm.com

Ruby: arr.index(x)
来源：http://uxe.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://rwf.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://krs.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mwb.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mmu.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://rxk.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://ims.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kxf.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xga.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hoq.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jwk.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://yxd.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://osf.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wrw.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://ntm.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://ras.cqqwz.cn


<!-- 参考信息 -->