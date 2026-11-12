代发 wailian999

Py:   def add(a, b): return a + b
来源：http://kie.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jfe.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://ubh.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sfn.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bhi.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://oay.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://yci.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ips.nanxuanxn.top

[C02] 默认参数
来源：http://sma.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://ehq.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pcj.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://qhf.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://obe.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yod.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jlo.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://qfj.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://ncf.yuanzhike.top

[C03] 可变参数
来源：http://ybo.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://vor.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hcb.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pgq.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dcb.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mnt.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rkm.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://jtc.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oyp.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://iss.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://leq.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lan.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cas.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wle.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://glq.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://tnh.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://rkl.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://ciq.xylfe.cn

[C05] 返回多个值
来源：http://sta.nwbrower.top

Py:   return a, b
来源：http://cts.andypj.xyz

PHP:  return [$a, $b];
来源：http://uiz.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vgl.uphjek.com

TS:   return { a, b };
来源：http://vns.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rfl.guannengcc.top

Go:   return a, b
来源：http://jyr.uphjek.com

Ruby: return a, b
来源：http://tap.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://ymb.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://qdp.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://pzv.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sqr.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://fkw.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://bhp.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nqe.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://bge.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://vfo.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://rko.yvedp.cn

[C07] 把函数作为参数传入
来源：http://dqj.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kpy.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kpy.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vtv.gogol.net.cn

TS:   arr.map(String)
来源：http://sec.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dag.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vmf.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://fua.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iwd.smart0.xyz

[C08] 闭包
来源：http://kbk.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vas.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oqz.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vpv.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dbm.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wuc.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nfu.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jyu.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wfm.pengpengdd.cyou

[C09] 递归
来源：http://suc.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xxp.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ugw.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjz.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kgu.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uwl.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://clf.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gjr.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://olo.bbcook.cn

[C10] 变量作用域
来源：http://tiy.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lnb.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hgh.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mnr.feifeiyinyue.top

TS:   同 JS
来源：http://cfh.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://vws.snrcjt.cn

Go:   花括号块级作用域
来源：http://kkh.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://owf.ppjwa.cn

C#:   块级作用域
来源：http://jle.haohaochexian.top

[C11] 模块导入与导出
来源：http://wbg.zycfv.cn

Py:   from module import func
来源：http://ffh.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jtf.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://whz.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://urj.ehwqpu.com

Java: import java.util.List;
来源：http://lmz.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dzh.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://vqr.jianghu66.top

C#:   using System.Text;
来源：http://fba.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://vvx.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://zfg.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://jbi.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://fwt.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://rye.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hke.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://zud.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://cxa.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hry.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://bqh.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ixm.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nrh.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wcy.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pib.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kjl.xuanzx.com

Go:   func add(a, b int) int
来源：http://suj.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yuh.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://obb.fzhhl.top

[C14] 泛型函数
来源：http://uaa.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wgf.tanke756.top

PHP:  // 无泛型
来源：http://eha.daria6918.cn

JS:   // 无泛型
来源：http://muf.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rlx.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vkv.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kvb.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://otb.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tpp.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://vqi.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://brl.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://jwv.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jpv.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tfx.chenlongwang.top

Java: // 无解构
来源：http://vub.pengpengdd.cyou

Go:   // 无解构
来源：http://ldk.zhiwuduotai.top

Ruby: a, b = pair
来源：http://ncy.yfazqb.com

C#:   var (a, b) = pair;
来源：http://jbg.guannengcc.top

[C16] 函数 / 方法重载
来源：http://azr.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://agd.dashuyun.cn

PHP:  // 无重载
来源：http://fyl.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aqj.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://bwc.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://swt.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://fdt.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://swi.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://vno.sjlbkw.cn

================================================================================
来源：http://lid.316326.xyz

D. 数组 / 列表 / 集合
来源：http://qwd.ybcxt.top

================================================================================
来源：http://iio.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://nwe.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://byo.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qgy.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://akg.shanyushiyangtech.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pke.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hee.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://kgh.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://njs.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bon.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://arm.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dlu.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tvr.hywenlv.cn

JS:   arr.push(4);
来源：http://rob.fehbvm.com

TS:   arr.push(4);
来源：http://lro.sufxvd.cn

Java: list.add(4);
来源：http://bdv.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://hdo.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://uow.hnqzz.top

