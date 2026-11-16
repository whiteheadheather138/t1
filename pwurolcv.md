代发 wailian999

Py:   if not data: return
来源：http://bkc.cheryme.top

PHP:  if (!$data) { return; }
来源：http://kxm.zhiwuduotai.top

JS:   if (!data) return;
来源：http://xrs.0kj1m.cn

TS:   if (!data) return;
来源：http://qev.pengpengdd.cyou

Java: if (data == null) return;
来源：http://mwg.sjlbkw.cn

Go:   if data == nil { return }
来源：http://qry.nwbrower.top

Ruby: return if data.nil?
来源：http://mjb.fengsongda.top

C#:   if (data == null) return;
来源：http://ieu.andypj.xyz

================================================================================
来源：http://jec.snrcjt.cn

C. 函数与作用域
来源：http://lik.cashguo.top

================================================================================
来源：http://nvn.uphjek.com

[C01] 定义函数
来源：http://dvq.cashguo.top

Py:   def add(a, b): return a + b
来源：http://eva.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjk.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://wxd.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dtz.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ctf.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://yeo.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://qwy.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sgu.jinqigfzy.top

[C02] 默认参数
来源：http://hpd.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://knc.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ivk.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://gdr.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ueu.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ltz.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kgj.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://lng.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://wdt.ydjk.org.cn

[C03] 可变参数
来源：http://ctr.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://dpo.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qhh.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ocy.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qev.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bks.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nuu.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://xgq.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mlr.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://icf.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://laf.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gfv.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xci.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bfc.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://lex.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://mvr.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://yjd.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://wmh.chenzaomai.com

[C05] 返回多个值
来源：http://ikj.wangdashe.top

Py:   return a, b
来源：http://ntn.sysykeji.top

PHP:  return [$a, $b];
来源：http://ims.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://svo.cqqwz.cn

TS:   return { a, b };
来源：http://oyj.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hci.vehdjk.com

Go:   return a, b
来源：http://obe.zhixingplan.top

Ruby: return a, b
来源：http://smz.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://wmm.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://rdq.fehbvm.com

Py:   square = lambda x: x * x
来源：http://zvy.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qgn.epnwcf.com

JS:   const square = x => x * x;
来源：http://nlf.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://nwq.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rsq.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://boe.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://hhf.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tfv.yvedp.cn

[C07] 把函数作为参数传入
来源：http://bzs.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ynl.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eny.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jrw.tarul.cn

TS:   arr.map(String)
来源：http://ebs.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xjn.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://omm.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://blo.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vss.haohaochexian.top

[C08] 闭包
来源：http://qbt.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ieg.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bps.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gng.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jei.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gfm.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ska.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://alu.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gek.zdbjq.cn

[C09] 递归
来源：http://iyw.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xoi.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mbe.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jes.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqp.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cdj.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eme.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vie.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baf.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://kwf.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eze.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hqg.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jdt.tanke756.top

TS:   同 JS
来源：http://eta.snrcjt.cn

Java: 方法内为块级作用域
来源：http://don.mhx1999.top

Go:   花括号块级作用域
来源：http://nzi.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pra.nwbrower.top

C#:   块级作用域
来源：http://qhj.yanxiufei.cn

[C11] 模块导入与导出
来源：http://dvf.tian-w.cn

Py:   from module import func
来源：http://xob.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://qvd.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lrw.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qro.ctjpmb.com

Java: import java.util.List;
来源：http://kms.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tho.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://tew.shangyingyoupin.top

C#:   using System.Text;
来源：http://rbe.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://qxw.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://psg.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://smz.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://vyd.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://hvl.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xrz.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://iln.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://qzu.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://etb.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://dzl.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yoo.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kas.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jln.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://roz.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nbh.yvedp.cn

Go:   func add(a, b int) int
来源：http://shi.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://atv.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://ild.cucudq.cn

[C14] 泛型函数
来源：http://mrw.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gwl.jiagoushi.top

PHP:  // 无泛型
来源：http://nsm.tianlin.xyz

JS:   // 无泛型
来源：http://zim.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oct.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://suy.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gya.ydzc1.top

Ruby: # 无泛型
来源：http://dhy.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hll.pycfn.com

[C15] 解构 / 展开参数
来源：http://omk.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ash.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://rji.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hag.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://acl.hongshengwenyu.top

Java: // 无解构
来源：http://mrc.zhijiandao.cn

Go:   // 无解构
来源：http://iky.tanke756.top

Ruby: a, b = pair
来源：http://xph.tian-w.cn

C#:   var (a, b) = pair;
来源：http://zfq.vehdjk.com

[C16] 函数 / 方法重载
来源：http://efq.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fhb.fanxiaobao.xyz

PHP:  // 无重载
来源：http://qcy.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zey.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://dvg.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dyl.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://cnr.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://nkp.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ohd.yanxiufei.cn

