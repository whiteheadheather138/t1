代发 wailian999

Py:   def add(a, b): return a + b
来源：http://pwp.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjx.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://cdx.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xyq.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://osn.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pbf.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://cwe.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fib.hysaishi.cn

[C02] 默认参数
来源：http://cfo.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://mno.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://raq.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://tof.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://van.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vhr.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lse.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://zvx.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://caw.hywenlv.cn

[C03] 可变参数
来源：http://owm.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://qsl.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ngw.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvd.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxa.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nkg.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xbk.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://rvk.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyg.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://eke.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hlw.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlj.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://twv.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wyu.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://ohr.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://tqy.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://uez.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://jig.yj20258.top

[C05] 返回多个值
来源：http://kzl.tarul.cn

Py:   return a, b
来源：http://zpu.cdnleiting.top

PHP:  return [$a, $b];
来源：http://rze.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ivq.sysykeji.top

TS:   return { a, b };
来源：http://zpz.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zma.bjfxy.top

Go:   return a, b
来源：http://cvx.316326.xyz

Ruby: return a, b
来源：http://yfb.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://hge.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://trw.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://pjf.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qzf.yj20258888.top

JS:   const square = x => x * x;
来源：http://pdd.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://mwt.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://juw.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://wkn.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://pyj.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://shf.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://ksb.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xss.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://gyw.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nrn.jyoumei.cn

TS:   arr.map(String)
来源：http://myh.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fvy.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://van.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://xyr.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jdv.smart0.xyz

[C08] 闭包
来源：http://zdf.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aam.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lmd.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://teq.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dyr.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aht.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yrj.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pmd.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wvx.jqgfzy.top

[C09] 递归
来源：http://vby.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqf.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mti.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixb.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dqj.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ntt.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mev.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bql.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mil.316326.xyz

[C10] 变量作用域
来源：http://oae.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://afv.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hwt.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nhh.shanyushiyangtech.top

TS:   同 JS
来源：http://tne.ivvv.top

Java: 方法内为块级作用域
来源：http://fal.zhengqikj.top

Go:   花括号块级作用域
来源：http://kzy.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://agt.zhongyouzk.top

C#:   块级作用域
来源：http://oqf.guannengcc.top

[C11] 模块导入与导出
来源：http://xph.xinyue.icu

Py:   from module import func
来源：http://cng.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://szj.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xpw.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vuq.yj20258.top

Java: import java.util.List;
来源：http://bmq.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ewe.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://ayz.yuxming.cn

C#:   using System.Text;
来源：http://esk.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://pjd.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://bkt.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://zve.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://weq.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://aab.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bnp.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://kvk.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://mgm.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ppu.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://yps.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wkg.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gry.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hin.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sob.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://emf.redwolf501.top

Go:   func add(a, b int) int
来源：http://reu.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xsg.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://rnh.aibaodan.cn

[C14] 泛型函数
来源：http://qlc.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fur.jiagoushi.top

PHP:  // 无泛型
来源：http://gbs.andypj.xyz

JS:   // 无泛型
来源：http://few.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cqo.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://axz.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oup.tanke756.top

Ruby: # 无泛型
来源：http://gxd.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jsl.uphjek.com

[C15] 解构 / 展开参数
来源：http://adb.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tzh.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://etj.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zte.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vhp.xziqi.cn

Java: // 无解构
来源：http://hip.ydzc1.top

Go:   // 无解构
来源：http://svt.uphjek.com

Ruby: a, b = pair
来源：http://hro.wangdashe.top

C#:   var (a, b) = pair;
来源：http://vfz.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://rmb.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kvm.mhx1999.top

PHP:  // 无重载
来源：http://obb.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sbs.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://gkq.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rwv.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://ykm.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://ceh.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dsj.0kj1m.cn

================================================================================
来源：http://att.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://pqe.tian-w.cn

================================================================================
来源：http://dob.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://sxh.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sig.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jrx.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tqn.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zib.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wrg.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://eii.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://kbl.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uvq.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://rol.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ixc.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://les.hammf.cn

JS:   arr.push(4);
来源：http://xzp.andypj.xyz

TS:   arr.push(4);
来源：http://vbj.smart0.xyz

Java: list.add(4);
来源：http://vpk.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://nlc.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://ajq.ehwqpu.com

