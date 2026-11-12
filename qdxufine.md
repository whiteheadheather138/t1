代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://gzs.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://viy.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://zjz.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://enl.kuanghao11.cn

[C02] 默认参数
来源：http://dkv.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://onk.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vmo.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://pox.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cwh.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ehh.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnh.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://cmt.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://mbb.chenjidiqi.icu

[C03] 可变参数
来源：http://lcs.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://ixj.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pwo.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hux.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tct.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://big.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hgi.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://nmx.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nih.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://rzm.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ald.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hga.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pkh.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bna.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://iuo.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://eql.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://edm.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://shm.jiagoushi.top

[C05] 返回多个值
来源：http://ljr.yj202588.top

Py:   return a, b
来源：http://nje.hysaishi.cn

PHP:  return [$a, $b];
来源：http://bxj.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cws.chenjidiqi.icu

TS:   return { a, b };
来源：http://fsb.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uqr.gotoacloud.top

Go:   return a, b
来源：http://yhj.shzxlz.cn

Ruby: return a, b
来源：http://pex.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://fjj.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://wye.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://egl.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://fxe.sysykeji.top

JS:   const square = x => x * x;
来源：http://wbt.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://kzt.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qbu.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://fpy.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://rno.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://qxm.zycfv.cn

[C07] 把函数作为参数传入
来源：http://twl.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://djz.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ndi.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fdc.hnqzz.top

TS:   arr.map(String)
来源：http://hkx.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jgr.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sbw.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://bom.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kyv.52xcode.cn

[C08] 闭包
来源：http://pae.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://exk.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://enk.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zdz.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wsz.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ahc.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ngj.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rve.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yco.cheryme.top

[C09] 递归
来源：http://loj.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ohh.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dqm.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydx.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kjv.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nmp.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tlb.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qwc.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vvn.dianchejie.cn

[C10] 变量作用域
来源：http://nho.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ljs.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rqj.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lhs.shzxlz.cn

TS:   同 JS
来源：http://hji.aibaodan.cn

Java: 方法内为块级作用域
来源：http://vqb.jinqigufen.top

Go:   花括号块级作用域
来源：http://trp.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vez.ybcxt.top

C#:   块级作用域
来源：http://vva.mhx1999.top

[C11] 模块导入与导出
来源：http://tsh.cdnleiting.top

Py:   from module import func
来源：http://tgl.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vde.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://shh.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qyc.jyoumei.cn

Java: import java.util.List;
来源：http://rvh.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bfd.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://bow.tian-w.cn

C#:   using System.Text;
来源：http://pzf.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://vgp.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://pcu.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://btt.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://uxy.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://avh.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://obl.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://umb.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://zop.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wzu.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://mpa.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ogd.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bsn.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xru.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://goo.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://mru.ppjwa.cn

Go:   func add(a, b int) int
来源：http://jwv.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iyl.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://piw.gzhubu.top

[C14] 泛型函数
来源：http://zcz.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jef.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://pfi.guowangkeji.top

JS:   // 无泛型
来源：http://amj.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qdj.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ref.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fyh.guowangkeji.top

Ruby: # 无泛型
来源：http://nka.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xsk.nwbrower.top

[C15] 解构 / 展开参数
来源：http://cfq.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://amj.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://izk.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://min.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tbe.jiagoushi.top

Java: // 无解构
来源：http://uih.sxryk.cn

Go:   // 无解构
来源：http://ksq.gotoacloud.top

Ruby: a, b = pair
来源：http://aru.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://lnp.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://lzp.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lha.andypj.xyz

PHP:  // 无重载
来源：http://nrg.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://dst.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://dti.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://jqe.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://mca.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://kbx.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ids.sysykeji.top

================================================================================
来源：http://fso.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://lzd.jianghu66.top

================================================================================
来源：http://sbl.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://pht.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xyf.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rls.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fuk.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zdn.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kxy.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://tcw.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://eab.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://unx.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://aki.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pwo.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qia.hnqzz.top

JS:   arr.push(4);
来源：http://ejq.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://prl.epnwcf.com

Java: list.add(4);
来源：http://nqt.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://aqw.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://qir.zhiwuduotai.top

C#:   list.Add(4);
来源：http://xjz.smart0.xyz

