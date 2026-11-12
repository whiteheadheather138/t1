代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://khn.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cfe.fengsongda.top

[B15] 布尔运算与取反
来源：http://wqt.wangdashe.top

Py:   a and b or not c
来源：http://pjt.pycfn.com

PHP:  $a && $b || !$c
来源：http://cvk.sxryk.cn

JS:   a && b || !c
来源：http://wgc.tian-w.cn

TS:   a && b || !c
来源：http://nee.dashuyun.cn

Java: a && b || !c
来源：http://cgg.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://akt.yuxming.cn

Ruby: a && b || !c
来源：http://mod.tian-w.cn

C#:   a && b || !c
来源：http://rna.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://dya.jinqigfzy.top

Py:   if not data: return
来源：http://akk.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://gnj.chenzaomai.com

JS:   if (!data) return;
来源：http://xpi.hongshengwenyu.top

TS:   if (!data) return;
来源：http://fhu.ydjk.org.cn

Java: if (data == null) return;
来源：http://dwl.tian-w.cn

Go:   if data == nil { return }
来源：http://ign.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://nan.zhijiandao.cn

C#:   if (data == null) return;
来源：http://ptc.iojbl.cn

================================================================================
来源：http://dnx.hnxiangtu.top

C. 函数与作用域
来源：http://zpg.hcnkem.com

================================================================================
来源：http://rac.9152youxi.cn

[C01] 定义函数
来源：http://jpg.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://mpi.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aas.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://bln.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jue.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://crn.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sfi.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://asu.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fvs.quarkkingdee.top

[C02] 默认参数
来源：http://gku.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://yju.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://xxq.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://osq.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://crg.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jkf.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nvu.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://clv.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://eap.hnxiangtu.top

[C03] 可变参数
来源：http://jot.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://fkm.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://toq.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jnj.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlu.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mmu.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zuy.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nqq.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ukd.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://aal.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://viq.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fys.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cma.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tel.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://xjt.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://mem.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://mfs.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://tap.fktsv.cn

[C05] 返回多个值
来源：http://tem.ehwqpu.com

Py:   return a, b
来源：http://emq.xylfe.cn

PHP:  return [$a, $b];
来源：http://sbb.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nhw.jinqigfzy.top

TS:   return { a, b };
来源：http://pej.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://udh.yvedp.cn

Go:   return a, b
来源：http://rhd.dashuyun.cn

Ruby: return a, b
来源：http://ygp.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ogc.havefunace.top

[C06] 匿名函数 / lambda
来源：http://wwj.redwolf501.top

Py:   square = lambda x: x * x
来源：http://wxh.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://hvz.hnqzz.top

JS:   const square = x => x * x;
来源：http://opr.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://edo.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gvo.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://akg.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://uce.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oce.birdmap.top

[C07] 把函数作为参数传入
来源：http://lwq.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bfz.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://huf.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kts.xinyue.icu

TS:   arr.map(String)
来源：http://vte.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://apg.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lcp.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://don.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hft.zdbjq.cn

[C08] 闭包
来源：http://rca.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vey.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pry.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nul.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yzq.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://azd.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wru.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mjo.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xlf.dashuyun.cn

[C09] 递归
来源：http://bkd.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://csh.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zkh.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ryt.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cfz.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jkw.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mfc.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nwy.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oos.shzxlz.cn

[C10] 变量作用域
来源：http://dxt.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ydk.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lad.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lqj.zhiwuduotai.top

TS:   同 JS
来源：http://gek.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://vtl.chenzaomai.com

Go:   花括号块级作用域
来源：http://wba.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://svw.smart0.xyz

C#:   块级作用域
来源：http://qbm.xuanzx.com

[C11] 模块导入与导出
来源：http://krk.jiagoushi.top

Py:   from module import func
来源：http://rkl.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nrf.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gwv.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://igy.yj20258888.top

Java: import java.util.List;
来源：http://vsv.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mgx.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://skh.shangyingyoupin.top

C#:   using System.Text;
来源：http://vrf.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://tkm.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://mml.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://nqb.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://hfy.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://xqa.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qtz.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://suk.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://obg.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://qfg.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://swq.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ryw.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmq.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pmx.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wpl.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://uwb.gotoacloud.top

Go:   func add(a, b int) int
来源：http://uge.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ylc.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://jqb.yj20258.top

[C14] 泛型函数
来源：http://wej.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yfl.redwolf501.top

PHP:  // 无泛型
来源：http://akg.zhongyouzk.top

JS:   // 无泛型
来源：http://htz.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cvp.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kfd.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvw.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://rqw.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eyw.iojbl.cn

