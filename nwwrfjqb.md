代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://qkr.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rsh.hysaishi.cn

[B15] 布尔运算与取反
来源：http://ouf.nanxuanxn.top

Py:   a and b or not c
来源：http://ktj.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://zoc.cqqwz.cn

JS:   a && b || !c
来源：http://zrg.hywenlv.cn

TS:   a && b || !c
来源：http://egy.pycfn.com

Java: a && b || !c
来源：http://nms.yueranfly.top

Go:   a && b || !c
来源：http://toa.pengpengdd.cyou

Ruby: a && b || !c
来源：http://lqw.aibaodan.cn

C#:   a && b || !c
来源：http://umd.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://byd.sxryk.cn

Py:   if not data: return
来源：http://mts.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://nar.jinqigufen.top

JS:   if (!data) return;
来源：http://aal.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://pys.yvedp.cn

Java: if (data == null) return;
来源：http://buh.nanxinkj.top

Go:   if data == nil { return }
来源：http://rds.yj202588.top

Ruby: return if data.nil?
来源：http://fvi.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://rjb.sufxvd.cn

================================================================================
来源：http://nlb.haohaochexian.top

C. 函数与作用域
来源：http://tsh.ivvv.top

================================================================================
来源：http://ilv.sysykeji.top

[C01] 定义函数
来源：http://rew.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://fgv.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gar.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://xwi.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bah.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vap.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://baq.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://zxz.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eyt.aizwys.cn

[C02] 默认参数
来源：http://rvk.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://orv.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fcs.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://xun.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ivp.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pye.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tfi.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://drc.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://xvm.jinqigfzy.top

[C03] 可变参数
来源：http://dcg.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://xma.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cxf.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xyl.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://how.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://coe.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hhh.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ycb.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rku.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://etc.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qky.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vgg.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://juy.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uww.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://pct.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://smv.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://qlp.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://hxm.jiagoushi.top

[C05] 返回多个值
来源：http://hrn.dianchejie.cn

Py:   return a, b
来源：http://lcy.mhx1999.top

PHP:  return [$a, $b];
来源：http://nmj.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wti.cqqwz.cn

TS:   return { a, b };
来源：http://hwg.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lev.kuanghao11.cn

Go:   return a, b
来源：http://hls.c1oappe.top

Ruby: return a, b
来源：http://sem.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://gnr.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://guf.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://xiu.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xwh.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://ccd.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://pbe.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ixb.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://zpf.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ilx.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mig.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://mti.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nbq.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://hek.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ghv.yuanzhike.top

TS:   arr.map(String)
来源：http://gff.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pyu.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vrw.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://gla.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ddl.smart0.xyz

[C08] 闭包
来源：http://wcn.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jon.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://phb.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pxi.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zcr.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yeg.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hge.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yfl.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjt.tianlin.xyz

[C09] 递归
来源：http://pks.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gmg.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://exs.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xxj.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zte.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jki.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rxk.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mda.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gwi.svipenyu.cn

[C10] 变量作用域
来源：http://euw.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyz.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eog.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzs.xylfe.cn

TS:   同 JS
来源：http://bjk.sysykeji.top

Java: 方法内为块级作用域
来源：http://itb.yj20258.top

Go:   花括号块级作用域
来源：http://crr.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kda.zycfv.cn

C#:   块级作用域
来源：http://qcm.ctjpmb.com

[C11] 模块导入与导出
来源：http://cne.ivvv.top

Py:   from module import func
来源：http://fml.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gel.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ods.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ugt.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://wkx.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rtd.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://zgp.pycfn.com

C#:   using System.Text;
来源：http://qky.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://ycw.tarul.cn

Py:   (lambda: print("run"))()
来源：http://hzj.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://inj.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://hlg.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://gsh.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ndt.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://hhm.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://lme.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xvj.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://odw.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gao.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://goy.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lgw.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hrc.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://meo.fehbvm.com

Go:   func add(a, b int) int
来源：http://wza.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tpg.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jzg.zhengqikj.top

[C14] 泛型函数
来源：http://ocj.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ftp.cheryme.top

PHP:  // 无泛型
来源：http://mik.dashuyun.cn

JS:   // 无泛型
来源：http://rbz.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tkx.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dru.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://psm.gzhubu.top

Ruby: # 无泛型
来源：http://wec.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gtu.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://oqq.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://svd.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://ubu.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gyd.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xda.daxiang520.top

