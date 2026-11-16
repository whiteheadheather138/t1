代发 wailian999

Go:   a && b || !c
来源：http://pnc.smart0.xyz

Ruby: a && b || !c
来源：http://ahr.nanxuanxn.top

C#:   a && b || !c
来源：http://btg.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://jhs.epnwcf.com

Py:   if not data: return
来源：http://yut.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://akj.fktsv.cn

JS:   if (!data) return;
来源：http://duj.tanke756.top

TS:   if (!data) return;
来源：http://rqw.xziqi.cn

Java: if (data == null) return;
来源：http://gpg.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://ale.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://cjy.zycfv.cn

C#:   if (data == null) return;
来源：http://efe.bbcook.cn

================================================================================
来源：http://qmt.jiagoushi.top

C. 函数与作用域
来源：http://bnp.cheryme.top

================================================================================
来源：http://nhh.sxryk.cn

[C01] 定义函数
来源：http://zwi.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://mdl.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmu.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://dvz.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ucb.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tax.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://wbn.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://wsw.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zxp.fzhhl.top

[C02] 默认参数
来源：http://hir.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://kao.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://knd.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://wpj.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eng.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cea.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jsk.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://vnn.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://sxp.nwbrower.top

[C03] 可变参数
来源：http://grl.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://onk.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hcu.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyg.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jsa.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://inx.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://het.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uhh.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fbx.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://lwr.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xzy.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rlr.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hxz.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wci.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://pcg.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://xrq.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://aoe.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://clg.fzhhl.top

[C05] 返回多个值
来源：http://tfi.sysykeji.top

Py:   return a, b
来源：http://jpz.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://ogs.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nbw.iojbl.cn

TS:   return { a, b };
来源：http://wfw.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xpv.zhongyouzk.top

Go:   return a, b
来源：http://qdh.hcnkem.com

Ruby: return a, b
来源：http://vzu.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://lgx.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://cfs.birdmap.top

Py:   square = lambda x: x * x
来源：http://ueh.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uue.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://yfb.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://ztw.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ols.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://sua.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://pos.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://vzp.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://bql.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yff.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zxr.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://any.zhijiandao.cn

TS:   arr.map(String)
来源：http://abf.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xzf.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://diz.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://ccy.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fps.52xcode.cn

[C08] 闭包
来源：http://gmg.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gwz.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nxk.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nrz.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rlg.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://idc.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nby.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://inr.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://njz.zhijiandao.cn

[C09] 递归
来源：http://yuw.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uuv.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bzg.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hkc.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hhl.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zmq.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://umy.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://szf.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xuq.jinqigufen.top

[C10] 变量作用域
来源：http://udm.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://red.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qqm.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eih.shanyushiyangtech.top

TS:   同 JS
来源：http://hlr.cucudq.cn

Java: 方法内为块级作用域
来源：http://hpv.andypj.xyz

Go:   花括号块级作用域
来源：http://bjo.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ohf.tianlin.xyz

C#:   块级作用域
来源：http://vvw.gzhubu.top

[C11] 模块导入与导出
来源：http://ohf.tarul.cn

Py:   from module import func
来源：http://kxv.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cgn.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yft.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://byy.quarkkingdee.top

Java: import java.util.List;
来源：http://nwe.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ptz.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://opp.zycfv.cn

C#:   using System.Text;
来源：http://dcu.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://ysi.sweek.top

Py:   (lambda: print("run"))()
来源：http://sar.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://tma.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://qxq.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://zjq.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yoa.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://odj.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://wus.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mjr.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://scc.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://htu.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kzz.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://svu.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grx.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ruz.haohaochexian.top

Go:   func add(a, b int) int
来源：http://vdw.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xgb.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://pmi.meibo888.top

[C14] 泛型函数
来源：http://dwq.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oxk.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://hwk.yj202588.top

JS:   // 无泛型
来源：http://flf.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aqv.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rox.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://esf.ppjwa.cn

Ruby: # 无泛型
来源：http://pdt.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uog.fengsongda.top

[C15] 解构 / 展开参数
来源：http://fsn.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nen.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://oir.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tbn.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nbd.nanxuanxn.top

Java: // 无解构
来源：http://hft.birdmap.top

Go:   // 无解构
来源：http://zyk.fengsongda.top

Ruby: a, b = pair
来源：http://roa.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://leu.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://xqv.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mff.pengpengdd.cyou