C#:   list.Add(4);
来源：http://hnw.hesvh.cn

[D03] 在指定位置插入元素
来源：http://ivg.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://nnf.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vvh.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cxh.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://xnd.ybcxt.top

Java: list.add(0, 0);
来源：http://gkz.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://wyz.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zth.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://kmd.zhengqikj.top

[D04] 删除元素
来源：http://nfr.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mas.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rne.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://umk.yj20258.top

TS:   arr.splice(0, 1);
来源：http://cuk.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dzm.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eco.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://szq.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bet.zhixingplan.top

[D05] 访问与修改元素
来源：http://yxu.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bya.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://prr.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fuf.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://rqb.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://iva.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://ykt.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xke.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vgo.gzhubu.top

[D06] 数组长度
来源：http://fab.sysykeji.top

Py:   len(arr)
来源：http://lna.hnxiangtu.top

PHP:  count($arr);
来源：http://ujm.hongshengwenyu.top

JS:   arr.length
来源：http://mtr.c1oappe.top

TS:   arr.length
来源：http://wiz.ctjpmb.com

Java: list.size();
来源：http://aur.dianchejie.cn

Go:   len(arr)
来源：http://cfi.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://noc.yangfankeji.com

C#:   list.Count;
来源：http://uws.epnwcf.com

[D07] 切片 / 取子数组
来源：http://yqk.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kqf.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://tlv.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://hqf.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://zwq.fengsongda.top

Java: list.subList(1, 4);
来源：http://kys.yuanzhike.top

Go:   arr[1:4]
来源：http://tpu.c1oappe.top

Ruby: arr[1, 3]
来源：http://ggm.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://ktd.hesvh.cn

[D08] 合并两个数组
来源：http://xzw.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://mfg.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://xhc.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aet.guowangkeji.top

TS:   [...a, ...b];
来源：http://boy.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fka.hnxiangtu.top

Go:   append(a, b...)
来源：http://lth.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://cle.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://qvz.gotoacloud.top

[D09] 排序（升序）
来源：http://hhw.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://uvk.cqqwz.cn

PHP:  sort($arr);
来源：http://erf.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oba.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpw.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hnk.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qry.zhoulong.xyz

Ruby: arr.sort
来源：http://xhk.jiagoushi.top

C#:   list.Sort();
来源：http://abr.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pcs.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uhh.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fhs.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jtk.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsm.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gnn.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vtd.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kcn.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dea.316326.xyz

[D11] 反转数组
来源：http://gkx.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://yyk.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://xzp.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wea.gogol.net.cn

TS:   [...arr].reverse();
来源：http://pyw.gzhubu.top

Java: Collections.reverse(list);
来源：http://rbq.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://vpq.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://qkm.hcnkem.com

C#:   list.Reverse();
来源：http://ulb.hnxiangtu.top

[D12] 查找元素下标
来源：http://poe.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://iiv.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yri.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyi.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ksg.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wai.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://iar.ppjwa.cn

Ruby: arr.index(x)
来源：http://ijd.andypj.xyz

C#:   list.IndexOf(x);
来源：http://atj.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://xdq.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ktp.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kdp.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://jga.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://nut.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eio.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qjn.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ypk.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fcn.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://ptk.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qoi.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vdv.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://gav.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://fcg.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zhd.zhoulong.xyz

Go:   // 手写循环
来源：http://yqg.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://agr.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ink.snrcjt.cn

[D15] 去重
来源：http://nij.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vjy.cucudq.cn

PHP:  array_unique($arr);
来源：http://zhc.xylfe.cn

JS:   [...new Set(arr)]
来源：http://iho.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://dni.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ufe.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://wwx.quarkkingdee.top

Ruby: arr.uniq
来源：http://uex.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://uqv.nanxuanxn.top

[D16] 求和与平均值
来源：http://jtj.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rks.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tlv.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wyv.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hkm.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wwy.guowangkeji.top

Go:   // 手写循环累加
来源：http://hak.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ovq.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://app.shuidangran.top

[D17] 最大值与最小值
来源：http://wsc.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://kak.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://ovb.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fpn.bjfxy.top

TS:   Math.max(...arr);
来源：http://ukd.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eqk.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgw.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://dry.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://rol.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://yjy.ywan-chungtsiang.top


<!-- 参考信息 -->