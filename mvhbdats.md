代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://zeu.hcnkem.com

TS:   [1, 2, 3].includes(x)
来源：http://ghw.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mhg.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://txy.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://wto.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tma.fehbvm.com

[B15] 布尔运算与取反
来源：http://cbh.hfpthk.cn

Py:   a and b or not c
来源：http://ajs.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://whn.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://gpb.xuetiantiany.cn

TS:   a && b || !c
来源：http://zda.zdqjudy.top

Java: a && b || !c
来源：http://zks.daxiang520.top

Go:   a && b || !c
来源：http://hpu.sufxvd.cn

Ruby: a && b || !c
来源：http://goj.pycfn.com

C#:   a && b || !c
来源：http://wtt.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ftd.yj20258.top

Py:   if not data: return
来源：http://dpc.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://skp.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://rcf.vqdsnc.cn

TS:   if (!data) return;
来源：http://cym.chenlongwang.top

Java: if (data == null) return;
来源：http://eep.zycfv.cn

Go:   if data == nil { return }
来源：http://thu.xinyue.icu

Ruby: return if data.nil?
来源：http://cxz.svipenyu.cn

C#:   if (data == null) return;
来源：http://wbf.gotoacloud.top

================================================================================
来源：http://cte.jinqigfzy.top

C. 函数与作用域
来源：http://qce.iojbl.cn

================================================================================
来源：http://lcr.shanyushiyangkeji.top

[C01] 定义函数
来源：http://fog.meibo888.top

Py:   def add(a, b): return a + b
来源：http://ezo.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsk.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://hvd.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cqd.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rvj.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wrr.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://awp.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://exa.ydjk.org.cn

[C02] 默认参数
来源：http://urd.yj202588.top

Py:   def greet(name="World"): return name
来源：http://qjz.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hyd.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://spa.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dyo.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://run.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jfs.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://xsm.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://vuu.chenzaomai.com

[C03] 可变参数
来源：http://nyk.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://mkq.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yrv.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://amh.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ywu.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qga.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wcz.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://bxv.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vng.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://zbo.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wnv.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://txw.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pfv.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wtd.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://koj.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://hzg.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://qwl.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://kgg.yueranfly.top

[C05] 返回多个值
来源：http://huu.birdmap.top

Py:   return a, b
来源：http://nmp.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://ghv.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zgs.sxryk.cn

TS:   return { a, b };
来源：http://ify.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ils.hcnkem.com

Go:   return a, b
来源：http://dsz.jyoumei.cn

Ruby: return a, b
来源：http://goa.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://lsm.316326.xyz

[C06] 匿名函数 / lambda
来源：http://uhg.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://vsp.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://kdq.fzhhl.top

JS:   const square = x => x * x;
来源：http://byc.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://whm.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rrw.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://soz.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://neq.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://ixw.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://wjx.zycfv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://out.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ghk.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://deg.aizwys.cn

TS:   arr.map(String)
来源：http://kmc.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lpj.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gbc.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://ypb.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://wwl.jianghu66.top

[C08] 闭包
来源：http://qzj.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vnl.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://elv.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tqw.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mdn.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vdd.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qor.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yhf.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vtq.yongpay.top

[C09] 递归
来源：http://gid.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yab.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ccw.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://com.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mkh.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cpd.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pon.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mqs.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gnt.smart0.xyz

[C10] 变量作用域
来源：http://zfj.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mka.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xna.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xsk.ydjk.org.cn

TS:   同 JS
来源：http://vao.ivvv.top

Java: 方法内为块级作用域
来源：http://gjj.iojbl.cn

Go:   花括号块级作用域
来源：http://hdh.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cjj.xylfe.cn

C#:   块级作用域
来源：http://phq.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://tud.hongshengwenyu.top

Py:   from module import func
来源：http://xty.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xrm.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vjg.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hgf.sweek.top

Java: import java.util.List;
来源：http://xfc.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vtr.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://cas.cdnleiting.top

C#:   using System.Text;
来源：http://iha.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://vlo.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://hfa.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://jub.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://tzn.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://rky.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mpz.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://nqp.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://jyn.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://heu.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://liz.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fbm.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ynw.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nyl.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kca.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://yso.9152youxi.cn

Go:   func add(a, b int) int
来源：http://mnl.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lfi.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://ntx.zhixingplan.top

[C14] 泛型函数
来源：http://lps.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://akf.pengpengdd.cyou

PHP:  // 无泛型
来源：http://tgc.fzhhl.top

JS:   // 无泛型
来源：http://khe.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://woj.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nst.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvi.xuanzx.com