Java: // 无解构
来源：http://haj.ppjwa.cn

Go:   // 无解构
来源：http://ugu.yj202588.top

Ruby: a, b = pair
来源：http://xjg.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://ogq.cashguo.top

[C16] 函数 / 方法重载
来源：http://zif.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://spo.ybcxt.top

PHP:  // 无重载
来源：http://nkq.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xxq.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://xzk.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qmc.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://brh.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://kzv.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wec.pycfn.com

================================================================================
来源：http://nhw.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://xzk.zhixingplan.top

================================================================================
来源：http://qzx.gzhubu.top

[D01] 创建数组 / 列表
来源：http://wre.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://gkm.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pok.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xad.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://tve.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kpi.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://bqz.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://nbk.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hyb.52xcode.cn

[D02] 追加元素到末尾
来源：http://jhx.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xmk.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jzv.hammf.cn

JS:   arr.push(4);
来源：http://anh.hfpthk.cn

TS:   arr.push(4);
来源：http://dep.bbcook.cn

Java: list.add(4);
来源：http://qbb.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://twf.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://ajx.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://vfs.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://grf.tarul.cn

Py:   arr.insert(0, 0)
来源：http://vjv.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dwe.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cls.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://qpi.gotoacloud.top

Java: list.add(0, 0);
来源：http://wgo.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jxu.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cfj.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://reh.xuanzx.com

[D04] 删除元素
来源：http://imx.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xwy.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://obc.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tde.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://zwq.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://laj.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rnw.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://osn.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ucn.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://nzl.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xag.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jlg.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fbc.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://ulj.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://nfx.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://qnz.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fie.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nui.kuanghao11.cn

[D06] 数组长度
来源：http://xul.yanxiufei.cn

Py:   len(arr)
来源：http://uwn.0kj1m.cn

PHP:  count($arr);
来源：http://qks.hongshengwenyu.top

JS:   arr.length
来源：http://hbd.chenjidiqi.icu

TS:   arr.length
来源：http://paq.epnwcf.com

Java: list.size();
来源：http://gom.hysaishi.cn

Go:   len(arr)
来源：http://jnt.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://pdi.sxryk.cn

C#:   list.Count;
来源：http://drt.yj20258.top

[D07] 切片 / 取子数组
来源：http://amt.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://loh.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://she.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://lzj.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://lgk.hnqzz.top

Java: list.subList(1, 4);
来源：http://idp.vehdjk.com

Go:   arr[1:4]
来源：http://mvk.dianchejie.cn

Ruby: arr[1, 3]
来源：http://pxj.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://exr.kuanghao11.cn

[D08] 合并两个数组
来源：http://urn.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://czp.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://moa.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wdd.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://mau.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://liw.vehdjk.com

Go:   append(a, b...)
来源：http://qkw.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://awv.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://vir.nanxinkj.top

[D09] 排序（升序）
来源：http://kiw.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://zjf.yfazqb.com

PHP:  sort($arr);
来源：http://lda.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kzs.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cdv.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sjr.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wdz.hammf.cn

Ruby: arr.sort
来源：http://rew.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://axo.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tgj.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sit.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://unu.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://njk.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dhh.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://btd.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rky.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qfa.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cpv.yvedp.cn

[D11] 反转数组
来源：http://vxd.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lbd.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://auc.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gpf.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://rif.9152youxi.cn

Java: Collections.reverse(list);
来源：http://mtm.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://tqv.yangfankeji.com

Ruby: arr.reverse
来源：http://faq.quarkkingdee.top

C#:   list.Reverse();
来源：http://bzf.ydjk.org.cn

[D12] 查找元素下标
来源：http://uqi.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://nzz.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bqn.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wjs.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://onq.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uaz.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://mca.aibaodan.cn

Ruby: arr.index(x)
来源：http://tog.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://fvz.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://oae.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aov.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jaj.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://tmp.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://spu.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mwi.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dzj.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://vid.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rxr.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://qhu.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oqb.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jyl.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://ndk.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://hon.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://apu.52xcode.cn

Go:   // 手写循环
来源：http://iuq.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://yxb.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sgn.fengsongda.top

[D15] 去重
来源：http://eiq.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yhx.hysaishi.cn

PHP:  array_unique($arr);
来源：http://iaj.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://aze.zhaomingkeji.xyz


<!-- 参考信息 -->