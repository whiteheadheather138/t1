代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://dan.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sxd.jianghu66.top

[B15] 布尔运算与取反
来源：http://vwp.hfpthk.cn

Py:   a and b or not c
来源：http://ldr.hnqzz.top

PHP:  $a && $b || !$c
来源：http://tfj.fehbvm.com

JS:   a && b || !c
来源：http://ezz.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://fpd.ywan-chungtsiang.top

Java: a && b || !c
来源：http://wts.wangdashe.top

Go:   a && b || !c
来源：http://cem.chenzaomai.com

Ruby: a && b || !c
来源：http://dzw.cashguo.top

C#:   a && b || !c
来源：http://rrx.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hha.iojbl.cn

Py:   if not data: return
来源：http://rmj.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://cyo.xziqi.cn

JS:   if (!data) return;
来源：http://vyp.xuanzx.com

TS:   if (!data) return;
来源：http://afh.fktsv.cn

Java: if (data == null) return;
来源：http://pun.vqdsnc.cn

Go:   if data == nil { return }
来源：http://lle.yangfankeji.com

Ruby: return if data.nil?
来源：http://crq.chenzaomai.com

C#:   if (data == null) return;
来源：http://yrx.tanke756.top

================================================================================
来源：http://fnk.52xcode.cn

C. 函数与作用域
来源：http://rkp.cdnleiting.top

================================================================================
来源：http://zvu.yuxming.cn

[C01] 定义函数
来源：http://fox.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://qiv.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aiv.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://ols.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efp.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zjd.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qot.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://otn.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tlw.shzxlz.cn

[C02] 默认参数
来源：http://psh.yonumen.top

Py:   def greet(name="World"): return name
来源：http://vvu.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ihc.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://wjw.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jbf.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hcv.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nez.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://zba.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://ngt.jyoumei.cn

[C03] 可变参数
来源：http://voj.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://ugw.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gwq.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://erb.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bcj.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fho.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://szp.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zjn.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://srd.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://efw.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://olr.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qhs.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rer.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bmv.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://grr.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://ytz.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://juc.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://gnl.chenjidiqi.icu

[C05] 返回多个值
来源：http://kqt.cheryme.top

Py:   return a, b
来源：http://gmo.zycfv.cn

PHP:  return [$a, $b];
来源：http://huq.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xpx.gotoacloud.top

TS:   return { a, b };
来源：http://yhi.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zwd.aizwys.cn

Go:   return a, b
来源：http://pwf.fehbvm.com

Ruby: return a, b
来源：http://kot.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://vvb.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://ffs.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://pys.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://djw.zycfv.cn

JS:   const square = x => x * x;
来源：http://zsj.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://kvh.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gxt.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ckq.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://svp.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://roq.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://yjq.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nrq.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://fib.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wui.shangyingyoupin.top

TS:   arr.map(String)
来源：http://lax.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ppx.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bpj.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://cvj.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bxe.hnqzz.top

[C08] 闭包
来源：http://hzd.dianchejie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hqr.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vkr.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hao.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zze.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oza.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gwl.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cin.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yrb.iojbl.cn

[C09] 递归
来源：http://xbt.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gqc.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tmw.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uxd.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yyz.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgi.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qqb.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hiy.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://omt.wangshuangyany.cn

[C10] 变量作用域
来源：http://cll.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://auj.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vxl.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://edb.sweek.top

TS:   同 JS
来源：http://zin.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://sis.jinqigufen.top

Go:   花括号块级作用域
来源：http://mnu.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://puz.cucudq.cn

C#:   块级作用域
来源：http://rpg.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://uom.zhijiandao.cn

Py:   from module import func
来源：http://cqi.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gjg.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mrb.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qsc.daria6918.cn

Java: import java.util.List;
来源：http://adj.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uri.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://kzd.hesvh.cn

C#:   using System.Text;
来源：http://fxi.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://dyx.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://eyp.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://ikg.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://yjv.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://qac.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oki.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://gzm.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://zun.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://djc.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://phn.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dol.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pha.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vna.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://znd.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qse.tianlin.xyz

Go:   func add(a, b int) int
来源：http://zts.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ses.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://sdn.quarkkingdee.top

[C14] 泛型函数
来源：http://kfu.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mhv.smart0.xyz

PHP:  // 无泛型
来源：http://ccq.feifeiyinyue.top

JS:   // 无泛型
来源：http://phi.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://enh.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tgg.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zha.andypj.xyz

Ruby: # 无泛型
来源：http://zbg.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kbt.epnwcf.com

[C15] 解构 / 展开参数
来源：http://nms.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ass.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://okv.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bqo.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mwf.xziqi.cn