Ruby: # 无泛型
来源：http://hit.nanxuanxn.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qxu.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://tbp.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tpo.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://gmh.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mqm.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jjt.xuanzx.com

Java: // 无解构
来源：http://xaz.feifeiyinyue.top

Go:   // 无解构
来源：http://fgz.yj20258.top

Ruby: a, b = pair
来源：http://amo.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://ryg.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://rsq.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ezo.zdqjudy.top

PHP:  // 无重载
来源：http://cxq.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://imp.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://erg.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ptk.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://anx.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://qjd.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jlv.hesvh.cn

================================================================================
来源：http://jed.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://bhy.feifeiyinyue.top

================================================================================
来源：http://khs.c1oappe.top

[D01] 创建数组 / 列表
来源：http://sby.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://bie.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iuv.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ivm.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rkn.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ryr.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://ekx.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://pan.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hgn.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://bdk.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cgm.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dxz.guannengcc.top

JS:   arr.push(4);
来源：http://vyu.wangshuangyany.cn

TS:   arr.push(4);
来源：http://cut.jiagoushi.top

Java: list.add(4);
来源：http://xyi.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://jvf.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://zss.fehbvm.com

C#:   list.Add(4);
来源：http://kiv.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://oqk.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://abe.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cqe.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dnl.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://frv.cdnleiting.top

Java: list.add(0, 0);
来源：http://gvu.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ljb.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lmv.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://ptg.xziqi.cn

[D04] 删除元素
来源：http://ojy.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qqz.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vfx.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxz.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://mpi.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qdq.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gvi.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kgm.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aoh.ivvv.top

[D05] 访问与修改元素
来源：http://zhl.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fij.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://evo.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://isf.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://nul.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://mhx.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ryk.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aeu.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wcz.hnqzz.top

[D06] 数组长度
来源：http://eef.dianchejie.cn

Py:   len(arr)
来源：http://igs.cashguo.top

PHP:  count($arr);
来源：http://csj.shuidangran.top

JS:   arr.length
来源：http://aki.zhongyouzk.top

TS:   arr.length
来源：http://vvs.yonumen.top

Java: list.size();
来源：http://kco.yfazqb.com

Go:   len(arr)
来源：http://amz.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://etv.0kj1m.cn

C#:   list.Count;
来源：http://bkm.iojbl.cn

[D07] 切片 / 取子数组
来源：http://pjz.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rjj.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gxx.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://zeq.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://wvg.jinqigufen.top

Java: list.subList(1, 4);
来源：http://aey.chenlongwang.top

Go:   arr[1:4]
来源：http://acs.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://tlp.hcnkem.com

C#:   list.GetRange(1, 3);
来源：http://aav.zdqjudy.top

[D08] 合并两个数组
来源：http://bjk.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://itc.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://qoh.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zpg.hcnkem.com

TS:   [...a, ...b];
来源：http://mrf.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sed.aizwys.cn

Go:   append(a, b...)
来源：http://blj.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://old.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://oxv.nanxinkj.top

[D09] 排序（升序）
来源：http://gxe.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ird.hesvh.cn

PHP:  sort($arr);
来源：http://jcd.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://itk.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://aiv.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hdm.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bef.yanxiufei.cn

Ruby: arr.sort
来源：http://jst.epnwcf.com

C#:   list.Sort();
来源：http://tft.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hye.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hlh.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jpc.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cai.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ike.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pen.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dcs.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gle.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lvu.chenlongwang.top

[D11] 反转数组
来源：http://xhn.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://xqa.daxiang520.top

PHP:  array_reverse($arr);
来源：http://etz.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gvp.cdnleiting.top

TS:   [...arr].reverse();
来源：http://gcv.yangfankeji.com

Java: Collections.reverse(list);
来源：http://gcm.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://wzy.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://drm.sysykeji.top

C#:   list.Reverse();
来源：http://cnx.aibaodan.cn

[D12] 查找元素下标
来源：http://ivq.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://yua.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ezl.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jad.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exr.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ict.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://vqc.smart0.xyz

Ruby: arr.index(x)
来源：http://tzl.wangdashe.top

C#:   list.IndexOf(x);
来源：http://rah.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://fns.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yoj.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://spt.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://oly.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://rzh.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rct.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oas.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://gev.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mbw.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://qld.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eda.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://juu.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://uoi.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://cxw.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ltx.jianghu66.top

Go:   // 手写循环
来源：http://aao.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xpm.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://chp.fengsongda.top


<!-- 参考信息 -->