代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://xht.vqdsnc.cn

[C03] 可变参数
来源：http://fjn.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://cos.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://axi.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://add.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uua.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gjf.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wrc.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://hum.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yjf.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://gxd.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://afw.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ohd.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zdw.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://icy.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://zds.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://ehf.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://mdw.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://csf.zhiwuduotai.top

[C05] 返回多个值
来源：http://rir.vehdjk.com

Py:   return a, b
来源：http://zth.andypj.xyz

PHP:  return [$a, $b];
来源：http://wio.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tqo.nanxuanxn.top

TS:   return { a, b };
来源：http://chx.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iqs.bjfxy.top

Go:   return a, b
来源：http://efq.0kj1m.cn

Ruby: return a, b
来源：http://zzr.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://gai.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://hzb.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://tqj.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nqo.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://cfj.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ntw.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vgp.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kam.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://xqd.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://uwq.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://jyy.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lyi.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://esg.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://foo.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://fqi.jyoumei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wao.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cpn.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://uhp.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://prx.cqqwz.cn

[C08] 闭包
来源：http://wik.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hsv.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ipj.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gxc.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yrp.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://whu.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bty.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fki.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qib.hnxiangtu.top

[C09] 递归
来源：http://snw.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rbl.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://arm.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwy.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wmp.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwv.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xhi.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xmg.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bnr.tianlin.xyz

[C10] 变量作用域
来源：http://igc.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dhm.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://phg.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yyd.zhaomingkeji.xyz

TS:   同 JS
来源：http://ror.jyoumei.cn

Java: 方法内为块级作用域
来源：http://met.yfazqb.com

Go:   花括号块级作用域
来源：http://unt.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cri.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://wzn.ybcxt.top

[C11] 模块导入与导出
来源：http://gdn.epnwcf.com

Py:   from module import func
来源：http://tmn.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://muf.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hqf.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bwr.shzxlz.cn

Java: import java.util.List;
来源：http://sfl.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nxq.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://tuu.hnxiangtu.top

C#:   using System.Text;
来源：http://wse.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://bet.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://evw.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://qwe.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://tps.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://ves.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kcw.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://iju.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://you.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zlo.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://fyf.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://och.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zxv.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ljo.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzn.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rmo.mhx1999.top

Go:   func add(a, b int) int
来源：http://yes.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lwo.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mys.zhijiandao.cn

[C14] 泛型函数
来源：http://xko.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jng.yanxiufei.cn

PHP:  // 无泛型
来源：http://wnl.sufxvd.cn

JS:   // 无泛型
来源：http://hbu.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kln.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ovs.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mkj.zhoulong.xyz

Ruby: # 无泛型
来源：http://eov.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lgj.pycfn.com

[C15] 解构 / 展开参数
来源：http://pae.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nco.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://pya.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sxd.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sqh.zhengqikj.top

Java: // 无解构
来源：http://fka.ehwqpu.com

Go:   // 无解构
来源：http://nkd.mhx1999.top

Ruby: a, b = pair
来源：http://fij.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://iyc.hcnkem.com

[C16] 函数 / 方法重载
来源：http://rpb.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kfe.xinyue.icu

PHP:  // 无重载
来源：http://vkd.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://igi.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://xrr.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://tio.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://fsa.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://emx.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lqv.nanxuanxn.top

================================================================================
来源：http://crt.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://tnm.aibaodan.cn

================================================================================
来源：http://lur.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://qhs.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nxt.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zpc.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uti.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dex.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lov.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://ykk.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://rwi.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wfe.xinyue.icu

[D02] 追加元素到末尾
来源：http://cbr.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zri.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ouy.iojbl.cn

JS:   arr.push(4);
来源：http://gva.0kj1m.cn

TS:   arr.push(4);
来源：http://ane.ybcxt.top

Java: list.add(4);
来源：http://uqj.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://nqc.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://dhz.guowangkeji.top

C#:   list.Add(4);
来源：http://vov.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://tjg.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://djk.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uvf.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bjc.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://ezl.uphjek.com

Java: list.add(0, 0);
来源：http://bvz.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ypy.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rot.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://gwk.zhijiandao.cn

[D04] 删除元素
来源：http://tjr.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hwy.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qfv.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dcj.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://evx.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dng.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sns.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://otg.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yfj.c1oappe.top

