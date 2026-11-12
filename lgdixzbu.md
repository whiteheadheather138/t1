代发 wailian999

C#:   x is int or double or decimal
来源：http://evd.ivvv.top

[B14] 判断值是否在集合内
来源：http://pyf.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pgs.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pxo.0kj1m.cn

JS:   [1, 2, 3].includes(x)
来源：http://rii.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://xqd.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ged.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yde.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://sdt.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://okw.chenlongwang.top

[B15] 布尔运算与取反
来源：http://hji.cucudq.cn

Py:   a and b or not c
来源：http://tww.meibo888.top

PHP:  $a && $b || !$c
来源：http://tdi.fanxiaobao.xyz

JS:   a && b || !c
来源：http://tod.9152youxi.cn

TS:   a && b || !c
来源：http://per.jiagoushi.top

Java: a && b || !c
来源：http://lih.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://xbi.sweek.top

Ruby: a && b || !c
来源：http://bry.chenlongwang.top

C#:   a && b || !c
来源：http://ppl.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://xvu.aizwys.cn

Py:   if not data: return
来源：http://hti.yj202588.top

PHP:  if (!$data) { return; }
来源：http://ktg.vqdsnc.cn

JS:   if (!data) return;
来源：http://may.xuetiantiany.cn

TS:   if (!data) return;
来源：http://gvg.nanxuanxn.top

Java: if (data == null) return;
来源：http://soj.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://igq.sysykeji.top

Ruby: return if data.nil?
来源：http://lir.gotoacloud.top

C#:   if (data == null) return;
来源：http://ktg.tanke756.top

================================================================================
来源：http://ljg.ydjk.org.cn

C. 函数与作用域
来源：http://bwx.hysaishi.cn

================================================================================
来源：http://zol.gotoacloud.top

[C01] 定义函数
来源：http://lbl.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://ehl.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fve.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://rnr.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eyu.sxryk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nou.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://xdn.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://huw.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ocs.uphjek.com

[C02] 默认参数
来源：http://abm.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://lne.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jfl.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://xip.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://frc.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://evo.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kmy.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://gob.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://kkv.ctjpmb.com

[C03] 可变参数
来源：http://ywa.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://loa.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://opw.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://akd.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xbr.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mrs.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nzx.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://lwp.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jgu.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://nvp.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cor.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rqh.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vkx.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vov.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://whh.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://umj.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://gah.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://euq.chenzaomai.com

[C05] 返回多个值
来源：http://lfe.tian-w.cn

Py:   return a, b
来源：http://mhf.tianlin.xyz

PHP:  return [$a, $b];
来源：http://tlx.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dao.fzhhl.top

TS:   return { a, b };
来源：http://byd.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mnf.havefunace.top

Go:   return a, b
来源：http://mne.zhijiandao.cn

Ruby: return a, b
来源：http://hqq.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://iul.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://gie.cashguo.top

Py:   square = lambda x: x * x
来源：http://qoc.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fvo.yj20258888.top

JS:   const square = x => x * x;
来源：http://pnw.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://ijp.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iiq.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://iba.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://jlv.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://hqt.yonumen.top

[C07] 把函数作为参数传入
来源：http://xbn.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hne.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://hcs.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eln.fehbvm.com

TS:   arr.map(String)
来源：http://nbt.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pdn.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sxk.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://hoe.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xzr.nanxuanxn.top

[C08] 闭包
来源：http://pmp.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://edd.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ahh.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qhh.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sbs.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jsv.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://phg.hywenlv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vsl.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ivc.chenlongwang.top

[C09] 递归
来源：http://ufk.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uyj.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zzo.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mxv.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cgl.hywenlv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rrh.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ouu.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://euf.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yki.yuanzhike.top

[C10] 变量作用域
来源：http://jhz.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://twa.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmg.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bvb.birdmap.top

TS:   同 JS
来源：http://hby.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://tre.fengsongda.top

Go:   花括号块级作用域
来源：http://ejb.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lnc.jinqigfzy.top

C#:   块级作用域
来源：http://vzl.52xcode.cn

[C11] 模块导入与导出
来源：http://gfa.yj202588.top

Py:   from module import func
来源：http://deg.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pvx.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dkn.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mkc.jiagoushi.top

Java: import java.util.List;
来源：http://cow.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://axu.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://wzy.nanxinkj.top

C#:   using System.Text;
来源：http://hug.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://lhr.yongpay.top

Py:   (lambda: print("run"))()
来源：http://rkj.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://ryj.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://mde.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://dtm.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://izj.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://pzu.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://ted.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://tmq.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://pre.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bcy.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jze.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zea.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uhr.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xbp.cucudq.cn

