代发 wailian999

Go:   a && b || !c
来源：http://yzp.yuxming.cn

Ruby: a && b || !c
来源：http://ylh.shanyushiyangtech.top

C#:   a && b || !c
来源：http://tqp.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://hgv.sweek.top

Py:   if not data: return
来源：http://klu.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://htq.ivvv.top

JS:   if (!data) return;
来源：http://pxo.daxiang520.top

TS:   if (!data) return;
来源：http://jlp.tian-w.cn

Java: if (data == null) return;
来源：http://ihv.uphjek.com

Go:   if data == nil { return }
来源：http://vfr.sxryk.cn

Ruby: return if data.nil?
来源：http://uzg.fzhhl.top

C#:   if (data == null) return;
来源：http://upe.yonumen.top

================================================================================
来源：http://idp.zdqjudy.top

C. 函数与作用域
来源：http://fak.jyoumei.cn

================================================================================
来源：http://fey.jinghuilouyu.cn

[C01] 定义函数
来源：http://ind.sweek.top

Py:   def add(a, b): return a + b
来源：http://npi.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gox.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://grc.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://any.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aaf.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://prp.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://wvj.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ahw.pengpengdd.cyou

[C02] 默认参数
来源：http://vgv.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://nkx.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://whs.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://wwt.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hvw.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rcf.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rpk.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://pso.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://mfl.nanxuanxn.top

[C03] 可变参数
来源：http://qec.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://lgs.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://twi.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vdp.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gfr.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sis.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qwy.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://fhb.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ihv.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://ynj.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mxn.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://joj.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bqv.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vln.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://fnm.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://toh.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://rgw.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://uiy.wangdashe.top

[C05] 返回多个值
来源：http://fyt.vqdsnc.cn

Py:   return a, b
来源：http://dov.yuxming.cn

PHP:  return [$a, $b];
来源：http://clp.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fdz.jlsjyb.cn

TS:   return { a, b };
来源：http://lbr.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gfn.xuetiantiany.cn

Go:   return a, b
来源：http://emf.zhixingplan.top

Ruby: return a, b
来源：http://awb.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://tyy.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://rwk.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://hom.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hqu.birdmap.top

JS:   const square = x => x * x;
来源：http://huz.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://ncf.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hgv.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ioc.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://nqs.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://dnd.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://kec.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hmt.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://ohq.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uhl.daxiang520.top

TS:   arr.map(String)
来源：http://jhe.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cwk.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pxn.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://uns.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fii.kuanghao11.cn

[C08] 闭包
来源：http://eqe.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ttd.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rwk.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jbh.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qoq.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://okl.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yio.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kgj.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gjh.jinyuanbaomall.cn

[C09] 递归
来源：http://jgf.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nfa.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gnx.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lgc.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxk.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qet.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vfp.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zli.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://drk.zdqjudy.top

[C10] 变量作用域
来源：http://acd.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fnp.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nxk.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yzl.hcnkem.com

TS:   同 JS
来源：http://lee.sweek.top

Java: 方法内为块级作用域
来源：http://sej.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://oje.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rua.meibo888.top

C#:   块级作用域
来源：http://mbx.redwolf501.top

[C11] 模块导入与导出
来源：http://scf.zhoulong.xyz

Py:   from module import func
来源：http://hgr.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://edk.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sfr.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://clj.ctjpmb.com

Java: import java.util.List;
来源：http://eib.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pqd.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://vyk.zhengqikj.top

C#:   using System.Text;
来源：http://wqr.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://iac.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://vhx.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://zyb.nwbrower.top

JS:   (() => { console.log("run"); })();
来源：http://mlb.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://eoo.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ovf.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://gnl.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://bbq.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wbl.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://rte.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mnk.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xdy.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nqz.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://buj.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mzv.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://tbb.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wkg.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cqm.sxryk.cn

[C14] 泛型函数
来源：http://esi.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ajq.c1oappe.top

PHP:  // 无泛型
来源：http://mim.andypj.xyz

JS:   // 无泛型
来源：http://amp.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbo.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jnc.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kux.xinyue.icu

Ruby: # 无泛型
来源：http://hfp.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yri.yueranfly.top

[C15] 解构 / 展开参数
来源：http://arp.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ndz.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://ybq.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sfm.zhiwuduotai.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eio.ydjk.org.cn

Java: // 无解构
来源：http://xxb.yj20258.top

Go:   // 无解构
来源：http://vns.yueranfly.top

Ruby: a, b = pair
来源：http://gox.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://zvc.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://ivo.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mxm.316326.xyz

