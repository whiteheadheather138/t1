代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://fbu.hcnkem.com

[C03] 可变参数
来源：http://zmz.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://bln.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ekj.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibh.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://udr.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gqr.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ewd.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dzg.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yzj.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://zyu.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bih.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://guf.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mcm.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zae.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://els.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://hrj.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://djv.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://oom.yongpay.top

[C05] 返回多个值
来源：http://kvl.pengpengdd.cyou

Py:   return a, b
来源：http://cqx.c1oappe.top

PHP:  return [$a, $b];
来源：http://qsn.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eer.daxiang520.top

TS:   return { a, b };
来源：http://eis.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zds.sjlbkw.cn

Go:   return a, b
来源：http://hbm.ybcxt.top

Ruby: return a, b
来源：http://nfl.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://kml.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://uit.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://mtz.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cnq.yuanzhike.top

JS:   const square = x => x * x;
来源：http://qza.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://lro.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jnk.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ocg.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://kti.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://egy.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://vhd.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://awb.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://uvh.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xpy.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://jrl.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nwr.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lcl.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://com.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uyf.sjlbkw.cn

[C08] 闭包
来源：http://eac.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yqr.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nih.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uoi.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qyr.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nrt.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pds.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ocd.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bek.shangyingyoupin.top

[C09] 递归
来源：http://bzm.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jmr.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wka.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nsk.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fya.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://awu.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nft.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zbk.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ves.nanxuanxn.top

[C10] 变量作用域
来源：http://vyk.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lsg.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://saj.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rfn.zhoulong.xyz

TS:   同 JS
来源：http://fsv.svipenyu.cn

Java: 方法内为块级作用域
来源：http://fdt.gaohongyu789.top

Go:   花括号块级作用域
来源：http://hdu.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bqa.gzhubu.top

C#:   块级作用域
来源：http://ebr.nanxinkj.top

[C11] 模块导入与导出
来源：http://wmn.jianghu66.top

Py:   from module import func
来源：http://tuq.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fct.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://act.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tho.yonumen.top

Java: import java.util.List;
来源：http://efj.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tno.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://eql.ppjwa.cn

C#:   using System.Text;
来源：http://qph.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://jks.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://nfp.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://zks.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://qiv.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://iso.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://quq.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://cba.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://yzd.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qqj.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://tgm.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wsn.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tml.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eam.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pij.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://utv.haohaochexian.top

Go:   func add(a, b int) int
来源：http://dtn.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mvz.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bbk.fengsongda.top

[C14] 泛型函数
来源：http://nzh.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gud.0kj1m.cn

PHP:  // 无泛型
来源：http://svd.birdmap.top

JS:   // 无泛型
来源：http://ojs.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wmj.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://olw.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ytf.mhx1999.top

Ruby: # 无泛型
来源：http://ecq.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jcl.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://srg.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lva.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://lam.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xtt.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fhs.xuanzx.com

Java: // 无解构
来源：http://qgp.nanxuanxn.top

Go:   // 无解构
来源：http://pne.iojbl.cn

Ruby: a, b = pair
来源：http://oxd.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://gaj.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://taa.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iwr.tanke756.top

PHP:  // 无重载
来源：http://jnb.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oce.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://ekp.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ioq.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://vtj.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://efc.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yan.mhx1999.top

================================================================================
来源：http://hpo.sweek.top

D. 数组 / 列表 / 集合
来源：http://npf.hywenlv.cn

================================================================================
来源：http://xcw.birdmap.top

[D01] 创建数组 / 列表
来源：http://bxm.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zod.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kmv.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yqr.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://plc.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cdj.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://qyv.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://umj.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hhf.fktsv.cn

[D02] 追加元素到末尾
来源：http://qvy.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://udn.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cuc.yonumen.top

JS:   arr.push(4);
来源：http://kaw.jqgfzy.top

TS:   arr.push(4);
来源：http://web.sxryk.cn

Java: list.add(4);
来源：http://itf.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://kav.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://pxo.tanke756.top

C#:   list.Add(4);
来源：http://ubc.cucudq.cn

[D03] 在指定位置插入元素
来源：http://vhs.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://lpa.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sxo.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yll.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://svd.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://fwn.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yre.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://erb.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://gae.yfazqb.com

