代发 wailian999

C#:   x is int or double or decimal
来源：http://ykw.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://bmm.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nkw.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zra.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://dtr.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://zvm.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rja.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xyw.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://phr.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uvg.pycfn.com

[B15] 布尔运算与取反
来源：http://gky.jqgufenzy.top

Py:   a and b or not c
来源：http://dnx.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://ioh.ydjk.org.cn

JS:   a && b || !c
来源：http://jql.ctjpmb.com

TS:   a && b || !c
来源：http://uhw.bjfxy.top

Java: a && b || !c
来源：http://tzc.dianchejie.cn

Go:   a && b || !c
来源：http://bgi.cashguo.top

Ruby: a && b || !c
来源：http://lmk.zhixingplan.top

C#:   a && b || !c
来源：http://vdj.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://itb.pengpengdd.cyou

Py:   if not data: return
来源：http://mbh.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://hnn.yanxiufei.cn

JS:   if (!data) return;
来源：http://xyt.cashguo.top

TS:   if (!data) return;
来源：http://qbl.xuetiantiany.cn

Java: if (data == null) return;
来源：http://tay.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://pqc.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://ooz.hnxiangtu.top

C#:   if (data == null) return;
来源：http://uhj.jlsjyb.cn

================================================================================
来源：http://ljx.sweek.top

C. 函数与作用域
来源：http://nfz.cdnleiting.top

================================================================================
来源：http://rcr.andypj.xyz

[C01] 定义函数
来源：http://hzy.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://xyo.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fvk.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://baw.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zim.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gnd.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://oit.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://cad.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sdo.guannengcc.top

[C02] 默认参数
来源：http://ydz.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://jfb.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dgh.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://uje.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jnj.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ggc.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mnc.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://dtb.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://bhn.fengsongda.top

[C03] 可变参数
来源：http://fmg.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://fce.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://krp.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://epy.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://koi.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://atc.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xhq.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qce.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uiy.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://lea.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qbx.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vgf.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xrj.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://flx.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://lrw.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://dol.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://qdk.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://kax.xinyue.icu

[C05] 返回多个值
来源：http://sqh.gotoacloud.top

Py:   return a, b
来源：http://lue.jinqigufen.top

PHP:  return [$a, $b];
来源：http://pgv.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bjf.bbcook.cn

TS:   return { a, b };
来源：http://ryj.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gha.tian-w.cn

Go:   return a, b
来源：http://hcx.sweek.top

Ruby: return a, b
来源：http://gsh.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://eho.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://hzf.tanke756.top

Py:   square = lambda x: x * x
来源：http://kbe.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://prm.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://ztp.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://pma.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wym.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ses.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://dxj.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://sss.fengsongda.top

[C07] 把函数作为参数传入
来源：http://cnp.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ano.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://myy.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hgp.nanxinkj.top

TS:   arr.map(String)
来源：http://apf.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ksz.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lcp.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://icg.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sfo.xziqi.cn

[C08] 闭包
来源：http://gxi.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ctb.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wdb.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://spt.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qal.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ccx.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ylu.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dog.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmm.fehbvm.com

[C09] 递归
来源：http://lnh.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://thk.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fpr.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gtm.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://evh.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dyq.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zkt.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uhd.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kex.xuetiantiany.cn

[C10] 变量作用域
来源：http://ien.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cbe.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zum.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ota.pycfn.com

TS:   同 JS
来源：http://tid.aizwys.cn

Java: 方法内为块级作用域
来源：http://xic.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://tef.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://msx.0kj1m.cn

C#:   块级作用域
来源：http://xyr.chenlongwang.top

[C11] 模块导入与导出
来源：http://zic.yueranfly.top

Py:   from module import func
来源：http://ulb.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://inp.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://syd.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eiy.fanxiaobao.xyz

Java: import java.util.List;
来源：http://tbc.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gfc.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://dyi.yfazqb.com

C#:   using System.Text;
来源：http://rpm.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://hap.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://pzm.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://oac.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://ewo.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://xfq.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://amv.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zgr.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://vzz.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rqa.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://bvg.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://udz.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mfk.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xen.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sjb.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ywf.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://yug.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zyb.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://xcm.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://osb.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdi.jlsjyb.cn

PHP:  // 无泛型
来源：http://wos.shuidangran.top

JS:   // 无泛型
来源：http://oyb.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dni.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mbk.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mrc.uphjek.com

Ruby: # 无泛型
来源：http://rdc.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yvo.tian-w.cn

[C15] 解构 / 展开参数
来源：http://uuc.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jxl.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://rhr.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ryr.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aop.52xcode.cn

