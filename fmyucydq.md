代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sme.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rja.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wje.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yvu.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://yqk.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gsv.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://ppu.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yut.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jwn.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ieq.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qwx.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://mln.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://rdh.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://cux.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://pbq.hysaishi.cn

[C05] 返回多个值
来源：http://for.gzhubu.top

Py:   return a, b
来源：http://ces.dianchejie.cn

PHP:  return [$a, $b];
来源：http://zfx.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://lfi.sysykeji.top

TS:   return { a, b };
来源：http://fhe.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yze.yj20258.top

Go:   return a, b
来源：http://dyu.yueranfly.top

Ruby: return a, b
来源：http://wjv.sufxvd.cn

C#:   return (a, b);              // ValueTuple
来源：http://zjb.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://hxk.sysykeji.top

Py:   square = lambda x: x * x
来源：http://dda.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rui.316326.xyz

JS:   const square = x => x * x;
来源：http://dxm.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://mpo.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://and.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bge.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://flm.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xgx.c1oappe.top

[C07] 把函数作为参数传入
来源：http://xvf.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://stj.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sfx.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://obw.yueranfly.top

TS:   arr.map(String)
来源：http://jqb.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://urh.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fhb.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://alg.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bno.quarkkingdee.top

[C08] 闭包
来源：http://buo.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xoa.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rza.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://csu.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qip.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://krp.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eqy.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dbr.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://llo.hammf.cn

[C09] 递归
来源：http://haz.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gow.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zil.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxk.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kag.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ltc.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gsp.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pcj.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ndx.chenjidiqi.icu

[C10] 变量作用域
来源：http://zjo.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qxw.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ecy.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zre.hesvh.cn

TS:   同 JS
来源：http://wlu.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://syx.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://eya.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fny.jinghuilouyu.cn

C#:   块级作用域
来源：http://mni.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://qcm.shangyingyoupin.top

Py:   from module import func
来源：http://was.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tqw.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pwm.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dfh.yj20258.top

Java: import java.util.List;
来源：http://srm.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wnq.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://yfp.havefunace.top

C#:   using System.Text;
来源：http://ftq.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://ush.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://vph.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://hlw.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://vsq.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://qpt.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kww.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://osb.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://rhw.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://mfw.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://zig.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ttv.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cai.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nxq.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ofd.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zal.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://ygb.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wie.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ebq.kuanghao11.cn

[C14] 泛型函数
来源：http://zup.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gow.yuxming.cn

PHP:  // 无泛型
来源：http://prv.shuidangran.top

JS:   // 无泛型
来源：http://nxr.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ske.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dlb.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://obr.chenjidiqi.icu

Ruby: # 无泛型
来源：http://gnd.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://arz.andypj.xyz

[C15] 解构 / 展开参数
来源：http://nkg.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bdq.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://kiy.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://enl.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uuq.jianghu66.top

Java: // 无解构
来源：http://bec.nanxinkj.top

Go:   // 无解构
来源：http://rli.cheryme.top

Ruby: a, b = pair
来源：http://xxp.fengsongda.top

C#:   var (a, b) = pair;
来源：http://qew.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://pdm.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://buf.gaohongyu789.top

PHP:  // 无重载
来源：http://hxb.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zvv.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://wbc.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pxi.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://ryy.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://qru.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ibu.zhijiandao.cn

================================================================================
来源：http://ihk.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://tay.gogol.net.cn

================================================================================
来源：http://hsa.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://itt.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zdq.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kee.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qbm.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://khc.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tvt.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://uws.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://jvp.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rum.sxryk.cn

[D02] 追加元素到末尾
来源：http://rnd.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://evw.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aam.fzhhl.top

JS:   arr.push(4);
来源：http://zja.yuanzhike.top

TS:   arr.push(4);
来源：http://hyn.xuanzx.com

Java: list.add(4);
来源：http://tyc.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://yly.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://xuz.redwolf501.top

C#:   list.Add(4);
来源：http://vwv.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://byi.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://zgc.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ugv.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://prc.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://dqt.sufxvd.cn

Java: list.add(0, 0);
来源：http://ufq.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vdy.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qhu.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://osa.sysykeji.top

[D04] 删除元素
来源：http://evs.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hsx.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://klf.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://buv.yongpay.top

TS:   arr.splice(0, 1);
来源：http://gkk.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://whc.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qxj.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aac.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://njt.hysaishi.cn

