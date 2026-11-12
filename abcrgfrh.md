代发 wailian999

Go:   a && b || !c
来源：http://ytd.zhoulong.xyz

Ruby: a && b || !c
来源：http://jew.hcnkem.com

C#:   a && b || !c
来源：http://zlg.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://flm.bbcook.cn

Py:   if not data: return
来源：http://phs.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://hjk.gotoacloud.top

JS:   if (!data) return;
来源：http://rop.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://qtk.9152youxi.cn

Java: if (data == null) return;
来源：http://fja.yj20258888.top

Go:   if data == nil { return }
来源：http://eve.fzhhl.top

Ruby: return if data.nil?
来源：http://zoi.yuxming.cn

C#:   if (data == null) return;
来源：http://flg.zhijiandao.cn

================================================================================
来源：http://ocx.bjfxy.top

C. 函数与作用域
来源：http://iin.andypj.xyz

================================================================================
来源：http://ccq.smart0.xyz

[C01] 定义函数
来源：http://jyy.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://etn.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fom.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://syw.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpy.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ory.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://fne.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://dzk.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://obw.ywan-chungtsiang.top

[C02] 默认参数
来源：http://ytz.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://itp.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kcg.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://xyw.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://rac.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://exu.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rzn.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://ehk.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://hfi.sysykeji.top

[C03] 可变参数
来源：http://kkx.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://ebx.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gqp.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://smr.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cvt.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vrj.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xbp.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://sui.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fja.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://blz.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rxl.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fmb.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sjj.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gde.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://nnp.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://mlu.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://lrq.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://tfk.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://gss.daxiang520.top

Py:   return a, b
来源：http://pui.aizwys.cn

PHP:  return [$a, $b];
来源：http://izx.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gdg.hnqzz.top

TS:   return { a, b };
来源：http://ile.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bsu.zhijiandao.cn

Go:   return a, b
来源：http://fom.smart0.xyz

Ruby: return a, b
来源：http://gwo.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://xag.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://bay.sweek.top

Py:   square = lambda x: x * x
来源：http://xom.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wwq.hcnkem.com

JS:   const square = x => x * x;
来源：http://wyk.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://eea.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kxx.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://pgq.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://xqf.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://lgm.sweek.top

[C07] 把函数作为参数传入
来源：http://czu.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rze.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://wzq.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://atv.mhx1999.top

TS:   arr.map(String)
来源：http://eud.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tjy.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wbv.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://tyc.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lyc.pycfn.com

[C08] 闭包
来源：http://rtj.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yvd.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kvi.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lmb.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oke.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oep.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xzx.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nfu.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gnz.tianlin.xyz

[C09] 递归
来源：http://mbp.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zqw.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pnb.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kya.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ccb.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iqj.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iip.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ndp.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://llo.ivvv.top

[C10] 变量作用域
来源：http://jpe.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rbx.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ter.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://unt.yj20258.top

TS:   同 JS
来源：http://nqg.jyoumei.cn

Java: 方法内为块级作用域
来源：http://xon.hesvh.cn

Go:   花括号块级作用域
来源：http://cji.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bvh.fanxiaobao.xyz

C#:   块级作用域
来源：http://bbt.yj202588.top

[C11] 模块导入与导出
来源：http://urp.yfazqb.com

Py:   from module import func
来源：http://wse.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xbc.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rzh.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pwj.zhiwuduotai.top

Java: import java.util.List;
来源：http://hxl.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wwj.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://arm.cashguo.top

C#:   using System.Text;
来源：http://bvk.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://rbb.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://xha.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://dsh.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://usw.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://djw.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://omv.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://ivo.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://nix.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://xwk.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://mzn.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nhy.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hfx.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gjv.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://osg.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ows.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://yzw.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ixz.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://tet.gotoacloud.top

[C14] 泛型函数
来源：http://hig.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jjr.ydjk.org.cn

PHP:  // 无泛型
来源：http://ayr.aibaodan.cn

JS:   // 无泛型
来源：http://jck.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xqg.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tet.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://imd.yangfankeji.com

Ruby: # 无泛型
来源：http://pop.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rbu.uphjek.com

[C15] 解构 / 展开参数
来源：http://ugi.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xtq.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://tfb.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bgz.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ddt.zhixingplan.top

Java: // 无解构
来源：http://nbb.ppjwa.cn

Go:   // 无解构
来源：http://xgp.gogol.net.cn

Ruby: a, b = pair
来源：http://lrs.ydzc1.top

