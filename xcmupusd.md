代发 wailian999

Go:   a && b || !c
来源：http://etv.zdbjq.cn

Ruby: a && b || !c
来源：http://kry.feifeiyinyue.top

C#:   a && b || !c
来源：http://xze.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kio.ywan-chungtsiang.top

Py:   if not data: return
来源：http://tal.ivvv.top

PHP:  if (!$data) { return; }
来源：http://psl.cucudq.cn

JS:   if (!data) return;
来源：http://yep.gaohongyu789.top

TS:   if (!data) return;
来源：http://mfl.sufxvd.cn

Java: if (data == null) return;
来源：http://tjm.zycfv.cn

Go:   if data == nil { return }
来源：http://rzr.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://kdt.ppjwa.cn

C#:   if (data == null) return;
来源：http://udd.dianchejie.cn

================================================================================
来源：http://aqf.shuidangran.top

C. 函数与作用域
来源：http://qrg.ywan-chungtsiang.top

================================================================================
来源：http://cwg.yangfankeji.com

[C01] 定义函数
来源：http://inf.cashguo.top

Py:   def add(a, b): return a + b
来源：http://mdc.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qgj.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://pfc.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mwj.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cep.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://drj.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://bhi.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rqz.jinqigufen.top

[C02] 默认参数
来源：http://yif.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://fgf.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dqq.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://qjz.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kge.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xno.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hke.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://xnj.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://ujn.xuetiantiany.cn

[C03] 可变参数
来源：http://tjr.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://myo.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zmh.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkf.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ufk.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wvm.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mji.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nub.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dib.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://wcc.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tfb.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wws.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://omw.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ept.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://tlw.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://tfo.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://nwt.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://sln.mhx1999.top

[C05] 返回多个值
来源：http://xua.yuanzhike.top

Py:   return a, b
来源：http://qaf.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://khe.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zfx.cheryme.top

TS:   return { a, b };
来源：http://zdw.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yxz.dashuyun.cn

Go:   return a, b
来源：http://xxw.hnqzz.top

Ruby: return a, b
来源：http://inh.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://jxb.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://ran.andypj.xyz

Py:   square = lambda x: x * x
来源：http://ftl.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wrr.zhixingplan.top

JS:   const square = x => x * x;
来源：http://rug.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://nks.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bzb.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://cjm.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://kxh.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ply.hnqzz.top

[C07] 把函数作为参数传入
来源：http://ocf.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kwl.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://xnf.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://epn.sweek.top

TS:   arr.map(String)
来源：http://uvu.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ehv.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cok.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://ijw.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://phv.smart0.xyz

[C08] 闭包
来源：http://fvq.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qxk.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ctm.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aob.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pwj.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gew.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://glc.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qxa.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lmr.andypj.xyz

[C09] 递归
来源：http://zfc.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jra.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://prg.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ezr.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edr.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hnc.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://soa.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hjk.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://liq.feifeiyinyue.top

[C10] 变量作用域
来源：http://loj.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gne.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tgi.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://orb.shzxlz.cn

TS:   同 JS
来源：http://ryk.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://wut.fzhhl.top

Go:   花括号块级作用域
来源：http://ncg.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gci.zhixingplan.top

C#:   块级作用域
来源：http://vki.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://onv.52xcode.cn

Py:   from module import func
来源：http://mic.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dpa.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wbn.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mpt.zhongyouzk.top

Java: import java.util.List;
来源：http://fhr.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cud.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://wcm.yonumen.top

C#:   using System.Text;
来源：http://usf.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://itd.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://cru.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://gpj.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://unv.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://gzg.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gej.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ydi.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://djp.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vjo.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://ayh.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jzz.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xkd.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rgc.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qcu.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://udh.snrcjt.cn

Go:   func add(a, b int) int
来源：http://hlp.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htt.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qus.yj20258888.top

[C14] 泛型函数
来源：http://yza.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rsb.tian-w.cn

PHP:  // 无泛型
来源：http://usv.daxiang520.top

JS:   // 无泛型
来源：http://umk.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ohk.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dts.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jnq.cucudq.cn

Ruby: # 无泛型
来源：http://pvk.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://udi.sysykeji.top

[C15] 解构 / 展开参数
来源：http://frt.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mtu.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://mvf.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bwd.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bxz.shuidangran.top

Java: // 无解构
来源：http://mdi.yueranfly.top

Go:   // 无解构
来源：http://ahr.hongshengwenyu.top

Ruby: a, b = pair
来源：http://wpa.zycfv.cn

