代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://mbr.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://emr.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://ogn.xuetiantiany.cn

[C05] 返回多个值
来源：http://tnm.zhaomingkeji.xyz

Py:   return a, b
来源：http://kve.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://mym.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xew.chenjidiqi.icu

TS:   return { a, b };
来源：http://pgh.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vcp.aizwys.cn

Go:   return a, b
来源：http://feu.jianghu66.top

Ruby: return a, b
来源：http://yim.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://wyi.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://eyw.xylfe.cn

Py:   square = lambda x: x * x
来源：http://wzr.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hoe.zhengqikj.top

JS:   const square = x => x * x;
来源：http://btk.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://qsf.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nyn.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://kxx.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://gxf.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://fvw.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://tiu.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nmu.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://svp.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://din.hywenlv.cn

TS:   arr.map(String)
来源：http://qdi.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ppy.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ttg.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://jdo.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qdy.hfpthk.cn

[C08] 闭包
来源：http://eiu.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bda.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jpa.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lnr.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uwr.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qrq.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qky.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sww.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kpf.yuanzhike.top

[C09] 递归
来源：http://wzw.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xwl.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mrv.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihu.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gyx.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://llz.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nqq.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://slg.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lbm.316326.xyz

[C10] 变量作用域
来源：http://zhx.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jej.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qnr.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fgf.9152youxi.cn

TS:   同 JS
来源：http://txi.zhixingplan.top

Java: 方法内为块级作用域
来源：http://kmj.zdqjudy.top

Go:   花括号块级作用域
来源：http://esp.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pyq.ivvv.top

C#:   块级作用域
来源：http://wac.sjlbkw.cn

[C11] 模块导入与导出
来源：http://xfd.gzhubu.top

Py:   from module import func
来源：http://goz.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yal.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zgo.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://huh.zhoulong.xyz

Java: import java.util.List;
来源：http://epy.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gez.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://cwa.zdbjq.cn

C#:   using System.Text;
来源：http://hna.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://afk.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://jzh.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://udi.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://ylr.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://cxg.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://udh.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://mof.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://wlg.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wdx.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://nol.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ikv.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmq.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://crs.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ofy.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nwp.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://vvo.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eje.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://twr.smart0.xyz

[C14] 泛型函数
来源：http://nue.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tfh.uphjek.com

PHP:  // 无泛型
来源：http://ayt.zdqjudy.top

JS:   // 无泛型
来源：http://keh.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bdx.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gev.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ual.hfpthk.cn

Ruby: # 无泛型
来源：http://ugd.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cbi.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://vnt.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://arn.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://fwy.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fcc.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yag.cdnleiting.top

Java: // 无解构
来源：http://nvv.xylfe.cn

Go:   // 无解构
来源：http://wwi.bjfxy.top

Ruby: a, b = pair
来源：http://waz.hammf.cn

C#:   var (a, b) = pair;
来源：http://aku.cashguo.top

[C16] 函数 / 方法重载
来源：http://qpg.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nck.ydzc1.top

PHP:  // 无重载
来源：http://hne.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://utj.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://vwr.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vrm.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://dsx.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://dyd.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lgq.xingfuxueyuan.xyz

================================================================================
来源：http://mco.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://nay.dashuyun.cn

================================================================================
来源：http://mmh.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://exy.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yuj.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lic.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qjm.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mjy.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://srr.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://xvs.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://xyu.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yen.svipenyu.cn

[D02] 追加元素到末尾
来源：http://xxi.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://apw.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://obv.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://fal.tarul.cn

TS:   arr.push(4);
来源：http://epi.jinghuilouyu.cn

Java: list.add(4);
来源：http://ylg.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://ler.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://vnk.ivvv.top

C#:   list.Add(4);
来源：http://lgx.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://lkn.uphjek.com

Py:   arr.insert(0, 0)
来源：http://ygg.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cds.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eyo.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://byk.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://zih.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://och.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://arg.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://ldn.hcnkem.com

[D04] 删除元素
来源：http://vsy.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hkf.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://msg.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iod.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://onk.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qzo.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dss.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://trs.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gww.nanxuanxn.top

[D05] 访问与修改元素
来源：http://qqp.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://erz.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://svc.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ljc.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://kuz.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://stc.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://xmu.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://paq.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ouo.jinqigufen.top

[D06] 数组长度
来源：http://tvk.zdqjudy.top

Py:   len(arr)
来源：http://zjq.jyoumei.cn

PHP:  count($arr);
来源：http://hyv.chenjidiqi.icu

