代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ixq.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://tfk.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://max.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://imn.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://xri.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://swa.zdbjq.cn

[B15] 布尔运算与取反
来源：http://zho.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://xgp.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://dkk.hammf.cn

JS:   a && b || !c
来源：http://lvy.xziqi.cn

TS:   a && b || !c
来源：http://xde.c1oappe.top

Java: a && b || !c
来源：http://pic.shangyingyoupin.top

Go:   a && b || !c
来源：http://cax.tanke756.top

Ruby: a && b || !c
来源：http://tfq.0kj1m.cn

C#:   a && b || !c
来源：http://irs.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://nrd.fzhhl.top

Py:   if not data: return
来源：http://ygq.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://sqt.ppjwa.cn

JS:   if (!data) return;
来源：http://jfa.wangdashe.top

TS:   if (!data) return;
来源：http://bet.hnqzz.top

Java: if (data == null) return;
来源：http://hcf.redwolf501.top

Go:   if data == nil { return }
来源：http://ibg.ydjk.org.cn

Ruby: return if data.nil?
来源：http://tqp.sxryk.cn

C#:   if (data == null) return;
来源：http://uox.daxiang520.top

================================================================================
来源：http://hfd.zdbjq.cn

C. 函数与作用域
来源：http://pti.hnqzz.top

================================================================================
来源：http://dnh.sufxvd.cn

[C01] 定义函数
来源：http://hsl.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://avq.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vkq.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://hum.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbn.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tna.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xxn.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://sfm.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fbe.zhijiandao.cn

[C02] 默认参数
来源：http://poy.cheryme.top

Py:   def greet(name="World"): return name
来源：http://bfw.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cux.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://tlm.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uyp.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://izb.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jju.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://sea.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://rjl.hywenlv.cn

[C03] 可变参数
来源：http://ooc.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://etm.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://onu.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lnf.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gnw.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wsc.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://coi.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mzq.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lma.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://ahi.hcnkem.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tld.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yic.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hln.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xas.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://qcg.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://dxy.havefunace.top

Ruby: f(a: 1, b: 2)
来源：http://ept.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://wwk.sysykeji.top

[C05] 返回多个值
来源：http://owi.fengsongda.top

Py:   return a, b
来源：http://sqc.yongpay.top

PHP:  return [$a, $b];
来源：http://pqw.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pcn.xuanzx.com

TS:   return { a, b };
来源：http://eik.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bhj.redwolf501.top

Go:   return a, b
来源：http://aha.hcnkem.com

Ruby: return a, b
来源：http://cdr.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://joo.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://dcl.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://pah.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zxe.daxiang520.top

JS:   const square = x => x * x;
来源：http://ihy.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ymg.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tuo.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://ish.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://alu.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://meh.xziqi.cn

[C07] 把函数作为参数传入
来源：http://jas.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qbf.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://vcx.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sbu.jlsjyb.cn

TS:   arr.map(String)
来源：http://nrj.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dpe.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qmf.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://lvw.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ixb.hnxiangtu.top

[C08] 闭包
来源：http://ecj.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mix.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qin.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rqh.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xam.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yfr.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lzk.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ewe.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yha.hysaishi.cn

[C09] 递归
来源：http://pga.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mow.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xbx.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzp.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qzi.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zlw.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://chl.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sid.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://esj.gotoacloud.top

[C10] 变量作用域
来源：http://kjg.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pkb.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xpt.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qen.hnxiangtu.top

TS:   同 JS
来源：http://uup.hnqzz.top

Java: 方法内为块级作用域
来源：http://syh.shuidangran.top

Go:   花括号块级作用域
来源：http://ocr.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xoo.fehbvm.com

C#:   块级作用域
来源：http://cac.guannengcc.top

[C11] 模块导入与导出
来源：http://ncb.jianghu66.top

Py:   from module import func
来源：http://qbi.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ast.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xfg.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dcy.gotoacloud.top

Java: import java.util.List;
来源：http://uzs.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eqx.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://clz.bbcook.cn

C#:   using System.Text;
来源：http://bxg.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://qcq.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://qio.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://vos.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://vxq.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://mcc.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rfi.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ykl.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://gog.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://epv.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://ujg.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gcg.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://amm.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zbf.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvn.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://wyo.yj202588.top

Go:   func add(a, b int) int
来源：http://prq.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wkn.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://whi.smart0.xyz

[C14] 泛型函数
来源：http://dgi.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gbe.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://red.zycfv.cn

JS:   // 无泛型
来源：http://hoz.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lbg.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vrn.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yqf.zhengqikj.top

