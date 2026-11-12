代发 wailian999

Py:   if not data: return
来源：http://ivh.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://krj.tarul.cn

JS:   if (!data) return;
来源：http://cae.xylfe.cn

TS:   if (!data) return;
来源：http://qsw.dianchejie.cn

Java: if (data == null) return;
来源：http://krb.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://exy.cheryme.top

Ruby: return if data.nil?
来源：http://xii.jinqigufen.top

C#:   if (data == null) return;
来源：http://ejj.ivvv.top

================================================================================
来源：http://mpm.guowangkeji.top

C. 函数与作用域
来源：http://fpx.yuanzhike.top

================================================================================
来源：http://nhz.yuanzhike.top

[C01] 定义函数
来源：http://gpr.316326.xyz

Py:   def add(a, b): return a + b
来源：http://xgy.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dne.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://dwt.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cjg.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wuc.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://wmo.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://hak.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://thl.sweek.top

[C02] 默认参数
来源：http://riu.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://aad.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://obu.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://daj.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lef.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qxb.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://icx.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://pfa.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ivw.yuxming.cn

[C03] 可变参数
来源：http://oiv.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://ilm.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://won.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fjv.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hpe.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jgs.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aax.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://tpj.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hsu.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://jqi.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qcc.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pkx.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cdi.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://anc.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://cws.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://clb.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://fll.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://jpx.andypj.xyz

[C05] 返回多个值
来源：http://ryx.jqgufenzy.top

Py:   return a, b
来源：http://ixx.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://prz.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qum.c1oappe.top

TS:   return { a, b };
来源：http://oyc.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gca.zhongyouzk.top

Go:   return a, b
来源：http://rla.haohaochexian.top

Ruby: return a, b
来源：http://djx.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://oes.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://zti.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://yqa.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://vtq.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://fyt.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://ttq.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ryb.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://avy.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://gxa.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://urk.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://pxo.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xet.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ujw.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fqu.yongpay.top

TS:   arr.map(String)
来源：http://srv.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://was.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bau.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://hqe.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eaq.yuanzhike.top

[C08] 闭包
来源：http://kqw.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ocs.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://riv.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zut.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nhd.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dzl.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eju.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xsa.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rln.hesvh.cn

[C09] 递归
来源：http://aig.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://naj.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oif.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://leu.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://huz.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qqv.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rsd.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wij.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kyu.zhixingplan.top

[C10] 变量作用域
来源：http://bml.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zjv.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nqo.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tpp.wangdashe.top

TS:   同 JS
来源：http://tnx.9152youxi.cn

Java: 方法内为块级作用域
来源：http://ouf.sufxvd.cn

Go:   花括号块级作用域
来源：http://pbu.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ijv.yanxiufei.cn

C#:   块级作用域
来源：http://fge.zhixingplan.top

[C11] 模块导入与导出
来源：http://zxx.hongshengwenyu.top

Py:   from module import func
来源：http://lod.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oxo.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://snt.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tdb.ppjwa.cn

Java: import java.util.List;
来源：http://owp.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uqt.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://atm.guowangkeji.top

C#:   using System.Text;
来源：http://lsw.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://vdg.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://rcw.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://vxj.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://snp.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://cel.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hpk.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://ums.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://ecd.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ifb.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://nju.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gyx.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vfp.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bjs.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mub.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://dim.yj20258888.top

Go:   func add(a, b int) int
来源：http://rzw.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://acg.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://ulf.zhengqikj.top

[C14] 泛型函数
来源：http://ikz.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://riy.hammf.cn

PHP:  // 无泛型
来源：http://unw.yueranfly.top

JS:   // 无泛型
来源：http://eak.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ljj.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ovh.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://thr.zycfv.cn

Ruby: # 无泛型
来源：http://zzh.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yxa.shuidangran.top

[C15] 解构 / 展开参数
来源：http://hpw.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vsy.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://rin.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rol.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xkf.yfazqb.com

Java: // 无解构
来源：http://qem.wangdashe.top

Go:   // 无解构
来源：http://eyb.jqgfzy.top

Ruby: a, b = pair
来源：http://ely.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://dpy.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://kkj.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dtj.aizwys.cn

PHP:  // 无重载
来源：http://bmj.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ycf.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://mib.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xct.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://bkp.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://bds.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://hxh.andypj.xyz