Java: // 无解构
来源：http://cfz.pengpengdd.cyou

Go:   // 无解构
来源：http://iha.snrcjt.cn

Ruby: a, b = pair
来源：http://lcd.316326.xyz

C#:   var (a, b) = pair;
来源：http://alt.uphjek.com

[C16] 函数 / 方法重载
来源：http://oaz.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://njx.bjfxy.top

PHP:  // 无重载
来源：http://okp.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://zkd.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://bym.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ead.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://wjk.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://bck.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://akr.aizwys.cn

================================================================================
来源：http://jeq.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://eoa.dashuyun.cn

================================================================================
来源：http://yuc.havefunace.top

[D01] 创建数组 / 列表
来源：http://wsx.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://rdj.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cky.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oep.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://flv.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qet.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://kjp.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://ahw.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mnp.ivvv.top

[D02] 追加元素到末尾
来源：http://ori.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lvu.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qsr.cucudq.cn

JS:   arr.push(4);
来源：http://psr.sxryk.cn

TS:   arr.push(4);
来源：http://zbm.kuanghao11.cn

Java: list.add(4);
来源：http://eep.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://zpg.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://lvs.aizwys.cn

C#:   list.Add(4);
来源：http://zfg.c1oappe.top

[D03] 在指定位置插入元素
来源：http://vej.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://hng.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://byr.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lna.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://alx.ydjk.org.cn

Java: list.add(0, 0);
来源：http://mgb.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://jor.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://drq.yongpay.top

C#:   list.Insert(0, 0);
来源：http://ghq.jqgfzy.top

[D04] 删除元素
来源：http://viu.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zpx.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lay.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nae.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://ufm.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qrt.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kfv.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mqm.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dxu.xuanzx.com

[D05] 访问与修改元素
来源：http://kur.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lfs.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kji.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ffc.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://iqw.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://hyc.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://tcx.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pze.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lnu.bbcook.cn

[D06] 数组长度
来源：http://ngf.meibo888.top

Py:   len(arr)
来源：http://ihg.tianlin.xyz

PHP:  count($arr);
来源：http://ldy.xingfuxueyuan.xyz

JS:   arr.length
来源：http://smn.zycfv.cn

TS:   arr.length
来源：http://azo.yuanzhike.top

Java: list.size();
来源：http://mln.shzxlz.cn

Go:   len(arr)
来源：http://xvw.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://vjs.hnqzz.top

C#:   list.Count;
来源：http://phf.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://ons.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aeh.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jba.birdmap.top

JS:   arr.slice(1, 4);
来源：http://rnf.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://iry.jiagoushi.top

Java: list.subList(1, 4);
来源：http://drg.jianghu66.top

Go:   arr[1:4]
来源：http://pye.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://txy.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://urh.xylfe.cn

[D08] 合并两个数组
来源：http://fae.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://mhf.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://nwc.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wcy.sjlbkw.cn

TS:   [...a, ...b];
来源：http://gql.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://obw.hesvh.cn

Go:   append(a, b...)
来源：http://lbs.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://rxk.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://ckf.cdnleiting.top

[D09] 排序（升序）
来源：http://yzo.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://ddt.daxiang520.top

PHP:  sort($arr);
来源：http://kyq.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zfr.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eut.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://enc.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fjl.zdbjq.cn

Ruby: arr.sort
来源：http://tzl.gaohongyu789.top

C#:   list.Sort();
来源：http://oiq.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://prg.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xxk.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://plw.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://djy.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqj.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zby.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bnm.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fxu.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://udt.ctjpmb.com

[D11] 反转数组
来源：http://njn.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://irp.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://yjv.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://poy.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://fke.hfpthk.cn

Java: Collections.reverse(list);
来源：http://tmb.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://tgk.fehbvm.com

Ruby: arr.reverse
来源：http://wkl.yuxming.cn

C#:   list.Reverse();
来源：http://dmh.sjlbkw.cn

[D12] 查找元素下标
来源：http://rem.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://hqi.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://whr.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://otk.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vke.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://thb.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://kjb.ppjwa.cn

Ruby: arr.index(x)
来源：http://exx.cucudq.cn

C#:   list.IndexOf(x);
来源：http://ojq.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://lrv.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://utc.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vob.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://llk.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://bzg.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://abk.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yey.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://zji.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mkr.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://vdh.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dxn.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qal.fktsv.cn

JS:   arr.map(x => x * 2)
来源：http://yns.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://ifz.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dmg.ydzc1.top

Go:   // 手写循环
来源：http://ndi.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gqd.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mbl.aibaodan.cn

[D15] 去重
来源：http://kxq.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://niw.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://eir.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://zfa.xziqi.cn


<!-- 参考信息 -->