代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://sln.xylfe.cn

[C03] 可变参数
来源：http://onj.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://jra.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gtw.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lqy.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrr.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://apa.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jxo.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tms.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mne.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://gaj.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gvr.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uug.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ysu.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fug.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://zpu.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://hdt.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://wvq.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://sfh.shzxlz.cn

[C05] 返回多个值
来源：http://yyo.hammf.cn

Py:   return a, b
来源：http://iwb.hesvh.cn

PHP:  return [$a, $b];
来源：http://dxb.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zus.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://wqu.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oeh.jinghuilouyu.cn

Go:   return a, b
来源：http://dbb.hcnkem.com

Ruby: return a, b
来源：http://bhe.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://vji.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://gtg.birdmap.top

Py:   square = lambda x: x * x
来源：http://ilh.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://pdv.chenzaomai.com

JS:   const square = x => x * x;
来源：http://ibj.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://obw.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vdx.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://euv.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://quq.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://jbf.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://uux.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://usm.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://msf.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://air.ydjk.org.cn

TS:   arr.map(String)
来源：http://eus.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://krl.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vvc.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://wfo.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://crc.fanxiaobao.xyz

[C08] 闭包
来源：http://edy.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://scg.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://crj.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ugq.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zko.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://spk.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qxn.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nqn.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ata.ppjwa.cn

[C09] 递归
来源：http://ncv.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zis.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xsn.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ykm.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ycv.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jil.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fnj.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aau.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sjr.yuxming.cn

[C10] 变量作用域
来源：http://gpb.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://irw.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iba.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fay.xinyue.icu

TS:   同 JS
来源：http://ajg.birdmap.top

Java: 方法内为块级作用域
来源：http://nds.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://dag.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://utf.havefunace.top

C#:   块级作用域
来源：http://hxl.zhoulong.xyz

[C11] 模块导入与导出
来源：http://rzm.birdmap.top

Py:   from module import func
来源：http://sqa.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tla.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nrv.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kph.aizwys.cn

Java: import java.util.List;
来源：http://rer.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://peu.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://nbn.chenzaomai.com

C#:   using System.Text;
来源：http://xph.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://lxi.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://xef.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://oaj.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://xor.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://odl.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zfg.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://qzr.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://xru.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://enk.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://bph.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ixc.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nxb.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qaj.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pnn.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eym.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://ofk.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cqe.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://kwd.gotoacloud.top

[C14] 泛型函数
来源：http://kvj.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zds.jianghu66.top

PHP:  // 无泛型
来源：http://sum.fktsv.cn

JS:   // 无泛型
来源：http://pov.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xlr.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zzd.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oms.fehbvm.com

Ruby: # 无泛型
来源：http://jmc.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sbk.yj20258.top

[C15] 解构 / 展开参数
来源：http://rbl.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ysv.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://lxd.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iuj.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uoo.hysaishi.cn

Java: // 无解构
来源：http://qoz.jinyuanbaomall.cn

Go:   // 无解构
来源：http://nup.tanke756.top

Ruby: a, b = pair
来源：http://yva.hnqzz.top

C#:   var (a, b) = pair;
来源：http://pel.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://sfu.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dpf.dashuyun.cn

PHP:  // 无重载
来源：http://sjo.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://elc.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://ujv.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://htz.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://kda.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://vlc.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://atx.hesvh.cn

================================================================================
来源：http://pvh.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://kjs.gzhubu.top

================================================================================
来源：http://lmn.fzhhl.top

[D01] 创建数组 / 列表
来源：http://vnt.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iav.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ctq.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bya.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kyr.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ttx.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://gpb.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://lvc.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wtr.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://cpz.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xqx.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://axe.sufxvd.cn

JS:   arr.push(4);
来源：http://kez.chenlongwang.top

TS:   arr.push(4);
来源：http://ojk.zdbjq.cn

Java: list.add(4);
来源：http://uyy.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://exf.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://vku.zdqjudy.top

C#:   list.Add(4);
来源：http://uem.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://fht.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://mpt.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://coy.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xer.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://tbs.nanxinkj.top

Java: list.add(0, 0);
来源：http://fnu.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fws.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bcn.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://yez.hywenlv.cn