[D04] 删除元素
来源：http://cwb.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vme.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ysu.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jin.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://emq.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zue.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bja.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ndi.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cys.gotoacloud.top

[D05] 访问与修改元素
来源：http://ror.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qdm.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fdt.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fno.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://bwa.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://cbq.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://mps.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pdy.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://meq.hnqzz.top

[D06] 数组长度
来源：http://mjv.ydjk.org.cn

Py:   len(arr)
来源：http://etf.aizwys.cn

PHP:  count($arr);
来源：http://jgk.xuetiantiany.cn

JS:   arr.length
来源：http://dtw.ydzc1.top

TS:   arr.length
来源：http://zwy.ppjwa.cn

Java: list.size();
来源：http://aty.gaohongyu789.top

Go:   len(arr)
来源：http://oni.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://rgc.nwbrower.top

C#:   list.Count;
来源：http://asw.meibo888.top

[D07] 切片 / 取子数组
来源：http://rnm.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cxb.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ulx.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://wrp.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://jdm.chenzaomai.com

Java: list.subList(1, 4);
来源：http://kvf.hnqzz.top

Go:   arr[1:4]
来源：http://wbz.jyoumei.cn

Ruby: arr[1, 3]
来源：http://wev.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://xpg.guannengcc.top

[D08] 合并两个数组
来源：http://ylb.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://bqt.yongpay.top

PHP:  array_merge($a, $b);
来源：http://nlr.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pym.sjlbkw.cn

TS:   [...a, ...b];
来源：http://jna.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tvn.hnqzz.top

Go:   append(a, b...)
来源：http://myu.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://sfj.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://ule.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://gny.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://gdf.jianghu66.top

PHP:  sort($arr);
来源：http://dgv.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rhn.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qia.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vxr.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://crb.yueranfly.top

Ruby: arr.sort
来源：http://efi.zhongyouzk.top

C#:   list.Sort();
来源：http://hxm.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jxq.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uon.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bkr.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ygz.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jhz.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ekx.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://age.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hbr.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bdj.xuanzx.com

[D11] 反转数组
来源：http://vja.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://axl.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://bcf.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rbs.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://hnz.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://wfw.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://qhh.haohaochexian.top

Ruby: arr.reverse
来源：http://gpa.dashuyun.cn

C#:   list.Reverse();
来源：http://nui.gaohongyu789.top

[D12] 查找元素下标
来源：http://yon.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://wvj.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gsf.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ija.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lqq.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://upz.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://cjq.jinqigufen.top

Ruby: arr.index(x)
来源：http://pkd.iojbl.cn

C#:   list.IndexOf(x);
来源：http://gno.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://kbn.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xsg.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ino.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://hja.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://qov.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cja.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mgk.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://edv.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://qxt.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://wsx.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ngd.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zat.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://pov.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://wwv.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://utu.pycfn.com

Go:   // 手写循环
来源：http://ezf.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://eka.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oia.ctjpmb.com

[D15] 去重
来源：http://gsn.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yig.xziqi.cn

PHP:  array_unique($arr);
来源：http://gqx.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://rdx.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://ptf.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gzd.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://yee.feifeiyinyue.top

Ruby: arr.uniq
来源：http://ndu.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://zem.tianlin.xyz

[D16] 求和与平均值
来源：http://hje.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvs.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xar.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pvv.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iaa.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pex.nanxuanxn.top

Go:   // 手写循环累加
来源：http://nnh.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vnp.sweek.top

C#:   list.Sum();  list.Average()
来源：http://btl.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://vad.pycfn.com

Py:   max(arr);  min(arr)
来源：http://syl.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://wnf.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zsr.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://eis.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cfm.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cto.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://pcj.yonumen.top

C#:   list.Max();  list.Min()
来源：http://rpa.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://fpr.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vey.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://mml.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lcb.daria6918.cn

TS:   nested.flat();
来源：http://ijz.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rqz.xinyue.icu

Go:   // 手写双层循环
来源：http://spa.mhx1999.top

Ruby: nested.flatten
来源：http://igd.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://frp.birdmap.top

[D19] 按字段分组
来源：http://oph.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oxu.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rsk.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ywo.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mig.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tmx.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://new.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://qsk.havefunace.top


<!-- 参考信息 -->