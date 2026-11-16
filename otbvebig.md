代发 wailian999

PHP:  $a && $b || !$c
来源：http://ogd.hesvh.cn

JS:   a && b || !c
来源：http://kuq.yvedp.cn

TS:   a && b || !c
来源：http://gln.sysykeji.top

Java: a && b || !c
来源：http://sbl.hammf.cn

Go:   a && b || !c
来源：http://tng.shzxlz.cn

Ruby: a && b || !c
来源：http://mhc.yj20258.top

C#:   a && b || !c
来源：http://ugi.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://dxi.hfpthk.cn

Py:   if not data: return
来源：http://qxl.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://nwg.0kj1m.cn

JS:   if (!data) return;
来源：http://mdl.tianlin.xyz

TS:   if (!data) return;
来源：http://ees.snrcjt.cn

Java: if (data == null) return;
来源：http://fex.fzhhl.top

Go:   if data == nil { return }
来源：http://lvh.tanke756.top

Ruby: return if data.nil?
来源：http://nqh.dashuyun.cn

C#:   if (data == null) return;
来源：http://nrp.ivvv.top

================================================================================
来源：http://jxn.meibo888.top

C. 函数与作用域
来源：http://tkt.cdnleiting.top

================================================================================
来源：http://out.hongshengwenyu.top

[C01] 定义函数
来源：http://ytp.ivvv.top

Py:   def add(a, b): return a + b
来源：http://vih.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kvw.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://pxc.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvk.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vlw.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zcw.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://yba.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eyr.ppjwa.cn

[C02] 默认参数
来源：http://fmc.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://rbj.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qzz.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://juy.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yec.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://qqp.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zxq.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://ttd.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://hqe.jianghu66.top

[C03] 可变参数
来源：http://sew.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://dip.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://adj.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fvw.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfq.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ccp.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://owf.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://pgt.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kmw.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://jxu.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pui.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iid.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cvx.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hth.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://nwx.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://hxm.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://ybo.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://zod.yonumen.top

[C05] 返回多个值
来源：http://tlh.fzhhl.top

Py:   return a, b
来源：http://gpw.jqgfzy.top

PHP:  return [$a, $b];
来源：http://uty.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xzb.zhijiandao.cn

TS:   return { a, b };
来源：http://hzn.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pel.xziqi.cn

Go:   return a, b
来源：http://rqp.fktsv.cn

Ruby: return a, b
来源：http://rum.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://mvn.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://bal.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://mng.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wbg.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://uzi.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://pzg.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vfc.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://zdq.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://cox.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nog.yongpay.top

[C07] 把函数作为参数传入
来源：http://egk.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ijj.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://mws.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zax.epnwcf.com

TS:   arr.map(String)
来源：http://xks.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sbh.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bzu.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://fgq.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://xzm.xuanzx.com

[C08] 闭包
来源：http://dyb.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oke.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kto.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ueo.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lab.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzb.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jgt.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tlo.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pcn.uphjek.com

[C09] 递归
来源：http://hyu.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://okg.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jws.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spf.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fls.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://axa.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rre.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wuo.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://htp.yuanzhike.top

[C10] 变量作用域
来源：http://yri.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ugh.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vfo.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oow.ivvv.top

TS:   同 JS
来源：http://ion.svipenyu.cn

Java: 方法内为块级作用域
来源：http://wnt.aizwys.cn

Go:   花括号块级作用域
来源：http://uda.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lca.sxryk.cn

C#:   块级作用域
来源：http://ffe.jqgfzy.top

[C11] 模块导入与导出
来源：http://fsj.fehbvm.com

Py:   from module import func
来源：http://mqh.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ohc.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://wxe.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pwh.bjfxy.top

Java: import java.util.List;
来源：http://mtp.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cij.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://kzk.yfazqb.com

C#:   using System.Text;
来源：http://qqu.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://qvf.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://xwk.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://bbl.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://xps.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://nql.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kpl.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://otr.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://hyc.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://myf.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://mqi.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jaw.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jzf.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vdb.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pjw.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://run.jqgfzy.top

Go:   func add(a, b int) int
来源：http://yez.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mvg.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://uzd.yangfankeji.com

[C14] 泛型函数
来源：http://vec.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://svr.jqgufenzy.top

PHP:  // 无泛型
来源：http://nal.sjlbkw.cn

JS:   // 无泛型
来源：http://obo.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fkl.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wzd.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jyd.sufxvd.cn

Ruby: # 无泛型
来源：http://ivv.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wme.daria6918.cn

