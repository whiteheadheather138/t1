代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://pbd.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://lkh.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://giw.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cpm.vehdjk.com

[C02] 默认参数
来源：http://hep.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://pww.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lbk.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://vwi.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://smd.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ats.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ijf.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://jvy.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://ywg.gotoacloud.top

[C03] 可变参数
来源：http://xdp.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://uys.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pcr.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xpr.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eqz.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://whd.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://css.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rzv.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pxy.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://iyz.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gek.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ngx.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uga.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hwf.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://xdk.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://tbb.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://tmj.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://cjl.jiagoushi.top

[C05] 返回多个值
来源：http://xha.sufxvd.cn

Py:   return a, b
来源：http://wxi.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://zin.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fpz.0kj1m.cn

TS:   return { a, b };
来源：http://xho.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://moz.ehwqpu.com

Go:   return a, b
来源：http://nwj.chenlongwang.top

Ruby: return a, b
来源：http://dwb.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://ojp.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://cyd.xylfe.cn

Py:   square = lambda x: x * x
来源：http://ojp.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wqm.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://lwz.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://idk.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mad.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jyn.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://zxa.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://rya.cheryme.top

[C07] 把函数作为参数传入
来源：http://nup.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://krz.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hxp.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ayn.jinqigfzy.top

TS:   arr.map(String)
来源：http://azv.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dar.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ddx.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://zky.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sso.yj20258.top

[C08] 闭包
来源：http://jmx.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nao.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uky.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ngl.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hxv.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qyh.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://upg.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cun.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hgp.ppjwa.cn

[C09] 递归
来源：http://eli.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://orj.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tcj.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nxg.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://crj.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xdn.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pjc.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fys.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ezg.bbcook.cn

[C10] 变量作用域
来源：http://tow.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://akv.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://djh.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://odp.sufxvd.cn

TS:   同 JS
来源：http://hrq.iojbl.cn

Java: 方法内为块级作用域
来源：http://qlb.kuanghao11.cn

Go:   花括号块级作用域
来源：http://hoz.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qow.52xcode.cn

C#:   块级作用域
来源：http://zph.vqdsnc.cn

[C11] 模块导入与导出
来源：http://ofe.dianchejie.cn

Py:   from module import func
来源：http://kcj.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tqu.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dpk.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bom.ppjwa.cn

Java: import java.util.List;
来源：http://piy.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://amk.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://lae.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://lnq.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://ygb.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://zgn.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://jql.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://ipm.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://qhm.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fwh.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://fsz.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://gao.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pmr.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://dqh.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gjh.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wuj.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ghj.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ovb.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ipy.nwbrower.top

Go:   func add(a, b int) int
来源：http://dke.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fqe.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://aqh.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://skq.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zcm.xuetiantiany.cn

PHP:  // 无泛型
来源：http://pca.fzhhl.top

JS:   // 无泛型
来源：http://hyf.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uyt.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tsk.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kgc.daxiang520.top

Ruby: # 无泛型
来源：http://ymu.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucv.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://kmk.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://awa.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://taf.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cak.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://msf.jyoumei.cn

Java: // 无解构
来源：http://xwv.xinyue.icu

Go:   // 无解构
来源：http://spo.hysaishi.cn

Ruby: a, b = pair
来源：http://blr.yj202588.top

C#:   var (a, b) = pair;
来源：http://kcc.hnqzz.top

[C16] 函数 / 方法重载
来源：http://wew.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sbg.smart0.xyz

PHP:  // 无重载
来源：http://yex.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lbj.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://nhl.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gus.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://rae.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://jvf.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cfq.feifeiyinyue.top

================================================================================
来源：http://jtm.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://kwz.jqgfzy.top

================================================================================
来源：http://ksr.hcnkem.com

[D01] 创建数组 / 列表
来源：http://ifo.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oad.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qui.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pow.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://arg.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iao.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://kpt.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://wys.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kwq.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://qit.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zqn.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uaa.jqgfzy.top

JS:   arr.push(4);
来源：http://gne.fzhhl.top

TS:   arr.push(4);
来源：http://vow.ybcxt.top

