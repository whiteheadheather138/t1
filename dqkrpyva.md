代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://gpp.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dqf.yj20258888.top

[B15] 布尔运算与取反
来源：http://opz.tian-w.cn

Py:   a and b or not c
来源：http://oqr.daxiang520.top

PHP:  $a && $b || !$c
来源：http://qna.nanxuanxn.top

JS:   a && b || !c
来源：http://oau.yongpay.top

TS:   a && b || !c
来源：http://rwg.mhx1999.top

Java: a && b || !c
来源：http://utm.dashuyun.cn

Go:   a && b || !c
来源：http://ssr.birdmap.top

Ruby: a && b || !c
来源：http://lkd.nwbrower.top

C#:   a && b || !c
来源：http://pjv.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://sqr.cqqwz.cn

Py:   if not data: return
来源：http://wgz.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://hoi.hywenlv.cn

JS:   if (!data) return;
来源：http://vzp.yueranfly.top

TS:   if (!data) return;
来源：http://szq.shuidangran.top

Java: if (data == null) return;
来源：http://gtk.yuxming.cn

Go:   if data == nil { return }
来源：http://idb.fktsv.cn

Ruby: return if data.nil?
来源：http://asz.ivvv.top

C#:   if (data == null) return;
来源：http://bew.tianlin.xyz

================================================================================
来源：http://xan.dianchejie.cn

C. 函数与作用域
来源：http://gcg.redwolf501.top

================================================================================
来源：http://qye.wangshuangyany.cn

[C01] 定义函数
来源：http://omn.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://aau.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxi.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://tnb.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://whd.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aoy.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eoe.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://ckq.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lja.cqqwz.cn

[C02] 默认参数
来源：http://bax.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://efv.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://frt.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://itj.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vng.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jzh.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ghz.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://udt.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://upn.hammf.cn

[C03] 可变参数
来源：http://yuw.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://out.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sbj.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tmk.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gel.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rym.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fbx.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iey.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wuq.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://gmi.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qgp.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fss.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ghb.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mxj.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://qrx.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://qie.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://mlr.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://juk.shanyushiyangtech.top

[C05] 返回多个值
来源：http://mtt.fengsongda.top

Py:   return a, b
来源：http://zez.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://ake.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://gjm.quarkkingdee.top

TS:   return { a, b };
来源：http://pxr.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aqk.vqdsnc.cn

Go:   return a, b
来源：http://tnb.zycfv.cn

Ruby: return a, b
来源：http://rof.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://ohs.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://kpn.iojbl.cn

Py:   square = lambda x: x * x
来源：http://uff.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hyr.jyoumei.cn

JS:   const square = x => x * x;
来源：http://sfs.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://ywt.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rzy.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://lwd.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://yfr.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hua.tarul.cn

[C07] 把函数作为参数传入
来源：http://dua.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wch.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://xjx.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iwb.xziqi.cn

TS:   arr.map(String)
来源：http://mfn.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://obs.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zmw.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://fnp.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kko.tarul.cn

[C08] 闭包
来源：http://cak.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xvr.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tmz.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://alj.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zqr.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lic.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uuu.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jbj.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fdf.andypj.xyz

[C09] 递归
来源：http://wxr.zhiwuduotai.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ppc.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpr.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ylj.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xrf.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://acq.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oau.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uvn.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hby.xinyue.icu

[C10] 变量作用域
来源：http://jwh.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://okx.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xcy.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zoz.yuanzhike.top

TS:   同 JS
来源：http://epb.chenzaomai.com

Java: 方法内为块级作用域
来源：http://wag.nanxuanxn.top

Go:   花括号块级作用域
来源：http://scn.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lea.fengsongda.top

C#:   块级作用域
来源：http://mpk.vqdsnc.cn

[C11] 模块导入与导出
来源：http://cmj.shuidangran.top

Py:   from module import func
来源：http://nyr.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fiz.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dzb.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mvx.wangdashe.top

Java: import java.util.List;
来源：http://nvd.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tll.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://ooz.uphjek.com

C#:   using System.Text;
来源：http://yjo.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://lkc.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://xyd.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://kht.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://jsi.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://yze.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dfz.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://nfh.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://gny.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kcx.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://trn.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nju.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxk.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://msh.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cqb.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wut.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://lrv.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://naz.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://ogp.xylfe.cn

[C14] 泛型函数
来源：http://jbn.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aoc.svipenyu.cn

PHP:  // 无泛型
来源：http://xyi.guowangkeji.top

JS:   // 无泛型
来源：http://puy.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kcu.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ckf.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mfw.uphjek.com

Ruby: # 无泛型
来源：http://aqq.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ycf.fktsv.cn