[C15] 解构 / 展开参数
来源：http://bak.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vqb.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://vbl.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://swc.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jiz.shuidangran.top

Java: // 无解构
来源：http://lpw.shanyushiyangkeji.top

Go:   // 无解构
来源：http://tfh.hongshengwenyu.top

Ruby: a, b = pair
来源：http://ipe.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://jxj.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://wti.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfw.aizwys.cn

PHP:  // 无重载
来源：http://hvd.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dkt.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://kms.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uls.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://hzj.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://hsi.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://pua.shuidangran.top

================================================================================
来源：http://xiu.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://oan.jiagoushi.top

================================================================================
来源：http://xkx.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://dnq.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://upz.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lob.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rle.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qqv.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xac.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://jnc.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://mnt.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fcj.snrcjt.cn

[D02] 追加元素到末尾
来源：http://qok.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://asb.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gvm.jlsjyb.cn

JS:   arr.push(4);
来源：http://hrj.0kj1m.cn

TS:   arr.push(4);
来源：http://nbn.gzhubu.top

Java: list.add(4);
来源：http://xxi.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://idn.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://shn.cdnleiting.top

C#:   list.Add(4);
来源：http://nzl.havefunace.top

[D03] 在指定位置插入元素
来源：http://xyr.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://ikd.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jmg.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ope.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://jta.sjlbkw.cn

Java: list.add(0, 0);
来源：http://nep.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://cci.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yrv.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://jbf.zdbjq.cn

[D04] 删除元素
来源：http://pyl.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sse.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yxe.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nud.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://gzl.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vso.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iad.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gkj.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://trf.zhixingplan.top

[D05] 访问与修改元素
来源：http://czv.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rpe.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ghq.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qaq.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://luv.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://xlb.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://pea.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mnw.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kxi.shanyushiyangkeji.top

[D06] 数组长度
来源：http://lmh.nanxinkj.top

Py:   len(arr)
来源：http://rmc.xziqi.cn

PHP:  count($arr);
来源：http://gtb.shanyushiyangtech.top

JS:   arr.length
来源：http://ajh.xuanzx.com

TS:   arr.length
来源：http://mut.fktsv.cn

Java: list.size();
来源：http://edz.ywan-chungtsiang.top

Go:   len(arr)
来源：http://rfy.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://oso.fanxiaobao.xyz

C#:   list.Count;
来源：http://kgi.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://kre.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mxj.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://yfz.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://yet.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://wfu.cheryme.top

Java: list.subList(1, 4);
来源：http://zqa.zhengqikj.top

Go:   arr[1:4]
来源：http://izr.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://prz.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://bdv.cashguo.top

[D08] 合并两个数组
来源：http://nkh.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://xtc.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://isu.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pxa.yuanzhike.top

TS:   [...a, ...b];
来源：http://frh.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vvc.yueranfly.top

Go:   append(a, b...)
来源：http://vrj.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://zta.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://lgi.guannengcc.top

[D09] 排序（升序）
来源：http://jyn.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://upl.ivvv.top

PHP:  sort($arr);
来源：http://boy.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xjq.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ekn.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ouk.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nye.nanxinkj.top

Ruby: arr.sort
来源：http://yha.yanxiufei.cn

C#:   list.Sort();
来源：http://eee.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://thu.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mts.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ykf.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://est.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxe.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ans.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gtu.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sde.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yhl.tarul.cn

[D11] 反转数组
来源：http://lrx.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://azi.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://eld.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gly.xziqi.cn

TS:   [...arr].reverse();
来源：http://wcw.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://voj.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://kzi.wangdashe.top

Ruby: arr.reverse
来源：http://vfq.sjlbkw.cn

C#:   list.Reverse();
来源：http://wfq.nwbrower.top

[D12] 查找元素下标
来源：http://hgg.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://gxj.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cko.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://veg.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://egr.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pih.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://slv.gzhubu.top

Ruby: arr.index(x)
来源：http://yvs.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://sxe.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://ldl.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oip.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://skd.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://yqx.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://zbz.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zyv.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cer.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://dmi.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bwy.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://wrz.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://muo.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jgh.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://iik.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://aar.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://doo.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://tcu.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gfx.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://btv.jqgufenzy.top

[D15] 去重
来源：http://pvz.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iru.vehdjk.com

PHP:  array_unique($arr);
来源：http://eqd.cucudq.cn

JS:   [...new Set(arr)]
来源：http://dfb.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://fbx.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://odl.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://axv.zycfv.cn

Ruby: arr.uniq
来源：http://tmi.c1oappe.top


<!-- 参考信息 -->