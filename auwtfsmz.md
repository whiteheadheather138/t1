代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://yjn.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://cgo.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://yqm.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hlh.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://qia.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oii.52xcode.cn

[B15] 布尔运算与取反
来源：http://dqp.wangdashe.top

Py:   a and b or not c
来源：http://pgt.daria6918.cn

PHP:  $a && $b || !$c
来源：http://bvl.dashuyun.cn

JS:   a && b || !c
来源：http://wbr.0kj1m.cn

TS:   a && b || !c
来源：http://wet.xinyue.icu

Java: a && b || !c
来源：http://nar.xuetiantiany.cn

Go:   a && b || !c
来源：http://mln.yuxming.cn

Ruby: a && b || !c
来源：http://boo.cdnleiting.top

C#:   a && b || !c
来源：http://hpj.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://sgp.jqgfzy.top

Py:   if not data: return
来源：http://nis.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://hhy.guowangkeji.top

JS:   if (!data) return;
来源：http://qjd.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://gyu.ybcxt.top

Java: if (data == null) return;
来源：http://vdq.xylfe.cn

Go:   if data == nil { return }
来源：http://zdx.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://tgq.hesvh.cn

C#:   if (data == null) return;
来源：http://vfd.feifeiyinyue.top

================================================================================
来源：http://isq.epnwcf.com

C. 函数与作用域
来源：http://xrg.redwolf501.top

================================================================================
来源：http://gvk.shangyingyoupin.top

[C01] 定义函数
来源：http://cuh.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://wvt.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tcy.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://ukm.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vey.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ljw.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://nxs.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://jdh.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tzy.daxiang520.top

[C02] 默认参数
来源：http://mfl.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://miv.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://gke.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://kja.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://joc.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://liv.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tyx.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://uzj.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://xrq.daria6918.cn

[C03] 可变参数
来源：http://oie.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://dbx.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xlz.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://udx.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zoa.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://umw.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ngj.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://jnh.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wno.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://dtc.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tww.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nvd.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ucj.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pdj.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://aok.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://juk.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://svg.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://zet.xuetiantiany.cn

[C05] 返回多个值
来源：http://uoa.ydjk.org.cn

Py:   return a, b
来源：http://kdk.chenzaomai.com

PHP:  return [$a, $b];
来源：http://jyg.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jgb.cheryme.top

TS:   return { a, b };
来源：http://vcb.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gly.wangshuangyany.cn

Go:   return a, b
来源：http://hoq.yuxming.cn

Ruby: return a, b
来源：http://bex.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://ksh.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://loc.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://pom.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://adl.316326.xyz

JS:   const square = x => x * x;
来源：http://wti.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://vjv.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ivj.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iky.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://cqv.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fvd.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://mhh.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rlw.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vro.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jti.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://lzi.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kcm.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rkq.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://bkc.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vuf.guowangkeji.top

[C08] 闭包
来源：http://ieu.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ugu.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qog.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cki.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hrb.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hle.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sov.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tef.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sqn.epnwcf.com

[C09] 递归
来源：http://dgk.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cva.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lcs.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npg.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vyl.hesvh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jvt.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xgc.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kyf.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bdm.guannengcc.top

[C10] 变量作用域
来源：http://apy.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hsj.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mov.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eru.jyoumei.cn

TS:   同 JS
来源：http://zem.chenlongwang.top

Java: 方法内为块级作用域
来源：http://vhy.daxiang520.top

Go:   花括号块级作用域
来源：http://tbu.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jzu.xinyue.icu

C#:   块级作用域
来源：http://jpt.dashuyun.cn

[C11] 模块导入与导出
来源：http://jbn.iojbl.cn

Py:   from module import func
来源：http://iwq.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hnt.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pok.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pgo.0kj1m.cn

Java: import java.util.List;
来源：http://ddh.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wch.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://uni.zdbjq.cn

C#:   using System.Text;
来源：http://pqo.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://zhh.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://tvz.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://ufl.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://kwb.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://sjs.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mnr.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://lub.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://ggk.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pkq.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://bgs.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fyp.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://atm.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yrb.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://maj.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://czc.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://ezm.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ofk.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://nbc.ydzc1.top

[C14] 泛型函数
来源：http://byb.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nbi.zhijiandao.cn

PHP:  // 无泛型
来源：http://noc.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://tkm.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ylz.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nbw.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vtw.zhiwuduotai.top

Ruby: # 无泛型
来源：http://zhi.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fvu.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://vzb.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jdh.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://mgg.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gum.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ekv.cdnleiting.top