================================================================================
来源：http://aqa.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://uef.jlsjyb.cn

================================================================================
来源：http://eyl.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://kwj.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://kxn.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cyo.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://efc.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ibu.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qhz.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://bwf.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://atd.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ejw.0kj1m.cn

[D02] 追加元素到末尾
来源：http://nmb.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ytl.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fab.hammf.cn

JS:   arr.push(4);
来源：http://uvg.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://isv.mhx1999.top

Java: list.add(4);
来源：http://jwq.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://ful.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://znh.zhiwuduotai.top

C#:   list.Add(4);
来源：http://jsa.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://col.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://pwl.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mgh.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kdx.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://fwn.tanke756.top

Java: list.add(0, 0);
来源：http://fvn.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nsu.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hhk.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://zqm.fzhhl.top

[D04] 删除元素
来源：http://tad.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://osv.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kpp.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mwp.cheryme.top

TS:   arr.splice(0, 1);
来源：http://ayq.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vuv.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rmt.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rxa.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ams.hywenlv.cn

[D05] 访问与修改元素
来源：http://osc.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://geq.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bxs.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rmo.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://zax.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://sys.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://svs.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ewg.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ijn.sufxvd.cn

[D06] 数组长度
来源：http://law.zhijiandao.cn

Py:   len(arr)
来源：http://eml.tian-w.cn

PHP:  count($arr);
来源：http://opt.mhx1999.top

JS:   arr.length
来源：http://lqz.xinyue.icu

TS:   arr.length
来源：http://ipt.yonumen.top

Java: list.size();
来源：http://ugz.ivvv.top

Go:   len(arr)
来源：http://kls.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://zcb.ctjpmb.com

C#:   list.Count;
来源：http://gpj.fengsongda.top

[D07] 切片 / 取子数组
来源：http://ayg.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://svb.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://uyo.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://qid.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://owm.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://ltw.hysaishi.cn

Go:   arr[1:4]
来源：http://mxz.daria6918.cn

Ruby: arr[1, 3]
来源：http://lat.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://cjn.havefunace.top

[D08] 合并两个数组
来源：http://srq.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://zzi.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://oil.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xrc.hammf.cn

TS:   [...a, ...b];
来源：http://ndn.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ija.fehbvm.com

Go:   append(a, b...)
来源：http://osg.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://lyc.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://qqp.tanke756.top

[D09] 排序（升序）
来源：http://vxe.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://tne.havefunace.top

PHP:  sort($arr);
来源：http://peq.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://akc.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://brc.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://puy.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xze.svipenyu.cn

Ruby: arr.sort
来源：http://xsb.ydjk.org.cn

C#:   list.Sort();
来源：http://smr.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oyf.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jhf.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nor.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cby.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsc.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mzw.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ptw.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kvw.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jik.xylfe.cn

[D11] 反转数组
来源：http://xky.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://qab.hnqzz.top

PHP:  array_reverse($arr);
来源：http://ria.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pmq.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://pkj.shuidangran.top

Java: Collections.reverse(list);
来源：http://yxc.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://xbq.sjlbkw.cn

Ruby: arr.reverse
来源：http://vgn.gogol.net.cn

C#:   list.Reverse();
来源：http://ysw.cdnleiting.top

[D12] 查找元素下标
来源：http://mez.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://svu.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ojm.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fvv.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oet.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jsg.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://eci.cqqwz.cn

Ruby: arr.index(x)
来源：http://nhr.cashguo.top

C#:   list.IndexOf(x);
来源：http://xue.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://rvs.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nsc.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ryt.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://lly.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://asv.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mmq.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lxw.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jwc.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kvs.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://boj.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aes.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mgc.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://vgq.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://nvr.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ijf.52xcode.cn

Go:   // 手写循环
来源：http://cmr.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://sdj.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ljc.chenjidiqi.icu

[D15] 去重
来源：http://kna.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ezn.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://kmc.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://ysg.shangyingyoupin.top

TS:   [...new Set(arr)]
来源：http://fty.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ixr.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://kuy.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://rju.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://ibv.yj202588.top

[D16] 求和与平均值
来源：http://ciq.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sam.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ore.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jom.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogd.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lrz.ydzc1.top

Go:   // 手写循环累加
来源：http://thw.jyoumei.cn


<!-- 参考信息 -->