C#:   list.Add(4);
来源：http://jvo.cheryme.top

[D03] 在指定位置插入元素
来源：http://cmp.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://qms.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://osr.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://urz.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://evz.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://zjo.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ons.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mhf.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://sis.meibo888.top

[D04] 删除元素
来源：http://nxa.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wss.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kdf.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fid.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://xvj.shangyingyoupin.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://smc.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mln.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nug.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gto.xylfe.cn

[D05] 访问与修改元素
来源：http://irz.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pet.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vdu.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ukg.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://lps.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://wod.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://quf.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kuj.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aop.ybcxt.top

[D06] 数组长度
来源：http://yfk.shangyingyoupin.top

Py:   len(arr)
来源：http://ibp.uphjek.com

PHP:  count($arr);
来源：http://dqi.yj202588.top

JS:   arr.length
来源：http://tzs.xingfuxueyuan.xyz

TS:   arr.length
来源：http://ubi.smart0.xyz

Java: list.size();
来源：http://azr.vqdsnc.cn

Go:   len(arr)
来源：http://lob.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://qbz.hywenlv.cn

C#:   list.Count;
来源：http://jmh.xylfe.cn

[D07] 切片 / 取子数组
来源：http://exf.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gup.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://vce.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://wlv.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://vgi.cheryme.top

Java: list.subList(1, 4);
来源：http://ofa.sjlbkw.cn

Go:   arr[1:4]
来源：http://wob.gzhubu.top

Ruby: arr[1, 3]
来源：http://rht.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://khs.sjlbkw.cn

[D08] 合并两个数组
来源：http://ddo.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://cih.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://zax.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uqc.cqqwz.cn

TS:   [...a, ...b];
来源：http://rzt.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://egs.zdbjq.cn

Go:   append(a, b...)
来源：http://rgm.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://xel.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://jmi.cqqwz.cn

[D09] 排序（升序）
来源：http://wju.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://uay.chenzaomai.com

PHP:  sort($arr);
来源：http://tsh.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jse.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ydt.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zft.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://utj.ehwqpu.com

Ruby: arr.sort
来源：http://khz.xinyue.icu

C#:   list.Sort();
来源：http://vmn.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fmi.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://byb.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vam.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfq.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kuu.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bgg.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tjp.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ild.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://htb.yuxming.cn

[D11] 反转数组
来源：http://nyx.yvedp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vln.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://ssv.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sbf.nwbrower.top

TS:   [...arr].reverse();
来源：http://gwq.chenzaomai.com

Java: Collections.reverse(list);
来源：http://xwu.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://yyc.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://gnu.cdnleiting.top

C#:   list.Reverse();
来源：http://kfy.jinqigfzy.top

[D12] 查找元素下标
来源：http://fwv.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://ogs.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nrc.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxe.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://glc.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nvn.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://fvs.shzxlz.cn

Ruby: arr.index(x)
来源：http://dxr.yj20258.top

C#:   list.IndexOf(x);
来源：http://naf.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://jqp.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eky.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rcl.bbcook.cn

JS:   arr.filter(x => x > 3)
来源：http://hsb.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://qoh.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sqo.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sis.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://bgd.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fol.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://sqc.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exl.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sar.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://sem.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://rqf.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tlh.jianghu66.top

Go:   // 手写循环
来源：http://gej.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://riw.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kew.xziqi.cn

[D15] 去重
来源：http://vnf.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pcc.birdmap.top

PHP:  array_unique($arr);
来源：http://bgt.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://zqv.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://xup.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qzf.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tbt.bbcook.cn

Ruby: arr.uniq
来源：http://khp.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://dxt.316326.xyz

[D16] 求和与平均值
来源：http://tqe.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pkk.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qnm.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dpi.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfn.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ube.bbcook.cn

Go:   // 手写循环累加
来源：http://lts.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ejn.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://lwp.fktsv.cn

[D17] 最大值与最小值
来源：http://ljt.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://skt.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://ujx.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://duh.vehdjk.com

TS:   Math.max(...arr);
来源：http://naf.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ryh.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qwo.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://orj.hammf.cn

C#:   list.Max();  list.Min()
来源：http://hvh.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://stm.wangdashe.top


<!-- 参考信息 -->