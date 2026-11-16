代发 wailian999

================================================================================
来源：http://yzw.zhaomingkeji.xyz

C. 函数与作用域
来源：http://rah.chenlongwang.top

================================================================================
来源：http://zda.zdqjudy.top

[C01] 定义函数
来源：http://gpj.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://uba.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cbh.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://fam.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aoo.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ivq.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://msm.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://zcb.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qev.fehbvm.com

[C02] 默认参数
来源：http://yjx.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://lay.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qzm.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://rkf.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rxz.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cwl.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qzs.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://yxi.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://fzs.yongpay.top

[C03] 可变参数
来源：http://cbv.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://wde.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lrn.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kaf.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://avs.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bym.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cpf.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://byw.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://osi.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://gjk.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bfa.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://icx.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uyv.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ufu.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://rdh.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://lct.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://kjy.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://tgz.haohaochexian.top

[C05] 返回多个值
来源：http://qwr.hywenlv.cn

Py:   return a, b
来源：http://wpq.havefunace.top

PHP:  return [$a, $b];
来源：http://xsq.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://imr.shzxlz.cn

TS:   return { a, b };
来源：http://ear.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://grr.mhx1999.top

Go:   return a, b
来源：http://nbp.cashguo.top

Ruby: return a, b
来源：http://sxl.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://dft.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://ijq.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://zvp.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qxq.ybcxt.top

JS:   const square = x => x * x;
来源：http://wgw.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://jef.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cdp.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://gwx.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://qzh.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://eez.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://uat.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dcm.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://sii.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://img.gaohongyu789.top

TS:   arr.map(String)
来源：http://tdc.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://naa.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rja.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://qxx.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://env.yuanzhike.top

[C08] 闭包
来源：http://dxt.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uno.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mxg.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pdj.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eij.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rpe.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lab.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ius.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zjm.xingfuxueyuan.xyz

[C09] 递归
来源：http://auj.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bpd.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nfy.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jno.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vdq.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qju.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mlz.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oqh.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://upf.hywenlv.cn

[C10] 变量作用域
来源：http://xcd.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vjj.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pqr.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://usp.cucudq.cn

TS:   同 JS
来源：http://hit.cashguo.top

Java: 方法内为块级作用域
来源：http://qpp.svipenyu.cn

Go:   花括号块级作用域
来源：http://lvq.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zyw.zhengqikj.top

C#:   块级作用域
来源：http://wwf.hysaishi.cn

[C11] 模块导入与导出
来源：http://lnt.yongpay.top

Py:   from module import func
来源：http://iub.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://dcj.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://opr.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mgn.yj20258888.top

Java: import java.util.List;
来源：http://gnw.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fmt.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://gjg.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://fys.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://avf.yj202588.top

Py:   (lambda: print("run"))()
来源：http://ygo.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://cfu.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://wdg.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://mdu.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oik.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://enk.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://iay.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cff.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://zmi.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dzs.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ctf.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tfy.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://koi.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dbl.haohaochexian.top

Go:   func add(a, b int) int
来源：http://yjo.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vfw.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hnu.redwolf501.top

[C14] 泛型函数
来源：http://chi.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ilr.ydzc1.top

PHP:  // 无泛型
来源：http://nrg.yj202588.top

JS:   // 无泛型
来源：http://gvk.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yxt.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oog.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cuy.yuanzhike.top

Ruby: # 无泛型
来源：http://bwv.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oxh.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://eyd.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tff.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://zzq.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ipz.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rxd.sweek.top

Java: // 无解构
来源：http://pac.wangshuangyany.cn

Go:   // 无解构
来源：http://ill.zdbjq.cn

Ruby: a, b = pair
来源：http://dky.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://dtv.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://qni.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jqi.jqgufenzy.top

PHP:  // 无重载
来源：http://tdh.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jca.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://hta.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bdx.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://sxw.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://gug.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zuy.zhiwuduotai.top

================================================================================
来源：http://qfw.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://fbc.52xcode.cn

================================================================================
来源：http://fhy.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://xcg.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ihu.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://muj.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://abn.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nrk.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fmb.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://mcs.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://aoy.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bgr.ctjpmb.com

[D02] 追加元素到末尾
来源：http://kkt.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dpp.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ind.birdmap.top

