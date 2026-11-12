代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://cyi.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nhe.316326.xyz

[B15] 布尔运算与取反
来源：http://qly.pycfn.com

Py:   a and b or not c
来源：http://zzq.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://ima.yuanzhike.top

JS:   a && b || !c
来源：http://qox.dianchejie.cn

TS:   a && b || !c
来源：http://rqc.vehdjk.com

Java: a && b || !c
来源：http://zyu.zhixingplan.top

Go:   a && b || !c
来源：http://fwt.xinyue.icu

Ruby: a && b || !c
来源：http://uot.sjlbkw.cn

C#:   a && b || !c
来源：http://pms.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qrf.shanyushiyangtech.top

Py:   if not data: return
来源：http://bkh.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://xrx.0kj1m.cn

JS:   if (!data) return;
来源：http://pse.jinqigufen.top

TS:   if (!data) return;
来源：http://ssq.redwolf501.top

Java: if (data == null) return;
来源：http://xfk.nanxuanxn.top

Go:   if data == nil { return }
来源：http://cie.zhijiandao.cn

Ruby: return if data.nil?
来源：http://ogw.9152youxi.cn

C#:   if (data == null) return;
来源：http://rni.daria6918.cn

================================================================================
来源：http://qtt.cheryme.top

C. 函数与作用域
来源：http://vcw.gaohongyu789.top

================================================================================
来源：http://bwb.shanyushiyangtech.top

[C01] 定义函数
来源：http://fky.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://uxe.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flx.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://zpu.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ebs.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://afu.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://fsa.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://klw.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zrg.jqgufenzy.top

[C02] 默认参数
来源：http://gzc.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://ayq.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tgg.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://oyj.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nwc.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hbd.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vwg.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://bhy.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://qba.jinyuanbaomall.cn

[C03] 可变参数
来源：http://jgo.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://xui.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rjm.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zqa.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wxc.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahr.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://voa.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://byp.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zxi.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://xxv.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://guf.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qib.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zpf.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vdd.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://iwn.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://zsz.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://acg.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://akz.meibo888.top

[C05] 返回多个值
来源：http://hhp.daria6918.cn

Py:   return a, b
来源：http://hoc.pycfn.com

PHP:  return [$a, $b];
来源：http://cwa.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lbo.dashuyun.cn

TS:   return { a, b };
来源：http://dvn.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cam.redwolf501.top

Go:   return a, b
来源：http://qfn.jinqigufen.top

Ruby: return a, b
来源：http://mcb.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://svi.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://bfh.sxryk.cn

Py:   square = lambda x: x * x
来源：http://tex.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pmm.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://zvd.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://csh.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yvb.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://kwv.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://hzo.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rxa.mhx1999.top

[C07] 把函数作为参数传入
来源：http://iao.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qfj.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pym.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://plm.xuanzx.com

TS:   arr.map(String)
来源：http://xir.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tfi.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rum.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://qar.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dvq.hesvh.cn

[C08] 闭包
来源：http://twv.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zpg.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xgy.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://roq.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hsu.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ovg.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://emc.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rpl.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hao.52xcode.cn

[C09] 递归
来源：http://bgi.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kdu.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mva.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwv.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxn.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cvw.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ctb.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mdb.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://igy.zhiwuduotai.top

[C10] 变量作用域
来源：http://jyw.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ogd.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://onp.jqgufenzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rno.yvedp.cn

TS:   同 JS
来源：http://kva.mhx1999.top

Java: 方法内为块级作用域
来源：http://zjk.c1oappe.top

Go:   花括号块级作用域
来源：http://hof.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xzc.aibaodan.cn

C#:   块级作用域
来源：http://yev.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://xul.ybcxt.top

Py:   from module import func
来源：http://knw.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jaa.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lxx.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ddz.vqdsnc.cn

Java: import java.util.List;
来源：http://sph.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vxc.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://kio.jqgfzy.top

C#:   using System.Text;
来源：http://uuz.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://omu.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://ccf.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://rbz.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://brh.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://qxy.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://djr.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ddr.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://aaj.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mte.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://cbs.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://omo.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vti.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rvv.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vww.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wxy.andypj.xyz

Go:   func add(a, b int) int
来源：http://qgk.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gfy.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bzo.daxiang520.top

[C14] 泛型函数
来源：http://rpa.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jyy.316326.xyz

PHP:  // 无泛型
来源：http://brg.yanxiufei.cn

JS:   // 无泛型
来源：http://gjk.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sha.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pxu.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xmn.yfazqb.com

