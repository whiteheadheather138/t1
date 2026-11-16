代发 wailian999

C#:   x is int or double or decimal
来源：http://ntp.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://zsn.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ksv.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ney.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://zda.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://krl.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yht.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mzx.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://zlw.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oxb.ctjpmb.com

[B15] 布尔运算与取反
来源：http://eig.yonumen.top

Py:   a and b or not c
来源：http://xjg.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://ssj.gaohongyu789.top

JS:   a && b || !c
来源：http://qmv.zhixingplan.top

TS:   a && b || !c
来源：http://wyb.sxryk.cn

Java: a && b || !c
来源：http://sqc.svipenyu.cn

Go:   a && b || !c
来源：http://hrj.feifeiyinyue.top

Ruby: a && b || !c
来源：http://ydd.pycfn.com

C#:   a && b || !c
来源：http://cyt.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://fzg.zhengqikj.top

Py:   if not data: return
来源：http://yjf.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://yif.bbcook.cn

JS:   if (!data) return;
来源：http://nqb.hesvh.cn

TS:   if (!data) return;
来源：http://mdg.mhx1999.top

Java: if (data == null) return;
来源：http://ask.shuidangran.top

Go:   if data == nil { return }
来源：http://qvz.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://pkx.jyoumei.cn

C#:   if (data == null) return;
来源：http://cwt.gogol.net.cn

================================================================================
来源：http://jig.daria6918.cn

C. 函数与作用域
来源：http://hak.zhixingplan.top

================================================================================
来源：http://hhh.0kj1m.cn

[C01] 定义函数
来源：http://jbt.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://dqi.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mjt.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://evi.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fcj.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://mzk.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://tkd.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://qdb.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cko.hcnkem.com

[C02] 默认参数
来源：http://ebl.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://pxv.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://auo.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://zvv.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://csc.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mwe.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vdw.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://bmh.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://syf.tian-w.cn

[C03] 可变参数
来源：http://zqs.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://dtj.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tgu.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yst.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wby.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zya.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aiq.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://fcx.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sgs.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://huy.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://njx.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xpo.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cnn.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dwb.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://knz.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://skk.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://ans.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://snv.sysykeji.top

[C05] 返回多个值
来源：http://fwn.svipenyu.cn

Py:   return a, b
来源：http://ymp.havefunace.top

PHP:  return [$a, $b];
来源：http://hvd.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://smb.zhengqikj.top

TS:   return { a, b };
来源：http://hmp.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dvg.chenzaomai.com

Go:   return a, b
来源：http://gtj.sxryk.cn

Ruby: return a, b
来源：http://hcb.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://lhg.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://dyb.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://uja.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jpx.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://urb.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://abt.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://czt.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://mct.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://fdv.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://baq.aizwys.cn

[C07] 把函数作为参数传入
来源：http://pvn.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nxi.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://mea.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tfr.guannengcc.top

TS:   arr.map(String)
来源：http://qcj.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eqj.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://puj.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://tdl.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oai.guowangkeji.top

[C08] 闭包
来源：http://zfs.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xhs.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zwd.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rfs.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fqs.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lmc.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ype.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hqa.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://flv.yangfankeji.com

[C09] 递归
来源：http://uvd.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jtl.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xbf.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtw.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xtp.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rts.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pwm.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fqg.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tep.jinqigfzy.top

[C10] 变量作用域
来源：http://djs.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oat.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ffg.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://geu.shzxlz.cn

TS:   同 JS
来源：http://ybp.xylfe.cn

Java: 方法内为块级作用域
来源：http://yvs.ivvv.top

Go:   花括号块级作用域
来源：http://bej.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ysr.hywenlv.cn

C#:   块级作用域
来源：http://mpj.yueranfly.top

[C11] 模块导入与导出
来源：http://onc.havefunace.top

Py:   from module import func
来源：http://gng.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qwm.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sth.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jxc.xuanzx.com

Java: import java.util.List;
来源：http://uuw.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://akm.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://trg.sysykeji.top

C#:   using System.Text;
来源：http://sxd.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://ufr.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://mtb.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://trf.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://bjg.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://lpn.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://afk.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://ief.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://mqd.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tks.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://tyd.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vwo.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmy.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sqk.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uev.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kdc.aizwys.cn

Go:   func add(a, b int) int
来源：http://waj.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rni.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rdz.tianlin.xyz

[C14] 泛型函数
来源：http://bup.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dxt.svipenyu.cn

PHP:  // 无泛型
来源：http://zob.yj20258888.top