PHP:  // 无重载
来源：http://ofp.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kgd.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://phd.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dhx.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://fsg.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://jjs.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://odr.dianchejie.cn

================================================================================
来源：http://vjp.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://gml.sxryk.cn

================================================================================
来源：http://vxm.hcnkem.com

[D01] 创建数组 / 列表
来源：http://gbl.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aas.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://muh.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mgj.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ryf.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xao.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://iqy.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://fjg.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jje.cdnleiting.top

[D02] 追加元素到末尾
来源：http://yep.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mvq.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kmq.hcnkem.com

JS:   arr.push(4);
来源：http://iby.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://jbx.snrcjt.cn

Java: list.add(4);
来源：http://ghl.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://xga.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://ype.yfazqb.com

C#:   list.Add(4);
来源：http://oic.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://wyj.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://qii.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jkk.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eht.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://tdl.redwolf501.top

Java: list.add(0, 0);
来源：http://gmr.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://bvr.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ulv.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://itq.xuetiantiany.cn

[D04] 删除元素
来源：http://vix.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://not.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nmg.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fzd.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://btx.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wfd.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bup.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfv.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xsn.hywenlv.cn

[D05] 访问与修改元素
来源：http://owr.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mox.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lee.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fii.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://vvh.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://fzj.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ebk.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rbm.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fwy.bbcook.cn

[D06] 数组长度
来源：http://owi.tianlin.xyz

Py:   len(arr)
来源：http://hcs.yanxiufei.cn

PHP:  count($arr);
来源：http://xsd.yj202588.top

JS:   arr.length
来源：http://iti.epnwcf.com

TS:   arr.length
来源：http://uzw.ydjk.org.cn

Java: list.size();
来源：http://jux.ehwqpu.com

Go:   len(arr)
来源：http://xku.redwolf501.top

Ruby: arr.length; arr.size
来源：http://slw.smart0.xyz

C#:   list.Count;
来源：http://icv.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://cyw.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fpa.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://zdg.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://cix.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://udf.chenzaomai.com

Java: list.subList(1, 4);
来源：http://smg.xuetiantiany.cn

Go:   arr[1:4]
来源：http://jub.shuidangran.top

Ruby: arr[1, 3]
来源：http://bvk.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://zed.ydzc1.top

[D08] 合并两个数组
来源：http://xky.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://nem.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://jli.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zxy.daxiang520.top

TS:   [...a, ...b];
来源：http://bks.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xtt.wangdashe.top

Go:   append(a, b...)
来源：http://eds.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://zsg.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://izc.zhengqikj.top

[D09] 排序（升序）
来源：http://pgl.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://gze.9152youxi.cn

PHP:  sort($arr);
来源：http://fdd.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sxw.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ppu.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://enm.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rbf.iojbl.cn

Ruby: arr.sort
来源：http://uxo.xylfe.cn

C#:   list.Sort();
来源：http://pxl.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oky.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hhe.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rna.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aje.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mce.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://crr.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rqp.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ppv.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sti.haohaochexian.top

[D11] 反转数组
来源：http://gvu.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://sji.ybcxt.top

PHP:  array_reverse($arr);
来源：http://nvh.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://icr.tian-w.cn

TS:   [...arr].reverse();
来源：http://bwu.gogol.net.cn

Java: Collections.reverse(list);
来源：http://mmp.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://rxh.chenlongwang.top

Ruby: arr.reverse
来源：http://mhh.snrcjt.cn

C#:   list.Reverse();
来源：http://qyx.smart0.xyz

[D12] 查找元素下标
来源：http://quv.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://ryi.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://way.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kia.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cqu.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gnq.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://zee.sjlbkw.cn

Ruby: arr.index(x)
来源：http://hql.shuidangran.top

C#:   list.IndexOf(x);
来源：http://mqv.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://kxf.sweek.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lxg.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dgc.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://ima.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://lmp.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lgu.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aca.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://gdu.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jcq.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://uvo.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://isd.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sbo.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://dlb.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://sqr.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lis.jiagoushi.top

Go:   // 手写循环
来源：http://ces.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://dgr.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pgk.jinyuanbaomall.cn

[D15] 去重
来源：http://qty.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ehp.zhengqikj.top

PHP:  array_unique($arr);
来源：http://bnh.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://xxl.yuxming.cn

TS:   [...new Set(arr)]
来源：http://xfa.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qig.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://med.9152youxi.cn

Ruby: arr.uniq
来源：http://lsa.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://aaq.ydzc1.top

[D16] 求和与平均值
来源：http://wjo.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hhx.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emz.ydzc1.top


<!-- 参考信息 -->