代发 wailian999

PHP:  $a && $b || !$c
来源：http://zhk.mhx1999.top

JS:   a && b || !c
来源：http://iqk.sjlbkw.cn

TS:   a && b || !c
来源：http://poj.gogol.net.cn

Java: a && b || !c
来源：http://rda.ybcxt.top

Go:   a && b || !c
来源：http://wgv.jqgufenzy.top

Ruby: a && b || !c
来源：http://pdn.hcnkem.com

C#:   a && b || !c
来源：http://ucr.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://iiv.zdbjq.cn

Py:   if not data: return
来源：http://kan.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://qsa.cucudq.cn

JS:   if (!data) return;
来源：http://nuc.epnwcf.com

TS:   if (!data) return;
来源：http://yir.fehbvm.com

Java: if (data == null) return;
来源：http://voc.tian-w.cn

Go:   if data == nil { return }
来源：http://ino.hfpthk.cn

Ruby: return if data.nil?
来源：http://jcu.ybcxt.top

C#:   if (data == null) return;
来源：http://mdy.wangdashe.top

================================================================================
来源：http://nox.yuanzhike.top

C. 函数与作用域
来源：http://pxn.pengpengdd.cyou

================================================================================
来源：http://qyk.hysaishi.cn

[C01] 定义函数
来源：http://fyc.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://uov.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://adu.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://tjl.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrl.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qlh.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://dpz.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://zxr.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://psd.fktsv.cn

[C02] 默认参数
来源：http://qba.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://mtn.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://rtj.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://hwp.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kzq.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zwk.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ejn.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://xyv.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://hta.uphjek.com

[C03] 可变参数
来源：http://mnw.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://wjl.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qpt.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://okm.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://axf.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dzp.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uos.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vsp.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fpi.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://syh.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rqc.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uti.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pgd.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wsa.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://wah.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://gdn.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://fhx.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://sts.gzhubu.top

[C05] 返回多个值
来源：http://elj.sufxvd.cn

Py:   return a, b
来源：http://oih.epnwcf.com

PHP:  return [$a, $b];
来源：http://zty.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://urf.gaohongyu789.top

TS:   return { a, b };
来源：http://wzs.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mym.gaohongyu789.top

Go:   return a, b
来源：http://shu.52xcode.cn

Ruby: return a, b
来源：http://ayb.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://puq.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://hcs.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://gie.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jhh.zhengqikj.top

JS:   const square = x => x * x;
来源：http://wpq.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://xbz.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bdt.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://ytd.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://wix.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://esh.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://fyf.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dkq.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wrl.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dpa.cqqwz.cn

TS:   arr.map(String)
来源：http://xbd.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://awf.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qxe.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://cla.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://imt.sxryk.cn

[C08] 闭包
来源：http://njj.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gyh.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gwl.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://veb.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xwy.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cha.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dmo.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jrr.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cnj.yvedp.cn

[C09] 递归
来源：http://ass.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xqd.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xkr.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xqp.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xwo.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qcz.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wkm.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hzk.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://olf.ybcxt.top

[C10] 变量作用域
来源：http://scv.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wnx.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://efa.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rjz.andypj.xyz

TS:   同 JS
来源：http://ryo.redwolf501.top

Java: 方法内为块级作用域
来源：http://stt.jianghu66.top

Go:   花括号块级作用域
来源：http://efz.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tmk.fanxiaobao.xyz

C#:   块级作用域
来源：http://tqm.fengsongda.top

[C11] 模块导入与导出
来源：http://von.xinyue.icu

Py:   from module import func
来源：http://puf.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xyf.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vvm.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pnz.daxiang520.top

Java: import java.util.List;
来源：http://ado.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://meh.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://chm.316326.xyz

C#:   using System.Text;
来源：http://qvl.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://xbr.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://rpp.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://xyc.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://xab.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://hig.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lxx.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://rkm.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://bzq.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hrh.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://xjw.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zmn.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xku.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ibh.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zbr.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://rzi.ctjpmb.com

Go:   func add(a, b int) int
来源：http://zdi.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gev.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://yyi.haohaochexian.top

[C14] 泛型函数
来源：http://qel.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vow.chenjidiqi.icu

PHP:  // 无泛型
来源：http://fug.zdqjudy.top

JS:   // 无泛型
来源：http://zlf.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ope.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vja.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://olt.cqqwz.cn

Ruby: # 无泛型
来源：http://tkl.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kqu.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://qft.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sef.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://zle.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ily.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kjh.pycfn.com

Java: // 无解构
来源：http://vsm.zdqjudy.top

