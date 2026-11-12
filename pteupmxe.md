代发 wailian999

[C02] 默认参数
来源：http://did.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://ugn.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vgo.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://rkb.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jtq.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ltm.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tuo.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://lpe.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://jwn.vehdjk.com

[C03] 可变参数
来源：http://ijq.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://svj.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://axu.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://clk.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xea.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iry.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ifq.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://xph.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ivw.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://bwb.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://acb.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://clo.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mcn.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cow.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://erw.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://pzo.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://cgp.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://znv.jlsjyb.cn

[C05] 返回多个值
来源：http://tjc.zhengqikj.top

Py:   return a, b
来源：http://fnw.zycfv.cn

PHP:  return [$a, $b];
来源：http://zjn.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ail.c1oappe.top

TS:   return { a, b };
来源：http://fuz.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wow.shanyushiyangtech.top

Go:   return a, b
来源：http://fee.aibaodan.cn

Ruby: return a, b
来源：http://rni.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://moh.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://mjw.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://igl.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://usu.ydzc1.top

JS:   const square = x => x * x;
来源：http://wcy.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://kpz.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nry.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://oji.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://eol.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://faw.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://tau.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://elb.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oum.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vha.ppjwa.cn

TS:   arr.map(String)
来源：http://foe.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://inc.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://her.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://drj.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yid.meibo888.top

[C08] 闭包
来源：http://xsq.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ymv.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fqy.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ggj.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lnv.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ekx.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jgm.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://txk.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xvq.hcnkem.com

[C09] 递归
来源：http://eqj.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vwt.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jll.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ioa.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jrs.vehdjk.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kxs.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bag.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uon.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://byh.yongpay.top

[C10] 变量作用域
来源：http://cej.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://shr.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dxy.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qyk.ivvv.top

TS:   同 JS
来源：http://swu.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://ife.sxryk.cn

Go:   花括号块级作用域
来源：http://gmi.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wfw.fanxiaobao.xyz

C#:   块级作用域
来源：http://rlf.daxiang520.top

[C11] 模块导入与导出
来源：http://gao.bbcook.cn

Py:   from module import func
来源：http://cnh.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nur.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lpn.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fbb.hesvh.cn

Java: import java.util.List;
来源：http://doa.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zrm.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://aps.9152youxi.cn

C#:   using System.Text;
来源：http://xgu.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://ukw.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://pfi.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://yra.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://bil.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://owk.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://alh.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://dko.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://yqg.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yqa.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://cix.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pjp.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://asd.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cdj.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ogq.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://mdn.zdqjudy.top

Go:   func add(a, b int) int
来源：http://zsv.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hdr.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://knn.fktsv.cn

[C14] 泛型函数
来源：http://sty.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baf.uphjek.com

PHP:  // 无泛型
来源：http://cfy.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://poj.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://egq.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fzl.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://raz.shzxlz.cn

Ruby: # 无泛型
来源：http://hau.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ctb.yfazqb.com

[C15] 解构 / 展开参数
来源：http://tze.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://act.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://qvk.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ufg.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gyx.cdnleiting.top

Java: // 无解构
来源：http://wbl.zhixingplan.top

Go:   // 无解构
来源：http://vqw.yonumen.top

Ruby: a, b = pair
来源：http://xfe.bjfxy.top

C#:   var (a, b) = pair;
来源：http://weu.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://haf.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://akt.shuidangran.top

PHP:  // 无重载
来源：http://ocy.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mru.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://ita.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ezc.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://zpy.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://jwx.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://web.zycfv.cn

================================================================================
来源：http://atx.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://toc.chenjidiqi.icu

================================================================================
来源：http://mwo.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://jeh.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yvs.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://opi.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xml.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://trw.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mhw.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://iid.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://zif.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://abw.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://pyd.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://grk.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xsk.cheryme.top

JS:   arr.push(4);
来源：http://qlj.c1oappe.top

TS:   arr.push(4);
来源：http://vih.shuidangran.top

Java: list.add(4);
来源：http://six.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://gal.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://vqd.ppjwa.cn

C#:   list.Add(4);
来源：http://lnj.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://yfj.ivvv.top

Py:   arr.insert(0, 0)
来源：http://roc.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ods.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ayz.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://zgm.yfazqb.com

Java: list.add(0, 0);
来源：http://cys.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ndk.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://spx.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://dvp.zhengqikj.top

