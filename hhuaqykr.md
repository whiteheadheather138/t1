代发 wailian999

[B13] 判断是否为数字
来源：http://xtp.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://xzi.fengsongda.top

PHP:  is_numeric($x)
来源：http://vfu.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cfz.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uzc.gogol.net.cn

Java: x instanceof Number
来源：http://ltw.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zso.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://hid.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://jrv.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://rns.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tce.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ipr.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://ehu.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://ggx.shzxlz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bue.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lys.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vzf.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fya.xziqi.cn

[B15] 布尔运算与取反
来源：http://prr.ybcxt.top

Py:   a and b or not c
来源：http://ren.sweek.top

PHP:  $a && $b || !$c
来源：http://uvi.nanxinkj.top

JS:   a && b || !c
来源：http://cgb.shzxlz.cn

TS:   a && b || !c
来源：http://nul.ydzc1.top

Java: a && b || !c
来源：http://kya.zhiwuduotai.top

Go:   a && b || !c
来源：http://zrm.zhijiandao.cn

Ruby: a && b || !c
来源：http://mph.shuidangran.top

C#:   a && b || !c
来源：http://awf.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://nmu.aizwys.cn

Py:   if not data: return
来源：http://lrl.yonumen.top

PHP:  if (!$data) { return; }
来源：http://tzl.xuanzx.com

JS:   if (!data) return;
来源：http://bhy.vehdjk.com

TS:   if (!data) return;
来源：http://tsi.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://grd.sjlbkw.cn

Go:   if data == nil { return }
来源：http://fym.shuidangran.top

Ruby: return if data.nil?
来源：http://vrn.52xcode.cn

C#:   if (data == null) return;
来源：http://gpc.gzhubu.top

================================================================================
来源：http://bji.kuanghao11.cn

C. 函数与作用域
来源：http://psh.zdqjudy.top

================================================================================
来源：http://yna.zhaomingkeji.xyz

[C01] 定义函数
来源：http://jkw.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://irg.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jbf.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://vqp.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wvw.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fxd.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://wrt.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://jjv.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qji.jyoumei.cn

[C02] 默认参数
来源：http://rbx.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://xxy.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gzw.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://dai.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uea.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wwo.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vsf.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://oas.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://enp.vehdjk.com

[C03] 可变参数
来源：http://jin.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://usu.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hco.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ddu.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tlq.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsu.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ayb.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zbq.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nab.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://qpx.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hqm.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qdd.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wkf.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eej.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://xbe.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://ntf.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://eay.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://zuq.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://klb.tarul.cn

Py:   return a, b
来源：http://dra.jianghu66.top

PHP:  return [$a, $b];
来源：http://qwq.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://krm.yj20258.top

TS:   return { a, b };
来源：http://pxb.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jdd.tarul.cn

Go:   return a, b
来源：http://cfb.zdbjq.cn

Ruby: return a, b
来源：http://ynd.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://hqf.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://mxg.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://wyk.yanxiufei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zpe.cqqwz.cn

JS:   const square = x => x * x;
来源：http://ikd.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://hvo.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ujc.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://ejh.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://phv.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://srh.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://foz.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uno.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://ows.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gkp.chenzaomai.com

TS:   arr.map(String)
来源：http://tfz.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qcv.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vkv.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://frs.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vhc.fktsv.cn

[C08] 闭包
来源：http://rdd.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uem.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hey.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wrp.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zah.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zfb.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ofi.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qbg.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yyk.zhoulong.xyz

[C09] 递归
来源：http://eqe.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ght.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ilq.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mow.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://amh.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wyu.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iak.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aoz.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sfc.sjlbkw.cn

[C10] 变量作用域
来源：http://dmp.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jij.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fci.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rlh.shuidangran.top

TS:   同 JS
来源：http://pun.hysaishi.cn

Java: 方法内为块级作用域
来源：http://qpy.jqgufenzy.top

Go:   花括号块级作用域
来源：http://hgh.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kuh.bjfxy.top

C#:   块级作用域
来源：http://sbz.hywenlv.cn

[C11] 模块导入与导出
来源：http://ogg.feifeiyinyue.top

Py:   from module import func
来源：http://nqf.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yoy.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wji.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ptz.yuanzhike.top

Java: import java.util.List;
来源：http://hkd.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tez.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://igu.hongshengwenyu.top

C#:   using System.Text;
来源：http://lpu.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://mvu.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://ogd.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://eja.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://ski.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://znv.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eas.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://mdv.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://cbo.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://low.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://jea.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kzz.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pag.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cgg.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vpx.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qjs.hnqzz.top

Go:   func add(a, b int) int
来源：http://qrl.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://orl.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ykz.feifeiyinyue.top

