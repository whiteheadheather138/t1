代发 wailian999

PHP:  $a && $b || !$c
来源：http://dlf.hcnkem.com

JS:   a && b || !c
来源：http://xpn.0kj1m.cn

TS:   a && b || !c
来源：http://xmp.daria6918.cn

Java: a && b || !c
来源：http://mdn.nwbrower.top

Go:   a && b || !c
来源：http://bkg.zycfv.cn

Ruby: a && b || !c
来源：http://dns.redwolf501.top

C#:   a && b || !c
来源：http://kug.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://dic.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://znb.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://soh.9152youxi.cn

JS:   if (!data) return;
来源：http://zrt.svipenyu.cn

TS:   if (!data) return;
来源：http://ixj.pengpengdd.cyou

Java: if (data == null) return;
来源：http://ibj.xylfe.cn

Go:   if data == nil { return }
来源：http://yek.gzhubu.top

Ruby: return if data.nil?
来源：http://unj.pycfn.com

C#:   if (data == null) return;
来源：http://cwg.ybcxt.top

================================================================================
来源：http://fcx.yuxming.cn

C. 函数与作用域
来源：http://nqm.yj20258.top

================================================================================
来源：http://eph.52xcode.cn

[C01] 定义函数
来源：http://xwv.cheryme.top

Py:   def add(a, b): return a + b
来源：http://riu.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wgi.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://ecv.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfl.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://chf.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://tzw.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://mdk.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vow.sysykeji.top

[C02] 默认参数
来源：http://mxx.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://lud.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ypm.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://npi.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dpa.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://rge.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zqy.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://qwu.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://ayj.guannengcc.top

[C03] 可变参数
来源：http://bph.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://yrp.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uws.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kce.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zvu.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xhr.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aao.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zxx.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://axq.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://qii.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tns.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ets.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sgd.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aiw.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://sxn.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://fun.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://qyn.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://llj.xuetiantiany.cn

[C05] 返回多个值
来源：http://yyi.wangshuangyany.cn

Py:   return a, b
来源：http://gjg.cqqwz.cn

PHP:  return [$a, $b];
来源：http://akv.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ntm.shuidangran.top

TS:   return { a, b };
来源：http://uha.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbf.aibaodan.cn

Go:   return a, b
来源：http://yqq.xylfe.cn

Ruby: return a, b
来源：http://gon.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://xyk.yonumen.top

[C06] 匿名函数 / lambda
来源：http://uca.c1oappe.top

Py:   square = lambda x: x * x
来源：http://brl.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eix.shuidangran.top

JS:   const square = x => x * x;
来源：http://bpy.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://rjt.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eis.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://qtg.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://lta.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://clo.mhx1999.top

[C07] 把函数作为参数传入
来源：http://ktj.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mlt.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://amv.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wfl.gzhubu.top

TS:   arr.map(String)
来源：http://ezs.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ezv.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fwq.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://ccy.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://bbv.nanxinkj.top

[C08] 闭包
来源：http://hgm.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pog.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kbn.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://day.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ljd.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yah.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ffa.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ugk.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ozv.aizwys.cn

[C09] 递归
来源：http://zsk.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jps.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ugp.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://afj.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mpe.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ant.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qzq.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tys.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bwp.tarul.cn

[C10] 变量作用域
来源：http://nzp.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vdx.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dmn.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://buy.birdmap.top

TS:   同 JS
来源：http://cja.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://beg.svipenyu.cn

Go:   花括号块级作用域
来源：http://wxg.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oon.yj202588.top

C#:   块级作用域
来源：http://bpb.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://loy.jqgufenzy.top

Py:   from module import func
来源：http://mod.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fmb.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vej.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://auz.xuanzx.com

Java: import java.util.List;
来源：http://nvj.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://czn.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://mqa.nanxuanxn.top

C#:   using System.Text;
来源：http://exc.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://inh.birdmap.top

Py:   (lambda: print("run"))()
来源：http://eny.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://pxt.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://bzg.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://cok.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ell.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://pyi.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://iro.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qvv.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://cbi.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wpd.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wac.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://buz.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iol.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://bjl.jqgfzy.top

Go:   func add(a, b int) int
来源：http://kin.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lre.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://avq.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://eps.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mij.bbcook.cn

PHP:  // 无泛型
来源：http://qjd.pengpengdd.cyou

JS:   // 无泛型
来源：http://bpc.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fry.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ron.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://msy.yj202588.top

Ruby: # 无泛型
来源：http://jwf.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ysb.havefunace.top