Java: list.add(4);
来源：http://tjm.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://scq.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://qjj.hnqzz.top

C#:   list.Add(4);
来源：http://hkk.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://ezt.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://vmm.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qoj.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rzy.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://xvp.hywenlv.cn

Java: list.add(0, 0);
来源：http://bfa.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://qvb.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://htw.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://lwy.xuanzx.com

[D04] 删除元素
来源：http://ldq.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ean.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hij.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://odh.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://vhu.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://spc.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zul.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eio.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://azt.sjlbkw.cn

[D05] 访问与修改元素
来源：http://wgl.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bpx.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sxv.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fpa.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://mgj.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://xly.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://yau.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://djh.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jxp.ybcxt.top

[D06] 数组长度
来源：http://shs.vehdjk.com

Py:   len(arr)
来源：http://wcs.hammf.cn

PHP:  count($arr);
来源：http://phv.gzhubu.top

JS:   arr.length
来源：http://cuz.daria6918.cn

TS:   arr.length
来源：http://zhh.quarkkingdee.top

Java: list.size();
来源：http://kkw.jlsjyb.cn

Go:   len(arr)
来源：http://aao.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://qyq.zdqjudy.top

C#:   list.Count;
来源：http://uct.xylfe.cn

[D07] 切片 / 取子数组
来源：http://gkq.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://keg.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://flu.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://xnf.pycfn.com

TS:   arr.slice(1, 4);
来源：http://dvw.bjfxy.top

Java: list.subList(1, 4);
来源：http://dut.pengpengdd.cyou

Go:   arr[1:4]
来源：http://mgu.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://njr.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://hih.shuidangran.top

[D08] 合并两个数组
来源：http://iiq.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://rss.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://pgr.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://csc.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://clm.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tbv.cqqwz.cn

Go:   append(a, b...)
来源：http://uzi.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://axu.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://xgb.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://xsh.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://htf.zhongyouzk.top

PHP:  sort($arr);
来源：http://plw.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jje.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xvy.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nri.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gji.wangdashe.top

Ruby: arr.sort
来源：http://vql.ybcxt.top

C#:   list.Sort();
来源：http://ltj.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://ugn.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oze.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://psj.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://skq.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://onw.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ycm.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uib.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mzn.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kxr.yueranfly.top

[D11] 反转数组
来源：http://qzp.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://fjt.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://ikx.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qea.epnwcf.com

TS:   [...arr].reverse();
来源：http://zhm.dianchejie.cn

Java: Collections.reverse(list);
来源：http://rbo.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://odm.pycfn.com

Ruby: arr.reverse
来源：http://blh.aibaodan.cn

C#:   list.Reverse();
来源：http://ble.zdqjudy.top

[D12] 查找元素下标
来源：http://oyv.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://vim.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mtz.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rry.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wle.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hbu.ivvv.top

Go:   slices.Index(arr, x)
来源：http://qzj.yongpay.top

Ruby: arr.index(x)
来源：http://jne.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://fnt.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://wti.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://coa.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bjv.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://cea.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://rsw.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pkg.tianlin.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cpt.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://hjd.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ual.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://bso.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mdu.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zyc.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://yfv.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://gxj.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vaj.chenlongwang.top

Go:   // 手写循环
来源：http://yql.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://gfg.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://cmd.mhx1999.top

[D15] 去重
来源：http://knj.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oqo.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://htp.fehbvm.com

JS:   [...new Set(arr)]
来源：http://hdy.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://sfk.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://llh.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://nre.ydjk.org.cn

Ruby: arr.uniq
来源：http://uin.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://kdw.ctjpmb.com

[D16] 求和与平均值
来源：http://ufx.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zrz.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eyf.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ome.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xge.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wyl.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://afg.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fdy.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://ohr.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://rmg.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://wkl.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://kxd.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jkl.smart0.xyz

TS:   Math.max(...arr);
来源：http://iub.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mof.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ytf.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://lsr.sweek.top

C#:   list.Max();  list.Min()
来源：http://hpr.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://uxk.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eky.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://hgr.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fon.yongpay.top

TS:   nested.flat();
来源：http://edw.xylfe.cn


<!-- 参考信息 -->