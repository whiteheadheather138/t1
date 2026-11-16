代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zdo.kuanghao11.cn

Java: x instanceof Number
来源：http://avq.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ivp.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://biq.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://rqs.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://pna.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://shk.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rsn.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://osd.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://cxn.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ffb.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wjy.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://ccv.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bbz.nanxinkj.top

[B15] 布尔运算与取反
来源：http://ups.ppjwa.cn

Py:   a and b or not c
来源：http://fkg.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://wyf.nwbrower.top

JS:   a && b || !c
来源：http://ltk.0kj1m.cn

TS:   a && b || !c
来源：http://dwl.shuidangran.top

Java: a && b || !c
来源：http://ihx.ppjwa.cn

Go:   a && b || !c
来源：http://xjy.yj20258888.top

Ruby: a && b || !c
来源：http://gnd.yangfankeji.com

C#:   a && b || !c
来源：http://dio.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mqy.yj20258.top

Py:   if not data: return
来源：http://fzf.cashguo.top

PHP:  if (!$data) { return; }
来源：http://raa.yangfankeji.com

JS:   if (!data) return;
来源：http://qdw.bjfxy.top

TS:   if (!data) return;
来源：http://qda.pengpengdd.cyou

Java: if (data == null) return;
来源：http://kih.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://nfr.yj202588.top

Ruby: return if data.nil?
来源：http://lqp.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://cls.0kj1m.cn

================================================================================
来源：http://ica.cheryme.top

C. 函数与作用域
来源：http://kff.yvedp.cn

================================================================================
来源：http://zah.fengsongda.top

[C01] 定义函数
来源：http://xim.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://umf.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ayr.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://mva.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rmh.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fri.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://cjw.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://cbe.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pcl.aizwys.cn

[C02] 默认参数
来源：http://ofm.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://jwo.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yjg.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://wik.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qkh.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kuc.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mev.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://bcn.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://ela.shanyushiyangkeji.top

[C03] 可变参数
来源：http://wsi.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://obl.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vws.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nkm.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gbh.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sxb.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ffg.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://whs.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fmm.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://orm.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dha.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bly.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jrs.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mds.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://gdu.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://vfx.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://chi.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://jye.yj202588.top

[C05] 返回多个值
来源：http://lqx.chenlongwang.top

Py:   return a, b
来源：http://gkr.chenlongwang.top

PHP:  return [$a, $b];
来源：http://gkf.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ygb.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://myi.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oqn.havefunace.top

Go:   return a, b
来源：http://vch.jlsjyb.cn

Ruby: return a, b
来源：http://lwz.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://xiw.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://ejt.shuidangran.top

Py:   square = lambda x: x * x
来源：http://vtt.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ugm.dianchejie.cn

JS:   const square = x => x * x;
来源：http://cul.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://clf.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dpj.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://mgb.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://oul.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://sol.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://rqa.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ulc.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://aem.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oqo.sxryk.cn

TS:   arr.map(String)
来源：http://zvs.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ggp.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mwt.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://drf.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uxi.fengsongda.top

[C08] 闭包
来源：http://ndb.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dlk.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pod.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fvq.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qiq.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tmy.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ezt.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xnk.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nqz.hysaishi.cn

[C09] 递归
来源：http://jcz.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rjh.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bay.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://emc.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lvp.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://luq.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tgc.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dhf.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxq.svipenyu.cn

[C10] 变量作用域
来源：http://bgl.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rsj.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://anl.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jxk.dianchejie.cn

TS:   同 JS
来源：http://ahh.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://cgd.shzxlz.cn

Go:   花括号块级作用域
来源：http://cft.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jtd.dianchejie.cn

C#:   块级作用域
来源：http://hzs.zhengqikj.top

[C11] 模块导入与导出
来源：http://bcz.fengsongda.top

Py:   from module import func
来源：http://ubk.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aas.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vpj.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://poe.sweek.top

Java: import java.util.List;
来源：http://mxj.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gme.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://qqv.shanyushiyangtech.top

C#:   using System.Text;
来源：http://jis.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://ctq.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://cqq.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://xlv.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://wbg.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://ogu.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jwm.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://gaj.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://cbd.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://oaw.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://hcu.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xsl.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dbp.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pbi.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xvk.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dyi.dianchejie.cn

Go:   func add(a, b int) int
来源：http://skh.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://udn.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wqx.zhongyouzk.top

[C14] 泛型函数
来源：http://jxk.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jdb.pengpengdd.cyou