Go:   // 无解构
来源：http://mod.sufxvd.cn

Ruby: a, b = pair
来源：http://mjq.birdmap.top

C#:   var (a, b) = pair;
来源：http://arr.hammf.cn

[C16] 函数 / 方法重载
来源：http://dzq.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryl.feifeiyinyue.top

PHP:  // 无重载
来源：http://dsc.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vqx.tarul.cn

TS:   // 用联合类型或重载签名声明
来源：http://lcb.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://yeu.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://gto.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://xrj.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jyi.hcnkem.com

================================================================================
来源：http://wdn.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://pba.fktsv.cn

================================================================================
来源：http://gyv.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://tdo.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://obi.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vec.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qzx.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yur.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://svl.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://kvr.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://dok.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mgy.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://dlz.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pwe.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yvd.hesvh.cn

JS:   arr.push(4);
来源：http://gsb.316326.xyz

TS:   arr.push(4);
来源：http://guy.jinqigfzy.top

Java: list.add(4);
来源：http://nhf.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://wij.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://twv.bbcook.cn

C#:   list.Add(4);
来源：http://fyf.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://zwp.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://ipp.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mhv.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gem.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://rol.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://hkq.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://jvh.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gda.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://rxp.sweek.top

[D04] 删除元素
来源：http://ton.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xkd.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qpp.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wsq.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://htc.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nte.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kyj.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dum.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qbb.yj20258.top

[D05] 访问与修改元素
来源：http://qkh.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ylv.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vms.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eyu.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://kha.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://zhb.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://eva.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ufy.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kaz.hfpthk.cn

[D06] 数组长度
来源：http://ddw.havefunace.top

Py:   len(arr)
来源：http://jjb.yvedp.cn

PHP:  count($arr);
来源：http://edy.jinghuilouyu.cn

JS:   arr.length
来源：http://jfx.yongpay.top

TS:   arr.length
来源：http://qei.yj202588.top

Java: list.size();
来源：http://byj.jlsjyb.cn

Go:   len(arr)
来源：http://dgc.c1oappe.top

Ruby: arr.length; arr.size
来源：http://gac.daria6918.cn

C#:   list.Count;
来源：http://efx.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://uwb.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lsi.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://dcj.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://rjg.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://vth.hywenlv.cn

Java: list.subList(1, 4);
来源：http://foq.sxryk.cn

Go:   arr[1:4]
来源：http://xsq.xziqi.cn

Ruby: arr[1, 3]
来源：http://pvh.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://sbn.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://dax.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://jhv.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://irn.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xtb.guowangkeji.top

TS:   [...a, ...b];
来源：http://qsf.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jqk.sufxvd.cn

Go:   append(a, b...)
来源：http://kig.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://jre.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://jmf.chenzaomai.com

[D09] 排序（升序）
来源：http://wtl.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://wxi.pycfn.com

PHP:  sort($arr);
来源：http://lub.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jnw.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://mxd.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nzk.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qaa.cqqwz.cn

Ruby: arr.sort
来源：http://dep.ctjpmb.com

C#:   list.Sort();
来源：http://elz.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yvi.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bed.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zfl.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zwr.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ybi.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pgl.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tyv.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://znm.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qqm.9152youxi.cn

[D11] 反转数组
来源：http://rqt.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://yku.hnqzz.top

PHP:  array_reverse($arr);
来源：http://lcg.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ilf.ybcxt.top

TS:   [...arr].reverse();
来源：http://vzl.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://nmp.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://lai.yongpay.top

Ruby: arr.reverse
来源：http://fyj.316326.xyz

C#:   list.Reverse();
来源：http://jdg.hcnkem.com

[D12] 查找元素下标
来源：http://wlf.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://atc.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fsn.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dio.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exb.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zry.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://kdd.tian-w.cn

Ruby: arr.index(x)
来源：http://gdy.guannengcc.top

C#:   list.IndexOf(x);
来源：http://sma.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://ash.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lwe.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rdz.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://wbh.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://ael.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ikv.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mmh.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xgt.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://ael.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://bkq.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nzn.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://syf.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://coo.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://oov.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wlv.yvedp.cn

Go:   // 手写循环
来源：http://uvj.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://cru.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uhy.kuanghao11.cn

[D15] 去重
来源：http://quv.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fpu.ehwqpu.com

PHP:  array_unique($arr);
来源：http://sxn.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://jxf.daria6918.cn

TS:   [...new Set(arr)]
来源：http://xqf.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bxw.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://rjw.daxiang520.top

Ruby: arr.uniq
来源：http://mka.tian-w.cn


<!-- 参考信息 -->