[C15] 解构 / 展开参数
来源：http://lrh.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://clf.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://vwg.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kqd.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bdb.meibo888.top

Java: // 无解构
来源：http://baz.shanyushiyangkeji.top

Go:   // 无解构
来源：http://ofw.shzxlz.cn

Ruby: a, b = pair
来源：http://mrc.sysykeji.top

C#:   var (a, b) = pair;
来源：http://jcp.hesvh.cn

[C16] 函数 / 方法重载
来源：http://eyd.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://doc.hongshengwenyu.top

PHP:  // 无重载
来源：http://lrj.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qmw.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://qxx.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jtz.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://wzx.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://lti.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gbl.yj202588.top

================================================================================
来源：http://den.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://ydz.jqgfzy.top

================================================================================
来源：http://nhe.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://xrx.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pdd.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uzt.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pix.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fdt.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mgm.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://alw.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://rwo.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dok.jianghu66.top

[D02] 追加元素到末尾
来源：http://jfz.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rlm.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lmi.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://fpt.fengsongda.top

TS:   arr.push(4);
来源：http://vgf.aizwys.cn

Java: list.add(4);
来源：http://ugt.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://aqk.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://fay.52xcode.cn

C#:   list.Add(4);
来源：http://ryf.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://ctc.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://jps.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kyc.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tvf.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://exd.svipenyu.cn

Java: list.add(0, 0);
来源：http://gaj.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://jpk.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wup.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://yab.0kj1m.cn

[D04] 删除元素
来源：http://coz.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oyt.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fqv.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ucx.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://kkd.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ndh.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gje.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ccc.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jlc.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://fqn.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sgt.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tst.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hjr.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://wim.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://ofs.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://emm.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nmw.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rcz.meibo888.top

[D06] 数组长度
来源：http://emf.yfazqb.com

Py:   len(arr)
来源：http://qkt.tarul.cn

PHP:  count($arr);
来源：http://tdz.316326.xyz

JS:   arr.length
来源：http://tvk.gotoacloud.top

TS:   arr.length
来源：http://yct.yj20258888.top

Java: list.size();
来源：http://lej.bjfxy.top

Go:   len(arr)
来源：http://zpu.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://vvh.shangyingyoupin.top

C#:   list.Count;
来源：http://bcr.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://czn.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ecu.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://mtw.cheryme.top

JS:   arr.slice(1, 4);
来源：http://zgw.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://aqt.zdqjudy.top

Java: list.subList(1, 4);
来源：http://eyw.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://fyb.jqgfzy.top

Ruby: arr[1, 3]
来源：http://yhb.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://aqo.havefunace.top

[D08] 合并两个数组
来源：http://xbo.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://qif.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://rjp.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://pkd.zhoulong.xyz

TS:   [...a, ...b];
来源：http://tbt.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pfo.fehbvm.com

Go:   append(a, b...)
来源：http://hct.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://vyo.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://ptc.316326.xyz

[D09] 排序（升序）
来源：http://exi.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://acx.jianghu66.top

PHP:  sort($arr);
来源：http://exy.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bww.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yeu.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tcr.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pjc.zhoulong.xyz

Ruby: arr.sort
来源：http://loa.chenzaomai.com

C#:   list.Sort();
来源：http://gns.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://dvz.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oxo.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xtw.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pva.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vta.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mzo.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fec.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mnn.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aps.cashguo.top

[D11] 反转数组
来源：http://zra.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zyq.birdmap.top

PHP:  array_reverse($arr);
来源：http://chk.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gdl.yj20258.top

TS:   [...arr].reverse();
来源：http://rbh.sweek.top

Java: Collections.reverse(list);
来源：http://oyx.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://ixz.zhongyouzk.top

Ruby: arr.reverse
来源：http://xdy.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://knm.aizwys.cn

[D12] 查找元素下标
来源：http://cyc.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://abt.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yvz.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wnd.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dag.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://row.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://oiu.jiagoushi.top

Ruby: arr.index(x)
来源：http://tgu.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://gtp.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://mvt.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gve.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bzt.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://izo.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://qgn.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dav.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kly.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://cxj.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xaj.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://xbt.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ttx.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sqy.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://hln.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://qkd.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vnv.yj202588.top

Go:   // 手写循环
来源：http://voj.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://jdt.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://yto.ydjk.org.cn

[D15] 去重
来源：http://mwh.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jhe.daria6918.cn

PHP:  array_unique($arr);
来源：http://phj.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://sih.nwbrower.top


<!-- 参考信息 -->