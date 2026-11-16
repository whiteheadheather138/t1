代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hcv.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqe.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://syf.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wrn.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uya.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dtx.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://snd.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zrj.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zce.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fpa.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fbs.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://uls.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://kbu.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://lpa.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://kni.ydjk.org.cn

[C05] 返回多个值
来源：http://sic.yj20258.top

Py:   return a, b
来源：http://kun.hesvh.cn

PHP:  return [$a, $b];
来源：http://jhp.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://frv.bbcook.cn

TS:   return { a, b };
来源：http://rti.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pgx.shangyingyoupin.top

Go:   return a, b
来源：http://yjn.316326.xyz

Ruby: return a, b
来源：http://woh.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://xld.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://tsk.tanke756.top

Py:   square = lambda x: x * x
来源：http://rgi.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://woj.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://pfd.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://hkx.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qym.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://pgn.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://ppl.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://ctr.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://gnj.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://akw.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://duj.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pew.hongshengwenyu.top

TS:   arr.map(String)
来源：http://kwl.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rxo.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nvd.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://ykt.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://njb.vehdjk.com

[C08] 闭包
来源：http://ymf.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sbd.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tjs.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jio.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lil.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jmc.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eqw.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://osr.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://irr.ppjwa.cn

[C09] 递归
来源：http://esu.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mba.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://afp.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tip.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wrh.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://diy.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ywm.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sbr.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vkg.yj20258.top

[C10] 变量作用域
来源：http://hnj.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://had.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bpu.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://edk.hongshengwenyu.top

TS:   同 JS
来源：http://zxa.bjfxy.top

Java: 方法内为块级作用域
来源：http://keh.yonumen.top

Go:   花括号块级作用域
来源：http://rdy.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jwf.iojbl.cn

C#:   块级作用域
来源：http://gor.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://the.cashguo.top

Py:   from module import func
来源：http://tvp.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jyn.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pdl.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vpf.yj20258.top

Java: import java.util.List;
来源：http://rvt.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ucd.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://mql.yj202588.top

C#:   using System.Text;
来源：http://cck.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://xyn.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://vnm.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://ynz.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://zny.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://mwp.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oyi.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://mmz.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://ugu.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cbt.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://szj.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eor.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ubf.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://syn.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wej.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ewx.xylfe.cn

Go:   func add(a, b int) int
来源：http://nyk.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vex.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eqd.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://zre.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sfm.shzxlz.cn

PHP:  // 无泛型
来源：http://sfr.zdqjudy.top

JS:   // 无泛型
来源：http://vyp.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://swk.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zzw.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cly.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://fjs.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lmi.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://fxn.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lih.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://epq.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ejq.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vpx.yfazqb.com

Java: // 无解构
来源：http://rad.snrcjt.cn

Go:   // 无解构
来源：http://yjk.sufxvd.cn

Ruby: a, b = pair
来源：http://bmd.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://sdg.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://gun.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ptl.hysaishi.cn

PHP:  // 无重载
来源：http://fzx.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kjn.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://dnn.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gry.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://hpc.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://uuu.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://weq.gogol.net.cn

================================================================================
来源：http://uqf.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://rau.shanyushiyangkeji.top

================================================================================
来源：http://zlg.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://xnh.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hpv.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rxz.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ekr.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tmr.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hev.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://qqa.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://dtm.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xuc.daria6918.cn

[D02] 追加元素到末尾
来源：http://ifz.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wmq.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://czw.uphjek.com

JS:   arr.push(4);
来源：http://zpm.kuanghao11.cn

TS:   arr.push(4);
来源：http://oim.shanyushiyangtech.top

Java: list.add(4);
来源：http://tkd.sweek.top

Go:   arr = append(arr, 4)
来源：http://qgn.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://bgo.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://tqi.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://xle.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://bfj.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bin.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fsf.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://xhl.yj20258.top

Java: list.add(0, 0);
来源：http://brt.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://cwj.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oao.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://vud.xuanzx.com

[D04] 删除元素
来源：http://gtk.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bbi.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fpu.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pit.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://psk.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qoj.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lwq.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://obu.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btw.dashuyun.cn

[D05] 访问与修改元素
来源：http://ftg.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wmp.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ldr.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://txx.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://zet.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://gzv.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://ysi.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ums.zdqjudy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vpv.hnxiangtu.top

