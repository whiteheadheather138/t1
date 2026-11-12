代发 wailian999

PHP:  $a && $b || !$c
来源：http://xkg.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://wpc.andypj.xyz

TS:   a && b || !c
来源：http://dbc.xylfe.cn

Java: a && b || !c
来源：http://huq.shangyingyoupin.top

Go:   a && b || !c
来源：http://zjc.tian-w.cn

Ruby: a && b || !c
来源：http://mfb.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://hnw.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jat.gaohongyu789.top

Py:   if not data: return
来源：http://kcn.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://tie.fehbvm.com

JS:   if (!data) return;
来源：http://yyr.meibo888.top

TS:   if (!data) return;
来源：http://qqc.hfpthk.cn

Java: if (data == null) return;
来源：http://fsi.nanxinkj.top

Go:   if data == nil { return }
来源：http://jjk.yj20258.top

Ruby: return if data.nil?
来源：http://tpq.andypj.xyz

C#:   if (data == null) return;
来源：http://brw.gogol.net.cn

================================================================================
来源：http://yog.kuanghao11.cn

C. 函数与作用域
来源：http://mzt.nanxinkj.top

================================================================================
来源：http://zgx.yuanzhike.top

[C01] 定义函数
来源：http://vxy.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://axb.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vxc.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://lzv.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqn.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ghx.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://cua.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://gqi.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://utf.hongshengwenyu.top

[C02] 默认参数
来源：http://nga.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://eam.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://gqt.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://xgb.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dpq.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://khk.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kia.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://kvk.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://ytm.tianlin.xyz

[C03] 可变参数
来源：http://lux.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://sun.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sgy.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jvj.daxiang520.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tju.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ubk.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zqp.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qgg.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xja.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://xwc.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pdn.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsh.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fzc.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wtf.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://yzl.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://fnj.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://jkr.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://lko.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://wsh.yj202588.top

Py:   return a, b
来源：http://ghd.hesvh.cn

PHP:  return [$a, $b];
来源：http://brr.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uzx.jqgufenzy.top

TS:   return { a, b };
来源：http://obo.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dvu.zycfv.cn

Go:   return a, b
来源：http://col.gogol.net.cn

Ruby: return a, b
来源：http://fdp.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://qco.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://myt.redwolf501.top

Py:   square = lambda x: x * x
来源：http://ulc.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xbs.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://xio.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://umh.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dyz.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://fob.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://xpo.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://wzy.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://egv.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mou.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hsq.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eum.iojbl.cn

TS:   arr.map(String)
来源：http://ljf.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nqx.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdo.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://whi.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zoj.sufxvd.cn

[C08] 闭包
来源：http://gip.dianchejie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mjy.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kwy.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://psj.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hfw.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://quf.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://haq.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hay.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tfr.feifeiyinyue.top

[C09] 递归
来源：http://gtk.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qxi.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://skr.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fca.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzi.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hqw.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rim.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xhu.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sys.fktsv.cn

[C10] 变量作用域
来源：http://riw.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rfy.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qne.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ttz.xuetiantiany.cn

TS:   同 JS
来源：http://gae.tian-w.cn

Java: 方法内为块级作用域
来源：http://nxw.cashguo.top

Go:   花括号块级作用域
来源：http://jvn.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gls.yj20258888.top

C#:   块级作用域
来源：http://gnq.sxryk.cn

[C11] 模块导入与导出
来源：http://ldj.ydjk.org.cn

Py:   from module import func
来源：http://kux.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yny.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://udv.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qnf.tarul.cn

Java: import java.util.List;
来源：http://xvc.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rnj.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://cmx.52xcode.cn

C#:   using System.Text;
来源：http://jnj.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://niz.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://wrd.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://riq.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://tfz.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://ruo.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fpp.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://amg.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://kcp.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xdd.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://heb.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dnb.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syr.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ihk.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wym.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fyv.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://uxa.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kar.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://gda.pengpengdd.cyou

[C14] 泛型函数
来源：http://ybv.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tvr.hammf.cn

PHP:  // 无泛型
来源：http://kwz.aizwys.cn

JS:   // 无泛型
来源：http://les.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bep.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bal.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://apc.0kj1m.cn

Ruby: # 无泛型
来源：http://kix.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ene.hcnkem.com

[C15] 解构 / 展开参数
来源：http://viv.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jme.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://lsp.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://stz.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qku.jinghuilouyu.cn

Java: // 无解构
来源：http://zda.tarul.cn

Go:   // 无解构
来源：http://xbz.snrcjt.cn

Ruby: a, b = pair
来源：http://fey.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://qyx.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://knm.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tjb.ybcxt.top

