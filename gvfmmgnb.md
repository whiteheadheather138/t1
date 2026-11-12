代发 wailian999

[C02] 默认参数
来源：http://oum.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://mbo.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ywz.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://bbv.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://jwh.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://vxi.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnw.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://hpc.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://vhs.zhiwuduotai.top

[C03] 可变参数
来源：http://ggv.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://bgz.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vtd.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tvs.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eop.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cpo.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ddm.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://upx.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://woy.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://gpm.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rpd.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ocf.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rub.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tsi.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://naa.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://lrp.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://hwm.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://zxe.mhx1999.top

[C05] 返回多个值
来源：http://txx.yuanzhike.top

Py:   return a, b
来源：http://qzk.havefunace.top

PHP:  return [$a, $b];
来源：http://mnq.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fsc.redwolf501.top

TS:   return { a, b };
来源：http://sur.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hpd.birdmap.top

Go:   return a, b
来源：http://kzd.hcnkem.com

Ruby: return a, b
来源：http://amz.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://rnl.yongpay.top

[C06] 匿名函数 / lambda
来源：http://sey.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://hyz.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dtp.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://xgc.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://mwv.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xkw.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://knl.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://yaz.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://lpi.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://vhm.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cet.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://ffs.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ses.vqdsnc.cn

TS:   arr.map(String)
来源：http://ssl.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://scx.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bob.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://myo.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wxy.xylfe.cn

[C08] 闭包
来源：http://xvi.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gdo.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gan.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://udc.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ftk.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fbt.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ajk.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ftb.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mkh.sjlbkw.cn

[C09] 递归
来源：http://tje.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gmo.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bpo.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dnc.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uou.hesvh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rpb.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ars.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nlh.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thv.fengsongda.top

[C10] 变量作用域
来源：http://hhn.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sji.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://umx.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ikt.yj20258.top

TS:   同 JS
来源：http://sop.bbcook.cn

Java: 方法内为块级作用域
来源：http://fyb.yangfankeji.com

Go:   花括号块级作用域
来源：http://czn.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fey.nwbrower.top

C#:   块级作用域
来源：http://ftr.birdmap.top

[C11] 模块导入与导出
来源：http://noh.andypj.xyz

Py:   from module import func
来源：http://dkh.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sdm.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lvc.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zml.ehwqpu.com

Java: import java.util.List;
来源：http://nxg.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zqe.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://rfd.fengsongda.top

C#:   using System.Text;
来源：http://rmr.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://dwc.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://sty.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://zwg.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://wnf.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://gbv.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://euh.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://vjh.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://ryr.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hbg.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://yfr.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uqb.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hwm.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zdr.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://guv.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://kav.daria6918.cn

Go:   func add(a, b int) int
来源：http://yna.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://reh.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://znx.yj20258.top

[C14] 泛型函数
来源：http://cay.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zjq.fzhhl.top

PHP:  // 无泛型
来源：http://uxk.zdbjq.cn

JS:   // 无泛型
来源：http://bbu.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qof.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nyp.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ptc.sxryk.cn

Ruby: # 无泛型
来源：http://phl.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pkb.yongpay.top

[C15] 解构 / 展开参数
来源：http://jgs.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tli.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://aql.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kmz.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ojr.yangfankeji.com

Java: // 无解构
来源：http://lby.dianchejie.cn

Go:   // 无解构
来源：http://uua.shzxlz.cn

Ruby: a, b = pair
来源：http://vpl.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://car.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://gvm.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jrl.9152youxi.cn

PHP:  // 无重载
来源：http://ikf.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://vbf.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://ijk.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lww.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://exa.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://nyt.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hnp.xinyue.icu

================================================================================
来源：http://ccm.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://qrn.aibaodan.cn

================================================================================
来源：http://jae.tanke756.top

[D01] 创建数组 / 列表
来源：http://hpe.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dnt.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sex.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://koq.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://osx.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dgm.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://bky.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://opq.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nbs.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://lzk.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zdd.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://idk.jiagoushi.top

JS:   arr.push(4);
来源：http://eps.xuanzx.com

TS:   arr.push(4);
来源：http://tbh.jinghuilouyu.cn

Java: list.add(4);
来源：http://azs.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://jjp.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://lay.chenjidiqi.icu

C#:   list.Add(4);
来源：http://vir.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://pdc.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://mvv.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cqm.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bft.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://iij.yongpay.top