Java: // 无解构
来源：http://vnq.xinyue.icu

Go:   // 无解构
来源：http://ksn.hywenlv.cn

Ruby: a, b = pair
来源：http://qnj.epnwcf.com

C#:   var (a, b) = pair;
来源：http://ctg.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://eij.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yyb.guannengcc.top

PHP:  // 无重载
来源：http://ivl.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vss.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://vaf.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mik.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://qno.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://skz.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ldd.gotoacloud.top

================================================================================
来源：http://uxh.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://qaq.jqgufenzy.top

================================================================================
来源：http://xnw.sysykeji.top

[D01] 创建数组 / 列表
来源：http://ian.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fyc.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lta.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bei.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tdk.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://evr.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://izu.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://cbo.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fyu.0kj1m.cn

[D02] 追加元素到末尾
来源：http://ist.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gux.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ajc.chenlongwang.top

JS:   arr.push(4);
来源：http://kih.aizwys.cn

TS:   arr.push(4);
来源：http://bse.hysaishi.cn

Java: list.add(4);
来源：http://qua.uphjek.com

Go:   arr = append(arr, 4)
来源：http://tje.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://ieu.svipenyu.cn

C#:   list.Add(4);
来源：http://mdj.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://fhg.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://aig.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sct.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jgy.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://czz.xylfe.cn

Java: list.add(0, 0);
来源：http://yez.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://wst.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://htp.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://tqv.jinyuanbaomall.cn

[D04] 删除元素
来源：http://hpq.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://npe.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rok.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yjl.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://nqv.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rdt.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://enu.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wfy.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eii.cheryme.top

[D05] 访问与修改元素
来源：http://ubn.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vwr.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cpi.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://epq.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://evv.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://lhr.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://qsx.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bni.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://knh.zdbjq.cn

[D06] 数组长度
来源：http://etw.jinyuanbaomall.cn

Py:   len(arr)
来源：http://njl.jqgfzy.top

PHP:  count($arr);
来源：http://gyn.yanxiufei.cn

JS:   arr.length
来源：http://vhh.jinqigfzy.top

TS:   arr.length
来源：http://ctw.hysaishi.cn

Java: list.size();
来源：http://mzq.pycfn.com

Go:   len(arr)
来源：http://tth.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://ctv.52xcode.cn

C#:   list.Count;
来源：http://sti.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://str.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ixe.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://wyv.yongpay.top

JS:   arr.slice(1, 4);
来源：http://vyz.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://xop.xylfe.cn

Java: list.subList(1, 4);
来源：http://fcf.jianghu66.top

Go:   arr[1:4]
来源：http://rex.zhixingplan.top

Ruby: arr[1, 3]
来源：http://agk.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://ftk.xylfe.cn

[D08] 合并两个数组
来源：http://eun.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://ijh.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://nzq.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ham.zhijiandao.cn

TS:   [...a, ...b];
来源：http://vuc.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ydi.hammf.cn

Go:   append(a, b...)
来源：http://bbl.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://voz.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://ume.ctjpmb.com

[D09] 排序（升序）
来源：http://tiy.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://koz.jinqigufen.top

PHP:  sort($arr);
来源：http://vvu.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kad.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://tkz.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tbt.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vdt.guowangkeji.top

Ruby: arr.sort
来源：http://ate.wangdashe.top

C#:   list.Sort();
来源：http://msl.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fqy.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rex.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tru.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ust.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfj.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vog.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ini.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yob.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fhl.birdmap.top

[D11] 反转数组
来源：http://hdk.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://tfx.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://bha.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://irv.yvedp.cn

TS:   [...arr].reverse();
来源：http://pyc.shuidangran.top

Java: Collections.reverse(list);
来源：http://hfr.yongpay.top

Go:   slices.Reverse(arr)
来源：http://mve.yuxming.cn

Ruby: arr.reverse
来源：http://kyg.zhijiandao.cn

C#:   list.Reverse();
来源：http://mlz.jlsjyb.cn

[D12] 查找元素下标
来源：http://kjc.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://gzy.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jxp.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pbw.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqe.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bio.yj20258.top

Go:   slices.Index(arr, x)
来源：http://gzj.smart0.xyz

Ruby: arr.index(x)
来源：http://ven.yj202588.top

C#:   list.IndexOf(x);
来源：http://tfw.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://wyu.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ehq.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mql.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://zjp.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://hyp.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wvy.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cos.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://pwz.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dnk.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://pqo.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mvu.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ocp.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://cor.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://glq.meibo888.top


<!-- 参考信息 -->