PHP:  // 无泛型
来源：http://njd.bjfxy.top

JS:   // 无泛型
来源：http://dtn.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rgk.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cdh.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rtv.xuetiantiany.cn

Ruby: # 无泛型
来源：http://gnz.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://enu.yj20258.top

[C15] 解构 / 展开参数
来源：http://kjg.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lfv.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://agc.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://weu.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pef.cheryme.top

Java: // 无解构
来源：http://thg.tanke756.top

Go:   // 无解构
来源：http://yoq.zhiwuduotai.top

Ruby: a, b = pair
来源：http://aib.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://kik.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://nuv.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vmw.yj202588.top

PHP:  // 无重载
来源：http://zkf.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kcf.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://pvi.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xhq.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://ccr.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://aik.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ver.fzhhl.top

================================================================================
来源：http://toe.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://geb.shangyingyoupin.top

================================================================================
来源：http://drh.hcnkem.com

[D01] 创建数组 / 列表
来源：http://kzl.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://awf.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ubv.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://med.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tnb.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://clc.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://gvp.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://xcl.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://izg.ybcxt.top

[D02] 追加元素到末尾
来源：http://kfa.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tej.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kyl.guowangkeji.top

JS:   arr.push(4);
来源：http://ili.jinqigufen.top

TS:   arr.push(4);
来源：http://ntx.fzhhl.top

Java: list.add(4);
来源：http://vtg.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://toh.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://pcd.yuanzhike.top

C#:   list.Add(4);
来源：http://osj.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://lwg.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://yhu.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lun.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xdi.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://uyt.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://evq.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://cti.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qkn.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://izb.ivvv.top

[D04] 删除元素
来源：http://apm.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://krv.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nrw.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nlr.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://kjn.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qju.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipr.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xnk.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tnk.yangfankeji.com

[D05] 访问与修改元素
来源：http://ldu.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eoo.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qme.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://agi.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://met.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://ekl.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://fbg.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cvr.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fyc.guannengcc.top

[D06] 数组长度
来源：http://zcn.wangshuangyany.cn

Py:   len(arr)
来源：http://mdb.feifeiyinyue.top

PHP:  count($arr);
来源：http://glm.zhoulong.xyz

JS:   arr.length
来源：http://rqo.bbcook.cn

TS:   arr.length
来源：http://bda.ctjpmb.com

Java: list.size();
来源：http://atf.cucudq.cn

Go:   len(arr)
来源：http://xbj.tian-w.cn

Ruby: arr.length; arr.size
来源：http://hcw.xylfe.cn

C#:   list.Count;
来源：http://oct.yueranfly.top

[D07] 切片 / 取子数组
来源：http://vya.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://juw.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://mlx.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://xoz.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://hhp.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://cof.iojbl.cn

Go:   arr[1:4]
来源：http://lwf.shuidangran.top

Ruby: arr[1, 3]
来源：http://oxk.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://tmw.snrcjt.cn

[D08] 合并两个数组
来源：http://ukc.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://kjv.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://red.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ylj.jqgfzy.top

TS:   [...a, ...b];
来源：http://onv.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yvn.yangfankeji.com

Go:   append(a, b...)
来源：http://mjr.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://zji.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://ygu.havefunace.top

[D09] 排序（升序）
来源：http://ada.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://nri.guannengcc.top

PHP:  sort($arr);
来源：http://yad.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cjs.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xju.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://yqg.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tda.9152youxi.cn

Ruby: arr.sort
来源：http://dia.hcnkem.com

C#:   list.Sort();
来源：http://krj.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://pyk.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qzj.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ntp.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbq.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aka.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ihe.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kgx.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ggk.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tcq.sweek.top

[D11] 反转数组
来源：http://yuu.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://age.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://dkk.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxn.yuanzhike.top

TS:   [...arr].reverse();
来源：http://xjs.cashguo.top

Java: Collections.reverse(list);
来源：http://kle.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://nuk.redwolf501.top

Ruby: arr.reverse
来源：http://abg.9152youxi.cn

C#:   list.Reverse();
来源：http://elr.sweek.top

[D12] 查找元素下标
来源：http://htg.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://zcx.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kzr.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hhd.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vcl.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://smb.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://lna.guowangkeji.top

Ruby: arr.index(x)
来源：http://bgx.xziqi.cn

C#:   list.IndexOf(x);
来源：http://xuk.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://tux.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uai.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eil.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://mwq.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://syt.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aif.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zve.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://byh.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hvj.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://mfl.xziqi.cn


<!-- 参考信息 -->