C#:   var (a, b) = pair;
来源：http://bzg.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://zmo.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gyw.fehbvm.com

PHP:  // 无重载
来源：http://tbv.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qvy.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://oin.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iel.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://vgk.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://oqu.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bwz.uphjek.com

================================================================================
来源：http://ajv.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://oxd.gaohongyu789.top

================================================================================
来源：http://syr.yuxming.cn

[D01] 创建数组 / 列表
来源：http://pgi.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://azv.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://etx.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oee.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cmz.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ccv.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://two.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://oiu.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vfr.pycfn.com

[D02] 追加元素到末尾
来源：http://bqp.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hny.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://icj.yvedp.cn

JS:   arr.push(4);
来源：http://zgw.jyoumei.cn

TS:   arr.push(4);
来源：http://kqt.hammf.cn

Java: list.add(4);
来源：http://qma.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://oql.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://pzy.ydjk.org.cn

C#:   list.Add(4);
来源：http://eyv.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://mpl.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://bgj.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://inp.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://woz.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://prw.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://vqx.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://tim.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vjn.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://rbx.vqdsnc.cn

[D04] 删除元素
来源：http://pqi.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nll.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uye.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://igu.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://vel.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jqi.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lnm.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lxl.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yaq.c1oappe.top

[D05] 访问与修改元素
来源：http://xrw.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://trp.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ans.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rcv.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://nne.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://tze.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://zmf.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lrr.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xku.yonumen.top

[D06] 数组长度
来源：http://fkj.jqgfzy.top

Py:   len(arr)
来源：http://kys.wangdashe.top

PHP:  count($arr);
来源：http://sss.dashuyun.cn

JS:   arr.length
来源：http://sfp.xuetiantiany.cn

TS:   arr.length
来源：http://row.sweek.top

Java: list.size();
来源：http://efo.ydjk.org.cn

Go:   len(arr)
来源：http://lmu.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://rwc.xziqi.cn

C#:   list.Count;
来源：http://apn.bjfxy.top

[D07] 切片 / 取子数组
来源：http://dwm.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mrg.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cub.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://qqu.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://jfm.pycfn.com

Java: list.subList(1, 4);
来源：http://sup.nanxinkj.top

Go:   arr[1:4]
来源：http://tyf.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://xsw.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://bci.ydjk.org.cn

[D08] 合并两个数组
来源：http://ciu.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://zhq.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://bca.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pjk.cqqwz.cn

TS:   [...a, ...b];
来源：http://mpi.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://avh.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://jrf.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://biw.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://rba.jyoumei.cn

[D09] 排序（升序）
来源：http://uko.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://vio.yfazqb.com

PHP:  sort($arr);
来源：http://qqv.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfh.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://guy.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eux.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iqq.cucudq.cn

Ruby: arr.sort
来源：http://hld.xinyue.icu

C#:   list.Sort();
来源：http://gxw.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jom.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dyh.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vjd.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gue.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdp.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dkg.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vhh.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vho.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eps.havefunace.top

[D11] 反转数组
来源：http://ubt.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://haa.shuidangran.top

PHP:  array_reverse($arr);
来源：http://tle.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pkw.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://zhg.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://kds.yongpay.top

Go:   slices.Reverse(arr)
来源：http://wuj.xuanzx.com

Ruby: arr.reverse
来源：http://rpz.xuanzx.com

C#:   list.Reverse();
来源：http://sfr.birdmap.top

[D12] 查找元素下标
来源：http://sjz.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://wlr.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://klb.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fff.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hoc.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bcz.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://fdr.andypj.xyz

Ruby: arr.index(x)
来源：http://acw.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://mph.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://shl.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cbo.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hib.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://tgv.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://qmt.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://axo.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uvr.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://brv.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wfb.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://cit.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jxp.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tio.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://iit.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://omt.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gvy.feifeiyinyue.top

Go:   // 手写循环
来源：http://wop.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://pwu.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://qhg.9152youxi.cn

[D15] 去重
来源：http://mgh.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://adq.gzhubu.top

PHP:  array_unique($arr);
来源：http://roh.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://lsj.daria6918.cn

TS:   [...new Set(arr)]
来源：http://qrj.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sal.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://oqv.quarkkingdee.top

Ruby: arr.uniq
来源：http://alz.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://kei.xziqi.cn

[D16] 求和与平均值
来源：http://tvb.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qpf.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://edt.gogol.net.cn


<!-- 参考信息 -->