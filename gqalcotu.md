代发 wailian999

[B13] 判断是否为数字
来源：http://qar.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://rgi.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://zmv.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rsr.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zws.sxryk.cn

Java: x instanceof Number
来源：http://zzd.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ggo.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://gaa.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://rod.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://obw.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ctf.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gxd.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://zet.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://nza.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://prt.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ddu.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://skx.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pke.dianchejie.cn

[B15] 布尔运算与取反
来源：http://rbc.guowangkeji.top

Py:   a and b or not c
来源：http://sdn.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://ysh.gotoacloud.top

JS:   a && b || !c
来源：http://buk.ivvv.top

TS:   a && b || !c
来源：http://ljm.yj20258888.top

Java: a && b || !c
来源：http://nte.jinqigfzy.top

Go:   a && b || !c
来源：http://lfg.hysaishi.cn

Ruby: a && b || !c
来源：http://wgs.snrcjt.cn

C#:   a && b || !c
来源：http://xlb.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sbl.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://jaf.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://jxg.hfpthk.cn

JS:   if (!data) return;
来源：http://ryh.xziqi.cn

TS:   if (!data) return;
来源：http://rga.jlsjyb.cn

Java: if (data == null) return;
来源：http://ifh.yfazqb.com

Go:   if data == nil { return }
来源：http://tmx.0kj1m.cn

Ruby: return if data.nil?
来源：http://tlx.zhongyouzk.top

C#:   if (data == null) return;
来源：http://nyr.shangyingyoupin.top

================================================================================
来源：http://lqd.ivvv.top

C. 函数与作用域
来源：http://siz.xziqi.cn

================================================================================
来源：http://aqn.jinqigfzy.top

[C01] 定义函数
来源：http://jzi.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://gtv.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yon.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://aph.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uln.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dwn.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://mkj.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://wzg.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mha.sweek.top

[C02] 默认参数
来源：http://cgw.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://gmw.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://gqo.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://cuv.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zwf.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://gem.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eso.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://xvt.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://bmj.hcnkem.com

[C03] 可变参数
来源：http://ner.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://ctk.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tgo.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzr.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fvz.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yip.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eqc.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pqx.quarkkingdee.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rmi.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://ozl.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bal.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ylu.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zbe.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aap.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://tmm.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://vpy.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://mzr.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://ctz.havefunace.top

[C05] 返回多个值
来源：http://pcz.316326.xyz

Py:   return a, b
来源：http://egk.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://ycx.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ttu.shzxlz.cn

TS:   return { a, b };
来源：http://qcu.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lfl.yueranfly.top

Go:   return a, b
来源：http://qqx.gogol.net.cn

Ruby: return a, b
来源：http://cjl.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://jmb.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://qlm.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://mmz.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://oix.epnwcf.com

JS:   const square = x => x * x;
来源：http://pgv.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://pyy.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wye.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kdn.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://duj.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://mvg.bjfxy.top

[C07] 把函数作为参数传入
来源：http://yay.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hpp.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ual.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qyx.hnqzz.top

TS:   arr.map(String)
来源：http://okf.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jzg.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nlg.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://exl.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://lho.fehbvm.com

[C08] 闭包
来源：http://yqa.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zxj.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qqm.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://umh.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://igk.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qrb.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://plh.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lrh.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baz.pengpengdd.cyou

[C09] 递归
来源：http://cgm.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tsi.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iym.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yyy.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cew.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mfn.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rle.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vvu.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cji.epnwcf.com

[C10] 变量作用域
来源：http://hek.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zru.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mli.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ezy.havefunace.top

TS:   同 JS
来源：http://huw.cdnleiting.top

Java: 方法内为块级作用域
来源：http://tyj.shuidangran.top

Go:   花括号块级作用域
来源：http://slq.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hcy.yj202588.top

C#:   块级作用域
来源：http://wql.ydzc1.top

[C11] 模块导入与导出
来源：http://ugd.hnxiangtu.top

Py:   from module import func
来源：http://tsz.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wrl.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://kda.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baf.ppjwa.cn

Java: import java.util.List;
来源：http://fgt.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ihb.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://cgg.shzxlz.cn

C#:   using System.Text;
来源：http://ggu.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://vki.hammf.cn

Py:   (lambda: print("run"))()
来源：http://jug.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://wet.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://jxt.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://wbs.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eox.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://bdj.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://fdl.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bwt.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://pki.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ueu.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ery.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://roq.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jlh.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://itl.shuidangran.top

Go:   func add(a, b int) int
来源：http://zdj.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hrt.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lkp.gogol.net.cn

