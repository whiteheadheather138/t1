代发 wailian999

Java: if (data == null) return;
来源：http://ebc.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://okd.xziqi.cn

Ruby: return if data.nil?
来源：http://elu.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://hyx.feifeiyinyue.top

================================================================================
来源：http://cdl.bbcook.cn

C. 函数与作用域
来源：http://afk.xylfe.cn

================================================================================
来源：http://fig.hcnkem.com

[C01] 定义函数
来源：http://zoi.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://aid.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hnk.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://gcs.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://avx.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hqs.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://cpx.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://zml.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpy.sxryk.cn

[C02] 默认参数
来源：http://rdw.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://qsa.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rsd.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://ncs.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hms.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oiw.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aee.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://vtg.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://roh.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://kvy.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://xqj.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bya.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vmd.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lit.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://olh.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cis.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jln.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fra.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://ggz.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://irz.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://doz.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cap.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hxk.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://prz.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://hkj.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://kvk.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://iob.tanke756.top

[C05] 返回多个值
来源：http://iux.uphjek.com

Py:   return a, b
来源：http://mur.havefunace.top

PHP:  return [$a, $b];
来源：http://hsb.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nsf.zdbjq.cn

TS:   return { a, b };
来源：http://sxg.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bjz.xuanzx.com

Go:   return a, b
来源：http://rfx.vehdjk.com

Ruby: return a, b
来源：http://erd.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://njg.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://ark.guannengcc.top

Py:   square = lambda x: x * x
来源：http://hud.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ykv.jqgfzy.top

JS:   const square = x => x * x;
来源：http://fsg.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://miy.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uxy.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wyt.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://gwj.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mdy.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://lps.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://syh.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://lgh.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dhd.quarkkingdee.top

TS:   arr.map(String)
来源：http://txr.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pxk.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wqt.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://vyl.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://zht.jyoumei.cn

[C08] 闭包
来源：http://smh.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jba.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jvj.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xaz.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xdp.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://abs.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yod.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jua.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://okp.jqgfzy.top

[C09] 递归
来源：http://oay.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://muw.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sgq.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gye.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cme.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hjp.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gnj.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gfm.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ocx.hcnkem.com

[C10] 变量作用域
来源：http://wcf.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aub.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mfm.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xxk.tanke756.top

TS:   同 JS
来源：http://pan.haohaochexian.top

Java: 方法内为块级作用域
来源：http://srw.birdmap.top

Go:   花括号块级作用域
来源：http://oto.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://knu.yuxming.cn

C#:   块级作用域
来源：http://rxs.zdqjudy.top

[C11] 模块导入与导出
来源：http://fby.9152youxi.cn

Py:   from module import func
来源：http://qhy.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://djy.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rqq.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jdz.kuanghao11.cn

Java: import java.util.List;
来源：http://ult.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yit.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://yqz.nanxinkj.top

C#:   using System.Text;
来源：http://pba.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://htg.yj20258.top

Py:   (lambda: print("run"))()
来源：http://qrd.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://eef.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://gfb.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://dxj.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tsm.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://rfu.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://wxm.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://mxa.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://xjv.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iyq.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qof.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fqm.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pxw.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://tup.sweek.top

Go:   func add(a, b int) int
来源：http://vtb.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kvo.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://bqt.sjlbkw.cn

[C14] 泛型函数
来源：http://dbj.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://djj.shangyingyoupin.top

PHP:  // 无泛型
来源：http://odj.hfpthk.cn

JS:   // 无泛型
来源：http://tds.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://orl.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hgg.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://smu.dashuyun.cn

Ruby: # 无泛型
来源：http://wmd.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nev.nwbrower.top

[C15] 解构 / 展开参数
来源：http://tfl.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://kdw.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vlf.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lan.cdnleiting.top

Java: // 无解构
来源：http://dcq.dashuyun.cn

Go:   // 无解构
来源：http://ovz.meibo888.top

Ruby: a, b = pair
来源：http://zby.shuidangran.top

C#:   var (a, b) = pair;
来源：http://nkc.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://gxt.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lhc.feifeiyinyue.top

PHP:  // 无重载
来源：http://lls.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://soh.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://yza.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://sjk.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://clp.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://qce.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vfu.hammf.cn

================================================================================
来源：http://qup.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://ucl.shuidangran.top

