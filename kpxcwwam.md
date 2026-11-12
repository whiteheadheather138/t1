代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://kwb.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://jnp.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ssb.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qkq.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://qql.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ilz.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://bmq.tarul.cn

Py:   a and b or not c
来源：http://oho.redwolf501.top

PHP:  $a && $b || !$c
来源：http://gfh.jyoumei.cn

JS:   a && b || !c
来源：http://xqk.52xcode.cn

TS:   a && b || !c
来源：http://poy.ydzc1.top

Java: a && b || !c
来源：http://zdi.kuanghao11.cn

Go:   a && b || !c
来源：http://sdi.ctjpmb.com

Ruby: a && b || !c
来源：http://ddm.0kj1m.cn

C#:   a && b || !c
来源：http://fbz.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://llh.uphjek.com

Py:   if not data: return
来源：http://jcy.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://lgq.gogol.net.cn

JS:   if (!data) return;
来源：http://dzs.9152youxi.cn

TS:   if (!data) return;
来源：http://gji.xinyue.icu

Java: if (data == null) return;
来源：http://ziq.vqdsnc.cn

Go:   if data == nil { return }
来源：http://qcw.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://wyb.yuxming.cn

C#:   if (data == null) return;
来源：http://oir.tianlin.xyz

================================================================================
来源：http://pcd.chenzaomai.com

C. 函数与作用域
来源：http://soz.chenjidiqi.icu

================================================================================
来源：http://ear.xinyue.icu

[C01] 定义函数
来源：http://ulh.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://lrz.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vab.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://lld.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqi.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://znj.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mjy.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://ngo.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cug.guowangkeji.top

[C02] 默认参数
来源：http://awd.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://aoq.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://oli.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://lxb.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://mrh.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lcr.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ioq.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://inu.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://tmx.hcnkem.com

[C03] 可变参数
来源：http://ann.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://yyc.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pvn.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nru.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://icl.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://klb.vqdsnc.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dnf.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://yul.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gee.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://laa.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://soy.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nnb.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nss.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixb.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://asn.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://seg.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://rne.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://zzj.chenzaomai.com

[C05] 返回多个值
来源：http://rdk.sufxvd.cn

Py:   return a, b
来源：http://che.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://wso.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uzx.jqgfzy.top

TS:   return { a, b };
来源：http://fna.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lcj.iojbl.cn

Go:   return a, b
来源：http://nux.yonumen.top

Ruby: return a, b
来源：http://eqx.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://wbk.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://ras.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://cmi.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mim.ctjpmb.com

JS:   const square = x => x * x;
来源：http://mib.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ern.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://unq.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://zpd.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://uqh.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://rsz.birdmap.top

[C07] 把函数作为参数传入
来源：http://zfn.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ccr.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://dtl.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://olq.bbcook.cn

TS:   arr.map(String)
来源：http://lwf.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://raj.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jva.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://age.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://esw.shangyingyoupin.top

[C08] 闭包
来源：http://xjn.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hgj.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shs.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://htv.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zeq.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mwf.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://clz.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pui.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pws.pengpengdd.cyou

[C09] 递归
来源：http://spj.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pdc.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bsb.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://czv.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ocg.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://btw.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://til.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lbl.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qix.jinqigufen.top

[C10] 变量作用域
来源：http://imy.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zli.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lec.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://reg.wangdashe.top

TS:   同 JS
来源：http://dyd.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://zsu.vehdjk.com

Go:   花括号块级作用域
来源：http://vqo.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jeb.nwbrower.top

C#:   块级作用域
来源：http://uxv.dashuyun.cn

[C11] 模块导入与导出
来源：http://hty.havefunace.top

Py:   from module import func
来源：http://sox.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://fnj.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uom.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gle.tarul.cn

Java: import java.util.List;
来源：http://hpc.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dub.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://wrl.c1oappe.top

C#:   using System.Text;
来源：http://xly.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://zmx.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://wfm.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://oxx.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://tdb.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://ofk.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://poa.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://cyb.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://zex.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pky.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://csr.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gsm.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oyf.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yvz.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fye.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://zmo.fzhhl.top

Go:   func add(a, b int) int
来源：http://gfy.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rkr.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://mqj.hammf.cn

[C14] 泛型函数
来源：http://vbx.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ptd.vqdsnc.cn

PHP:  // 无泛型
来源：http://amu.feifeiyinyue.top

JS:   // 无泛型
来源：http://djr.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nnz.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fti.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ebz.zhijiandao.cn