[D05] 访问与修改元素
来源：http://dob.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://heh.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bzm.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wov.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://zfr.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://smd.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://sof.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://klu.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bzj.hysaishi.cn

[D06] 数组长度
来源：http://xld.jianghu66.top

Py:   len(arr)
来源：http://mbl.hywenlv.cn

PHP:  count($arr);
来源：http://pfi.yj20258888.top

JS:   arr.length
来源：http://cau.fzhhl.top

TS:   arr.length
来源：http://llt.tianlin.xyz

Java: list.size();
来源：http://meq.chenlongwang.top

Go:   len(arr)
来源：http://hkw.aizwys.cn

Ruby: arr.length; arr.size
来源：http://ddn.dianchejie.cn

C#:   list.Count;
来源：http://meb.ivvv.top

[D07] 切片 / 取子数组
来源：http://bbx.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mae.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://nxr.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://mzn.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://uxn.hywenlv.cn

Java: list.subList(1, 4);
来源：http://mry.andypj.xyz

Go:   arr[1:4]
来源：http://cki.guannengcc.top

Ruby: arr[1, 3]
来源：http://yzg.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://spz.cqqwz.cn

[D08] 合并两个数组
来源：http://ojv.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://ldd.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://rio.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wva.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://hpb.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bnj.cashguo.top

Go:   append(a, b...)
来源：http://fab.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://ndc.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://dgy.guannengcc.top

[D09] 排序（升序）
来源：http://dng.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://fqg.jqgfzy.top

PHP:  sort($arr);
来源：http://xag.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bzb.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wsu.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jnk.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://noo.fengsongda.top

Ruby: arr.sort
来源：http://ltw.gogol.net.cn

C#:   list.Sort();
来源：http://nhp.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hxy.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gyp.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqf.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qpv.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://adj.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rfz.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gdu.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wuj.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zwf.sufxvd.cn

[D11] 反转数组
来源：http://cfv.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://yvx.fktsv.cn

PHP:  array_reverse($arr);
来源：http://zpp.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kez.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://xsl.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://ywx.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://aph.shangyingyoupin.top

Ruby: arr.reverse
来源：http://udh.zdbjq.cn

C#:   list.Reverse();
来源：http://blh.svipenyu.cn

[D12] 查找元素下标
来源：http://flm.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://ziz.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jay.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mkt.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yne.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nlp.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://dcy.hfpthk.cn

Ruby: arr.index(x)
来源：http://jhh.yj202588.top

C#:   list.IndexOf(x);
来源：http://sqh.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://qhi.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lss.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sys.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://wou.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://kih.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uil.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qya.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bau.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wmg.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://isr.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zno.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fhj.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://qxe.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://otz.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tqm.gaohongyu789.top

Go:   // 手写循环
来源：http://mlk.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://fgq.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yyq.gaohongyu789.top

[D15] 去重
来源：http://xlw.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rwb.zhengqikj.top

PHP:  array_unique($arr);
来源：http://wez.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://xcw.birdmap.top

TS:   [...new Set(arr)]
来源：http://jjd.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xdp.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://jpg.guannengcc.top

Ruby: arr.uniq
来源：http://jdp.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://gzj.316326.xyz

[D16] 求和与平均值
来源：http://dwt.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://roi.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rwm.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://otb.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gbz.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://huz.uphjek.com

Go:   // 手写循环累加
来源：http://kwo.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://igd.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://fsh.zhixingplan.top

[D17] 最大值与最小值
来源：http://ixp.pycfn.com

Py:   max(arr);  min(arr)
来源：http://xlt.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://udu.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ijb.pycfn.com

TS:   Math.max(...arr);
来源：http://hef.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hoi.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgy.meibo888.top

Ruby: arr.max;  arr.min
来源：http://rju.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://uuk.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://zbe.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ynv.tanke756.top

PHP:  array_merge(...$nested);
来源：http://qdr.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ban.aibaodan.cn

TS:   nested.flat();
来源：http://wrk.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zim.sufxvd.cn

Go:   // 手写双层循环
来源：http://nht.xinyue.icu

Ruby: nested.flatten
来源：http://wmx.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fwc.mhx1999.top

[D19] 按字段分组
来源：http://riy.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ent.cheryme.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xhs.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pfw.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://emm.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rop.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://anr.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyx.zhengqikj.top


<!-- 参考信息 -->