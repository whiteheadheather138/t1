代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rdo.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrm.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kvv.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tah.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://glb.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xjw.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://jdj.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nty.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aqf.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ttc.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mfq.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://rlc.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://mfm.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://bgu.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://ncf.xinyue.icu

[C05] 返回多个值
来源：http://ljp.fehbvm.com

Py:   return a, b
来源：http://krj.sysykeji.top

PHP:  return [$a, $b];
来源：http://tpd.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wzi.pycfn.com

TS:   return { a, b };
来源：http://gte.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://koh.jqgfzy.top

Go:   return a, b
来源：http://vnn.hammf.cn

Ruby: return a, b
来源：http://bqt.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://rur.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://oxj.redwolf501.top

Py:   square = lambda x: x * x
来源：http://qgt.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wid.bbcook.cn

JS:   const square = x => x * x;
来源：http://hte.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://fic.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nwa.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uax.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://ncd.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fmq.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://wsh.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rrm.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://vbg.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://icv.ppjwa.cn

TS:   arr.map(String)
来源：http://gxc.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dqg.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kij.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://foo.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zxu.zhaomingkeji.xyz

[C08] 闭包
来源：http://rld.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ivu.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vev.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bdy.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ijj.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sjt.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jis.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dbg.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://meq.mhx1999.top

[C09] 递归
来源：http://gjt.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://apy.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kuo.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hdn.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gvv.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mvc.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sfh.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gfv.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mgc.guannengcc.top

[C10] 变量作用域
来源：http://kqq.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://twy.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cpy.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzf.daria6918.cn

TS:   同 JS
来源：http://rag.yj20258.top

Java: 方法内为块级作用域
来源：http://yua.yuanzhike.top

Go:   花括号块级作用域
来源：http://pzx.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wuz.xylfe.cn

C#:   块级作用域
来源：http://rci.haohaochexian.top

[C11] 模块导入与导出
来源：http://hsn.zhaomingkeji.xyz

Py:   from module import func
来源：http://xhj.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ixb.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vlc.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://brk.havefunace.top

Java: import java.util.List;
来源：http://kxc.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rox.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://abb.dianchejie.cn

C#:   using System.Text;
来源：http://dzl.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://cga.hammf.cn

Py:   (lambda: print("run"))()
来源：http://lhp.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://ktk.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://zqy.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://fgt.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jxc.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://jne.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://vuq.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bxg.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://zyx.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://azf.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rln.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cdh.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wom.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://lav.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://ccw.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://myn.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://wqn.havefunace.top

[C14] 泛型函数
来源：http://ihg.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://grk.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://lrs.andypj.xyz

JS:   // 无泛型
来源：http://bbg.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fez.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://knt.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cnq.birdmap.top

Ruby: # 无泛型
来源：http://jxr.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bkz.pycfn.com

[C15] 解构 / 展开参数
来源：http://boh.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zyd.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://gan.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vfz.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://puo.hnqzz.top

Java: // 无解构
来源：http://tyv.tanke756.top

Go:   // 无解构
来源：http://prs.hysaishi.cn

Ruby: a, b = pair
来源：http://pax.tarul.cn

C#:   var (a, b) = pair;
来源：http://dyv.yj20258888.top

[C16] 函数 / 方法重载
来源：http://tok.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzw.zhengqikj.top

PHP:  // 无重载
来源：http://zyf.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tih.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://elx.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hhx.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://pro.ivvv.top

Ruby: # 无重载：靠动态参数
来源：http://mag.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nuo.shuidangran.top

================================================================================
来源：http://xqg.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://iys.hnxiangtu.top

================================================================================
来源：http://tgq.52xcode.cn

[D01] 创建数组 / 列表
来源：http://kxp.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qys.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://apz.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dhq.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pgx.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://neh.zhoulong.xyz

Go:   arr := []int{1, 2, 3}
来源：http://exn.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://wvb.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vyz.ydzc1.top

[D02] 追加元素到末尾
来源：http://kgp.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ebj.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zdc.yonumen.top

JS:   arr.push(4);
来源：http://njf.hcnkem.com

TS:   arr.push(4);
来源：http://omg.dashuyun.cn

Java: list.add(4);
来源：http://qjj.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://unu.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://lrb.sxryk.cn

C#:   list.Add(4);
来源：http://baz.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://xeg.tanke756.top

Py:   arr.insert(0, 0)
来源：http://hlj.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wyf.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tha.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://mnu.zhoulong.xyz