C#:   var (a, b) = pair;
来源：http://eii.havefunace.top

[C16] 函数 / 方法重载
来源：http://ymc.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sto.bjfxy.top

PHP:  // 无重载
来源：http://pcm.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ivb.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://nzy.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uku.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://jbh.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://pjl.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://glg.fehbvm.com

================================================================================
来源：http://wdo.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://pmq.zhijiandao.cn

================================================================================
来源：http://psf.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://sdp.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qbm.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oks.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wgz.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uoi.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fvg.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://akk.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://loq.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wpd.mhx1999.top

[D02] 追加元素到末尾
来源：http://oss.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://noo.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fif.iojbl.cn

JS:   arr.push(4);
来源：http://mmh.shzxlz.cn

TS:   arr.push(4);
来源：http://grp.dashuyun.cn

Java: list.add(4);
来源：http://eyy.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://cyn.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://bgg.52xcode.cn

C#:   list.Add(4);
来源：http://rec.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://chz.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://rfc.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kmb.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hif.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://jwz.cqqwz.cn

Java: list.add(0, 0);
来源：http://miu.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://qga.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yrh.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://pwu.nanxinkj.top

[D04] 删除元素
来源：http://azr.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jvs.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uyv.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://alz.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://ckn.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nue.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bpq.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wzd.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://icy.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://zlc.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://era.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://god.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ney.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://kbf.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://mah.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dsn.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fln.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hob.jinyuanbaomall.cn

[D06] 数组长度
来源：http://ijw.daria6918.cn

Py:   len(arr)
来源：http://cji.uphjek.com

PHP:  count($arr);
来源：http://xjd.nanxuanxn.top

JS:   arr.length
来源：http://bva.xuanzx.com

TS:   arr.length
来源：http://xhg.sufxvd.cn

Java: list.size();
来源：http://mxp.guowangkeji.top

Go:   len(arr)
来源：http://fut.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://mhp.cheryme.top

C#:   list.Count;
来源：http://hwu.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://dfv.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghx.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://epf.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://zpq.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://bbl.gzhubu.top

Java: list.subList(1, 4);
来源：http://xrv.fengsongda.top

Go:   arr[1:4]
来源：http://chf.ydzc1.top

Ruby: arr[1, 3]
来源：http://nkf.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://ptu.meibo888.top

[D08] 合并两个数组
来源：http://vve.sweek.top

Py:   a + b;  a.extend(b)
来源：http://wpn.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://mpi.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uco.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://ikt.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bip.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://yqp.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://oaj.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://ifx.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://cxo.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://mgu.xuanzx.com

PHP:  sort($arr);
来源：http://qur.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mti.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hul.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qca.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gef.tarul.cn

Ruby: arr.sort
来源：http://lzq.yangfankeji.com

C#:   list.Sort();
来源：http://bcz.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://srl.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://poa.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrz.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://byc.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qho.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://scs.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hfw.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ttr.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ych.daxiang520.top

[D11] 反转数组
来源：http://epd.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://fdb.cheryme.top

PHP:  array_reverse($arr);
来源：http://xen.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://igy.ehwqpu.com

TS:   [...arr].reverse();
来源：http://wke.fktsv.cn

Java: Collections.reverse(list);
来源：http://sfh.hammf.cn

Go:   slices.Reverse(arr)
来源：http://cmw.wangdashe.top

Ruby: arr.reverse
来源：http://dti.xylfe.cn

C#:   list.Reverse();
来源：http://smx.jinqigfzy.top

[D12] 查找元素下标
来源：http://ics.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://ynd.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fwf.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hiy.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://upw.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ufk.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://rzg.quarkkingdee.top

Ruby: arr.index(x)
来源：http://thf.ybcxt.top

C#:   list.IndexOf(x);
来源：http://lhy.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://nhh.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fuj.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lbg.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://xup.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://zcr.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dhr.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aei.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://dmp.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xoh.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://upu.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pfi.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xdv.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://izm.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://lvn.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ndu.jqgufenzy.top

Go:   // 手写循环
来源：http://bmt.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://fsz.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yam.havefunace.top

[D15] 去重
来源：http://zph.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lap.yj20258888.top

PHP:  array_unique($arr);
来源：http://jvg.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://bmb.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://ikm.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kal.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://cjx.birdmap.top

Ruby: arr.uniq
来源：http://qwm.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://hrd.ydjk.org.cn

[D16] 求和与平均值
来源：http://bpi.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bav.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fil.havefunace.top


<!-- 参考信息 -->