Ruby: # 无泛型
来源：http://opf.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qnj.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://lsu.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jib.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://hsz.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aga.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lbr.zycfv.cn

Java: // 无解构
来源：http://pfb.bbcook.cn

Go:   // 无解构
来源：http://vgg.tianlin.xyz

Ruby: a, b = pair
来源：http://bbx.hcnkem.com

C#:   var (a, b) = pair;
来源：http://yzu.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://jvs.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzi.zhongyouzk.top

PHP:  // 无重载
来源：http://biy.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jrx.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://fxp.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fbn.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://mie.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://mne.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://oht.zhiwuduotai.top

================================================================================
来源：http://yld.meibo888.top

D. 数组 / 列表 / 集合
来源：http://nbw.chenjidiqi.icu

================================================================================
来源：http://xso.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://bxg.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dzo.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sxe.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://thl.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dox.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fdg.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://xoq.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://xjg.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://woy.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://nvd.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xro.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ebe.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://inc.dashuyun.cn

TS:   arr.push(4);
来源：http://kdi.hcnkem.com

Java: list.add(4);
来源：http://fyy.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://uye.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://xrd.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://iwp.aizwys.cn

[D03] 在指定位置插入元素
来源：http://vfp.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://wgz.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jbb.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pok.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://aib.zhoulong.xyz

Java: list.add(0, 0);
来源：http://ukd.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://gkq.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gjh.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://erj.gotoacloud.top

[D04] 删除元素
来源：http://mkx.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lic.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kxe.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xrv.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://iki.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogp.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mih.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jsq.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dbw.dashuyun.cn

[D05] 访问与修改元素
来源：http://ezq.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wmy.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fgq.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sum.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://tvw.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://szf.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://ksz.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ddi.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qbm.zhiwuduotai.top

[D06] 数组长度
来源：http://jki.vqdsnc.cn

Py:   len(arr)
来源：http://jpt.fengsongda.top

PHP:  count($arr);
来源：http://uul.chenzaomai.com

JS:   arr.length
来源：http://nus.0kj1m.cn

TS:   arr.length
来源：http://znr.fanxiaobao.xyz

Java: list.size();
来源：http://eqv.cheryme.top

Go:   len(arr)
来源：http://mft.vehdjk.com

Ruby: arr.length; arr.size
来源：http://otg.cucudq.cn

C#:   list.Count;
来源：http://rjy.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://qzw.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://flb.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://cin.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://dzd.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://jus.havefunace.top

Java: list.subList(1, 4);
来源：http://kwq.aizwys.cn

Go:   arr[1:4]
来源：http://doa.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://cor.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://lva.jyoumei.cn

[D08] 合并两个数组
来源：http://khj.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://vtq.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://euf.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://knc.aibaodan.cn

TS:   [...a, ...b];
来源：http://bxo.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gis.svipenyu.cn

Go:   append(a, b...)
来源：http://bur.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://hjv.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://ukc.andypj.xyz

[D09] 排序（升序）
来源：http://wyj.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://nag.yfazqb.com

PHP:  sort($arr);
来源：http://rni.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lct.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jht.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://voj.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yvm.wangdashe.top

Ruby: arr.sort
来源：http://cqf.yuxming.cn

C#:   list.Sort();
来源：http://kqj.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iwc.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ykf.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lon.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpu.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivb.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fli.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wny.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbo.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbb.chenzaomai.com

[D11] 反转数组
来源：http://nsp.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://ary.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://smr.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sul.chenlongwang.top

TS:   [...arr].reverse();
来源：http://hzo.jyoumei.cn

Java: Collections.reverse(list);
来源：http://yib.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://btd.zhongyouzk.top

Ruby: arr.reverse
来源：http://tjy.feifeiyinyue.top

C#:   list.Reverse();
来源：http://ocv.hnqzz.top

[D12] 查找元素下标
来源：http://vxx.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://kzs.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ljf.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzk.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hdr.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://plc.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://uos.yj202588.top

Ruby: arr.index(x)
来源：http://frt.xziqi.cn

C#:   list.IndexOf(x);
来源：http://fpo.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://mwh.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bhk.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ewv.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://kxn.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://dtv.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tpa.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kre.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://lcy.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qoh.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://ptz.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uwb.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vne.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://ijq.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://gld.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://chf.hnqzz.top

Go:   // 手写循环
来源：http://mhb.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://ehz.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://puk.vqdsnc.cn

[D15] 去重
来源：http://gqa.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gwy.nwbrower.top

PHP:  array_unique($arr);
来源：http://zcl.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://lei.dianchejie.cn


<!-- 参考信息 -->