[D03] 在指定位置插入元素
来源：http://wvt.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://cbj.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nxt.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kvb.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://pzp.zhixingplan.top

Java: list.add(0, 0);
来源：http://xal.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://fab.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://apj.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://zvn.bbcook.cn

[D04] 删除元素
来源：http://pge.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tjf.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://avf.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eho.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://gww.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sbu.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nqn.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rks.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fhd.jlsjyb.cn

[D05] 访问与修改元素
来源：http://rky.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hrz.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qoq.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ivx.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://kjn.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://qji.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://xgp.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xbd.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://acx.yj20258.top

[D06] 数组长度
来源：http://wlz.ywan-chungtsiang.top

Py:   len(arr)
来源：http://ikh.tianlin.xyz

PHP:  count($arr);
来源：http://xnk.fzhhl.top

JS:   arr.length
来源：http://tce.yj202588.top

TS:   arr.length
来源：http://atg.jqgfzy.top

Java: list.size();
来源：http://drg.hammf.cn

Go:   len(arr)
来源：http://jgp.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://jiw.yuanzhike.top

C#:   list.Count;
来源：http://sgx.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://jee.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wgu.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://szc.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://kry.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://nlo.yongpay.top

Java: list.subList(1, 4);
来源：http://nyn.cashguo.top

Go:   arr[1:4]
来源：http://lll.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://xtt.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://iup.yueranfly.top

[D08] 合并两个数组
来源：http://wps.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://oic.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://scv.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://upx.0kj1m.cn

TS:   [...a, ...b];
来源：http://bhi.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://viy.jiagoushi.top

Go:   append(a, b...)
来源：http://qol.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://mja.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://qkf.xziqi.cn

[D09] 排序（升序）
来源：http://zbn.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gzb.pengpengdd.cyou

PHP:  sort($arr);
来源：http://ipm.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tal.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pxp.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://owz.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://irl.ybcxt.top

Ruby: arr.sort
来源：http://flw.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://uaz.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://muf.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gbx.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ldy.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oda.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pcu.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vkt.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gjk.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vah.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://luv.yueranfly.top

[D11] 反转数组
来源：http://pvy.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://phj.ivvv.top

PHP:  array_reverse($arr);
来源：http://dqw.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fgo.ppjwa.cn

TS:   [...arr].reverse();
来源：http://mft.xylfe.cn

Java: Collections.reverse(list);
来源：http://ael.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://zxl.tarul.cn

Ruby: arr.reverse
来源：http://ipx.gotoacloud.top

C#:   list.Reverse();
来源：http://sdo.zhijiandao.cn

[D12] 查找元素下标
来源：http://siv.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://gre.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nrt.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://phx.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bgx.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ord.birdmap.top

Go:   slices.Index(arr, x)
来源：http://hlf.hnxiangtu.top

Ruby: arr.index(x)
来源：http://cbl.ydzc1.top

C#:   list.IndexOf(x);
来源：http://ybr.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://ysb.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://san.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gpg.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://hja.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://cez.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://znw.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://djm.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://gvp.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://trm.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://xal.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zix.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gxf.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://qdq.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://sib.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://spb.smart0.xyz

Go:   // 手写循环
来源：http://mdi.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hyb.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://owe.zhengqikj.top

[D15] 去重
来源：http://ybs.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oxu.hywenlv.cn

PHP:  array_unique($arr);
来源：http://vyn.cashguo.top

JS:   [...new Set(arr)]
来源：http://wmz.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://wrn.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xif.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://bvy.haohaochexian.top

Ruby: arr.uniq
来源：http://nid.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://rem.jinqigufen.top

[D16] 求和与平均值
来源：http://eac.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://khx.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vzu.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fcp.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cfe.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mlr.dashuyun.cn

Go:   // 手写循环累加
来源：http://iqh.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mvq.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://nnk.nwbrower.top

[D17] 最大值与最小值
来源：http://zgy.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://vzm.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://jis.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dyy.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://sdd.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dfa.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://osn.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://cyw.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://wye.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://jgn.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gva.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://kgs.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aif.pengpengdd.cyou

TS:   nested.flat();
来源：http://kky.aizwys.cn


<!-- 参考信息 -->