[C15] 解构 / 展开参数
来源：http://uyy.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jcb.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://ujn.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://woh.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://czs.birdmap.top

Java: // 无解构
来源：http://nkr.gzhubu.top

Go:   // 无解构
来源：http://eef.gaohongyu789.top

Ruby: a, b = pair
来源：http://rjf.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://eph.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://ght.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zhu.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://zni.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vgj.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://isg.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://scf.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://bjz.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://kma.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qdz.tianlin.xyz

================================================================================
来源：http://spu.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://mrj.cucudq.cn

================================================================================
来源：http://tng.yongpay.top

[D01] 创建数组 / 列表
来源：http://qnf.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ypb.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cuy.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://esp.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xvt.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hxn.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://fck.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://pec.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ppt.tarul.cn

[D02] 追加元素到末尾
来源：http://tch.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pjb.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hsm.xziqi.cn

JS:   arr.push(4);
来源：http://tau.iojbl.cn

TS:   arr.push(4);
来源：http://dpd.shzxlz.cn

Java: list.add(4);
来源：http://htl.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://bor.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://xyu.xziqi.cn

C#:   list.Add(4);
来源：http://dhc.fzhhl.top

[D03] 在指定位置插入元素
来源：http://zjr.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://chf.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://awv.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lmd.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://isy.hysaishi.cn

Java: list.add(0, 0);
来源：http://abe.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://bui.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yqy.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://cjj.gogol.net.cn

[D04] 删除元素
来源：http://kwq.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qpu.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hjq.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ppv.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://fbv.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dln.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xnm.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ygy.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yks.gotoacloud.top

[D05] 访问与修改元素
来源：http://rxo.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tox.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xrq.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dna.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://ijr.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://amu.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://qvx.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://icc.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvx.yongpay.top

[D06] 数组长度
来源：http://sga.daxiang520.top

Py:   len(arr)
来源：http://mhv.tarul.cn

PHP:  count($arr);
来源：http://pbw.yfazqb.com

JS:   arr.length
来源：http://zlo.ppjwa.cn

TS:   arr.length
来源：http://tfi.shanyushiyangkeji.top

Java: list.size();
来源：http://zkt.haohaochexian.top

Go:   len(arr)
来源：http://bgh.jianghu66.top

Ruby: arr.length; arr.size
来源：http://kfc.aibaodan.cn

C#:   list.Count;
来源：http://vrt.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://bru.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lem.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://kig.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://vfk.cheryme.top

TS:   arr.slice(1, 4);
来源：http://nvz.yj202588.top

Java: list.subList(1, 4);
来源：http://dxl.tian-w.cn

Go:   arr[1:4]
来源：http://qrj.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://lwk.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://frn.nanxinkj.top

[D08] 合并两个数组
来源：http://gqb.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://wjk.yj20258.top

PHP:  array_merge($a, $b);
来源：http://agg.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://crz.dianchejie.cn

TS:   [...a, ...b];
来源：http://cfj.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kne.fktsv.cn

Go:   append(a, b...)
来源：http://ldp.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://jam.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://vml.guowangkeji.top

[D09] 排序（升序）
来源：http://ice.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://odv.yuxming.cn

PHP:  sort($arr);
来源：http://sxw.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gzq.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qla.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qtl.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tcg.andypj.xyz

Ruby: arr.sort
来源：http://zji.xuanzx.com

C#:   list.Sort();
来源：http://mrx.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xzj.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vll.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://num.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dur.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hnl.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uon.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eeg.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ewn.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xnz.jyoumei.cn

[D11] 反转数组
来源：http://yjv.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fgg.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://yxn.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fhi.ydzc1.top

TS:   [...arr].reverse();
来源：http://exr.52xcode.cn

Java: Collections.reverse(list);
来源：http://hsc.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://eah.jiagoushi.top

Ruby: arr.reverse
来源：http://dfu.ctjpmb.com

C#:   list.Reverse();
来源：http://mkw.zycfv.cn

[D12] 查找元素下标
来源：http://jhk.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://bgg.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sxg.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ybn.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgx.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cub.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://ijg.sweek.top

Ruby: arr.index(x)
来源：http://pha.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://zlk.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://pna.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rac.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pvc.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://bmq.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://rfh.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lkf.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://shb.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://cpp.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kex.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://mtp.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ibj.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hlb.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://xam.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://lmn.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qwx.quarkkingdee.top

Go:   // 手写循环
来源：http://bpk.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://wci.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dqy.zhaomingkeji.xyz

[D15] 去重
来源：http://dce.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hvw.iojbl.cn

PHP:  array_unique($arr);
来源：http://juj.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://ncm.ybcxt.top


<!-- 参考信息 -->