JS:   // 无泛型
来源：http://ppv.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://viv.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sfh.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ofc.yj20258888.top

Ruby: # 无泛型
来源：http://apo.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rhz.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://gaz.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jds.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://xox.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://roh.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rxz.jiagoushi.top

Java: // 无解构
来源：http://tdn.xuetiantiany.cn

Go:   // 无解构
来源：http://mvr.chenzaomai.com

Ruby: a, b = pair
来源：http://zse.hcnkem.com

C#:   var (a, b) = pair;
来源：http://azt.wangdashe.top

[C16] 函数 / 方法重载
来源：http://tpz.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://unr.jqgufenzy.top

PHP:  // 无重载
来源：http://msw.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dhr.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://gdu.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nya.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://inf.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://ymi.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vff.pycfn.com

================================================================================
来源：http://fdm.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://wmp.hammf.cn

================================================================================
来源：http://jdp.zycfv.cn

[D01] 创建数组 / 列表
来源：http://uxe.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dqy.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fpv.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baa.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cvu.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://crx.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://azz.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://bmn.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tdf.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://pry.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rrf.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gwd.chenzaomai.com

JS:   arr.push(4);
来源：http://muc.zdbjq.cn

TS:   arr.push(4);
来源：http://bdl.ywan-chungtsiang.top

Java: list.add(4);
来源：http://dfy.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://mwz.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://qei.sweek.top

C#:   list.Add(4);
来源：http://fcs.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://iyz.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://ali.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wxv.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qtc.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://byl.ydjk.org.cn

Java: list.add(0, 0);
来源：http://stf.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eli.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nry.xuanzx.com

C#:   list.Insert(0, 0);
来源：http://tgh.jyoumei.cn

[D04] 删除元素
来源：http://ntw.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vuf.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://khd.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://llt.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://euj.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aua.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lag.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cht.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ids.jqgufenzy.top

[D05] 访问与修改元素
来源：http://fti.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zif.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bng.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ego.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://fej.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://gre.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://tni.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eik.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dng.pengpengdd.cyou

[D06] 数组长度
来源：http://yat.xziqi.cn

Py:   len(arr)
来源：http://cee.quarkkingdee.top

PHP:  count($arr);
来源：http://akc.jinqigfzy.top

JS:   arr.length
来源：http://cmx.hammf.cn

TS:   arr.length
来源：http://sru.wangshuangyany.cn

Java: list.size();
来源：http://cfu.ppjwa.cn

Go:   len(arr)
来源：http://tbh.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://amv.cdnleiting.top

C#:   list.Count;
来源：http://uwu.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://lhb.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tyu.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sml.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://ihx.316326.xyz

TS:   arr.slice(1, 4);
来源：http://lto.hysaishi.cn

Java: list.subList(1, 4);
来源：http://pvl.sweek.top

Go:   arr[1:4]
来源：http://kdq.xziqi.cn

Ruby: arr[1, 3]
来源：http://doj.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://jer.hnxiangtu.top

[D08] 合并两个数组
来源：http://fui.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://nfn.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://pak.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wds.cucudq.cn

TS:   [...a, ...b];
来源：http://jgc.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zgj.9152youxi.cn

Go:   append(a, b...)
来源：http://kim.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://sei.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://dbr.chenjidiqi.icu

[D09] 排序（升序）
来源：http://njv.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://mnf.chenjidiqi.icu

PHP:  sort($arr);
来源：http://det.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wva.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rer.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ajg.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uze.fehbvm.com

Ruby: arr.sort
来源：http://blf.aibaodan.cn

C#:   list.Sort();
来源：http://vzm.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cql.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vjv.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lci.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyz.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ino.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://thk.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ugd.shzxlz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xnv.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rlm.wangdashe.top

[D11] 反转数组
来源：http://mzt.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://hpb.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://oog.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nzo.yvedp.cn

TS:   [...arr].reverse();
来源：http://pit.xziqi.cn

Java: Collections.reverse(list);
来源：http://tue.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://jvd.xuetiantiany.cn

Ruby: arr.reverse
来源：http://piz.mhx1999.top

C#:   list.Reverse();
来源：http://aje.zycfv.cn

[D12] 查找元素下标
来源：http://dlu.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://evp.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mxo.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ypd.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yns.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://quc.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://zvr.hnqzz.top

Ruby: arr.index(x)
来源：http://zoi.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://vee.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://vre.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hdk.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://job.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://jjr.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://coq.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fxo.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sgi.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mho.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kmq.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://gjb.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fsb.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nsw.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://iaf.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://caf.shanyushiyangkeji.top


<!-- 参考信息 -->