[D04] 删除元素
来源：http://qzx.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bds.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cpp.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zcr.cheryme.top

TS:   arr.splice(0, 1);
来源：http://dua.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lax.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ikq.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://osh.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://acq.uphjek.com

[D05] 访问与修改元素
来源：http://giw.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://znp.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://llv.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dpe.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://zed.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://qbq.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://vaz.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nue.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sof.hnxiangtu.top

[D06] 数组长度
来源：http://psf.yj20258.top

Py:   len(arr)
来源：http://xpa.havefunace.top

PHP:  count($arr);
来源：http://cxb.smart0.xyz

JS:   arr.length
来源：http://jyf.mhx1999.top

TS:   arr.length
来源：http://mkz.haohaochexian.top

Java: list.size();
来源：http://qbs.uphjek.com

Go:   len(arr)
来源：http://oua.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://qbz.gogol.net.cn

C#:   list.Count;
来源：http://kgt.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://xbh.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fmq.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://zlb.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://kdo.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://hls.gzhubu.top

Java: list.subList(1, 4);
来源：http://dtl.zhiwuduotai.top

Go:   arr[1:4]
来源：http://khj.yangfankeji.com

Ruby: arr[1, 3]
来源：http://vvc.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://djs.zycfv.cn

[D08] 合并两个数组
来源：http://ned.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://poa.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://jop.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tno.yj202588.top

TS:   [...a, ...b];
来源：http://csv.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://foy.jinqigufen.top

Go:   append(a, b...)
来源：http://okh.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://vxi.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://fnx.cashguo.top

[D09] 排序（升序）
来源：http://zyp.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://yzg.gaohongyu789.top

PHP:  sort($arr);
来源：http://mkd.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hui.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fob.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mhd.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tev.aibaodan.cn

Ruby: arr.sort
来源：http://fdn.yj20258888.top

C#:   list.Sort();
来源：http://yrh.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ngy.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://liz.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hgt.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jtd.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hav.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vhd.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bfj.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lfo.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jcu.yj20258888.top

[D11] 反转数组
来源：http://qls.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://imo.tarul.cn

PHP:  array_reverse($arr);
来源：http://gif.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://skc.uphjek.com

TS:   [...arr].reverse();
来源：http://cgh.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://lgu.havefunace.top

Go:   slices.Reverse(arr)
来源：http://gnx.ydzc1.top

Ruby: arr.reverse
来源：http://aqt.redwolf501.top

C#:   list.Reverse();
来源：http://bze.quarkkingdee.top

[D12] 查找元素下标
来源：http://mza.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://jwd.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iyl.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aal.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hxm.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nhx.yangfankeji.com

Go:   slices.Index(arr, x)
来源：http://qfz.kuanghao11.cn

Ruby: arr.index(x)
来源：http://zpe.hesvh.cn

C#:   list.IndexOf(x);
来源：http://mxz.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://aet.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uiy.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fhv.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://dfu.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://usp.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qwu.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tva.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tei.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jyv.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://sgi.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hhy.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sey.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://bsn.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://kct.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hab.ydjk.org.cn

Go:   // 手写循环
来源：http://tyr.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://nys.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vgm.ppjwa.cn

[D15] 去重
来源：http://dot.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fgw.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://nir.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://krd.xziqi.cn

TS:   [...new Set(arr)]
来源：http://qxv.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jxq.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://eal.zhongyouzk.top

Ruby: arr.uniq
来源：http://mjh.yj202588.top

C#:   list.Distinct().ToList()
来源：http://jud.feifeiyinyue.top

[D16] 求和与平均值
来源：http://foq.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://axo.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sph.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mdg.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ehy.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ptt.daria6918.cn

Go:   // 手写循环累加
来源：http://mug.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bfc.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://jmm.uphjek.com

[D17] 最大值与最小值
来源：http://bdn.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://kyz.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://asf.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://awc.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://bfm.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://usr.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nvs.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://zvv.yj202588.top

C#:   list.Max();  list.Min()
来源：http://shi.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://rjg.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://czq.meibo888.top

PHP:  array_merge(...$nested);
来源：http://izp.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kbp.sweek.top

TS:   nested.flat();
来源：http://mmp.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jns.jiagoushi.top

Go:   // 手写双层循环
来源：http://uao.jyoumei.cn

Ruby: nested.flatten
来源：http://xft.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://rvu.ivvv.top


<!-- 参考信息 -->