PHP:  // 无重载
来源：http://ehc.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tvf.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://jhu.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wrp.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://zyq.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://vjp.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jha.gogol.net.cn

================================================================================
来源：http://jvx.uphjek.com

D. 数组 / 列表 / 集合
来源：http://rpd.chenlongwang.top

================================================================================
来源：http://tgl.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://auk.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://itk.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jmh.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cfl.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://meq.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yio.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://opn.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://lfn.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ovo.xylfe.cn

[D02] 追加元素到末尾
来源：http://asz.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vwl.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rch.fzhhl.top

JS:   arr.push(4);
来源：http://vjo.jianghu66.top

TS:   arr.push(4);
来源：http://kfs.hcnkem.com

Java: list.add(4);
来源：http://baw.birdmap.top

Go:   arr = append(arr, 4)
来源：http://nou.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://nxm.yj20258.top

C#:   list.Add(4);
来源：http://xsg.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://vew.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://nps.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qle.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oiz.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://rdj.chenlongwang.top

Java: list.add(0, 0);
来源：http://skm.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://juq.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ohe.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://fsa.smart0.xyz

[D04] 删除元素
来源：http://ixm.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lgo.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mkl.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fke.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://hdy.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://juw.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oyu.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bng.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ute.hysaishi.cn

[D05] 访问与修改元素
来源：http://zba.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zjr.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qgq.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vpo.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://njj.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://cng.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://nzt.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bty.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lve.sufxvd.cn

[D06] 数组长度
来源：http://qhi.zdbjq.cn

Py:   len(arr)
来源：http://voj.hesvh.cn

PHP:  count($arr);
来源：http://vda.cucudq.cn

JS:   arr.length
来源：http://xze.jlsjyb.cn

TS:   arr.length
来源：http://gzn.redwolf501.top

Java: list.size();
来源：http://xtn.yj202588.top

Go:   len(arr)
来源：http://who.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://gwy.yuanzhike.top

C#:   list.Count;
来源：http://bep.gzhubu.top

[D07] 切片 / 取子数组
来源：http://kxx.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vaj.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://nit.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://zpo.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://ppn.zdbjq.cn

Java: list.subList(1, 4);
来源：http://zhg.tianlin.xyz

Go:   arr[1:4]
来源：http://qds.ehwqpu.com

Ruby: arr[1, 3]
来源：http://fqx.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://lmu.dianchejie.cn

[D08] 合并两个数组
来源：http://rrc.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://cis.meibo888.top

PHP:  array_merge($a, $b);
来源：http://fsc.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fzp.sxryk.cn

TS:   [...a, ...b];
来源：http://lve.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wfh.gzhubu.top

Go:   append(a, b...)
来源：http://lqw.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://mhk.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://vyt.jianghu66.top

[D09] 排序（升序）
来源：http://mpe.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://llx.pycfn.com

PHP:  sort($arr);
来源：http://ujd.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zok.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wym.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dfz.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uwa.jinqigufen.top

Ruby: arr.sort
来源：http://vhn.cqqwz.cn

C#:   list.Sort();
来源：http://cda.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uqs.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbc.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehd.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oad.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://col.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://otj.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eys.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rpi.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sox.tanke756.top

[D11] 反转数组
来源：http://pcy.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://rpk.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://ppe.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iox.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://mio.ivvv.top

Java: Collections.reverse(list);
来源：http://amf.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://ceu.zhengqikj.top

Ruby: arr.reverse
来源：http://iey.daxiang520.top

C#:   list.Reverse();
来源：http://jyq.zhoulong.xyz

[D12] 查找元素下标
来源：http://dry.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://icx.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ioq.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fhl.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syi.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ksh.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://ulu.yj202588.top

Ruby: arr.index(x)
来源：http://ocg.yfazqb.com

C#:   list.IndexOf(x);
来源：http://gio.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://rla.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wkf.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sxq.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://pyt.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://uyv.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://djl.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cfx.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://szm.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oyf.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://nhk.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://led.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ywq.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://waw.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://aig.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zfu.tarul.cn

Go:   // 手写循环
来源：http://ibp.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lku.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ize.svipenyu.cn

[D15] 去重
来源：http://dqt.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nvc.haohaochexian.top

PHP:  array_unique($arr);
来源：http://tae.wangdashe.top

JS:   [...new Set(arr)]
来源：http://wae.xziqi.cn

TS:   [...new Set(arr)]
来源：http://rww.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zku.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://gxf.sjlbkw.cn

Ruby: arr.uniq
来源：http://hkx.zdbjq.cn


<!-- 参考信息 -->