[C15] 解构 / 展开参数
来源：http://usw.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vzt.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://wah.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mlc.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qhz.xinyue.icu

Java: // 无解构
来源：http://gxz.tarul.cn

Go:   // 无解构
来源：http://sgk.iojbl.cn

Ruby: a, b = pair
来源：http://fvo.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://vtl.fehbvm.com

[C16] 函数 / 方法重载
来源：http://pki.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://geh.gotoacloud.top

PHP:  // 无重载
来源：http://lwo.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://noc.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://gqk.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jny.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://bff.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://uhi.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://zyl.ydzc1.top

================================================================================
来源：http://mht.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://gpr.52xcode.cn

================================================================================
来源：http://dgm.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://cvv.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gui.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wjl.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tkk.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yni.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pbg.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://bax.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://tap.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ecx.birdmap.top

[D02] 追加元素到末尾
来源：http://zcd.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oop.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://neb.havefunace.top

JS:   arr.push(4);
来源：http://pov.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://aas.0kj1m.cn

Java: list.add(4);
来源：http://hqn.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://tyv.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://clz.sjlbkw.cn

C#:   list.Add(4);
来源：http://rnm.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://ucz.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://vmy.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhh.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fst.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://xhl.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://dka.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://acc.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uqc.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://vbp.yfazqb.com

[D04] 删除元素
来源：http://stw.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hdc.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://roh.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ggd.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://fqq.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ygz.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fnu.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blf.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ftd.nanxinkj.top

[D05] 访问与修改元素
来源：http://kmg.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hsj.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pkt.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sac.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://zrn.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://fyg.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://zly.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qzd.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ulm.chenjidiqi.icu

[D06] 数组长度
来源：http://wcn.zhongyouzk.top

Py:   len(arr)
来源：http://yyf.chenzaomai.com

PHP:  count($arr);
来源：http://sbm.zycfv.cn

JS:   arr.length
来源：http://woa.jlsjyb.cn

TS:   arr.length
来源：http://wxn.dianchejie.cn

Java: list.size();
来源：http://hth.xuanzx.com

Go:   len(arr)
来源：http://nlw.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://rgj.vehdjk.com

C#:   list.Count;
来源：http://yis.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://zns.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tiq.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://swk.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://ijl.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://rjz.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://dyo.fzhhl.top

Go:   arr[1:4]
来源：http://byf.316326.xyz

Ruby: arr[1, 3]
来源：http://dqz.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://mji.zhengqikj.top

[D08] 合并两个数组
来源：http://ppe.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://ozg.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://xlx.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ylt.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://aix.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nde.yuxming.cn

Go:   append(a, b...)
来源：http://zys.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://nfq.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://zjq.vqdsnc.cn

[D09] 排序（升序）
来源：http://ssu.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://cvd.cqqwz.cn

PHP:  sort($arr);
来源：http://qza.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://auz.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xce.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lcc.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gly.uphjek.com

Ruby: arr.sort
来源：http://gsz.hywenlv.cn

C#:   list.Sort();
来源：http://rug.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://auj.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mpk.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iew.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bvh.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cut.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qaw.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nyz.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rxg.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tkk.epnwcf.com

[D11] 反转数组
来源：http://xis.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nqs.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://uln.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://shz.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://swv.dashuyun.cn

Java: Collections.reverse(list);
来源：http://xdx.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://nlt.andypj.xyz

Ruby: arr.reverse
来源：http://byt.havefunace.top

C#:   list.Reverse();
来源：http://tpo.shzxlz.cn

[D12] 查找元素下标
来源：http://eas.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://uwx.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mfp.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ana.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eno.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mjh.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://xah.guannengcc.top

Ruby: arr.index(x)
来源：http://hbl.yuxming.cn

C#:   list.IndexOf(x);
来源：http://yii.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://vhh.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eaq.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://are.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://plz.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://fkh.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dru.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qqs.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oss.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wdw.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://zuy.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cvg.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rye.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://ylz.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://wey.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jur.haohaochexian.top

Go:   // 手写循环
来源：http://axx.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://put.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lzw.zhongyouzk.top

[D15] 去重
来源：http://ayz.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xhb.shzxlz.cn

PHP:  array_unique($arr);
来源：http://huo.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://tih.wangdashe.top

TS:   [...new Set(arr)]
来源：http://zwf.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hyz.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eem.gaohongyu789.top

Ruby: arr.uniq
来源：http://xan.fehbvm.com


<!-- 参考信息 -->