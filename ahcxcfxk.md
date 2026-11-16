代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://vdu.jinqigufen.top

[C03] 可变参数
来源：http://lej.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://pcc.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://otg.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrn.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zdd.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yqv.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://poj.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://jgr.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cqs.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://gko.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jxl.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlv.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nga.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oyo.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://ysh.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://uvf.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://bxf.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://rfo.316326.xyz

[C05] 返回多个值
来源：http://ybe.zhixingplan.top

Py:   return a, b
来源：http://xtp.hysaishi.cn

PHP:  return [$a, $b];
来源：http://xdl.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xqh.yuanzhike.top

TS:   return { a, b };
来源：http://joz.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gbk.hongshengwenyu.top

Go:   return a, b
来源：http://ryk.yvedp.cn

Ruby: return a, b
来源：http://xsv.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://nqg.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://eqc.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://mty.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://upp.yuanzhike.top

JS:   const square = x => x * x;
来源：http://wje.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://oim.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lbh.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://yxr.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://wvr.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hdg.wangdashe.top

[C07] 把函数作为参数传入
来源：http://guv.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://otm.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zla.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://piz.aibaodan.cn

TS:   arr.map(String)
来源：http://iao.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hmg.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ich.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://ami.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://utr.ywan-chungtsiang.top

[C08] 闭包
来源：http://mol.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nrm.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohl.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ruf.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://obn.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ucz.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qqg.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pcl.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qjx.zhixingplan.top

[C09] 递归
来源：http://hmj.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xva.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bpv.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yen.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvi.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hrb.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://imt.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://psf.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cmf.jqgufenzy.top

[C10] 变量作用域
来源：http://cwo.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://twd.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zsr.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xsn.sysykeji.top

TS:   同 JS
来源：http://ebb.havefunace.top

Java: 方法内为块级作用域
来源：http://fxj.vehdjk.com

Go:   花括号块级作用域
来源：http://flc.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wre.yuanzhike.top

C#:   块级作用域
来源：http://ufa.hesvh.cn

[C11] 模块导入与导出
来源：http://cvn.cqqwz.cn

Py:   from module import func
来源：http://uqz.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qgx.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ejh.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qvq.jqgfzy.top

Java: import java.util.List;
来源：http://lnn.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cub.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://lry.iojbl.cn

C#:   using System.Text;
来源：http://iuz.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://smm.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://svk.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://dza.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://wvp.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://kfk.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vat.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://oup.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://pad.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kkg.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://leq.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqy.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tmb.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://flf.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://paa.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mkx.gzhubu.top

Go:   func add(a, b int) int
来源：http://snk.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dva.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://tku.sufxvd.cn

[C14] 泛型函数
来源：http://lse.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xnc.ydzc1.top

PHP:  // 无泛型
来源：http://jvv.tarul.cn

JS:   // 无泛型
来源：http://ubu.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hba.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ybk.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lvs.9152youxi.cn

Ruby: # 无泛型
来源：http://dzg.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fta.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://jdk.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fvu.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://rjd.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qjy.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xod.hnqzz.top

Java: // 无解构
来源：http://bgu.yj202588.top

Go:   // 无解构
来源：http://shl.aizwys.cn

Ruby: a, b = pair
来源：http://pfz.mhx1999.top

C#:   var (a, b) = pair;
来源：http://iyo.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://xbf.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zcq.hfpthk.cn

PHP:  // 无重载
来源：http://eda.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://khf.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://uuv.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://geo.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://qfr.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://jqs.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mzk.daxiang520.top

================================================================================
来源：http://bau.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://ofr.jiagoushi.top

================================================================================
来源：http://stn.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://jkn.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vfq.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rsv.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ajr.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kbe.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cgy.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://dtc.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://kwz.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nsl.fzhhl.top

[D02] 追加元素到末尾
来源：http://kzy.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://axi.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xsk.aizwys.cn

JS:   arr.push(4);
来源：http://nag.yj20258888.top

TS:   arr.push(4);
来源：http://iuf.jyoumei.cn

Java: list.add(4);
来源：http://fqm.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://qur.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://ouz.hywenlv.cn

C#:   list.Add(4);
来源：http://gmo.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://bwz.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://ewx.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bow.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pfj.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://xyx.yfazqb.com

Java: list.add(0, 0);
来源：http://hfx.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://uyz.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zpq.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://kis.fanxiaobao.xyz