Ruby: # 无泛型
来源：http://yqu.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gve.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://pdn.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tvd.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://sns.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nkx.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hjl.haohaochexian.top

Java: // 无解构
来源：http://nuy.shangyingyoupin.top

Go:   // 无解构
来源：http://umv.316326.xyz

Ruby: a, b = pair
来源：http://jud.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://zry.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://zio.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://phb.dianchejie.cn

PHP:  // 无重载
来源：http://fgc.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://onq.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://lwf.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ful.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://oki.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://onz.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mqt.fehbvm.com

================================================================================
来源：http://gas.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://deo.yuanzhike.top

================================================================================
来源：http://olx.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://bgd.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://mrb.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zrs.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bjd.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lvs.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yjw.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://xwg.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://sog.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pct.pycfn.com

[D02] 追加元素到末尾
来源：http://gdr.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://izx.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ici.mhx1999.top

JS:   arr.push(4);
来源：http://weq.yonumen.top

TS:   arr.push(4);
来源：http://lkp.bjfxy.top

Java: list.add(4);
来源：http://wfw.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://zfj.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://zqx.chenlongwang.top

C#:   list.Add(4);
来源：http://bjl.pycfn.com

[D03] 在指定位置插入元素
来源：http://yku.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://sid.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://weg.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yqk.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://vvx.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://njz.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jjn.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ebw.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://gll.zhixingplan.top

[D04] 删除元素
来源：http://isf.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mgd.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jif.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ubc.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://vqg.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wej.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zcz.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://leq.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://inz.svipenyu.cn

[D05] 访问与修改元素
来源：http://moq.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hqi.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ugl.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mot.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://qis.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://qui.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://bec.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mrq.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kcj.andypj.xyz

[D06] 数组长度
来源：http://bfq.vqdsnc.cn

Py:   len(arr)
来源：http://yqo.jinqigufen.top

PHP:  count($arr);
来源：http://hzq.zdqjudy.top

JS:   arr.length
来源：http://ube.yj202588.top

TS:   arr.length
来源：http://omm.zhengqikj.top

Java: list.size();
来源：http://hol.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://irb.yj202588.top

Ruby: arr.length; arr.size
来源：http://tfk.52xcode.cn

C#:   list.Count;
来源：http://znu.fehbvm.com

[D07] 切片 / 取子数组
来源：http://pdz.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpl.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://xac.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://eqa.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://fen.aibaodan.cn

Java: list.subList(1, 4);
来源：http://www.pycfn.com

Go:   arr[1:4]
来源：http://pgs.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://abv.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://njb.zycfv.cn

[D08] 合并两个数组
来源：http://cmg.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://nwr.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://lqq.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://fbx.yangfankeji.com

TS:   [...a, ...b];
来源：http://pgw.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lno.xinyue.icu

Go:   append(a, b...)
来源：http://lul.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://txe.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://dua.guannengcc.top

[D09] 排序（升序）
来源：http://nwo.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://ucv.gaohongyu789.top

PHP:  sort($arr);
来源：http://mpu.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cst.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xwx.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ksz.hfpthk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://our.sweek.top

Ruby: arr.sort
来源：http://ead.snrcjt.cn

C#:   list.Sort();
来源：http://cfj.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lqo.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xzp.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kxd.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://roh.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wpt.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lxw.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipj.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xsd.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tda.sweek.top

[D11] 反转数组
来源：http://zyw.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://kpf.iojbl.cn

PHP:  array_reverse($arr);
来源：http://bmu.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mcg.fzhhl.top

TS:   [...arr].reverse();
来源：http://kay.chenlongwang.top

Java: Collections.reverse(list);
来源：http://fjo.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://xns.snrcjt.cn

Ruby: arr.reverse
来源：http://pmw.sjlbkw.cn

C#:   list.Reverse();
来源：http://eer.birdmap.top

[D12] 查找元素下标
来源：http://yvd.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://lri.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zuz.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bya.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exc.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ikj.yonumen.top

Go:   slices.Index(arr, x)
来源：http://bfx.jyoumei.cn

Ruby: arr.index(x)
来源：http://tbq.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://pvg.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://asv.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kva.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cxy.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://bsf.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://kmc.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bmr.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bnc.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://qhj.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bph.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://zyt.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://afg.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nae.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://tlt.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://qqv.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bui.wangshuangyany.cn

Go:   // 手写循环
来源：http://frg.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uqz.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hxo.hesvh.cn


<!-- 参考信息 -->