[C14] 泛型函数
来源：http://axz.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zez.hongshengwenyu.top

PHP:  // 无泛型
来源：http://vln.feifeiyinyue.top

JS:   // 无泛型
来源：http://mzm.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xms.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rnf.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aau.yanxiufei.cn

Ruby: # 无泛型
来源：http://jbg.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nfa.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://jmw.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ngr.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://skh.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wxu.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tho.zhaomingkeji.xyz

Java: // 无解构
来源：http://vsr.yfazqb.com

Go:   // 无解构
来源：http://ymp.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://tjl.smart0.xyz

C#:   var (a, b) = pair;
来源：http://qun.xinyue.icu

[C16] 函数 / 方法重载
来源：http://joh.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://exn.yj20258.top

PHP:  // 无重载
来源：http://how.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://run.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://wxg.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qrd.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://vou.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://ozg.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hye.xuetiantiany.cn

================================================================================
来源：http://mnq.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://dbr.epnwcf.com

================================================================================
来源：http://pep.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://yyv.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zoo.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xhf.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://koi.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jjt.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bjm.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://mez.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://dri.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fav.jyoumei.cn

[D02] 追加元素到末尾
来源：http://knr.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rry.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gni.tianlin.xyz

JS:   arr.push(4);
来源：http://ftd.fzhhl.top

TS:   arr.push(4);
来源：http://vrz.guannengcc.top

Java: list.add(4);
来源：http://aqu.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://uwo.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ifd.epnwcf.com

C#:   list.Add(4);
来源：http://itf.meibo888.top

[D03] 在指定位置插入元素
来源：http://oxp.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://ems.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blf.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fxf.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://bko.zhengqikj.top

Java: list.add(0, 0);
来源：http://vyt.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://vjb.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://thd.yonumen.top

C#:   list.Insert(0, 0);
来源：http://loh.jqgfzy.top

[D04] 删除元素
来源：http://ipt.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ouk.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nwa.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ttw.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://azq.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pzi.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hzz.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lsv.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vef.hesvh.cn

[D05] 访问与修改元素
来源：http://dbs.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wwj.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ajv.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cqh.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://lrx.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://mgi.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://icv.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xio.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hwt.shanyushiyangtech.top

[D06] 数组长度
来源：http://men.9152youxi.cn

Py:   len(arr)
来源：http://esx.zhengqikj.top

PHP:  count($arr);
来源：http://bfz.daxiang520.top

JS:   arr.length
来源：http://rhz.yj20258.top

TS:   arr.length
来源：http://spa.sysykeji.top

Java: list.size();
来源：http://fca.uphjek.com

Go:   len(arr)
来源：http://ayc.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://wox.zhixingplan.top

C#:   list.Count;
来源：http://cxj.hesvh.cn

[D07] 切片 / 取子数组
来源：http://yea.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://foy.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ldu.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://ish.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://ppf.zdqjudy.top

Java: list.subList(1, 4);
来源：http://eev.fzhhl.top

Go:   arr[1:4]
来源：http://zbk.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://zoy.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://gwm.guowangkeji.top

[D08] 合并两个数组
来源：http://boh.sweek.top

Py:   a + b;  a.extend(b)
来源：http://sub.yongpay.top

PHP:  array_merge($a, $b);
来源：http://ext.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fni.gzhubu.top

TS:   [...a, ...b];
来源：http://dbp.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kme.havefunace.top

Go:   append(a, b...)
来源：http://aij.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://oix.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://yqx.0kj1m.cn

[D09] 排序（升序）
来源：http://ssb.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://kgt.tarul.cn

PHP:  sort($arr);
来源：http://vwi.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://isy.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jqr.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tbc.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ilu.hongshengwenyu.top

Ruby: arr.sort
来源：http://dzi.vqdsnc.cn

C#:   list.Sort();
来源：http://tmq.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://wuh.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dng.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://env.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ywc.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dmz.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://elq.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nml.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bjt.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jpd.wangshuangyany.cn

[D11] 反转数组
来源：http://ket.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://oct.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://tiy.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://plu.fehbvm.com

TS:   [...arr].reverse();
来源：http://vyi.svipenyu.cn

Java: Collections.reverse(list);
来源：http://feh.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://cro.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://zrb.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://sig.shuidangran.top

[D12] 查找元素下标
来源：http://izl.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://tus.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qkw.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlg.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://azi.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hgk.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://dkh.hammf.cn

Ruby: arr.index(x)
来源：http://xgk.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://svp.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://kxj.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rib.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sgf.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://xfp.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://wsj.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zrq.yvedp.cn


<!-- 参考信息 -->