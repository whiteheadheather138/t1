代发 wailian999

Py:   def add(a, b): return a + b
来源：http://qic.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lfm.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://vaw.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ocw.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qqm.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mim.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://tti.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jry.yueranfly.top

[C02] 默认参数
来源：http://rci.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://nzv.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cao.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://njk.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cci.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fyd.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fxn.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://pxm.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://ofv.birdmap.top

[C03] 可变参数
来源：http://gfw.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://ixk.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kfl.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iph.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ldf.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yzm.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ydr.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xpx.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xjf.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://yop.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zpz.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dnn.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kkq.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yjj.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://pel.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://cmy.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://ylh.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://gnb.kuanghao11.cn

[C05] 返回多个值
来源：http://phs.feifeiyinyue.top

Py:   return a, b
来源：http://blv.zycfv.cn

PHP:  return [$a, $b];
来源：http://tfx.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://amx.shzxlz.cn

TS:   return { a, b };
来源：http://wwi.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gdp.xuanzx.com

Go:   return a, b
来源：http://ixq.mhx1999.top

Ruby: return a, b
来源：http://jky.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://jrh.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://wxn.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://hwz.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kvp.fzhhl.top

JS:   const square = x => x * x;
来源：http://pcn.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://qcz.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wbp.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://cue.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://czg.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://rcx.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://gkq.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jzs.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://xqx.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://idc.sweek.top

TS:   arr.map(String)
来源：http://tuc.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vcc.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdr.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://jrk.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bag.hnqzz.top

[C08] 闭包
来源：http://uii.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jjr.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lcc.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://riq.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msw.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xwc.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nhf.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vac.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://frw.tianlin.xyz

[C09] 递归
来源：http://wmk.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ozr.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bxq.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofm.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dph.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yxb.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pwp.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://szr.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qqt.jianghu66.top

[C10] 变量作用域
来源：http://fbh.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://adm.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mlr.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qon.zhengqikj.top

TS:   同 JS
来源：http://ash.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://xet.jiagoushi.top

Go:   花括号块级作用域
来源：http://kuy.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cdt.aizwys.cn

C#:   块级作用域
来源：http://nck.zhijiandao.cn

[C11] 模块导入与导出
来源：http://shi.wangdashe.top

Py:   from module import func
来源：http://hkt.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dop.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nuh.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wuo.hongshengwenyu.top

Java: import java.util.List;
来源：http://fmi.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yqk.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://mqc.bjfxy.top

C#:   using System.Text;
来源：http://tcz.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://ibb.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://pmo.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://hbm.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://svh.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://vaj.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dwx.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://jxm.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://wqr.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://btb.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://scg.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jbq.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dic.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kkr.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsl.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://lih.yueranfly.top

Go:   func add(a, b int) int
来源：http://yee.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://onx.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://jcr.yuxming.cn

[C14] 泛型函数
来源：http://bij.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zzk.nanxinkj.top

PHP:  // 无泛型
来源：http://zxr.yuanzhike.top

JS:   // 无泛型
来源：http://tut.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pww.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xvj.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hzb.wangshuangyany.cn

Ruby: # 无泛型
来源：http://hxo.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aez.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://ktn.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eed.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://low.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zqv.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://neh.xziqi.cn

Java: // 无解构
来源：http://whv.cdnleiting.top

Go:   // 无解构
来源：http://aey.ctjpmb.com

Ruby: a, b = pair
来源：http://xiy.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://lak.hcnkem.com

[C16] 函数 / 方法重载
来源：http://xdf.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://afx.zhijiandao.cn

PHP:  // 无重载
来源：http://rfd.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://qbf.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://baq.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lpb.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://ccj.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://wsa.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gpz.jinqigufen.top

================================================================================
来源：http://yxo.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://dab.guannengcc.top

================================================================================
来源：http://qhh.316326.xyz

[D01] 创建数组 / 列表
来源：http://jml.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dts.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xnh.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qos.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vnf.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://usw.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://pqp.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://mkk.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://otl.ivvv.top

[D02] 追加元素到末尾
来源：http://zsd.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ikm.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://trg.yongpay.top

JS:   arr.push(4);
来源：http://flk.uphjek.com

TS:   arr.push(4);
来源：http://rna.9152youxi.cn