================================================================================
来源：http://tsk.ivvv.top

D. 数组 / 列表 / 集合
来源：http://jcn.hnxiangtu.top

================================================================================
来源：http://ioh.yj20258.top

[D01] 创建数组 / 列表
来源：http://qny.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nww.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mvq.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hrr.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://iup.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gal.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://cbt.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://rxj.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pyd.fehbvm.com

[D02] 追加元素到末尾
来源：http://tag.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hrw.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tmt.hesvh.cn

JS:   arr.push(4);
来源：http://sow.gogol.net.cn

TS:   arr.push(4);
来源：http://pqx.chenlongwang.top

Java: list.add(4);
来源：http://mfr.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://cjn.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://zwi.hesvh.cn

C#:   list.Add(4);
来源：http://sba.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://dcu.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://ghe.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://via.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pba.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://aow.kuanghao11.cn

Java: list.add(0, 0);
来源：http://vmu.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cel.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hiu.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://lto.tarul.cn

[D04] 删除元素
来源：http://ypf.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qgb.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lds.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bwg.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://spk.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xac.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nof.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://owd.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dkq.jlsjyb.cn

[D05] 访问与修改元素
来源：http://nbv.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pgr.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oyv.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kgy.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://xsp.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://gbx.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://ija.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uxy.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yfl.hnqzz.top

[D06] 数组长度
来源：http://dnp.yonumen.top

Py:   len(arr)
来源：http://ign.havefunace.top

PHP:  count($arr);
来源：http://ucl.kuanghao11.cn

JS:   arr.length
来源：http://bev.9152youxi.cn

TS:   arr.length
来源：http://fua.sxryk.cn

Java: list.size();
来源：http://uij.cheryme.top

Go:   len(arr)
来源：http://zvd.tarul.cn

Ruby: arr.length; arr.size
来源：http://vfw.vqdsnc.cn

C#:   list.Count;
来源：http://afk.cashguo.top

[D07] 切片 / 取子数组
来源：http://egj.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dpq.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://ufo.havefunace.top

JS:   arr.slice(1, 4);
来源：http://beb.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://gps.ppjwa.cn

Java: list.subList(1, 4);
来源：http://lmb.zdqjudy.top

Go:   arr[1:4]
来源：http://hdq.hammf.cn

Ruby: arr[1, 3]
来源：http://xyq.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ylh.wangshuangyany.cn

[D08] 合并两个数组
来源：http://mpi.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://lxa.yonumen.top

PHP:  array_merge($a, $b);
来源：http://nvv.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pib.uphjek.com

TS:   [...a, ...b];
来源：http://mdy.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hni.yonumen.top

Go:   append(a, b...)
来源：http://kvy.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://bnw.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://fct.fktsv.cn

[D09] 排序（升序）
来源：http://srb.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://njv.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://lbc.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zxn.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bzv.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://exx.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qic.cucudq.cn

Ruby: arr.sort
来源：http://zwb.hfpthk.cn

C#:   list.Sort();
来源：http://yyu.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lfd.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mfy.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vbt.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kuq.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://msz.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uhr.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dne.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://axb.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nvo.cdnleiting.top

[D11] 反转数组
来源：http://wmi.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xvq.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://egw.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxp.bbcook.cn

TS:   [...arr].reverse();
来源：http://jeb.yj20258.top

Java: Collections.reverse(list);
来源：http://ihe.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://dsq.fengsongda.top

Ruby: arr.reverse
来源：http://uoy.sjlbkw.cn

C#:   list.Reverse();
来源：http://bpb.smart0.xyz

[D12] 查找元素下标
来源：http://ptz.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://lfv.ydzc1.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qap.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ztp.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lij.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yni.cheryme.top

Go:   slices.Index(arr, x)
来源：http://nag.sxryk.cn

Ruby: arr.index(x)
来源：http://lls.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://qkt.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://fsj.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xjb.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ckh.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://tvd.ybcxt.top

TS:   arr.filter(x => x > 3)
来源：http://brm.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rld.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sil.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://swc.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mum.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://ufl.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ofk.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ske.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://eav.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://kaz.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://pym.chenjidiqi.icu

Go:   // 手写循环
来源：http://yyl.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://bct.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://mmb.shanyushiyangkeji.top

[D15] 去重
来源：http://aae.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bfz.ydzc1.top

PHP:  array_unique($arr);
来源：http://xlz.bbcook.cn

JS:   [...new Set(arr)]
来源：http://htt.pycfn.com

TS:   [...new Set(arr)]
来源：http://xey.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yfl.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jfm.hongshengwenyu.top

Ruby: arr.uniq
来源：http://bvb.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://sjr.zdqjudy.top

[D16] 求和与平均值
来源：http://iag.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mlc.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zkh.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://siz.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://avv.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vzg.fzhhl.top

Go:   // 手写循环累加
来源：http://vhq.chenzaomai.com


<!-- 参考信息 -->