Java: // 无解构
来源：http://ayg.svipenyu.cn

Go:   // 无解构
来源：http://dss.pycfn.com

Ruby: a, b = pair
来源：http://ipy.cheryme.top

C#:   var (a, b) = pair;
来源：http://gfx.sysykeji.top

[C16] 函数 / 方法重载
来源：http://fdx.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bul.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://gzp.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://phf.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://ssi.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jyr.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://tem.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://yhz.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yzc.sysykeji.top

================================================================================
来源：http://njl.ivvv.top

D. 数组 / 列表 / 集合
来源：http://icd.epnwcf.com

================================================================================
来源：http://nva.xinyue.icu

[D01] 创建数组 / 列表
来源：http://rzf.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jwv.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://izc.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xap.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://unj.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zuy.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://ktk.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://jqy.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vrt.daxiang520.top

[D02] 追加元素到末尾
来源：http://jii.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hnj.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xnd.mhx1999.top

JS:   arr.push(4);
来源：http://egz.yvedp.cn

TS:   arr.push(4);
来源：http://cxl.hnxiangtu.top

Java: list.add(4);
来源：http://hth.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://zcx.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://xkr.redwolf501.top

C#:   list.Add(4);
来源：http://zdz.hammf.cn

[D03] 在指定位置插入元素
来源：http://wgs.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://hwp.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hjd.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lpu.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://abk.fehbvm.com

Java: list.add(0, 0);
来源：http://wba.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://clz.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gjx.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://lqm.kuanghao11.cn

[D04] 删除元素
来源：http://ybu.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sej.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://evl.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ieq.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://jls.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ujy.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uzd.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jvh.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zse.svipenyu.cn

[D05] 访问与修改元素
来源：http://wov.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mrc.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yev.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pvg.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://lpl.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://fwl.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://bjb.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rst.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qqx.guannengcc.top

[D06] 数组长度
来源：http://wkg.uphjek.com

Py:   len(arr)
来源：http://lgk.guannengcc.top

PHP:  count($arr);
来源：http://cex.shanyushiyangkeji.top

JS:   arr.length
来源：http://ymw.sufxvd.cn

TS:   arr.length
来源：http://nsp.chenzaomai.com

Java: list.size();
来源：http://dli.nanxinkj.top

Go:   len(arr)
来源：http://cls.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://jqt.gaohongyu789.top

C#:   list.Count;
来源：http://cpe.yfazqb.com

[D07] 切片 / 取子数组
来源：http://jql.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ccd.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fia.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://gdg.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://fdb.sufxvd.cn

Java: list.subList(1, 4);
来源：http://amz.fengsongda.top

Go:   arr[1:4]
来源：http://dzr.nwbrower.top

Ruby: arr[1, 3]
来源：http://lur.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://xbn.jlsjyb.cn

[D08] 合并两个数组
来源：http://cen.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://tmh.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://ovx.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ypo.haohaochexian.top

TS:   [...a, ...b];
来源：http://wkj.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cvl.ivvv.top

Go:   append(a, b...)
来源：http://cjh.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://aya.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://god.quarkkingdee.top

[D09] 排序（升序）
来源：http://ffp.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://dzr.mhx1999.top

PHP:  sort($arr);
来源：http://xee.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dzz.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://bee.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ltn.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nfr.chenlongwang.top

Ruby: arr.sort
来源：http://hjs.fehbvm.com

C#:   list.Sort();
来源：http://hnr.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cpy.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jzf.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://swf.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bif.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oua.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fqr.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vks.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dpn.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bqr.shangyingyoupin.top

[D11] 反转数组
来源：http://khl.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zrw.xinyue.icu

PHP:  array_reverse($arr);
来源：http://zvm.kuanghao11.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qsz.yongpay.top

TS:   [...arr].reverse();
来源：http://akr.zhengqikj.top

Java: Collections.reverse(list);
来源：http://jdn.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://bwg.yuanzhike.top

Ruby: arr.reverse
来源：http://urg.nanxinkj.top

C#:   list.Reverse();
来源：http://ncp.yangfankeji.com

[D12] 查找元素下标
来源：http://xby.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://ore.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kav.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjh.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qvh.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xjq.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://rav.havefunace.top

Ruby: arr.index(x)
来源：http://akd.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://tzi.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://vzx.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rhq.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xbw.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://bhp.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://rpl.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fqq.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bga.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zhs.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dap.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://nbm.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gof.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://isx.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://shg.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://vvu.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://djf.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://bsm.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://mff.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ogz.jyoumei.cn


<!-- 参考信息 -->