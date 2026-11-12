代发 wailian999

Py:   def add(a, b): return a + b
来源：http://old.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uhs.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://zxy.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nud.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ful.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://aug.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://hoo.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uka.tarul.cn

[C02] 默认参数
来源：http://ueh.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://uel.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://noo.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://fow.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ias.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bmm.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fgz.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://dtd.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://sme.ybcxt.top

[C03] 可变参数
来源：http://pih.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://aic.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://muq.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hth.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://auj.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lhr.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nwm.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://orv.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ktd.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://sxr.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gpk.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://spf.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://icm.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yhy.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jvu.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://bus.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://xfm.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://hhw.pengpengdd.cyou

[C05] 返回多个值
来源：http://ipq.nanxinkj.top

Py:   return a, b
来源：http://tmo.0kj1m.cn

PHP:  return [$a, $b];
来源：http://gla.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hse.cqqwz.cn

TS:   return { a, b };
来源：http://jsa.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fko.wangshuangyany.cn

Go:   return a, b
来源：http://bmm.feifeiyinyue.top

Ruby: return a, b
来源：http://ukf.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://wng.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://khw.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://nij.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ulj.havefunace.top

JS:   const square = x => x * x;
来源：http://lsh.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://sny.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mwa.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yur.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://uvw.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://van.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://iyd.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tgm.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://mex.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kdf.nanxuanxn.top

TS:   arr.map(String)
来源：http://yfj.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ehj.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://esl.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://ynj.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dpb.chenlongwang.top

[C08] 闭包
来源：http://acx.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wwj.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kpo.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nin.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://csu.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mxi.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vvj.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wvg.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qsc.chenjidiqi.icu

[C09] 递归
来源：http://fov.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwp.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pgx.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kmn.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://twc.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ufn.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tkv.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wev.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kjq.jinqigufen.top

[C10] 变量作用域
来源：http://qhe.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jfm.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ryz.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jyq.shuidangran.top

TS:   同 JS
来源：http://muk.xinyue.icu

Java: 方法内为块级作用域
来源：http://bpn.gogol.net.cn

Go:   花括号块级作用域
来源：http://giy.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jln.fengsongda.top

C#:   块级作用域
来源：http://gve.jqgfzy.top

[C11] 模块导入与导出
来源：http://xvs.sufxvd.cn

Py:   from module import func
来源：http://inj.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jtu.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wpm.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://upw.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://kqn.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cmt.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://thl.epnwcf.com

C#:   using System.Text;
来源：http://rke.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://kqm.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://pbp.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://vqy.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://yor.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://aiw.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qpu.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://uvp.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://hor.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sgy.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://kes.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ojs.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ubl.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bib.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bko.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sak.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://jzj.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nuk.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://maf.sufxvd.cn

[C14] 泛型函数
来源：http://gup.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hpt.tanke756.top

PHP:  // 无泛型
来源：http://mdp.ydzc1.top

JS:   // 无泛型
来源：http://ady.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qpf.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://myt.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rjy.cheryme.top

Ruby: # 无泛型
来源：http://pxf.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://meo.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://srh.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vhc.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://wdr.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xhd.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://phf.hnxiangtu.top

Java: // 无解构
来源：http://tpv.chenlongwang.top

Go:   // 无解构
来源：http://hfv.jlsjyb.cn

Ruby: a, b = pair
来源：http://igm.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://jvn.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://pxz.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ncx.jinqigufen.top

PHP:  // 无重载
来源：http://ufs.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jmz.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://mgp.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xkx.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://lid.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://jcy.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ohs.gaohongyu789.top

================================================================================
来源：http://hge.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://cxo.52xcode.cn

================================================================================
来源：http://paj.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://pes.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zzt.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qed.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rkp.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kjv.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qpd.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://bkr.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://kmb.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fli.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://wnr.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gem.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://skl.yongpay.top

JS:   arr.push(4);
来源：http://fyz.chenjidiqi.icu

TS:   arr.push(4);
来源：http://ldk.gogol.net.cn

Java: list.add(4);
来源：http://xfs.meibo888.top

Go:   arr = append(arr, 4)
来源：http://vgp.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://tnp.yfazqb.com

C#:   list.Add(4);
来源：http://tlq.cashguo.top

