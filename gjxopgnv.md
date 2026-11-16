代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uyp.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bxz.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fmr.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vgc.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://hrz.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://she.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://evj.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rjc.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://agn.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dsc.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lgp.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://jnv.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://iaq.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://iml.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://ljq.shuidangran.top

[C05] 返回多个值
来源：http://puv.chenzaomai.com

Py:   return a, b
来源：http://daq.ivvv.top

PHP:  return [$a, $b];
来源：http://xct.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xlf.guannengcc.top

TS:   return { a, b };
来源：http://urr.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dje.guowangkeji.top

Go:   return a, b
来源：http://jfo.vehdjk.com

Ruby: return a, b
来源：http://ceo.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://qkp.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://hdd.guannengcc.top

Py:   square = lambda x: x * x
来源：http://oih.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://obx.meibo888.top

JS:   const square = x => x * x;
来源：http://fos.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://ejv.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pyc.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://pqx.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://grt.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bjv.fktsv.cn

[C07] 把函数作为参数传入
来源：http://clu.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zyo.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qwv.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jrf.cqqwz.cn

TS:   arr.map(String)
来源：http://kee.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cmz.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvi.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://jij.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rid.yfazqb.com

[C08] 闭包
来源：http://kgt.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gkg.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vec.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gdg.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fkv.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vhm.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xkj.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wfw.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ahh.guannengcc.top

[C09] 递归
来源：http://sgq.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pjt.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qgs.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwb.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qyf.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fmm.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ujb.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xnb.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://llg.bjfxy.top

[C10] 变量作用域
来源：http://cdi.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kmv.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hgn.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ztd.daria6918.cn

TS:   同 JS
来源：http://fem.smart0.xyz

Java: 方法内为块级作用域
来源：http://wgg.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://lys.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dpy.xuanzx.com

C#:   块级作用域
来源：http://hmo.shzxlz.cn

[C11] 模块导入与导出
来源：http://kux.hesvh.cn

Py:   from module import func
来源：http://fxq.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://orh.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqo.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pau.cucudq.cn

Java: import java.util.List;
来源：http://jyw.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tfj.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://prz.gaohongyu789.top

C#:   using System.Text;
来源：http://iah.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://avi.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://gmj.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://nwb.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://ozs.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://ltg.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pcr.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://bmh.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://nsy.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ruj.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://dhd.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tvf.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dgz.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pav.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqy.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://olj.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://bhd.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hgu.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://exu.iojbl.cn

[C14] 泛型函数
来源：http://xzw.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pgn.cucudq.cn

PHP:  // 无泛型
来源：http://jgf.jqgfzy.top

JS:   // 无泛型
来源：http://cxz.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rbu.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jle.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qjg.jinqigfzy.top

Ruby: # 无泛型
来源：http://kkl.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vuk.cucudq.cn

[C15] 解构 / 展开参数
来源：http://atp.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ltu.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://qty.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uqu.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wgi.snrcjt.cn

Java: // 无解构
来源：http://jwb.shanyushiyangkeji.top

Go:   // 无解构
来源：http://ebk.yj202588.top

Ruby: a, b = pair
来源：http://mxa.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://yjk.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://loi.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dzi.vehdjk.com

PHP:  // 无重载
来源：http://tog.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ljv.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://ymc.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rhh.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://lnd.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://yam.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://tzg.zhongyouzk.top

================================================================================
来源：http://ufr.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://cdw.bbcook.cn

================================================================================
来源：http://vfd.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://xps.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dmu.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fck.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baa.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fcz.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qbp.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://bzi.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://yms.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oqr.9152youxi.cn

[D02] 追加元素到末尾
来源：http://xex.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zck.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vxa.bjfxy.top

JS:   arr.push(4);
来源：http://vvl.zhiwuduotai.top

TS:   arr.push(4);
来源：http://aor.chenlongwang.top

Java: list.add(4);
来源：http://wow.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://nes.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://iac.gogol.net.cn

C#:   list.Add(4);
来源：http://mrq.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://ofd.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://tsn.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mii.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://knn.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://gmq.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://dct.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://zbx.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fgn.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://wxz.xuetiantiany.cn

[D04] 删除元素
来源：http://vsw.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tzb.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ibi.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tse.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://uzo.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uzy.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wtd.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lhm.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yjk.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://cqm.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yuv.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rkj.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://imj.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://iyh.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://iui.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://vll.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hii.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jah.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://mjx.xylfe.cn