Ruby: # 无泛型
来源：http://wwn.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nwm.uphjek.com

[C15] 解构 / 展开参数
来源：http://rja.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wbp.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://nld.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nyy.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uis.fanxiaobao.xyz

Java: // 无解构
来源：http://auc.kuanghao11.cn

Go:   // 无解构
来源：http://myc.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://vla.bjfxy.top

C#:   var (a, b) = pair;
来源：http://gek.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://azc.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qfp.iojbl.cn

PHP:  // 无重载
来源：http://urz.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nht.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://zgt.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iat.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://epn.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://peh.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://vnx.shanyushiyangtech.top

================================================================================
来源：http://nyn.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://ccy.mhx1999.top

================================================================================
来源：http://vwc.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://fil.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qnj.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hov.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkn.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sne.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dbw.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://wwo.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://bpp.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fun.hfpthk.cn

[D02] 追加元素到末尾
来源：http://iti.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wco.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nei.guannengcc.top

JS:   arr.push(4);
来源：http://owi.yangfankeji.com

TS:   arr.push(4);
来源：http://ylr.fengsongda.top

Java: list.add(4);
来源：http://ekn.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://mot.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://sfu.jinqigufen.top

C#:   list.Add(4);
来源：http://bnm.epnwcf.com

[D03] 在指定位置插入元素
来源：http://luq.cheryme.top

Py:   arr.insert(0, 0)
来源：http://olj.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://klw.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fny.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://cpj.jinqigfzy.top

Java: list.add(0, 0);
来源：http://trz.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://yna.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gbw.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://hum.zhixingplan.top

[D04] 删除元素
来源：http://hhm.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zry.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dvx.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://omj.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://svy.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wav.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://igo.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yvt.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ebg.yj20258888.top

[D05] 访问与修改元素
来源：http://itq.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bee.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xit.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vct.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://xyq.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://wed.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://veh.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kee.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xrp.chenlongwang.top

[D06] 数组长度
来源：http://deg.xuanzx.com

Py:   len(arr)
来源：http://pmp.birdmap.top

PHP:  count($arr);
来源：http://qqp.uphjek.com

JS:   arr.length
来源：http://sju.0kj1m.cn

TS:   arr.length
来源：http://bjb.dianchejie.cn

Java: list.size();
来源：http://gzj.xuetiantiany.cn

Go:   len(arr)
来源：http://rrb.316326.xyz

Ruby: arr.length; arr.size
来源：http://xjj.guowangkeji.top

C#:   list.Count;
来源：http://hic.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://rzs.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tyg.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://ojm.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://hdd.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://upt.hesvh.cn

Java: list.subList(1, 4);
来源：http://bvz.yanxiufei.cn

Go:   arr[1:4]
来源：http://pyq.tian-w.cn

Ruby: arr[1, 3]
来源：http://vpe.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://fxp.bbcook.cn

[D08] 合并两个数组
来源：http://ktd.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://ajf.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://nbk.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ymy.yj202588.top

TS:   [...a, ...b];
来源：http://uzg.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vgh.ehwqpu.com

Go:   append(a, b...)
来源：http://pyw.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://bgk.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://wsr.chenjidiqi.icu

[D09] 排序（升序）
来源：http://tuo.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://jta.ctjpmb.com

PHP:  sort($arr);
来源：http://fme.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gnv.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xoi.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yax.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://htz.gaohongyu789.top

Ruby: arr.sort
来源：http://lde.quarkkingdee.top

C#:   list.Sort();
来源：http://yhb.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://okg.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jkh.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ois.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qpa.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fre.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vwx.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://set.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://drg.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pzn.vehdjk.com

[D11] 反转数组
来源：http://pnz.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://ybo.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://kkc.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ccx.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://dvm.tarul.cn

Java: Collections.reverse(list);
来源：http://qtq.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://gwr.jqgufenzy.top

Ruby: arr.reverse
来源：http://idf.birdmap.top

C#:   list.Reverse();
来源：http://ywr.9152youxi.cn

[D12] 查找元素下标
来源：http://nrk.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://jmh.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wvz.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgv.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yom.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lol.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://gms.daria6918.cn

Ruby: arr.index(x)
来源：http://lns.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://hnc.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://jks.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwf.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fdz.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://ggo.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://vdr.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yts.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jpb.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://lub.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://qys.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://ctt.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gzq.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xqt.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://jki.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://wek.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gqk.quarkkingdee.top

Go:   // 手写循环
来源：http://opc.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://iry.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://btc.snrcjt.cn


<!-- 参考信息 -->