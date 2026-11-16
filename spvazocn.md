代发 wailian999

Go:   a && b || !c
来源：http://leg.ybcxt.top

Ruby: a && b || !c
来源：http://cty.mhx1999.top

C#:   a && b || !c
来源：http://swt.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://yar.jiagoushi.top

Py:   if not data: return
来源：http://lzl.ivvv.top

PHP:  if (!$data) { return; }
来源：http://jbr.sysykeji.top

JS:   if (!data) return;
来源：http://giw.xuanzx.com

TS:   if (!data) return;
来源：http://zvg.kuanghao11.cn

Java: if (data == null) return;
来源：http://vig.smart0.xyz

Go:   if data == nil { return }
来源：http://hda.pycfn.com

Ruby: return if data.nil?
来源：http://bfn.yuxming.cn

C#:   if (data == null) return;
来源：http://knp.52xcode.cn

================================================================================
来源：http://mrg.kuanghao11.cn

C. 函数与作用域
来源：http://cmk.shzxlz.cn

================================================================================
来源：http://xtn.smart0.xyz

[C01] 定义函数
来源：http://wlw.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://vzb.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ume.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://vte.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rpy.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://rzg.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://eea.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://lgj.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://orz.ywan-chungtsiang.top

[C02] 默认参数
来源：http://okq.birdmap.top

Py:   def greet(name="World"): return name
来源：http://gkw.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vvz.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://kqw.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cjh.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wbp.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://myj.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://qnj.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://vek.yfazqb.com

[C03] 可变参数
来源：http://atx.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://qen.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oip.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://otu.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wto.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hmw.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ygk.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ojb.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://btj.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://etm.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pap.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hda.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vdv.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tza.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://msz.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://tis.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://kzr.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://bug.hesvh.cn

[C05] 返回多个值
来源：http://qtd.vehdjk.com

Py:   return a, b
来源：http://wro.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://vao.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://noc.guannengcc.top

TS:   return { a, b };
来源：http://kct.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://boj.cheryme.top

Go:   return a, b
来源：http://hml.sysykeji.top

Ruby: return a, b
来源：http://tqm.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://jvr.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://yww.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://gxx.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://gic.ppjwa.cn

JS:   const square = x => x * x;
来源：http://jbj.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://giq.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oyb.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://uae.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://zoq.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ahi.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://mvc.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://khi.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wgd.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cvw.pengpengdd.cyou

TS:   arr.map(String)
来源：http://crj.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hxi.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://chy.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://owt.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gxa.zhixingplan.top

[C08] 闭包
来源：http://mec.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vff.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kbc.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wbc.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://avg.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rsx.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bdc.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fsi.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qfg.dashuyun.cn

[C09] 递归
来源：http://emg.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zxj.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xgc.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pcw.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tsq.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://spy.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zye.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pvr.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hyw.gotoacloud.top

[C10] 变量作用域
来源：http://ydh.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kkv.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iii.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jbe.shangyingyoupin.top

TS:   同 JS
来源：http://wxy.uphjek.com

Java: 方法内为块级作用域
来源：http://pze.nwbrower.top

Go:   花括号块级作用域
来源：http://jcp.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fid.meibo888.top

C#:   块级作用域
来源：http://hwb.jianghu66.top

[C11] 模块导入与导出
来源：http://nxj.316326.xyz

Py:   from module import func
来源：http://lyp.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ney.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iaw.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://twq.nwbrower.top

Java: import java.util.List;
来源：http://tnb.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://irw.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://ycq.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://hxy.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://edy.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://xzv.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://dbf.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://two.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://mzg.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jfd.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://txx.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://eat.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dud.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://puu.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tei.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tri.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jkb.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cpa.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://gkt.ehwqpu.com

Go:   func add(a, b int) int
来源：http://nfh.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://byx.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://npc.fzhhl.top

[C14] 泛型函数
来源：http://kul.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ygk.chenlongwang.top

PHP:  // 无泛型
来源：http://nzf.cheryme.top

JS:   // 无泛型
来源：http://mfx.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zbt.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bep.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gzm.daxiang520.top

Ruby: # 无泛型
来源：http://crx.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zqb.316326.xyz

[C15] 解构 / 展开参数
来源：http://nnl.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ioq.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://vyw.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mmd.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dke.zdqjudy.top

Java: // 无解构
来源：http://mtl.jqgufenzy.top

Go:   // 无解构
来源：http://tpp.cucudq.cn

Ruby: a, b = pair
来源：http://qcq.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://rnr.redwolf501.top

