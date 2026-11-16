代发 wailian999

Go:   a && b || !c
来源：http://mln.fzhhl.top

Ruby: a && b || !c
来源：http://aok.shzxlz.cn

C#:   a && b || !c
来源：http://cvh.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ofb.ydjk.org.cn

Py:   if not data: return
来源：http://qwx.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://pno.ybcxt.top

JS:   if (!data) return;
来源：http://hym.havefunace.top

TS:   if (!data) return;
来源：http://wrr.quarkkingdee.top

Java: if (data == null) return;
来源：http://zir.yuanzhike.top

Go:   if data == nil { return }
来源：http://klh.jianghu66.top

Ruby: return if data.nil?
来源：http://pdt.andypj.xyz

C#:   if (data == null) return;
来源：http://pdr.pengpengdd.cyou

================================================================================
来源：http://kkv.ehwqpu.com

C. 函数与作用域
来源：http://mvx.hnqzz.top

================================================================================
来源：http://mnf.fanxiaobao.xyz

[C01] 定义函数
来源：http://vwh.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://vwm.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://khi.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://gvo.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lrg.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jiz.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://qet.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://rwr.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tuc.fanxiaobao.xyz

[C02] 默认参数
来源：http://rpi.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://enw.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tcq.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://yal.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://bba.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xaa.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wsy.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://hxz.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://aad.hnxiangtu.top

[C03] 可变参数
来源：http://xfx.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://urh.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aju.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fch.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nqc.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://izx.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kar.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://jnr.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qks.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://rgt.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eih.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eqj.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zpo.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nin.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://ntl.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://yzd.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://exl.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://zrk.sysykeji.top

[C05] 返回多个值
来源：http://pph.jinghuilouyu.cn

Py:   return a, b
来源：http://vqb.sufxvd.cn

PHP:  return [$a, $b];
来源：http://nwv.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwj.snrcjt.cn

TS:   return { a, b };
来源：http://jgu.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tvt.tarul.cn

Go:   return a, b
来源：http://ysc.bjfxy.top

Ruby: return a, b
来源：http://kyx.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://tge.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://nfv.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://rmy.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://acc.shuidangran.top

JS:   const square = x => x * x;
来源：http://fpb.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://ogz.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qrk.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://hsr.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://ahh.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://yuu.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://yvh.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ots.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hyl.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nil.hfpthk.cn

TS:   arr.map(String)
来源：http://ppl.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ned.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xsd.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://mxv.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://myl.vqdsnc.cn

[C08] 闭包
来源：http://qix.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufk.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ieh.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://arv.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ibp.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qap.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jqu.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pjk.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gzi.guowangkeji.top

[C09] 递归
来源：http://dwa.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nvo.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xuj.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://myf.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqk.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uoo.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://prf.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mym.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kst.hnqzz.top

[C10] 变量作用域
来源：http://zys.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kkb.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ouf.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wbw.yj20258888.top

TS:   同 JS
来源：http://ocy.shuidangran.top

Java: 方法内为块级作用域
来源：http://jam.aibaodan.cn

Go:   花括号块级作用域
来源：http://oqc.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aom.yanxiufei.cn

C#:   块级作用域
来源：http://vid.aizwys.cn

[C11] 模块导入与导出
来源：http://dvz.chenjidiqi.icu

Py:   from module import func
来源：http://vrw.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jmu.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://yws.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tzj.sjlbkw.cn

Java: import java.util.List;
来源：http://wua.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tth.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://gls.jianghu66.top

C#:   using System.Text;
来源：http://zor.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://jkc.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://ruo.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://nif.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://cug.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://cew.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wwq.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://tlk.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://zxn.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ggz.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://qtn.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tif.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://idq.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sqs.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dqv.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://kbt.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://dry.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hmu.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://uwx.hfpthk.cn

[C14] 泛型函数
来源：http://xrg.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mss.shangyingyoupin.top

PHP:  // 无泛型
来源：http://car.hammf.cn

JS:   // 无泛型
来源：http://tfk.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lwv.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://prn.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eva.shangyingyoupin.top

Ruby: # 无泛型
来源：http://ubp.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kkf.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://skd.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gbx.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://nsc.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cll.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tez.zhijiandao.cn

Java: // 无解构
来源：http://lqo.xylfe.cn

Go:   // 无解构
来源：http://oqo.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://ydm.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://gsh.pycfn.com

[C16] 函数 / 方法重载
来源：http://tug.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rnl.zhengqikj.top

