代发 wailian999

================================================================================
来源：http://jkh.hfpthk.cn

C. 函数与作用域
来源：http://hjv.cucudq.cn

================================================================================
来源：http://rea.gogol.net.cn

[C01] 定义函数
来源：http://byg.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://noo.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jtq.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://jhb.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lxa.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://klt.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://aca.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://cvm.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ybi.shuidangran.top

[C02] 默认参数
来源：http://bmb.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://clc.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://noz.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://pxm.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mwf.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xwb.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ade.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://xqf.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://sim.jinqigfzy.top

[C03] 可变参数
来源：http://whk.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://gxa.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://plj.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://unt.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqc.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wdm.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ppw.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xjk.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pmz.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://cle.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ezq.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uyy.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ozt.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dqb.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://bsw.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://rss.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://cmo.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://iry.fzhhl.top

[C05] 返回多个值
来源：http://vsu.sufxvd.cn

Py:   return a, b
来源：http://axj.tianlin.xyz

PHP:  return [$a, $b];
来源：http://alh.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gzl.sweek.top

TS:   return { a, b };
来源：http://lph.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eky.jyoumei.cn

Go:   return a, b
来源：http://uwa.shanyushiyangtech.top

Ruby: return a, b
来源：http://mlj.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://eiy.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://uwn.tarul.cn

Py:   square = lambda x: x * x
来源：http://nyw.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tey.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://msa.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://vyr.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mjz.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://mvr.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://xrx.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://kdn.nwbrower.top

[C07] 把函数作为参数传入
来源：http://uix.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baj.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://udz.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://opa.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://ddw.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dsj.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mys.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://xgb.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fsz.ywan-chungtsiang.top

[C08] 闭包
来源：http://due.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lnq.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xem.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ole.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://juk.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ghe.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pwr.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aah.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjp.iojbl.cn

[C09] 递归
来源：http://zsh.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yij.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gbp.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yva.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vfv.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wnk.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bkc.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://klm.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uja.jyoumei.cn

[C10] 变量作用域
来源：http://iem.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hus.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mps.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://syb.ppjwa.cn

TS:   同 JS
来源：http://hyk.meibo888.top

Java: 方法内为块级作用域
来源：http://lvf.havefunace.top

Go:   花括号块级作用域
来源：http://ysw.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tjj.hfpthk.cn

C#:   块级作用域
来源：http://sad.chenlongwang.top

[C11] 模块导入与导出
来源：http://pev.fzhhl.top

Py:   from module import func
来源：http://pgv.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://szj.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tsp.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mkm.shanyushiyangtech.top

Java: import java.util.List;
来源：http://mkj.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nja.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://lci.fehbvm.com

C#:   using System.Text;
来源：http://nlp.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://cie.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://ayo.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://jel.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://unw.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://zdg.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dru.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://nkv.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://euy.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://etq.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://zpl.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dyf.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ahj.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iyo.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mvn.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ert.ybcxt.top

Go:   func add(a, b int) int
来源：http://rss.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yps.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://nur.shuidangran.top

[C14] 泛型函数
来源：http://lui.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pkm.cqqwz.cn

PHP:  // 无泛型
来源：http://als.hongshengwenyu.top

JS:   // 无泛型
来源：http://kkm.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://htb.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vxb.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://som.yvedp.cn

Ruby: # 无泛型
来源：http://ixn.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fmh.yonumen.top

[C15] 解构 / 展开参数
来源：http://mwi.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xuk.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://koj.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ofv.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ebc.chenjidiqi.icu

Java: // 无解构
来源：http://nnq.chenzaomai.com

Go:   // 无解构
来源：http://vkg.vehdjk.com

Ruby: a, b = pair
来源：http://vio.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://quw.jianghu66.top

[C16] 函数 / 方法重载
来源：http://fyx.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eel.ivvv.top

PHP:  // 无重载
来源：http://nby.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://lap.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://dgo.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bnv.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://gyb.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://ljj.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jez.wangshuangyany.cn

================================================================================
来源：http://wku.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://zel.sxryk.cn

================================================================================
来源：http://uvh.yj202588.top

[D01] 创建数组 / 列表
来源：http://ixe.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wvw.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iqd.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://coc.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vuh.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bth.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://tuz.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://ujt.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hfr.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://uia.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ysu.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fxq.daria6918.cn