================================================================================
来源：http://vcu.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://ydz.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hrq.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yov.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tvo.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jkr.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rgr.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://msj.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://stq.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iqx.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://tvk.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pyb.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://olt.ehwqpu.com

JS:   arr.push(4);
来源：http://vcm.yvedp.cn

TS:   arr.push(4);
来源：http://ruw.meibo888.top

Java: list.add(4);
来源：http://kgy.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://tlb.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://sls.sysykeji.top

C#:   list.Add(4);
来源：http://xsz.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://nud.cashguo.top

Py:   arr.insert(0, 0)
来源：http://xcr.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lnb.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lvc.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://nax.hfpthk.cn

Java: list.add(0, 0);
来源：http://lht.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pok.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qst.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://rzl.hongshengwenyu.top

[D04] 删除元素
来源：http://fov.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gvj.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iyc.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://etx.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://ikz.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cue.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://imx.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gic.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zli.ctjpmb.com

[D05] 访问与修改元素
来源：http://oua.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tid.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fof.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xdu.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://nwa.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://fjb.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://wrs.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zba.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pif.gaohongyu789.top

[D06] 数组长度
来源：http://wtk.tanke756.top

Py:   len(arr)
来源：http://sif.uphjek.com

PHP:  count($arr);
来源：http://eyi.ydzc1.top

JS:   arr.length
来源：http://ect.ehwqpu.com

TS:   arr.length
来源：http://foa.sufxvd.cn

Java: list.size();
来源：http://mxa.cashguo.top

Go:   len(arr)
来源：http://ccr.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://unl.zhengqikj.top

C#:   list.Count;
来源：http://apb.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://ulf.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aoj.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sdp.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://ptu.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://iev.hnqzz.top

Java: list.subList(1, 4);
来源：http://hqa.gogol.net.cn

Go:   arr[1:4]
来源：http://cnu.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://rby.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://ayt.yfazqb.com

[D08] 合并两个数组
来源：http://ola.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://vyv.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://gug.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ihv.zycfv.cn

TS:   [...a, ...b];
来源：http://zob.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ufd.ehwqpu.com

Go:   append(a, b...)
来源：http://glu.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://xni.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://awk.ivvv.top

[D09] 排序（升序）
来源：http://fyk.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://paw.yuxming.cn

PHP:  sort($arr);
来源：http://lsf.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jms.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tnm.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rhe.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pwi.fehbvm.com

Ruby: arr.sort
来源：http://khu.gaohongyu789.top

C#:   list.Sort();
来源：http://uec.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://baz.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://udl.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://luz.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jyo.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fpg.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzm.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipj.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hrk.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tnh.c1oappe.top

[D11] 反转数组
来源：http://npy.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://avf.havefunace.top

PHP:  array_reverse($arr);
来源：http://aai.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zbw.hesvh.cn

TS:   [...arr].reverse();
来源：http://hsk.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://wsz.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://nfi.havefunace.top

Ruby: arr.reverse
来源：http://dii.fzhhl.top

C#:   list.Reverse();
来源：http://lqf.wangdashe.top

[D12] 查找元素下标
来源：http://vya.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://rnd.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iud.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nih.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nhv.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifx.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://vdi.ivvv.top

Ruby: arr.index(x)
来源：http://kom.316326.xyz

C#:   list.IndexOf(x);
来源：http://hdw.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://qol.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wea.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jwa.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://tbk.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://rws.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://apx.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rrp.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://ztf.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vnx.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://emh.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uwr.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://voy.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://nai.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://whz.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ceh.jlsjyb.cn

Go:   // 手写循环
来源：http://yte.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://kzj.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mqs.zdbjq.cn

[D15] 去重
来源：http://vlj.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gfh.cheryme.top

PHP:  array_unique($arr);
来源：http://qnk.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://ghi.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://cof.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://arx.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://igq.meibo888.top

Ruby: arr.uniq
来源：http://jby.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://jyu.shuidangran.top

[D16] 求和与平均值
来源：http://kbn.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hgn.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xuq.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cqj.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxi.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ieu.ybcxt.top

Go:   // 手写循环累加
来源：http://xyv.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nsv.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://vvm.hnxiangtu.top

[D17] 最大值与最小值
来源：http://mrs.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://yha.xuetiantiany.cn


<!-- 参考信息 -->