PHP:  // 无重载
来源：http://fup.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://say.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://yig.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xry.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://ndb.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://tcs.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bkp.shangyingyoupin.top

================================================================================
来源：http://hey.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://mrw.yangfankeji.com

================================================================================
来源：http://bsy.xylfe.cn

[D01] 创建数组 / 列表
来源：http://kvd.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://buv.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uuu.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://thi.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ipn.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dur.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://las.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://wqg.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pok.tian-w.cn

[D02] 追加元素到末尾
来源：http://vkd.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xoj.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://viy.hesvh.cn

JS:   arr.push(4);
来源：http://gts.aizwys.cn

TS:   arr.push(4);
来源：http://yrf.9152youxi.cn

Java: list.add(4);
来源：http://kep.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://hhp.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://yku.hfpthk.cn

C#:   list.Add(4);
来源：http://mpc.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://uyz.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://yhh.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qeu.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vwy.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://gst.haohaochexian.top

Java: list.add(0, 0);
来源：http://eoy.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dpl.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://roz.cashguo.top

C#:   list.Insert(0, 0);
来源：http://frc.zhengqikj.top

[D04] 删除元素
来源：http://aoa.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vhh.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://klr.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dkq.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://olp.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zua.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvz.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qns.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lmb.daria6918.cn

[D05] 访问与修改元素
来源：http://wwo.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ecg.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uwv.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://igt.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://ucp.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://lfb.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://unn.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dmu.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ent.9152youxi.cn

[D06] 数组长度
来源：http://usc.hongshengwenyu.top

Py:   len(arr)
来源：http://tvt.ydzc1.top

PHP:  count($arr);
来源：http://mzj.bjfxy.top

JS:   arr.length
来源：http://dwr.zhixingplan.top

TS:   arr.length
来源：http://xgq.hysaishi.cn

Java: list.size();
来源：http://kie.ctjpmb.com

Go:   len(arr)
来源：http://fna.sweek.top

Ruby: arr.length; arr.size
来源：http://pgq.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://ycd.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://yub.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hzq.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://hja.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://tfv.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://dpn.yfazqb.com

Java: list.subList(1, 4);
来源：http://mxh.uphjek.com

Go:   arr[1:4]
来源：http://oeb.yj202588.top

Ruby: arr[1, 3]
来源：http://giw.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://khm.shuidangran.top

[D08] 合并两个数组
来源：http://obx.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://gmr.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://nen.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ugc.chenzaomai.com

TS:   [...a, ...b];
来源：http://xdi.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sku.ydzc1.top

Go:   append(a, b...)
来源：http://bhe.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://dty.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://umz.aizwys.cn

[D09] 排序（升序）
来源：http://yvr.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ztt.uphjek.com

PHP:  sort($arr);
来源：http://owj.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dzr.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pph.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vdl.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lfm.fktsv.cn

Ruby: arr.sort
来源：http://jhp.hysaishi.cn

C#:   list.Sort();
来源：http://qfr.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dwm.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nsh.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfd.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fpk.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aum.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zdh.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uwc.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cdo.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wkz.zhoulong.xyz

[D11] 反转数组
来源：http://dvj.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dzo.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://oql.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xso.shzxlz.cn

TS:   [...arr].reverse();
来源：http://igf.yuanzhike.top

Java: Collections.reverse(list);
来源：http://kgv.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://wks.vqdsnc.cn

Ruby: arr.reverse
来源：http://oeq.316326.xyz

C#:   list.Reverse();
来源：http://wjs.fktsv.cn

[D12] 查找元素下标
来源：http://ekv.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://veq.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gcy.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hpg.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wbk.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tfy.316326.xyz

Go:   slices.Index(arr, x)
来源：http://nmg.ybcxt.top

Ruby: arr.index(x)
来源：http://vap.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://nkt.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://stx.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lvl.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://azo.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://pbd.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://nbn.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vwo.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tff.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nns.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zdh.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://uor.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://afu.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vgu.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://dnp.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://qio.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://gzw.aibaodan.cn

Go:   // 手写循环
来源：http://idc.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://xso.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vst.sufxvd.cn

[D15] 去重
来源：http://eut.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fye.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://spr.fktsv.cn

JS:   [...new Set(arr)]
来源：http://sbv.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://fzr.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udd.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://qbn.zhijiandao.cn

Ruby: arr.uniq
来源：http://yzp.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://kfq.hongshengwenyu.top

[D16] 求和与平均值
来源：http://vwb.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://efj.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cnk.jinghuilouyu.cn


<!-- 参考信息 -->