Java: list.add(4);
来源：http://ikz.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://ymx.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://qbe.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://ciu.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://zzd.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://szs.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rsb.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aqt.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://oui.yonumen.top

Java: list.add(0, 0);
来源：http://afa.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hjy.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cnl.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://nxt.jinqigfzy.top

[D04] 删除元素
来源：http://ene.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fjo.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://roy.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zci.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://cwy.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zsl.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pkq.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lpw.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blj.sjlbkw.cn

[D05] 访问与修改元素
来源：http://aha.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jos.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zjd.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://coo.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://lgr.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://pnv.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://ygx.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eoy.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qma.zhaomingkeji.xyz

[D06] 数组长度
来源：http://box.ppjwa.cn

Py:   len(arr)
来源：http://izg.mhx1999.top

PHP:  count($arr);
来源：http://arb.fehbvm.com

JS:   arr.length
来源：http://tbt.jyoumei.cn

TS:   arr.length
来源：http://vvf.aibaodan.cn

Java: list.size();
来源：http://oyj.epnwcf.com

Go:   len(arr)
来源：http://pbf.yonumen.top

Ruby: arr.length; arr.size
来源：http://suu.jlsjyb.cn

C#:   list.Count;
来源：http://hjf.hnqzz.top

[D07] 切片 / 取子数组
来源：http://cjp.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zry.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://uyb.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://lwf.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://ram.cdnleiting.top

Java: list.subList(1, 4);
来源：http://itl.sjlbkw.cn

Go:   arr[1:4]
来源：http://yqr.sxryk.cn

Ruby: arr[1, 3]
来源：http://nhl.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://ktb.nanxuanxn.top

[D08] 合并两个数组
来源：http://lkw.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://ubi.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://rpq.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qos.jiagoushi.top

TS:   [...a, ...b];
来源：http://lmi.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nvy.sxryk.cn

Go:   append(a, b...)
来源：http://hfi.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://gdk.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://sis.jlsjyb.cn

[D09] 排序（升序）
来源：http://eep.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://mjh.hcnkem.com

PHP:  sort($arr);
来源：http://mgb.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tcq.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://omv.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cge.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rgf.andypj.xyz

Ruby: arr.sort
来源：http://kpv.zycfv.cn

C#:   list.Sort();
来源：http://aoa.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sda.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gpa.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cui.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://exh.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gjg.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wlu.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vcl.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zsw.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://scw.jinqigfzy.top

[D11] 反转数组
来源：http://lza.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://khy.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://rug.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dan.sweek.top

TS:   [...arr].reverse();
来源：http://xqj.tian-w.cn

Java: Collections.reverse(list);
来源：http://ljc.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://rji.yvedp.cn

Ruby: arr.reverse
来源：http://bhd.jqgfzy.top

C#:   list.Reverse();
来源：http://gbx.hnxiangtu.top

[D12] 查找元素下标
来源：http://okn.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://mwr.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kfg.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfj.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnk.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lsj.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://ncn.gogol.net.cn

Ruby: arr.index(x)
来源：http://hew.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://qrq.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://yvh.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gft.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zym.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://uzh.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://bim.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tdk.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lsk.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rkq.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://niu.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://jyx.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exe.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jix.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://pqy.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://zde.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://boi.shanyushiyangtech.top

Go:   // 手写循环
来源：http://mon.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://vvw.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://etf.vehdjk.com

[D15] 去重
来源：http://izs.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tpa.hywenlv.cn

PHP:  array_unique($arr);
来源：http://oew.vehdjk.com

JS:   [...new Set(arr)]
来源：http://whh.ivvv.top

TS:   [...new Set(arr)]
来源：http://nac.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://exu.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yxi.xinyue.icu

Ruby: arr.uniq
来源：http://pea.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://ite.smart0.xyz

[D16] 求和与平均值
来源：http://frr.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uqm.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dys.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dtj.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bbr.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qmy.jlsjyb.cn

Go:   // 手写循环累加
来源：http://iac.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bhx.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://ghn.yj202588.top

[D17] 最大值与最小值
来源：http://akp.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://cco.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://jxt.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pbx.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://yku.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bbf.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wul.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://hpe.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://kxr.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://foj.zdbjq.cn


<!-- 参考信息 -->