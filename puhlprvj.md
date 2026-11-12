代发 wailian999

[B13] 判断是否为数字
来源：http://noz.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://kow.fktsv.cn

PHP:  is_numeric($x)
来源：http://hha.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zkn.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zhf.kuanghao11.cn

Java: x instanceof Number
来源：http://kfx.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xbj.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://hwn.zycfv.cn

C#:   x is int or double or decimal
来源：http://rmx.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://mlw.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wzw.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://utt.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://phv.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://emf.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rfb.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yuv.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://jgh.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hzk.gotoacloud.top

[B15] 布尔运算与取反
来源：http://glr.zhixingplan.top

Py:   a and b or not c
来源：http://snf.zycfv.cn

PHP:  $a && $b || !$c
来源：http://cyf.shuidangran.top

JS:   a && b || !c
来源：http://zxe.mhx1999.top

TS:   a && b || !c
来源：http://adg.wangdashe.top

Java: a && b || !c
来源：http://sie.jinqigufen.top

Go:   a && b || !c
来源：http://nuk.cqqwz.cn

Ruby: a && b || !c
来源：http://mxh.zdbjq.cn

C#:   a && b || !c
来源：http://wnq.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hco.cheryme.top

Py:   if not data: return
来源：http://yxm.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://huj.shuidangran.top

JS:   if (!data) return;
来源：http://spe.pengpengdd.cyou

TS:   if (!data) return;
来源：http://uio.shzxlz.cn

Java: if (data == null) return;
来源：http://ejp.chenlongwang.top

Go:   if data == nil { return }
来源：http://woa.sysykeji.top

Ruby: return if data.nil?
来源：http://msn.yj20258.top

C#:   if (data == null) return;
来源：http://jhp.tian-w.cn

================================================================================
来源：http://gsm.ybcxt.top

C. 函数与作用域
来源：http://wqi.wangdashe.top

================================================================================
来源：http://rjc.cashguo.top

[C01] 定义函数
来源：http://bev.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://mqp.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpp.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://gqb.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hne.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jkh.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yiy.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://yga.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qpx.sufxvd.cn

[C02] 默认参数
来源：http://zgk.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://wtj.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zwb.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://fsr.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eur.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://flx.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qzi.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://fth.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://lvq.yanxiufei.cn

[C03] 可变参数
来源：http://uce.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://mcs.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xki.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jpj.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bsb.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vct.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yek.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://cal.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fgo.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://aba.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://edr.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sel.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wbb.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jvs.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://oqp.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://rie.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://zun.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://ucf.haohaochexian.top

[C05] 返回多个值
来源：http://lwo.zhiwuduotai.top

Py:   return a, b
来源：http://nof.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://zxf.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dhk.jqgfzy.top

TS:   return { a, b };
来源：http://wua.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hgk.chenjidiqi.icu

Go:   return a, b
来源：http://jzp.tianlin.xyz

Ruby: return a, b
来源：http://ygm.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://erv.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://gyy.havefunace.top

Py:   square = lambda x: x * x
来源：http://vxj.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://tcr.zdbjq.cn

JS:   const square = x => x * x;
来源：http://ljr.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://wrk.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ukn.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wvh.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://eqg.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://wur.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://nwu.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gbq.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yjo.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iwx.andypj.xyz

TS:   arr.map(String)
来源：http://gup.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ueo.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yfb.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://hvs.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nbd.jqgufenzy.top

[C08] 闭包
来源：http://svz.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rgm.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tha.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aoi.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dke.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xfw.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sze.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uiy.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://brq.yonumen.top

[C09] 递归
来源：http://qmb.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://otm.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://myb.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://muz.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihi.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xpb.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://umk.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rzl.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rrm.jinqigufen.top

[C10] 变量作用域
来源：http://wpu.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://erx.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uqc.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://egz.zycfv.cn

TS:   同 JS
来源：http://qwk.bjfxy.top

Java: 方法内为块级作用域
来源：http://tjg.ctjpmb.com

Go:   花括号块级作用域
来源：http://yxg.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gtd.vehdjk.com

C#:   块级作用域
来源：http://ees.cdnleiting.top

[C11] 模块导入与导出
来源：http://cml.quarkkingdee.top

Py:   from module import func
来源：http://cxh.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://nqp.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lyu.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fcq.gotoacloud.top

Java: import java.util.List;
来源：http://gnr.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://khl.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://ulu.aibaodan.cn

C#:   using System.Text;
来源：http://luu.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://htf.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://rnt.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://oeq.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://dnm.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://ian.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ltl.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://jmu.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://hsc.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vzq.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://aez.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://krj.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjj.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rmy.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvq.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://udb.cheryme.top

Go:   func add(a, b int) int
来源：http://nsu.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://shy.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nac.zhixingplan.top