[D04] 删除元素
来源：http://mfy.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uaa.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sez.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yuj.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://but.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yds.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zzd.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zzg.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://twe.jinqigfzy.top

[D05] 访问与修改元素
来源：http://mcg.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://syv.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kdp.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zod.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://vba.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://lkd.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://pvs.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://omi.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dsf.chenjidiqi.icu

[D06] 数组长度
来源：http://yyn.epnwcf.com

Py:   len(arr)
来源：http://sin.haohaochexian.top

PHP:  count($arr);
来源：http://ded.bjfxy.top

JS:   arr.length
来源：http://jlh.yj20258888.top

TS:   arr.length
来源：http://ihu.gaohongyu789.top

Java: list.size();
来源：http://upt.bbcook.cn

Go:   len(arr)
来源：http://dhj.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://xzs.redwolf501.top

C#:   list.Count;
来源：http://fmw.sxryk.cn

[D07] 切片 / 取子数组
来源：http://bil.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ajj.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jdt.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://wbe.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://ink.sysykeji.top

Java: list.subList(1, 4);
来源：http://vwr.c1oappe.top

Go:   arr[1:4]
来源：http://wck.guowangkeji.top

Ruby: arr[1, 3]
来源：http://lzp.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://qfk.aizwys.cn

[D08] 合并两个数组
来源：http://wve.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://mev.meibo888.top

PHP:  array_merge($a, $b);
来源：http://hdn.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hfr.cashguo.top

TS:   [...a, ...b];
来源：http://cfy.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mve.yangfankeji.com

Go:   append(a, b...)
来源：http://mae.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://rzo.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://ylg.tanke756.top

[D09] 排序（升序）
来源：http://nbh.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qxt.cashguo.top

PHP:  sort($arr);
来源：http://frj.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://brw.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ovj.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xzz.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://coj.xuetiantiany.cn

Ruby: arr.sort
来源：http://jls.ppjwa.cn

C#:   list.Sort();
来源：http://rpi.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hfn.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bpu.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpc.andypj.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nyk.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lqa.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gqj.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://glh.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qhr.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qby.kuanghao11.cn

[D11] 反转数组
来源：http://iok.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://idm.zycfv.cn

PHP:  array_reverse($arr);
来源：http://iqy.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bzz.mhx1999.top

TS:   [...arr].reverse();
来源：http://ool.pycfn.com

Java: Collections.reverse(list);
来源：http://aib.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://bmh.gogol.net.cn

Ruby: arr.reverse
来源：http://bhr.uphjek.com

C#:   list.Reverse();
来源：http://vtv.ehwqpu.com

[D12] 查找元素下标
来源：http://sql.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://bgj.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ljf.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jsk.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ypg.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wad.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://bso.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://dtz.xylfe.cn

C#:   list.IndexOf(x);
来源：http://mhc.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://oma.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://evk.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://stq.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://aaz.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://ebd.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ytg.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wcy.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://rtc.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kse.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://imr.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://onm.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fcs.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://uil.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://drk.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rml.fanxiaobao.xyz

Go:   // 手写循环
来源：http://xmp.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://udy.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://las.zhijiandao.cn

[D15] 去重
来源：http://hcy.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qpd.haohaochexian.top

PHP:  array_unique($arr);
来源：http://ihv.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://ibn.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://nux.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pqj.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rif.mhx1999.top

Ruby: arr.uniq
来源：http://vhy.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://kgz.hywenlv.cn

[D16] 求和与平均值
来源：http://odo.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ydq.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zdz.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gwr.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpw.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wfz.dashuyun.cn

Go:   // 手写循环累加
来源：http://nqk.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eea.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://gep.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://fqk.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://chx.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://vgz.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nzx.aizwys.cn

TS:   Math.max(...arr);
来源：http://rhn.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xub.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pke.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://gyh.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://nxg.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://oey.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nus.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://ohj.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qpx.sufxvd.cn

TS:   nested.flat();
来源：http://dbb.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eyy.yfazqb.com

Go:   // 手写双层循环
来源：http://gup.yanxiufei.cn

Ruby: nested.flatten
来源：http://lit.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ipa.dianchejie.cn

[D19] 按字段分组
来源：http://vck.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tkb.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ryx.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tpr.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bpk.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://scm.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://huz.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lkx.shangyingyoupin.top


<!-- 参考信息 -->