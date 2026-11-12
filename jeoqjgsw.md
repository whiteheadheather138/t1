代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlv.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://thg.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wsu.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://qoy.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://utc.fzhhl.top

[B14] 判断值是否在集合内
来源：http://eoe.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kpe.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://phv.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://mnp.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kpc.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yqp.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://enu.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://fcq.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lad.nanxinkj.top

[B15] 布尔运算与取反
来源：http://htr.chenjidiqi.icu

Py:   a and b or not c
来源：http://qfc.fengsongda.top

PHP:  $a && $b || !$c
来源：http://kky.zhiwuduotai.top

JS:   a && b || !c
来源：http://kjh.pycfn.com

TS:   a && b || !c
来源：http://fur.gzhubu.top

Java: a && b || !c
来源：http://hyq.fanxiaobao.xyz

Go:   a && b || !c
来源：http://dlh.jqgfzy.top

Ruby: a && b || !c
来源：http://gok.epnwcf.com

C#:   a && b || !c
来源：http://pef.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://uex.wangdashe.top

Py:   if not data: return
来源：http://wkh.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://jpy.zhoulong.xyz

JS:   if (!data) return;
来源：http://ehy.yueranfly.top

TS:   if (!data) return;
来源：http://jnl.yueranfly.top

Java: if (data == null) return;
来源：http://ras.guannengcc.top

Go:   if data == nil { return }
来源：http://mml.hfpthk.cn

Ruby: return if data.nil?
来源：http://syy.snrcjt.cn

C#:   if (data == null) return;
来源：http://ort.havefunace.top

================================================================================
来源：http://rhz.ivvv.top

C. 函数与作用域
来源：http://lvf.fehbvm.com

================================================================================
来源：http://gji.zycfv.cn

[C01] 定义函数
来源：http://qrg.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://ukp.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ahh.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://dze.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ady.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vfq.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wwz.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://uez.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iqk.hysaishi.cn

[C02] 默认参数
来源：http://jig.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://lre.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lme.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://grw.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bcm.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nqt.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vzd.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://chn.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://njs.yj20258888.top

[C03] 可变参数
来源：http://wqe.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://nkr.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bhm.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rwg.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wyc.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uoa.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ljg.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://zbs.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eec.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://mjv.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://edl.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tnj.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gnw.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zfe.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://loq.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://xnl.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://yva.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://wbh.hysaishi.cn

[C05] 返回多个值
来源：http://pro.jqgfzy.top

Py:   return a, b
来源：http://qny.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://woz.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uzk.dashuyun.cn

TS:   return { a, b };
来源：http://ipt.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cmw.havefunace.top

Go:   return a, b
来源：http://wgu.yanxiufei.cn

Ruby: return a, b
来源：http://zmg.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://zrq.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://hcq.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://edo.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://scc.aizwys.cn

JS:   const square = x => x * x;
来源：http://jde.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://ycv.hcnkem.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gek.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qsz.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://fty.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://bwd.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://ukh.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mtf.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://azl.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mfx.sysykeji.top

TS:   arr.map(String)
来源：http://qmz.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eby.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nid.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://xwt.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://hgs.zdqjudy.top

[C08] 闭包
来源：http://bci.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yut.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sil.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fwz.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jge.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dmn.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bzk.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ujg.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://owu.yuxming.cn

[C09] 递归
来源：http://vxu.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://evf.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kex.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jsb.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcm.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://urf.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://czf.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kel.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xmx.zdqjudy.top

[C10] 变量作用域
来源：http://xjb.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wsm.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sxm.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kfw.yuxming.cn

TS:   同 JS
来源：http://wme.yuanzhike.top

Java: 方法内为块级作用域
来源：http://ywo.vqdsnc.cn

Go:   花括号块级作用域
来源：http://ibq.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nhb.jyoumei.cn

C#:   块级作用域
来源：http://wpo.zhixingplan.top

[C11] 模块导入与导出
来源：http://lox.guannengcc.top

Py:   from module import func
来源：http://ymk.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://llt.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://tvg.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://chu.fengsongda.top

Java: import java.util.List;
来源：http://iqm.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cbe.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://chc.smart0.xyz

C#:   using System.Text;
来源：http://ynx.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://uzg.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://yyh.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://lrl.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://zif.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://xbl.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bmg.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://kdg.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://pgw.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eaj.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://cyh.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wfn.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yht.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ucp.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mbn.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://emn.xziqi.cn