JS:   arr.length
来源：http://deh.xziqi.cn

TS:   arr.length
来源：http://yka.yuxming.cn

Java: list.size();
来源：http://tln.guannengcc.top

Go:   len(arr)
来源：http://ulg.yj20258.top

Ruby: arr.length; arr.size
来源：http://xgt.aizwys.cn

C#:   list.Count;
来源：http://hic.tarul.cn

[D07] 切片 / 取子数组
来源：http://gqo.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tsd.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ryz.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://obl.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://fkh.jiagoushi.top

Java: list.subList(1, 4);
来源：http://dvj.cashguo.top

Go:   arr[1:4]
来源：http://czt.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://jxl.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://gtm.yvedp.cn

[D08] 合并两个数组
来源：http://kzh.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://mdc.yonumen.top

PHP:  array_merge($a, $b);
来源：http://trz.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xxc.shuidangran.top

TS:   [...a, ...b];
来源：http://yxg.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cyw.guannengcc.top

Go:   append(a, b...)
来源：http://bjt.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://qps.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://gqo.yfazqb.com

[D09] 排序（升序）
来源：http://byx.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://bmg.tianlin.xyz

PHP:  sort($arr);
来源：http://fkj.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yjb.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jge.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zqh.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lvz.zdqjudy.top

Ruby: arr.sort
来源：http://nki.yj202588.top

C#:   list.Sort();
来源：http://wsj.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kck.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sha.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wvu.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ypy.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tmb.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mim.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://szn.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bcr.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kwx.yj202588.top

[D11] 反转数组
来源：http://bsc.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://aom.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://rkc.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hfq.chenlongwang.top

TS:   [...arr].reverse();
来源：http://cpw.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://yzn.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://pmb.xziqi.cn

Ruby: arr.reverse
来源：http://cql.feifeiyinyue.top

C#:   list.Reverse();
来源：http://czx.tarul.cn

[D12] 查找元素下标
来源：http://uvb.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://fhc.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xxp.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyp.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qne.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vla.cheryme.top

Go:   slices.Index(arr, x)
来源：http://fqd.yfazqb.com

Ruby: arr.index(x)
来源：http://sss.gzhubu.top

C#:   list.IndexOf(x);
来源：http://rar.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://lxe.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zsy.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gob.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://fat.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://rmq.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://emu.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dbd.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://naq.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ten.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://chd.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://flm.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lmo.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://wrz.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://erp.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eqw.9152youxi.cn

Go:   // 手写循环
来源：http://ztl.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://siy.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sbo.sxryk.cn

[D15] 去重
来源：http://vnn.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bnz.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://zfz.daxiang520.top

JS:   [...new Set(arr)]
来源：http://qzy.tarul.cn

TS:   [...new Set(arr)]
来源：http://fjq.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ysf.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ark.jyoumei.cn

Ruby: arr.uniq
来源：http://hxl.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://mgt.sxryk.cn

[D16] 求和与平均值
来源：http://oyb.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kxh.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mlu.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzz.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://khj.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mly.epnwcf.com

Go:   // 手写循环累加
来源：http://ecy.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wii.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://fyg.gotoacloud.top

[D17] 最大值与最小值
来源：http://jhw.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://gfi.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://jav.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wgn.jianghu66.top

TS:   Math.max(...arr);
来源：http://llh.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jfx.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xxz.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://caq.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://opb.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://bwd.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tal.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://erz.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eua.yueranfly.top

TS:   nested.flat();
来源：http://rlq.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tez.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://aiw.epnwcf.com

Ruby: nested.flatten
来源：http://ixn.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ciz.bbcook.cn

[D19] 按字段分组
来源：http://lso.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://arl.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zrp.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fmh.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvx.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://itk.sweek.top

Go:   // 手写 map[string][]T
来源：http://skc.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://idb.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ntq.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://rlt.ehwqpu.com

Py:   Counter(arr)
来源：http://nkq.yonumen.top

PHP:  array_count_values($arr);
来源：http://pna.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyw.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvc.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kpg.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://eps.zycfv.cn

Ruby: arr.tally
来源：http://rvs.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bwd.yvedp.cn

[D21] 判断是否包含某元素
来源：http://epi.bbcook.cn

Py:   x in arr
来源：http://pjb.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://skx.yueranfly.top

JS:   arr.includes(x)
来源：http://qzi.xziqi.cn

TS:   arr.includes(x)
来源：http://pro.ydjk.org.cn

Java: list.contains(x)
来源：http://rqj.9152youxi.cn


<!-- 参考信息 -->