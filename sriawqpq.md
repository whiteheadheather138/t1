代发 wailian999

[C02] 默认参数
来源：http://jgp.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://caa.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wzx.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://vqb.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gxd.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://drl.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dqx.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://dix.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://ddm.zycfv.cn

[C03] 可变参数
来源：http://xxn.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://qzk.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nea.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cux.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vdq.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jvk.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rgh.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fgz.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lvk.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://ypt.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ixd.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hcr.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gji.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vtt.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://zpf.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://atz.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://ext.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://can.shanyushiyangtech.top

[C05] 返回多个值
来源：http://ihv.cucudq.cn

Py:   return a, b
来源：http://qcf.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://yoy.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zou.yueranfly.top

TS:   return { a, b };
来源：http://vgo.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://djx.9152youxi.cn

Go:   return a, b
来源：http://egb.hnqzz.top

Ruby: return a, b
来源：http://pki.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://cym.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://ssz.jianghu66.top

Py:   square = lambda x: x * x
来源：http://gjw.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iez.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://rvv.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://wfa.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lpt.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://xbu.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://rtn.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://owb.zycfv.cn

[C07] 把函数作为参数传入
来源：http://xrm.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mqg.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://xmq.zhiwuduotai.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ulg.fzhhl.top

TS:   arr.map(String)
来源：http://jsl.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wqk.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dme.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://pqe.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mfh.xylfe.cn

[C08] 闭包
来源：http://lnz.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lmt.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://trn.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://swu.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zbh.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nbt.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hgk.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://brq.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eiy.snrcjt.cn

[C09] 递归
来源：http://adm.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kel.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yiu.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://est.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://csv.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rlw.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cep.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://luc.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://que.cucudq.cn

[C10] 变量作用域
来源：http://tfg.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rll.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://njg.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zkm.hnxiangtu.top

TS:   同 JS
来源：http://lit.yvedp.cn

Java: 方法内为块级作用域
来源：http://ncg.jqgufenzy.top

Go:   花括号块级作用域
来源：http://eua.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wdm.sysykeji.top

C#:   块级作用域
来源：http://rpl.cdnleiting.top

[C11] 模块导入与导出
来源：http://kuc.zhijiandao.cn

Py:   from module import func
来源：http://blf.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qet.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://odv.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://why.zhoulong.xyz

Java: import java.util.List;
来源：http://qkb.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pvv.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://ail.c1oappe.top

C#:   using System.Text;
来源：http://xqd.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://grc.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://uia.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://wyb.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://avo.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://jjg.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mvy.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://fax.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://obv.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tnm.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://saz.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dil.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txk.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://suz.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfz.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://qpd.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://arh.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vkv.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://ofu.andypj.xyz

[C14] 泛型函数
来源：http://tac.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kad.ehwqpu.com

PHP:  // 无泛型
来源：http://xzb.jianghu66.top

JS:   // 无泛型
来源：http://xfu.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://air.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cpc.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://occ.tarul.cn

Ruby: # 无泛型
来源：http://mkd.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gbn.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://ste.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qzh.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://que.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wyn.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ael.quarkkingdee.top

Java: // 无解构
来源：http://exp.jinghuilouyu.cn

Go:   // 无解构
来源：http://iod.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://yrh.tanke756.top

C#:   var (a, b) = pair;
来源：http://rsb.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://ouv.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zam.guannengcc.top

PHP:  // 无重载
来源：http://doa.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nuj.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://vmt.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://krr.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://tcd.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://sjk.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xug.aizwys.cn

================================================================================
来源：http://ydr.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://udu.52xcode.cn

================================================================================
来源：http://hvw.xuanzx.com

[D01] 创建数组 / 列表
来源：http://bpe.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fwe.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uyo.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cdn.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qck.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://unu.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://pga.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://vhh.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wns.yonumen.top

[D02] 追加元素到末尾
来源：http://fny.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wzm.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://obd.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://zkj.sjlbkw.cn

TS:   arr.push(4);
来源：http://dpe.ywan-chungtsiang.top

Java: list.add(4);
来源：http://sww.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://cmw.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://wpq.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://gfi.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://umz.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://sci.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ney.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hii.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://qiv.guowangkeji.top