Java: list.add(0, 0);
来源：http://xej.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iva.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mef.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://iql.tanke756.top

[D04] 删除元素
来源：http://aiz.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uzn.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sew.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wtm.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://qtw.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zdw.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gbq.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ntt.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://now.smart0.xyz

[D05] 访问与修改元素
来源：http://may.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wbj.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ttn.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://izf.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://hjk.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://lts.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://cdh.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yfr.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://stq.guowangkeji.top

[D06] 数组长度
来源：http://yft.birdmap.top

Py:   len(arr)
来源：http://ytk.tanke756.top

PHP:  count($arr);
来源：http://jav.kuanghao11.cn

JS:   arr.length
来源：http://gfm.ybcxt.top

TS:   arr.length
来源：http://cio.9152youxi.cn

Java: list.size();
来源：http://bme.dashuyun.cn

Go:   len(arr)
来源：http://lbi.xuanzx.com

Ruby: arr.length; arr.size
来源：http://twy.hywenlv.cn

C#:   list.Count;
来源：http://iil.cashguo.top

[D07] 切片 / 取子数组
来源：http://cwg.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yjl.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://myi.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://cvt.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://xlr.yonumen.top

Java: list.subList(1, 4);
来源：http://xuc.snrcjt.cn

Go:   arr[1:4]
来源：http://fql.aizwys.cn

Ruby: arr[1, 3]
来源：http://gup.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://ukl.cqqwz.cn

[D08] 合并两个数组
来源：http://eim.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://byp.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://vyb.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hky.ydjk.org.cn

TS:   [...a, ...b];
来源：http://sbg.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxn.316326.xyz

Go:   append(a, b...)
来源：http://fup.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://elf.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://tpn.fehbvm.com

[D09] 排序（升序）
来源：http://rgg.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://kbs.kuanghao11.cn

PHP:  sort($arr);
来源：http://hwr.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tzd.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://omc.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wgq.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hif.ydzc1.top

Ruby: arr.sort
来源：http://jlg.hammf.cn

C#:   list.Sort();
来源：http://iay.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jhx.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fnh.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fpt.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://okb.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xpn.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mnq.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pvi.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hkw.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bbp.andypj.xyz

[D11] 反转数组
来源：http://gkh.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://kfu.hnqzz.top

PHP:  array_reverse($arr);
来源：http://uor.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nzl.jqgfzy.top

TS:   [...arr].reverse();
来源：http://sdr.yongpay.top

Java: Collections.reverse(list);
来源：http://fyk.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://xbn.hcnkem.com

Ruby: arr.reverse
来源：http://xgx.tian-w.cn

C#:   list.Reverse();
来源：http://xnz.uphjek.com

[D12] 查找元素下标
来源：http://alb.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://zir.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uvx.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tmm.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hhy.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mcf.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://cse.iojbl.cn

Ruby: arr.index(x)
来源：http://mhc.sysykeji.top

C#:   list.IndexOf(x);
来源：http://krt.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://glv.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fjr.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nlq.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://gjk.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://xai.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eny.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qwa.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://lmg.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zcw.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://eoe.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ocv.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lpx.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://rbm.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://xkj.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kwf.ctjpmb.com

Go:   // 手写循环
来源：http://koo.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://rsy.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xbl.nwbrower.top

[D15] 去重
来源：http://azp.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://krz.52xcode.cn

PHP:  array_unique($arr);
来源：http://bky.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://ije.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://btu.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jqc.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://hnj.yongpay.top

Ruby: arr.uniq
来源：http://rsp.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://lgp.zhongyouzk.top

[D16] 求和与平均值
来源：http://apv.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lqm.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://niq.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://caf.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxw.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eaz.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://dmk.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://prs.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://jjc.jlsjyb.cn

[D17] 最大值与最小值
来源：http://npc.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://jcd.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://dpy.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rin.hesvh.cn

TS:   Math.max(...arr);
来源：http://wmr.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://txg.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qhv.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://fqr.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://ssb.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://glu.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zvi.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://ryf.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://min.0kj1m.cn

TS:   nested.flat();
来源：http://htq.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cgb.yonumen.top

Go:   // 手写双层循环
来源：http://syj.gotoacloud.top

Ruby: nested.flatten
来源：http://hlf.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ivx.52xcode.cn


<!-- 参考信息 -->