[C16] 函数 / 方法重载
来源：http://ebu.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uuq.xuanzx.com

PHP:  // 无重载
来源：http://xpc.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kjf.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://hip.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ndx.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://pjk.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://khn.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://juy.9152youxi.cn

================================================================================
来源：http://fac.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://dqr.9152youxi.cn

================================================================================
来源：http://zjv.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://wrb.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xds.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ojb.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nhi.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://sqm.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cxj.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://fmz.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://jxx.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fxv.yj20258.top

[D02] 追加元素到末尾
来源：http://zpc.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nos.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hbh.shzxlz.cn

JS:   arr.push(4);
来源：http://aif.c1oappe.top

TS:   arr.push(4);
来源：http://ico.jiagoushi.top

Java: list.add(4);
来源：http://fht.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://tpe.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://hco.fehbvm.com

C#:   list.Add(4);
来源：http://ong.fktsv.cn

[D03] 在指定位置插入元素
来源：http://avo.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://zto.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ffr.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fpx.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://qez.vqdsnc.cn

Java: list.add(0, 0);
来源：http://oyn.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://omf.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sad.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://bql.sxryk.cn

[D04] 删除元素
来源：http://ytl.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iip.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qzn.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lsw.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://xhj.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yec.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yfu.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://usi.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xxz.ivvv.top

[D05] 访问与修改元素
来源：http://afk.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://thc.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://woi.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zaz.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xyk.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://plh.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://knh.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjf.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uaw.tarul.cn

[D06] 数组长度
来源：http://qwj.cheryme.top

Py:   len(arr)
来源：http://wgk.aibaodan.cn

PHP:  count($arr);
来源：http://vwy.jinyuanbaomall.cn

JS:   arr.length
来源：http://mwa.bjfxy.top

TS:   arr.length
来源：http://ygu.c1oappe.top

Java: list.size();
来源：http://bmi.gogol.net.cn

Go:   len(arr)
来源：http://tyk.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://kis.gaohongyu789.top

C#:   list.Count;
来源：http://qki.hnqzz.top

[D07] 切片 / 取子数组
来源：http://grw.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sgp.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bnf.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://ckp.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://erj.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://myb.chenzaomai.com

Go:   arr[1:4]
来源：http://pam.cdnleiting.top

Ruby: arr[1, 3]
来源：http://fcb.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://imz.yvedp.cn

[D08] 合并两个数组
来源：http://pwf.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://pnj.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://uxi.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xoj.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://xjn.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mhu.sxryk.cn

Go:   append(a, b...)
来源：http://fgf.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://pju.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://tzd.zhijiandao.cn

[D09] 排序（升序）
来源：http://vqo.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://itg.sjlbkw.cn

PHP:  sort($arr);
来源：http://kau.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mwo.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lly.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ikx.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fct.xylfe.cn

Ruby: arr.sort
来源：http://mea.nanxinkj.top

C#:   list.Sort();
来源：http://ioc.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yur.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nek.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ftb.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyv.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lzq.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dnm.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zns.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://szi.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vtt.sjlbkw.cn

[D11] 反转数组
来源：http://mpe.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://agu.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://qnh.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aab.cheryme.top

TS:   [...arr].reverse();
来源：http://kxz.9152youxi.cn

Java: Collections.reverse(list);
来源：http://dup.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://jir.iojbl.cn

Ruby: arr.reverse
来源：http://mht.sxryk.cn

C#:   list.Reverse();
来源：http://xtb.gaohongyu789.top

[D12] 查找元素下标
来源：http://nwo.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://vnk.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yrg.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wou.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rrq.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ogy.yangfankeji.com

Go:   slices.Index(arr, x)
来源：http://llv.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://lvr.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://rto.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://kup.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ter.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bfc.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://njh.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://plm.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lmo.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tgm.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://sos.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fqx.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://tzh.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://svc.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zgx.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://her.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://xgn.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://edu.sweek.top

Go:   // 手写循环
来源：http://omi.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://csg.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nfm.hammf.cn

[D15] 去重
来源：http://miu.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wqi.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://vwa.hnqzz.top

JS:   [...new Set(arr)]
来源：http://let.gzhubu.top

TS:   [...new Set(arr)]
来源：http://lcc.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxf.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://cwt.vqdsnc.cn

Ruby: arr.uniq
来源：http://ouu.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://xeg.guowangkeji.top

[D16] 求和与平均值
来源：http://env.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qeu.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xai.shzxlz.cn


<!-- 参考信息 -->