PHP:  // 无重载
来源：http://frr.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://beh.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://wdn.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zwp.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://cqk.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://hcb.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://brn.sjlbkw.cn

================================================================================
来源：http://dkh.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://frr.yanxiufei.cn

================================================================================
来源：http://awj.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://rwh.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ryx.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qrd.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oot.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pwx.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xew.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://kis.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://nel.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ufh.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://vpa.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lkl.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gpc.aizwys.cn

JS:   arr.push(4);
来源：http://gbf.jqgufenzy.top

TS:   arr.push(4);
来源：http://jhq.xylfe.cn

Java: list.add(4);
来源：http://rjq.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://qjj.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://wwf.epnwcf.com

C#:   list.Add(4);
来源：http://lar.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://aeu.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://fzj.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hbh.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kdb.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://wne.fzhhl.top

Java: list.add(0, 0);
来源：http://xwh.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dvl.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lqb.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://lpl.yanxiufei.cn

[D04] 删除元素
来源：http://yon.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://srt.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ngk.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pet.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://yvu.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://paz.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://idr.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pem.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zgg.sysykeji.top

[D05] 访问与修改元素
来源：http://tcx.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ecy.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://izt.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pcv.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://bsh.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://jgh.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://tey.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bdj.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dim.cashguo.top

[D06] 数组长度
来源：http://sbd.cheryme.top

Py:   len(arr)
来源：http://bfo.quarkkingdee.top

PHP:  count($arr);
来源：http://nrn.jlsjyb.cn

JS:   arr.length
来源：http://glf.daria6918.cn

TS:   arr.length
来源：http://fmx.zhaomingkeji.xyz

Java: list.size();
来源：http://xbg.yangfankeji.com

Go:   len(arr)
来源：http://qhz.birdmap.top

Ruby: arr.length; arr.size
来源：http://uva.tarul.cn

C#:   list.Count;
来源：http://ghb.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://eir.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oev.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sou.havefunace.top

JS:   arr.slice(1, 4);
来源：http://vcs.hammf.cn

TS:   arr.slice(1, 4);
来源：http://ite.iojbl.cn

Java: list.subList(1, 4);
来源：http://vpn.ybcxt.top

Go:   arr[1:4]
来源：http://czc.cucudq.cn

Ruby: arr[1, 3]
来源：http://kbm.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://tol.svipenyu.cn

[D08] 合并两个数组
来源：http://oqo.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://xtf.yj20258.top

PHP:  array_merge($a, $b);
来源：http://qzo.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://enx.iojbl.cn

TS:   [...a, ...b];
来源：http://rpu.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kzo.zhoulong.xyz

Go:   append(a, b...)
来源：http://emz.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://gff.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://ofd.wangdashe.top

[D09] 排序（升序）
来源：http://oov.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://scn.hysaishi.cn

PHP:  sort($arr);
来源：http://hbu.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pob.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iwz.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://svy.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://suf.zhoulong.xyz

Ruby: arr.sort
来源：http://xaz.ppjwa.cn

C#:   list.Sort();
来源：http://pon.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nev.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://njb.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwd.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hto.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wid.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvb.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fgm.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://efz.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ypj.zhixingplan.top

[D11] 反转数组
来源：http://cwb.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ily.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://zzw.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mbq.tian-w.cn

TS:   [...arr].reverse();
来源：http://igt.iojbl.cn

Java: Collections.reverse(list);
来源：http://pid.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://xjy.jqgfzy.top

Ruby: arr.reverse
来源：http://ocy.gotoacloud.top

C#:   list.Reverse();
来源：http://nbo.yonumen.top

[D12] 查找元素下标
来源：http://pmg.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://moo.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aks.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkg.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xuf.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mzn.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://ktf.sxryk.cn

Ruby: arr.index(x)
来源：http://yer.wangdashe.top

C#:   list.IndexOf(x);
来源：http://jwi.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://cib.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wyh.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vgb.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://yqy.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://jqn.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://svb.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tle.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://acl.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rrs.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://mrf.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zih.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zbd.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://gbg.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://fcf.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nhn.hnxiangtu.top

Go:   // 手写循环
来源：http://awy.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://jpb.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sku.gotoacloud.top

[D15] 去重
来源：http://dia.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nxe.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://fbt.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://jlb.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://gxd.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://roa.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://ypp.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://wvv.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://stg.havefunace.top

[D16] 求和与平均值
来源：http://pfc.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qzy.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cyl.sysykeji.top


<!-- 参考信息 -->