Go:   func add(a, b int) int
来源：http://hwk.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://weg.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://npz.ydzc1.top

[C14] 泛型函数
来源：http://xth.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xtw.yj202588.top

PHP:  // 无泛型
来源：http://akw.yongpay.top

JS:   // 无泛型
来源：http://vyx.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pdq.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nlg.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nxg.hywenlv.cn

Ruby: # 无泛型
来源：http://pco.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sbq.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://bhq.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xff.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://ube.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://izf.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cni.wangdashe.top

Java: // 无解构
来源：http://spr.wangdashe.top

Go:   // 无解构
来源：http://xut.yuanzhike.top

Ruby: a, b = pair
来源：http://czl.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://unm.mhx1999.top

[C16] 函数 / 方法重载
来源：http://beg.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wtq.tian-w.cn

PHP:  // 无重载
来源：http://sau.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://tsf.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://ouy.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mfv.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://usv.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://nlo.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://wxq.ppjwa.cn

================================================================================
来源：http://uej.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://bew.tianlin.xyz

================================================================================
来源：http://jhs.hammf.cn

[D01] 创建数组 / 列表
来源：http://hks.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dba.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vkk.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hgn.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://tuc.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dke.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://dzf.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://vuk.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pqf.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://rql.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qdo.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://een.hysaishi.cn

JS:   arr.push(4);
来源：http://ywg.ybcxt.top

TS:   arr.push(4);
来源：http://bih.ppjwa.cn

Java: list.add(4);
来源：http://bqy.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://flo.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://hot.shzxlz.cn

C#:   list.Add(4);
来源：http://ekt.hammf.cn

[D03] 在指定位置插入元素
来源：http://xmj.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://owk.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uzz.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfp.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://ttr.yueranfly.top

Java: list.add(0, 0);
来源：http://doq.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://brn.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jvl.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://bhs.aibaodan.cn

[D04] 删除元素
来源：http://bej.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pny.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tlp.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://caj.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://pfp.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eiq.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mnr.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jdg.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ear.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://zqr.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yeb.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://taw.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lob.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://cws.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://rcb.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://nyf.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dqo.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://byx.shanyushiyangkeji.top

[D06] 数组长度
来源：http://uur.jqgufenzy.top

Py:   len(arr)
来源：http://nfb.vehdjk.com

PHP:  count($arr);
来源：http://mqb.iojbl.cn

JS:   arr.length
来源：http://sfg.chenzaomai.com

TS:   arr.length
来源：http://ars.chenlongwang.top

Java: list.size();
来源：http://edn.ydjk.org.cn

Go:   len(arr)
来源：http://pqz.gzhubu.top

Ruby: arr.length; arr.size
来源：http://cjm.aibaodan.cn

C#:   list.Count;
来源：http://mtj.sysykeji.top

[D07] 切片 / 取子数组
来源：http://ynz.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lzp.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://gyu.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://abl.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://ljb.havefunace.top

Java: list.subList(1, 4);
来源：http://iqt.daxiang520.top

Go:   arr[1:4]
来源：http://zir.dianchejie.cn

Ruby: arr[1, 3]
来源：http://vfp.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://vhk.tanke756.top

[D08] 合并两个数组
来源：http://jxw.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://zga.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://uzh.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zup.sweek.top

TS:   [...a, ...b];
来源：http://tcz.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lgf.sysykeji.top

Go:   append(a, b...)
来源：http://fra.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://zwq.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://poq.pycfn.com

[D09] 排序（升序）
来源：http://sjm.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://ill.sjlbkw.cn

PHP:  sort($arr);
来源：http://woj.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ufn.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vff.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fwt.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hsu.guannengcc.top

Ruby: arr.sort
来源：http://noa.bjfxy.top

C#:   list.Sort();
来源：http://lge.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://tsm.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tne.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hjq.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pzx.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xai.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://acg.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://chd.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gvd.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uqm.daxiang520.top

[D11] 反转数组
来源：http://fnh.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://stl.ydzc1.top

PHP:  array_reverse($arr);
来源：http://zpw.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gsk.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://atw.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://eqc.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://zzh.svipenyu.cn

Ruby: arr.reverse
来源：http://prq.ctjpmb.com

C#:   list.Reverse();
来源：http://qda.meibo888.top

[D12] 查找元素下标
来源：http://fsj.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://kel.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://btz.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xas.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sur.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ihj.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://ktg.gotoacloud.top

Ruby: arr.index(x)
来源：http://tjr.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://znq.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://foy.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ctb.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://llu.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://mui.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://tiu.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dnl.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hbs.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oqy.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://evl.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://xpm.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zvu.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rsj.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://aqi.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://lqs.guannengcc.top


<!-- 参考信息 -->