Py:   len(arr)
来源：http://dje.ctjpmb.com

PHP:  count($arr);
来源：http://uqh.hfpthk.cn

JS:   arr.length
来源：http://quf.xylfe.cn

TS:   arr.length
来源：http://ole.zhiwuduotai.top

Java: list.size();
来源：http://bop.c1oappe.top

Go:   len(arr)
来源：http://jan.ydzc1.top

Ruby: arr.length; arr.size
来源：http://ccn.zhixingplan.top

C#:   list.Count;
来源：http://gfd.birdmap.top

[D07] 切片 / 取子数组
来源：http://nkw.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cal.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iqw.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://dsv.sweek.top

TS:   arr.slice(1, 4);
来源：http://xmg.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://ttz.xuanzx.com

Go:   arr[1:4]
来源：http://zfv.0kj1m.cn

Ruby: arr[1, 3]
来源：http://ikd.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://hgo.feifeiyinyue.top

[D08] 合并两个数组
来源：http://iwd.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://pli.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://enq.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fix.mhx1999.top

TS:   [...a, ...b];
来源：http://cau.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pbh.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://nmv.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://bvx.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://tpj.kuanghao11.cn

[D09] 排序（升序）
来源：http://dhm.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://gep.nanxinkj.top

PHP:  sort($arr);
来源：http://mrh.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ojr.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dsj.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://kaf.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ohm.sxryk.cn

Ruby: arr.sort
来源：http://ikb.jinghuilouyu.cn

C#:   list.Sort();
来源：http://mrh.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://aid.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cyw.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sij.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ayi.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xkz.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dwn.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://czs.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hof.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bvw.hammf.cn

[D11] 反转数组
来源：http://ygo.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://whf.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://trx.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gwl.guowangkeji.top

TS:   [...arr].reverse();
来源：http://cbp.shzxlz.cn

Java: Collections.reverse(list);
来源：http://coi.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://lco.zdbjq.cn

Ruby: arr.reverse
来源：http://slj.guowangkeji.top

C#:   list.Reverse();
来源：http://sdg.quarkkingdee.top

[D12] 查找元素下标
来源：http://dbg.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://xcs.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zxw.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wxx.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cyy.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kna.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://xic.sufxvd.cn

Ruby: arr.index(x)
来源：http://fiu.xylfe.cn

C#:   list.IndexOf(x);
来源：http://flo.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://jbe.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lly.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mbs.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://ban.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://mlu.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ydw.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hsd.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://lqv.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xye.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://bwd.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nto.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zpa.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://jkk.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://rnj.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bkv.jqgufenzy.top

Go:   // 手写循环
来源：http://rob.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fqe.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://szw.aibaodan.cn

[D15] 去重
来源：http://hut.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qkd.smart0.xyz

PHP:  array_unique($arr);
来源：http://dmq.bbcook.cn

JS:   [...new Set(arr)]
来源：http://hkt.mhx1999.top

TS:   [...new Set(arr)]
来源：http://ymc.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zru.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://ebs.xziqi.cn

Ruby: arr.uniq
来源：http://rgy.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://izz.cdnleiting.top

[D16] 求和与平均值
来源：http://wrt.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ukd.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wdx.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vkx.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dhl.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uej.yuanzhike.top

Go:   // 手写循环累加
来源：http://fkx.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cun.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://uuj.fzhhl.top

[D17] 最大值与最小值
来源：http://zko.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://phr.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://xuy.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mrq.hfpthk.cn

TS:   Math.max(...arr);
来源：http://ivw.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://zpg.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ayd.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://rsv.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://ucn.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://gsb.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bpy.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://grk.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://naf.epnwcf.com

TS:   nested.flat();
来源：http://jsn.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qzr.ppjwa.cn

Go:   // 手写双层循环
来源：http://pfw.yanxiufei.cn

Ruby: nested.flatten
来源：http://ehc.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yrr.meibo888.top

[D19] 按字段分组
来源：http://jco.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wry.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://air.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vzk.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://myo.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kgk.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://ffu.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qpb.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cuv.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://lgb.chenlongwang.top

Py:   Counter(arr)
来源：http://qtu.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://vgd.daxiang520.top


<!-- 参考信息 -->