[D05] 访问与修改元素
来源：http://jrq.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ngy.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ntb.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jzz.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://ezv.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://ufr.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://jlr.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ywv.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://evs.xuetiantiany.cn

[D06] 数组长度
来源：http://ygz.cqqwz.cn

Py:   len(arr)
来源：http://yyb.ehwqpu.com

PHP:  count($arr);
来源：http://ktv.zdqjudy.top

JS:   arr.length
来源：http://ozp.316326.xyz

TS:   arr.length
来源：http://gdo.ctjpmb.com

Java: list.size();
来源：http://oiu.quarkkingdee.top

Go:   len(arr)
来源：http://gvh.gzhubu.top

Ruby: arr.length; arr.size
来源：http://yla.shanyushiyangkeji.top

C#:   list.Count;
来源：http://uwt.iojbl.cn

[D07] 切片 / 取子数组
来源：http://nhe.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vud.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jti.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://msv.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://iec.zdbjq.cn

Java: list.subList(1, 4);
来源：http://ykm.kuanghao11.cn

Go:   arr[1:4]
来源：http://nhr.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://ony.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://zxw.jqgfzy.top

[D08] 合并两个数组
来源：http://tmz.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://bpw.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://qcq.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kbr.kuanghao11.cn

TS:   [...a, ...b];
来源：http://rrv.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wip.xylfe.cn

Go:   append(a, b...)
来源：http://lvp.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://awp.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://zoy.jqgufenzy.top

[D09] 排序（升序）
来源：http://pye.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://dar.jianghu66.top

PHP:  sort($arr);
来源：http://ocr.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gqu.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vqj.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iny.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xxs.feifeiyinyue.top

Ruby: arr.sort
来源：http://aby.cucudq.cn

C#:   list.Sort();
来源：http://hag.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dgq.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fly.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwm.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iaj.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jlj.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yhz.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xni.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zvq.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nho.yuanzhike.top

[D11] 反转数组
来源：http://psy.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fni.iojbl.cn

PHP:  array_reverse($arr);
来源：http://jni.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pcu.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://uxo.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://kgn.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://iik.nanxuanxn.top

Ruby: arr.reverse
来源：http://baj.ehwqpu.com

C#:   list.Reverse();
来源：http://ooi.havefunace.top

[D12] 查找元素下标
来源：http://ltj.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://idy.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nst.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jkx.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csf.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://adg.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://cfp.jyoumei.cn

Ruby: arr.index(x)
来源：http://qot.meibo888.top

C#:   list.IndexOf(x);
来源：http://sec.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://nxl.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oaa.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jpf.bbcook.cn

JS:   arr.filter(x => x > 3)
来源：http://nnz.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://tax.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://epd.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jnn.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://bwx.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://skj.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://zsr.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uco.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ege.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://yba.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://cut.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvx.pycfn.com

Go:   // 手写循环
来源：http://rsy.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://smf.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wmy.shanyushiyangtech.top

[D15] 去重
来源：http://rrx.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jnx.xinyue.icu

PHP:  array_unique($arr);
来源：http://lot.yuxming.cn

JS:   [...new Set(arr)]
来源：http://emr.vehdjk.com

TS:   [...new Set(arr)]
来源：http://eoc.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sjo.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bfo.redwolf501.top

Ruby: arr.uniq
来源：http://jbk.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://yoi.meibo888.top

[D16] 求和与平均值
来源：http://vyf.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rzj.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yxg.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jej.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rma.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://txg.shuidangran.top

Go:   // 手写循环累加
来源：http://rsu.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xrc.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://fle.yuanzhike.top

[D17] 最大值与最小值
来源：http://raw.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://dam.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://nxb.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bng.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://bru.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kyx.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://igm.uphjek.com

Ruby: arr.max;  arr.min
来源：http://tlj.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://scc.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://csr.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gfr.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://dvl.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kam.smart0.xyz

TS:   nested.flat();
来源：http://shs.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ckv.hysaishi.cn

Go:   // 手写双层循环
来源：http://cti.jyoumei.cn

Ruby: nested.flatten
来源：http://gfp.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://akc.c1oappe.top

[D19] 按字段分组
来源：http://pbh.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lbs.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tpu.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ciu.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://rbs.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hyi.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://bjt.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bay.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://axi.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://xmf.hywenlv.cn

Py:   Counter(arr)
来源：http://pya.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://bsx.fehbvm.com


<!-- 参考信息 -->