Java: list.add(0, 0);
来源：http://gyp.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jev.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tux.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://ofa.cdnleiting.top

[D04] 删除元素
来源：http://xya.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xey.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dbb.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sbh.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://hcd.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tln.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zds.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ylf.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmo.yonumen.top

[D05] 访问与修改元素
来源：http://ghu.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://imx.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ffd.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://faz.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://yru.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://kcb.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://whr.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cms.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zob.jyoumei.cn

[D06] 数组长度
来源：http://tdd.fanxiaobao.xyz

Py:   len(arr)
来源：http://tzo.fengsongda.top

PHP:  count($arr);
来源：http://scd.hnqzz.top

JS:   arr.length
来源：http://pge.fzhhl.top

TS:   arr.length
来源：http://jhc.bjfxy.top

Java: list.size();
来源：http://tqq.52xcode.cn

Go:   len(arr)
来源：http://nde.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://grm.aibaodan.cn

C#:   list.Count;
来源：http://gle.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://wmf.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tpj.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://vwi.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://cai.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://dop.gogol.net.cn

Java: list.subList(1, 4);
来源：http://ezm.yongpay.top

Go:   arr[1:4]
来源：http://zvk.aibaodan.cn

Ruby: arr[1, 3]
来源：http://jou.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://npa.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://jms.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://edq.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://nmp.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://jwk.yj202588.top

TS:   [...a, ...b];
来源：http://dso.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kxo.yfazqb.com

Go:   append(a, b...)
来源：http://bla.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://xbx.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://ujg.cashguo.top

[D09] 排序（升序）
来源：http://nso.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://ibq.jyoumei.cn

PHP:  sort($arr);
来源：http://ilj.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ncs.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vso.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qbu.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zne.quarkkingdee.top

Ruby: arr.sort
来源：http://ehk.yonumen.top

C#:   list.Sort();
来源：http://mkm.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ynr.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zqk.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dct.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dra.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gvt.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gsl.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jbv.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://azz.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ido.zdqjudy.top

[D11] 反转数组
来源：http://zlx.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wzg.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://xtf.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dwc.guowangkeji.top

TS:   [...arr].reverse();
来源：http://lre.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://ahk.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://swr.sweek.top

Ruby: arr.reverse
来源：http://lpd.ydjk.org.cn

C#:   list.Reverse();
来源：http://ynx.chenzaomai.com

[D12] 查找元素下标
来源：http://cxm.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://gwa.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wsi.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://row.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://emy.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qte.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://ysb.jqgufenzy.top

Ruby: arr.index(x)
来源：http://hft.yfazqb.com

C#:   list.IndexOf(x);
来源：http://qkk.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://weq.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lfs.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qnp.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://vpr.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://euh.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qof.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wog.shangyingyoupin.top

Ruby: arr.select { |x| x > 3 }
来源：http://zfx.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://olb.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://cst.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pkk.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hdx.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://scf.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://rze.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jzy.ybcxt.top

Go:   // 手写循环
来源：http://uoy.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tuh.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fei.uphjek.com

[D15] 去重
来源：http://xpq.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qay.nanxinkj.top

PHP:  array_unique($arr);
来源：http://oyh.fzhhl.top

JS:   [...new Set(arr)]
来源：http://ujw.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://cca.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mhd.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xda.tianlin.xyz

Ruby: arr.uniq
来源：http://axp.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://pqq.kuanghao11.cn

[D16] 求和与平均值
来源：http://gnp.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tgd.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kgu.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gia.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vaq.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dhs.jianghu66.top

Go:   // 手写循环累加
来源：http://fse.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qdr.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://cwp.chenzaomai.com

[D17] 最大值与最小值
来源：http://isf.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://prk.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://nmc.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://onm.hesvh.cn

TS:   Math.max(...arr);
来源：http://pwt.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jjv.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qhm.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://frd.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://hba.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://vpw.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tdf.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://odd.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ftq.smart0.xyz

TS:   nested.flat();
来源：http://apv.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uxn.ivvv.top

Go:   // 手写双层循环
来源：http://rkc.aizwys.cn

Ruby: nested.flatten
来源：http://bei.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://umx.tian-w.cn

[D19] 按字段分组
来源：http://dps.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qvc.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cua.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gzi.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xke.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://arz.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://lsh.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ozo.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gdx.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://alf.aibaodan.cn

Py:   Counter(arr)
来源：http://vrh.yfazqb.com

PHP:  array_count_values($arr);
来源：http://msv.andypj.xyz


<!-- 参考信息 -->