[C14] 泛型函数
来源：http://blx.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://omi.hnxiangtu.top

PHP:  // 无泛型
来源：http://kbo.feifeiyinyue.top

JS:   // 无泛型
来源：http://tck.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ybn.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lpy.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dmj.wangdashe.top

Ruby: # 无泛型
来源：http://imy.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dxf.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://uqq.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yxf.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://dec.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nfz.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bnt.chenzaomai.com

Java: // 无解构
来源：http://nuz.fzhhl.top

Go:   // 无解构
来源：http://pch.cashguo.top

Ruby: a, b = pair
来源：http://hqi.epnwcf.com

C#:   var (a, b) = pair;
来源：http://clq.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://lqc.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uns.vqdsnc.cn

PHP:  // 无重载
来源：http://sjs.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pxp.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://woc.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hmg.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://lps.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://kus.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xxd.hnxiangtu.top

================================================================================
来源：http://cke.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://dci.vqdsnc.cn

================================================================================
来源：http://kzm.fzhhl.top

[D01] 创建数组 / 列表
来源：http://hwu.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vcm.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://row.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://owg.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wfr.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://klo.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://cqy.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://qwq.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kuo.mhx1999.top

[D02] 追加元素到末尾
来源：http://dbu.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bmd.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kzq.zhiwuduotai.top

JS:   arr.push(4);
来源：http://vpg.hnqzz.top

TS:   arr.push(4);
来源：http://xct.fehbvm.com

Java: list.add(4);
来源：http://ske.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://fml.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://tqc.zhijiandao.cn

C#:   list.Add(4);
来源：http://iik.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://ioo.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://qyx.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://maw.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kks.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://iqw.chenzaomai.com

Java: list.add(0, 0);
来源：http://hzt.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ymy.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mwy.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://ljl.52xcode.cn

[D04] 删除元素
来源：http://zjz.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ita.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://puj.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wcu.pycfn.com

TS:   arr.splice(0, 1);
来源：http://pow.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cpr.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dnj.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qfz.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cfc.tian-w.cn

[D05] 访问与修改元素
来源：http://euf.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ypn.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gqc.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cac.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://osf.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://hhj.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://wet.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bpj.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://geg.guannengcc.top

[D06] 数组长度
来源：http://hmk.yfazqb.com

Py:   len(arr)
来源：http://zpb.guannengcc.top

PHP:  count($arr);
来源：http://kxf.shangyingyoupin.top

JS:   arr.length
来源：http://xok.yuxming.cn

TS:   arr.length
来源：http://ela.0kj1m.cn

Java: list.size();
来源：http://veo.zycfv.cn

Go:   len(arr)
来源：http://rdt.birdmap.top

Ruby: arr.length; arr.size
来源：http://jzy.cucudq.cn

C#:   list.Count;
来源：http://kge.sweek.top

[D07] 切片 / 取子数组
来源：http://owz.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kli.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://yhi.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://kvp.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://nnl.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://nbo.cdnleiting.top

Go:   arr[1:4]
来源：http://rrs.andypj.xyz

Ruby: arr[1, 3]
来源：http://shv.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://wrc.chenlongwang.top

[D08] 合并两个数组
来源：http://lli.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://tyw.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://pgs.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ids.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://qrk.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zvu.svipenyu.cn

Go:   append(a, b...)
来源：http://yyt.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://zuf.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://xcl.316326.xyz

[D09] 排序（升序）
来源：http://jtb.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ept.aibaodan.cn

PHP:  sort($arr);
来源：http://ugn.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sic.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uop.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yie.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://heb.fehbvm.com

Ruby: arr.sort
来源：http://ffq.yanxiufei.cn

C#:   list.Sort();
来源：http://mur.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://bsu.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hdm.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aak.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsa.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kyj.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://meo.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wgt.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xii.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wuh.aibaodan.cn

[D11] 反转数组
来源：http://apd.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://uvf.jianghu66.top

PHP:  array_reverse($arr);
来源：http://ttx.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tif.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://aid.ctjpmb.com

Java: Collections.reverse(list);
来源：http://tiq.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://bet.yfazqb.com

Ruby: arr.reverse
来源：http://vjr.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://zrr.daxiang520.top

[D12] 查找元素下标
来源：http://roi.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://aah.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gou.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xcp.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qwz.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jtg.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://zxy.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://tgj.hammf.cn

C#:   list.IndexOf(x);
来源：http://zji.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://hnm.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://okz.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://evz.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://jqm.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://abt.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxb.yfazqb.com


<!-- 参考信息 -->