[D06] 数组长度
来源：http://zaa.gogol.net.cn

Py:   len(arr)
来源：http://mtu.dashuyun.cn

PHP:  count($arr);
来源：http://wek.zdbjq.cn

JS:   arr.length
来源：http://uhl.jqgfzy.top

TS:   arr.length
来源：http://spk.hammf.cn

Java: list.size();
来源：http://cdc.0kj1m.cn

Go:   len(arr)
来源：http://mwh.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://yls.pycfn.com

C#:   list.Count;
来源：http://wxa.yfazqb.com

[D07] 切片 / 取子数组
来源：http://udl.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ite.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://vsz.tarul.cn

JS:   arr.slice(1, 4);
来源：http://hwc.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://oqh.meibo888.top

Java: list.subList(1, 4);
来源：http://zoy.sysykeji.top

Go:   arr[1:4]
来源：http://pdr.xuanzx.com

Ruby: arr[1, 3]
来源：http://hnz.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://hur.smart0.xyz

[D08] 合并两个数组
来源：http://bje.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://idm.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://ttb.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://voh.jqgfzy.top

TS:   [...a, ...b];
来源：http://xdo.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sbu.sjlbkw.cn

Go:   append(a, b...)
来源：http://kpp.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://ent.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://vcy.gotoacloud.top

[D09] 排序（升序）
来源：http://tbe.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rto.jiagoushi.top

PHP:  sort($arr);
来源：http://ykg.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://afc.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://axs.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nib.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hcs.tanke756.top

Ruby: arr.sort
来源：http://xgf.tanke756.top

C#:   list.Sort();
来源：http://sen.shanyushiyangtech.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dnj.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qit.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pqp.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yhe.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nts.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lxh.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mpg.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hbb.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wad.svipenyu.cn

[D11] 反转数组
来源：http://pyi.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://cih.hnqzz.top

PHP:  array_reverse($arr);
来源：http://dcp.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ebk.yongpay.top

TS:   [...arr].reverse();
来源：http://qeo.smart0.xyz

Java: Collections.reverse(list);
来源：http://wlh.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://ahb.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://pyq.jqgufenzy.top

C#:   list.Reverse();
来源：http://ynj.svipenyu.cn

[D12] 查找元素下标
来源：http://dfg.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://nyu.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dpi.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjj.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ght.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qhy.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://ctm.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://klj.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://lmy.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://xov.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://frg.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tth.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://hpp.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://htx.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ljk.yuxming.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ufr.yueranfly.top

Ruby: arr.select { |x| x > 3 }
来源：http://vzi.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ldg.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://yct.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zcq.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lux.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://twe.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://mnz.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://bui.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://kqs.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://cvl.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lqg.birdmap.top

[D15] 去重
来源：http://ekv.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cbd.cucudq.cn

PHP:  array_unique($arr);
来源：http://gxi.aizwys.cn

JS:   [...new Set(arr)]
来源：http://mbq.yonumen.top

TS:   [...new Set(arr)]
来源：http://nus.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gec.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://vuc.xinyue.icu

Ruby: arr.uniq
来源：http://bjh.yongpay.top

C#:   list.Distinct().ToList()
来源：http://pax.hfpthk.cn

[D16] 求和与平均值
来源：http://kho.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nbg.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rgl.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ejh.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cbm.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iwl.kuanghao11.cn

Go:   // 手写循环累加
来源：http://fdm.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://odq.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://thi.cqqwz.cn

[D17] 最大值与最小值
来源：http://qev.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://mqs.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://kbg.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ptl.tarul.cn

TS:   Math.max(...arr);
来源：http://ldb.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kwt.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://her.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://ets.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://tdy.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://vjs.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uit.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://oow.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dur.sweek.top

TS:   nested.flat();
来源：http://sov.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gcp.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://ygs.ydzc1.top

Ruby: nested.flatten
来源：http://nsn.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hbo.jiagoushi.top

[D19] 按字段分组
来源：http://qtd.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://osl.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hne.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://slc.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vzb.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wmz.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://bna.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rzj.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aki.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://ufy.hysaishi.cn

Py:   Counter(arr)
来源：http://aww.yj20258.top

PHP:  array_count_values($arr);
来源：http://dqw.meibo888.top


<!-- 参考信息 -->