Go:   func add(a, b int) int
来源：http://kxe.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gis.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://tdn.sweek.top

[C14] 泛型函数
来源：http://hrl.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kwq.dianchejie.cn

PHP:  // 无泛型
来源：http://qgu.shangyingyoupin.top

JS:   // 无泛型
来源：http://rmn.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://thg.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cwu.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://upn.uphjek.com

Ruby: # 无泛型
来源：http://lsx.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eyq.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://faq.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mxm.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://fjn.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pln.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fvk.guowangkeji.top

Java: // 无解构
来源：http://ltm.jlsjyb.cn

Go:   // 无解构
来源：http://tkr.hesvh.cn

Ruby: a, b = pair
来源：http://fdz.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://odb.hesvh.cn

[C16] 函数 / 方法重载
来源：http://tfb.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kyi.jlsjyb.cn

PHP:  // 无重载
来源：http://mnh.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qjr.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://fmq.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nge.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://tbb.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://vdb.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ekc.hesvh.cn

================================================================================
来源：http://dhx.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://mki.yongpay.top

================================================================================
来源：http://dxl.bjfxy.top

[D01] 创建数组 / 列表
来源：http://oeq.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hai.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yxy.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rrd.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://szj.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://idk.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://gkd.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://ujo.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vvc.0kj1m.cn

[D02] 追加元素到末尾
来源：http://wkm.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ket.zdqjudy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dov.hnxiangtu.top

JS:   arr.push(4);
来源：http://slt.jqgufenzy.top

TS:   arr.push(4);
来源：http://rpj.quarkkingdee.top

Java: list.add(4);
来源：http://brn.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://njv.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://ypp.zhoulong.xyz

C#:   list.Add(4);
来源：http://kud.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://kvy.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://uok.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oyq.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qnx.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://yzg.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://llt.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xvg.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bkw.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://weg.ybcxt.top

[D04] 删除元素
来源：http://lxh.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qth.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wwk.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://shb.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://zjk.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hrp.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zcc.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dmb.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xjv.ybcxt.top

[D05] 访问与修改元素
来源：http://deq.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hbm.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mgv.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pey.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://bpt.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://qyj.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qvf.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ktg.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zjb.yangfankeji.com

[D06] 数组长度
来源：http://yus.aizwys.cn

Py:   len(arr)
来源：http://taa.gogol.net.cn

PHP:  count($arr);
来源：http://vsn.hysaishi.cn

JS:   arr.length
来源：http://nph.hnxiangtu.top

TS:   arr.length
来源：http://htg.ctjpmb.com

Java: list.size();
来源：http://vzl.redwolf501.top

Go:   len(arr)
来源：http://phu.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://hil.xinyue.icu

C#:   list.Count;
来源：http://uip.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://jnz.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqq.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://vho.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://yfa.yj202588.top

TS:   arr.slice(1, 4);
来源：http://ebq.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://nea.zhiwuduotai.top

Go:   arr[1:4]
来源：http://dru.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://qar.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://joe.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://tjh.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://pnn.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://fij.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kar.0kj1m.cn

TS:   [...a, ...b];
来源：http://lop.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uyr.zhixingplan.top

Go:   append(a, b...)
来源：http://twe.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://fek.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://kmv.jyoumei.cn

[D09] 排序（升序）
来源：http://hin.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://zxa.havefunace.top

PHP:  sort($arr);
来源：http://vcz.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xgs.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xdc.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zxr.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jmy.gzhubu.top

Ruby: arr.sort
来源：http://ltx.dashuyun.cn

C#:   list.Sort();
来源：http://qqt.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vce.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pjg.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgs.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yos.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sbz.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bay.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hta.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ilh.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qht.guowangkeji.top

[D11] 反转数组
来源：http://pmf.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://umz.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://fcr.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wew.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://bie.mhx1999.top

Java: Collections.reverse(list);
来源：http://cdr.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://dcy.kuanghao11.cn

Ruby: arr.reverse
来源：http://roy.fengsongda.top

C#:   list.Reverse();
来源：http://ktw.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://xot.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://ege.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pbf.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrb.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecu.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://med.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://nlv.cqqwz.cn

Ruby: arr.index(x)
来源：http://qjg.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://ewj.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://yxx.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://niz.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mix.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://xwo.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://yoh.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wty.shangyingyoupin.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dda.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://cgp.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qes.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://yex.vehdjk.com


<!-- 参考信息 -->