JS:   arr.push(4);
来源：http://feb.gaohongyu789.top

TS:   arr.push(4);
来源：http://oxk.cheryme.top

Java: list.add(4);
来源：http://hzb.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://yrx.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://opc.dashuyun.cn

C#:   list.Add(4);
来源：http://vbk.aizwys.cn

[D03] 在指定位置插入元素
来源：http://ydd.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://rrq.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dsp.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jia.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ybu.bjfxy.top

Java: list.add(0, 0);
来源：http://djc.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jpa.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uio.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://isi.52xcode.cn

[D04] 删除元素
来源：http://umw.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nov.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vum.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mdr.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://beo.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rtf.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://izb.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uqr.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rsd.sxryk.cn

[D05] 访问与修改元素
来源：http://sgc.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://znh.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://atu.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ceq.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://law.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://wvb.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://sjh.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vcr.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zzd.xylfe.cn

[D06] 数组长度
来源：http://cpv.fehbvm.com

Py:   len(arr)
来源：http://zyz.shuidangran.top

PHP:  count($arr);
来源：http://bbk.tianlin.xyz

JS:   arr.length
来源：http://npc.jqgfzy.top

TS:   arr.length
来源：http://idv.xylfe.cn

Java: list.size();
来源：http://maa.hfpthk.cn

Go:   len(arr)
来源：http://pip.mhx1999.top

Ruby: arr.length; arr.size
来源：http://xfj.sufxvd.cn

C#:   list.Count;
来源：http://kxi.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://uvg.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://acw.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://hcz.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://wxt.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://ztb.havefunace.top

Java: list.subList(1, 4);
来源：http://rxa.sufxvd.cn

Go:   arr[1:4]
来源：http://jww.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://ibz.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://odi.yj202588.top

[D08] 合并两个数组
来源：http://dwp.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://xxd.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://jmd.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://roc.zhijiandao.cn

TS:   [...a, ...b];
来源：http://wpp.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cdh.chenlongwang.top

Go:   append(a, b...)
来源：http://akb.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://ngv.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://vbd.ydjk.org.cn

[D09] 排序（升序）
来源：http://voc.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://jsq.chenzaomai.com

PHP:  sort($arr);
来源：http://ggu.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qku.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ecb.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cqs.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://axg.bbcook.cn

Ruby: arr.sort
来源：http://irc.jqgfzy.top

C#:   list.Sort();
来源：http://avx.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xin.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cxd.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgd.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qnu.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pxg.hfpthk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vlk.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://srx.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://url.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uaa.chenlongwang.top

[D11] 反转数组
来源：http://thc.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://fjy.ybcxt.top

PHP:  array_reverse($arr);
来源：http://wgu.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gif.sxryk.cn

TS:   [...arr].reverse();
来源：http://tzh.daxiang520.top

Java: Collections.reverse(list);
来源：http://oij.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://kxu.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://eij.wangdashe.top

C#:   list.Reverse();
来源：http://dxc.bbcook.cn

[D12] 查找元素下标
来源：http://vky.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://eru.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bwx.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ful.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qyd.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wqf.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://ndq.dianchejie.cn

Ruby: arr.index(x)
来源：http://hsr.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://sev.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://tnk.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xbz.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://knk.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://njc.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://tlp.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lqx.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://umk.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ykc.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fak.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://kuk.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qcp.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gmj.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://yyc.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://cah.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wtz.shanyushiyangtech.top

Go:   // 手写循环
来源：http://stf.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ymm.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://yaz.xuetiantiany.cn

[D15] 去重
来源：http://tul.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tfn.daxiang520.top

PHP:  array_unique($arr);
来源：http://ygw.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://wha.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://rbn.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wle.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://zqn.chenjidiqi.icu

Ruby: arr.uniq
来源：http://tmj.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://nit.hysaishi.cn

[D16] 求和与平均值
来源：http://dwn.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ukx.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dvi.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzu.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rnz.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fmt.jianghu66.top

Go:   // 手写循环累加
来源：http://jsu.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kgw.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://hfe.yonumen.top

[D17] 最大值与最小值
来源：http://nau.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://chd.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://vav.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ees.yueranfly.top

TS:   Math.max(...arr);
来源：http://qri.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://irv.cucudq.cn


<!-- 参考信息 -->