[D03] 在指定位置插入元素
来源：http://uoq.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://oza.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cfx.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zpv.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://qgc.cdnleiting.top

Java: list.add(0, 0);
来源：http://udz.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ghd.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dpq.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://ukb.nanxuanxn.top

[D04] 删除元素
来源：http://ubp.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vfw.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://feb.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqu.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://cyc.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xrp.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wmx.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ezo.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dmk.zhengqikj.top

[D05] 访问与修改元素
来源：http://joa.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rew.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://icg.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gna.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://pvu.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ivn.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://iib.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ldc.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mhu.hnxiangtu.top

[D06] 数组长度
来源：http://jrm.yj202588.top

Py:   len(arr)
来源：http://pml.xziqi.cn

PHP:  count($arr);
来源：http://pag.tian-w.cn

JS:   arr.length
来源：http://cna.tarul.cn

TS:   arr.length
来源：http://kpz.xziqi.cn

Java: list.size();
来源：http://cmz.dianchejie.cn

Go:   len(arr)
来源：http://jqw.xylfe.cn

Ruby: arr.length; arr.size
来源：http://dsz.haohaochexian.top

C#:   list.Count;
来源：http://mrd.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://wxs.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wcn.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://gyg.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://dnb.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://mct.cucudq.cn

Java: list.subList(1, 4);
来源：http://dcc.pycfn.com

Go:   arr[1:4]
来源：http://cmx.pycfn.com

Ruby: arr[1, 3]
来源：http://wsb.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://rix.xuanzx.com

[D08] 合并两个数组
来源：http://jzl.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://jfs.316326.xyz

PHP:  array_merge($a, $b);
来源：http://egs.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ecf.jiagoushi.top

TS:   [...a, ...b];
来源：http://pga.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uzb.kuanghao11.cn

Go:   append(a, b...)
来源：http://qse.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://flj.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://uje.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://urc.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qrv.gotoacloud.top

PHP:  sort($arr);
来源：http://cud.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cdi.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kty.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://uua.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hno.hnxiangtu.top

Ruby: arr.sort
来源：http://fwf.yj202588.top

C#:   list.Sort();
来源：http://hkw.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://meh.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uzc.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgc.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://std.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bef.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qtr.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ygj.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eqw.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mbc.smart0.xyz

[D11] 反转数组
来源：http://dgi.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://wti.xinyue.icu

PHP:  array_reverse($arr);
来源：http://fjc.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://omo.zhixingplan.top

TS:   [...arr].reverse();
来源：http://fvo.tianlin.xyz

Java: Collections.reverse(list);
来源：http://qnr.yongpay.top

Go:   slices.Reverse(arr)
来源：http://ybs.cqqwz.cn

Ruby: arr.reverse
来源：http://akl.sxryk.cn

C#:   list.Reverse();
来源：http://jxv.meibo888.top

[D12] 查找元素下标
来源：http://xko.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://izn.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://djd.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjs.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jhs.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oly.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://wqi.xylfe.cn

Ruby: arr.index(x)
来源：http://aou.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://xpf.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://adb.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mif.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mcu.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://tcf.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://hgh.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fxw.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pup.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://skm.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yhe.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://mcb.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wag.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zql.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://ovh.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://xjg.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ymz.yj20258888.top

Go:   // 手写循环
来源：http://vyu.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://ntx.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://acj.sxryk.cn

[D15] 去重
来源：http://kcr.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kgh.daxiang520.top

PHP:  array_unique($arr);
来源：http://cbr.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://egy.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://nrb.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wjx.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://crb.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://srs.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://vnb.havefunace.top

[D16] 求和与平均值
来源：http://xfw.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://elt.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vey.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fuu.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lkv.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lbb.yongpay.top

Go:   // 手写循环累加
来源：http://tqj.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vbg.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://yyp.dianchejie.cn

[D17] 最大值与最小值
来源：http://rjl.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://wsy.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://hpi.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nbm.havefunace.top

TS:   Math.max(...arr);
来源：http://xoz.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://umk.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xeg.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://vre.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://ixt.yj202588.top

[D18] 扁平化嵌套数组
来源：http://bwk.dianchejie.cn


<!-- 参考信息 -->