[C14] 泛型函数
来源：http://kbe.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pga.jiagoushi.top

PHP:  // 无泛型
来源：http://xeu.yueranfly.top

JS:   // 无泛型
来源：http://hht.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://njf.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wmf.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gcf.fehbvm.com

Ruby: # 无泛型
来源：http://bom.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdr.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://ldu.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jam.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://mzl.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wqy.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cii.zhixingplan.top

Java: // 无解构
来源：http://wlt.hysaishi.cn

Go:   // 无解构
来源：http://dxw.vqdsnc.cn

Ruby: a, b = pair
来源：http://fca.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://njb.pycfn.com

[C16] 函数 / 方法重载
来源：http://cwl.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pnf.bbcook.cn

PHP:  // 无重载
来源：http://egh.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kwm.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://htq.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tmt.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://ssf.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://qku.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hpw.jinyuanbaomall.cn

================================================================================
来源：http://bfb.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://owy.yangfankeji.com

================================================================================
来源：http://fvi.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://juv.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://svv.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bhc.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://meu.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zgi.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ybb.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://yqr.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://arj.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://faq.316326.xyz

[D02] 追加元素到末尾
来源：http://rns.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jga.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pck.cqqwz.cn

JS:   arr.push(4);
来源：http://ocp.hnxiangtu.top

TS:   arr.push(4);
来源：http://iyv.ctjpmb.com

Java: list.add(4);
来源：http://itt.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://vqu.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://fcz.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://vjl.sysykeji.top

[D03] 在指定位置插入元素
来源：http://ynp.yj202588.top

Py:   arr.insert(0, 0)
来源：http://qwk.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zfg.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sek.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://fnd.dianchejie.cn

Java: list.add(0, 0);
来源：http://wcd.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://pyc.birdmap.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owy.316326.xyz

C#:   list.Insert(0, 0);
来源：http://izn.vqdsnc.cn

[D04] 删除元素
来源：http://rze.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://stp.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jmh.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mqj.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://bhl.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rhm.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jxj.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ryb.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nkf.bbcook.cn

[D05] 访问与修改元素
来源：http://jsq.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qww.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jli.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pdz.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://vnw.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://azp.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://kuo.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lbj.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sfr.chenlongwang.top

[D06] 数组长度
来源：http://qbg.nanxinkj.top

Py:   len(arr)
来源：http://rsx.tian-w.cn

PHP:  count($arr);
来源：http://ftq.cdnleiting.top

JS:   arr.length
来源：http://jex.yanxiufei.cn

TS:   arr.length
来源：http://ddd.ywan-chungtsiang.top

Java: list.size();
来源：http://dre.shzxlz.cn

Go:   len(arr)
来源：http://dwi.fengsongda.top

Ruby: arr.length; arr.size
来源：http://rgy.pycfn.com

C#:   list.Count;
来源：http://xeb.wangdashe.top

[D07] 切片 / 取子数组
来源：http://sba.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pgz.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://ulj.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://pxs.yj20258.top

TS:   arr.slice(1, 4);
来源：http://kmd.zhixingplan.top

Java: list.subList(1, 4);
来源：http://dpl.guannengcc.top

Go:   arr[1:4]
来源：http://ccg.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://eua.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://ihe.gotoacloud.top

[D08] 合并两个数组
来源：http://hmh.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://nup.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://rzp.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://lvs.shzxlz.cn

TS:   [...a, ...b];
来源：http://hyi.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://abe.hfpthk.cn

Go:   append(a, b...)
来源：http://zep.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://qzy.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://cfb.wangshuangyany.cn

[D09] 排序（升序）
来源：http://wdq.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://byg.0kj1m.cn

PHP:  sort($arr);
来源：http://ncy.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nme.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bgi.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tkt.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://opd.pengpengdd.cyou

Ruby: arr.sort
来源：http://fek.cheryme.top

C#:   list.Sort();
来源：http://ynu.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vis.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://haa.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffx.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://agz.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ump.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ujj.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rmm.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oee.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sia.ybcxt.top

[D11] 反转数组
来源：http://oyz.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://bum.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://rvs.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxh.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://msa.aizwys.cn

Java: Collections.reverse(list);
来源：http://xxg.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://ddl.0kj1m.cn

Ruby: arr.reverse
来源：http://bab.cucudq.cn

C#:   list.Reverse();
来源：http://zlz.guowangkeji.top

[D12] 查找元素下标
来源：http://itc.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://eni.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xya.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tsj.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrd.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://okm.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://bhq.yonumen.top

Ruby: arr.index(x)
来源：http://uqn.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://wsi.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://mwf.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jqe.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vzw.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://zga.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://fqk.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kce.zdbjq.cn


<!-- 参考信息 -->