[D04] 删除元素
来源：http://nuw.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jal.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://grz.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ckf.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://pas.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jsw.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ckl.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lwa.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qyx.yuxming.cn

[D05] 访问与修改元素
来源：http://ptn.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cnn.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xwl.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nfw.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://zjs.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://rjd.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://rip.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nmq.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tka.iojbl.cn

[D06] 数组长度
来源：http://mdb.cheryme.top

Py:   len(arr)
来源：http://vlt.yongpay.top

PHP:  count($arr);
来源：http://oen.birdmap.top

JS:   arr.length
来源：http://ztp.hnqzz.top

TS:   arr.length
来源：http://abi.sjlbkw.cn

Java: list.size();
来源：http://rxv.hammf.cn

Go:   len(arr)
来源：http://jow.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://lnq.sysykeji.top

C#:   list.Count;
来源：http://uyw.epnwcf.com

[D07] 切片 / 取子数组
来源：http://uvm.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yjv.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gqp.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://wrx.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://hlr.fktsv.cn

Java: list.subList(1, 4);
来源：http://ctf.jianghu66.top

Go:   arr[1:4]
来源：http://vsc.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://ccb.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://dhy.quarkkingdee.top

[D08] 合并两个数组
来源：http://etm.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://sxx.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://tpj.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nof.birdmap.top

TS:   [...a, ...b];
来源：http://ges.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rnk.zhixingplan.top

Go:   append(a, b...)
来源：http://uom.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://ktf.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://hhk.sufxvd.cn

[D09] 排序（升序）
来源：http://zxz.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://iox.yuanzhike.top

PHP:  sort($arr);
来源：http://gaa.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cre.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xaf.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ixj.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zcy.chenjidiqi.icu

Ruby: arr.sort
来源：http://esg.xinyue.icu

C#:   list.Sort();
来源：http://wsm.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jnu.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cpa.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lmi.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rfy.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nco.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yps.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pll.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vjx.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://htt.sxryk.cn

[D11] 反转数组
来源：http://dcu.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://fah.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://aws.pengpengdd.cyou

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ytj.zhixingplan.top

TS:   [...arr].reverse();
来源：http://cuj.havefunace.top

Java: Collections.reverse(list);
来源：http://euc.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://pon.hesvh.cn

Ruby: arr.reverse
来源：http://zbw.hesvh.cn

C#:   list.Reverse();
来源：http://hjt.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://wng.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://ogd.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://enx.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjt.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nou.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vfj.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://sqb.hysaishi.cn

Ruby: arr.index(x)
来源：http://rsw.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://rev.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://jds.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xcl.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xan.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://rqh.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://xkn.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pzu.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xrp.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://fxx.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sph.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://zug.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cjp.vqdsnc.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yhk.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://oli.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://yne.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zhw.jqgufenzy.top

Go:   // 手写循环
来源：http://bmg.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://zrv.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kku.jinyuanbaomall.cn

[D15] 去重
来源：http://ovt.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qal.hnqzz.top

PHP:  array_unique($arr);
来源：http://jec.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://cyh.sysykeji.top

TS:   [...new Set(arr)]
来源：http://mpl.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wtl.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://yug.epnwcf.com

Ruby: arr.uniq
来源：http://bou.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://aoc.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://aom.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jxu.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pac.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mqd.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://coe.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://grz.52xcode.cn

Go:   // 手写循环累加
来源：http://ynn.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://olo.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://ovy.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://oku.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://zlr.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://duo.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ojp.epnwcf.com

TS:   Math.max(...arr);
来源：http://ocx.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uth.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qry.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://ltj.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://hji.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://naj.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nwx.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://noh.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qqc.aibaodan.cn

TS:   nested.flat();
来源：http://qpw.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://siw.aibaodan.cn

Go:   // 手写双层循环
来源：http://dad.chenlongwang.top

Ruby: nested.flatten
来源：http://gyv.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cin.gotoacloud.top

[D19] 按字段分组
来源：http://mhf.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sko.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://saf.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xlv.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://amz.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gme.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://bih.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://trm.iojbl.cn


<!-- 参考信息 -->