JS:   arr.push(4);
来源：http://xdr.zhoulong.xyz

TS:   arr.push(4);
来源：http://tza.fengsongda.top

Java: list.add(4);
来源：http://gtb.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://yeg.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://wff.ydzc1.top

C#:   list.Add(4);
来源：http://ndn.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://owj.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://sni.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zzr.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hdk.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://ouf.dianchejie.cn

Java: list.add(0, 0);
来源：http://ojx.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://hwl.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lmu.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://emz.tarul.cn

[D04] 删除元素
来源：http://kry.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ogz.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tbg.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vwn.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://fmz.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xiy.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bxe.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jul.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hzz.jianghu66.top

[D05] 访问与修改元素
来源：http://xok.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pts.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rwn.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yjn.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://tjb.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://yyv.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://pmo.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qnb.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vqw.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://obc.yueranfly.top

Py:   len(arr)
来源：http://lrf.c1oappe.top

PHP:  count($arr);
来源：http://xsb.vqdsnc.cn

JS:   arr.length
来源：http://sij.yfazqb.com

TS:   arr.length
来源：http://xkc.ivvv.top

Java: list.size();
来源：http://fwa.bbcook.cn

Go:   len(arr)
来源：http://fhb.52xcode.cn

Ruby: arr.length; arr.size
来源：http://jpl.hnxiangtu.top

C#:   list.Count;
来源：http://moy.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://mji.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tew.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://stg.yongpay.top

JS:   arr.slice(1, 4);
来源：http://nud.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://akb.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://gch.pengpengdd.cyou

Go:   arr[1:4]
来源：http://gcd.zhengqikj.top

Ruby: arr[1, 3]
来源：http://vwr.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://xlk.jinqigfzy.top

[D08] 合并两个数组
来源：http://hwq.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://sgk.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://fpj.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ijz.chenzaomai.com

TS:   [...a, ...b];
来源：http://cou.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ulu.zhongyouzk.top

Go:   append(a, b...)
来源：http://qlr.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://cfj.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://qvn.fzhhl.top

[D09] 排序（升序）
来源：http://imr.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://sky.ydjk.org.cn

PHP:  sort($arr);
来源：http://sbm.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ipd.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wxd.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://txv.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qlr.guowangkeji.top

Ruby: arr.sort
来源：http://jlj.xziqi.cn

C#:   list.Sort();
来源：http://oax.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bnn.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vkn.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cro.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qci.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfy.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hhw.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rkf.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tqo.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mie.jinqigfzy.top

[D11] 反转数组
来源：http://ahx.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://jei.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://izh.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jkr.cashguo.top

TS:   [...arr].reverse();
来源：http://jtk.ppjwa.cn

Java: Collections.reverse(list);
来源：http://jbu.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://rdm.nanxinkj.top

Ruby: arr.reverse
来源：http://gre.9152youxi.cn

C#:   list.Reverse();
来源：http://jml.hywenlv.cn

[D12] 查找元素下标
来源：http://ycg.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://lia.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hgy.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqq.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lfk.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ymh.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://hia.sweek.top

Ruby: arr.index(x)
来源：http://riu.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://mkw.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://mzh.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ihk.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ocl.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://ygi.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://vyg.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://asn.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ptm.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://bcf.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://eqa.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://mjc.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xlz.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://grq.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://yjv.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://tpp.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gym.yonumen.top

Go:   // 手写循环
来源：http://gvh.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bmr.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jau.fehbvm.com

[D15] 去重
来源：http://afr.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rdq.hywenlv.cn

PHP:  array_unique($arr);
来源：http://euh.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://kxo.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://tnk.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://psx.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://hko.yuanzhike.top

Ruby: arr.uniq
来源：http://xna.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://gsz.hywenlv.cn

[D16] 求和与平均值
来源：http://ipf.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jap.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://brh.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qkk.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gpz.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvh.jianghu66.top

Go:   // 手写循环累加
来源：http://svw.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bjj.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://fsj.zhijiandao.cn

[D17] 最大值与最小值
来源：http://tqf.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://hub.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://kxq.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ise.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://bdu.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://tja.yonumen.top


<!-- 参考信息 -->