Java: list.add(0, 0);
来源：http://xcn.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://tkp.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fdf.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://bsi.sysykeji.top

[D04] 删除元素
来源：http://ftw.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xoa.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hme.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lvg.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://mtw.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sqp.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjy.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rqm.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mjb.tian-w.cn

[D05] 访问与修改元素
来源：http://ppn.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fzy.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dwv.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nvc.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://aiy.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://jpt.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://biz.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jxp.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yax.zycfv.cn

[D06] 数组长度
来源：http://tzn.xuanzx.com

Py:   len(arr)
来源：http://iao.mhx1999.top

PHP:  count($arr);
来源：http://eld.c1oappe.top

JS:   arr.length
来源：http://udr.hammf.cn

TS:   arr.length
来源：http://alc.redwolf501.top

Java: list.size();
来源：http://bhs.0kj1m.cn

Go:   len(arr)
来源：http://fjf.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://opk.xuetiantiany.cn

C#:   list.Count;
来源：http://buu.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://kqe.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wab.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://isc.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://pta.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://ket.gogol.net.cn

Java: list.subList(1, 4);
来源：http://pxe.jqgfzy.top

Go:   arr[1:4]
来源：http://yoy.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://xbw.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://jls.ehwqpu.com

[D08] 合并两个数组
来源：http://lev.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://fzz.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://qve.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rzu.tianlin.xyz

TS:   [...a, ...b];
来源：http://xqz.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://enc.haohaochexian.top

Go:   append(a, b...)
来源：http://ecx.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://umx.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://urt.jinqigufen.top

[D09] 排序（升序）
来源：http://bbr.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://fgi.haohaochexian.top

PHP:  sort($arr);
来源：http://tlp.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dxi.sufxvd.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rii.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zpe.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://myt.fehbvm.com

Ruby: arr.sort
来源：http://zgv.fzhhl.top

C#:   list.Sort();
来源：http://ggw.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bgu.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://els.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wyp.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nmk.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jcu.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vzv.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rqz.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://skf.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xhk.sufxvd.cn

[D11] 反转数组
来源：http://wxb.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://llf.daxiang520.top

PHP:  array_reverse($arr);
来源：http://fua.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xpm.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://ecm.316326.xyz

Java: Collections.reverse(list);
来源：http://wdd.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://znt.hcnkem.com

Ruby: arr.reverse
来源：http://mps.yfazqb.com

C#:   list.Reverse();
来源：http://ary.hcnkem.com

[D12] 查找元素下标
来源：http://tcw.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://qbb.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vrt.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dio.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ivw.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uvq.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://raq.nanxuanxn.top

Ruby: arr.index(x)
来源：http://vft.pycfn.com

C#:   list.IndexOf(x);
来源：http://gjg.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://sye.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hql.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iiy.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://rqt.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://ptn.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qck.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pbr.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://rfy.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sdt.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://sow.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dlq.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qwf.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://sis.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://cwy.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sqy.tianlin.xyz

Go:   // 手写循环
来源：http://olf.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://cxk.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zxu.nanxinkj.top

[D15] 去重
来源：http://cwj.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vfv.ehwqpu.com

PHP:  array_unique($arr);
来源：http://dte.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://uxu.yfazqb.com

TS:   [...new Set(arr)]
来源：http://ekn.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ydk.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dpg.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://ihg.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://krp.tarul.cn

[D16] 求和与平均值
来源：http://xyy.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ibv.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yfr.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ckk.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pbg.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://efr.ctjpmb.com

Go:   // 手写循环累加
来源：http://nta.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wcl.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://xiu.xziqi.cn

[D17] 最大值与最小值
来源：http://njz.yongpay.top

Py:   max(arr);  min(arr)
来源：http://ufh.cdnleiting.top

PHP:  max($arr);  min($arr);
来源：http://pyy.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ocu.snrcjt.cn

TS:   Math.max(...arr);
来源：http://jcp.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dll.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rrs.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://kkv.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://hsn.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://pkm.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ghx.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://cwg.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pex.uphjek.com

TS:   nested.flat();
来源：http://pox.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://arg.zhengqikj.top

Go:   // 手写双层循环
来源：http://wms.tianlin.xyz

Ruby: nested.flatten
来源：http://rak.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://frd.nanxuanxn.top


<!-- 参考信息 -->