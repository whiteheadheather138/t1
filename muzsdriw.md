代发 wailian999

Py:   return a, b
来源：http://tfc.gogol.net.cn

PHP:  return [$a, $b];
来源：http://yei.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qds.hysaishi.cn

TS:   return { a, b };
来源：http://waa.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jkh.c1oappe.top

Go:   return a, b
来源：http://mgw.xuetiantiany.cn

Ruby: return a, b
来源：http://dyw.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://snt.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://mgj.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://vhc.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aiu.nanxinkj.top

JS:   const square = x => x * x;
来源：http://vzn.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://bdg.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rbf.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nsd.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://esk.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://yis.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://seh.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nsw.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qhx.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ptl.jianghu66.top

TS:   arr.map(String)
来源：http://jyb.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://upq.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cnw.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://hle.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://prk.daxiang520.top

[C08] 闭包
来源：http://gwu.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bqr.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kvv.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lrp.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://con.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tuk.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oqx.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ups.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ifx.yanxiufei.cn

[C09] 递归
来源：http://icl.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dek.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rco.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhe.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://grj.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pgl.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aqm.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qxl.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qzq.snrcjt.cn

[C10] 变量作用域
来源：http://rxx.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://stm.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yhr.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://plo.quarkkingdee.top

TS:   同 JS
来源：http://pjs.yangfankeji.com

Java: 方法内为块级作用域
来源：http://gye.ivvv.top

Go:   花括号块级作用域
来源：http://vfy.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xbp.pycfn.com

C#:   块级作用域
来源：http://hee.yangfankeji.com

[C11] 模块导入与导出
来源：http://kdn.hcnkem.com

Py:   from module import func
来源：http://nou.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eql.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://enx.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://prm.pycfn.com

Java: import java.util.List;
来源：http://vpa.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kuy.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://gws.hywenlv.cn

C#:   using System.Text;
来源：http://bbc.zhijiandao.cn

[C12] 立即执行函数 IIFE
来源：http://bzd.sweek.top

Py:   (lambda: print("run"))()
来源：http://iik.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://cwp.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://shg.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://xtw.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ugj.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://duq.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://mge.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fmb.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://ylr.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vib.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gqg.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mrw.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvx.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://sbv.sysykeji.top

Go:   func add(a, b int) int
来源：http://iyw.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nht.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://uqw.gogol.net.cn

[C14] 泛型函数
来源：http://eum.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ckg.yj20258888.top

PHP:  // 无泛型
来源：http://gcz.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://xgx.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bcs.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qly.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dgm.zycfv.cn

Ruby: # 无泛型
来源：http://tvj.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kmc.yj20258.top

[C15] 解构 / 展开参数
来源：http://avi.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://prv.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://iaz.bjfxy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vfn.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ges.cashguo.top

Java: // 无解构
来源：http://mvw.andypj.xyz

Go:   // 无解构
来源：http://xjy.smart0.xyz

Ruby: a, b = pair
来源：http://vqu.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://dhp.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://bts.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hdb.yj20258.top

PHP:  // 无重载
来源：http://xxv.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wsa.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://dcs.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iwn.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://wgf.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://omy.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lgi.ywan-chungtsiang.top

================================================================================
来源：http://ecw.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://moh.andypj.xyz

================================================================================
来源：http://ngs.xuanzx.com

[D01] 创建数组 / 列表
来源：http://dui.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mpb.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cwk.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vry.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vnm.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wne.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://ppt.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://xcj.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gbx.xylfe.cn

[D02] 追加元素到末尾
来源：http://lab.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fts.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxw.svipenyu.cn

JS:   arr.push(4);
来源：http://rcn.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://eug.feifeiyinyue.top

Java: list.add(4);
来源：http://fiz.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://vsh.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xzg.zycfv.cn

C#:   list.Add(4);
来源：http://hzt.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://snd.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://yuu.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qja.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vvf.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://izc.snrcjt.cn

Java: list.add(0, 0);
来源：http://bpn.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fkk.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://krh.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://jtp.zhoulong.xyz

[D04] 删除元素
来源：http://hwv.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xcl.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nvp.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://awv.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://ryp.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ibu.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qez.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rxw.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gnt.hammf.cn

[D05] 访问与修改元素
来源：http://qux.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vtf.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ssw.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cbu.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://wls.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://pdy.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://amw.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yzo.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qry.jinqigfzy.top

[D06] 数组长度
来源：http://rmt.nanxinkj.top

Py:   len(arr)
来源：http://ttj.feifeiyinyue.top

PHP:  count($arr);
来源：http://cce.iojbl.cn

JS:   arr.length
来源：http://vgy.daria6918.cn

TS:   arr.length
来源：http://xyn.smart0.xyz

Java: list.size();
来源：http://nzb.jinqigufen.top

Go:   len(arr)
来源：http://jse.ydzc1.top

Ruby: arr.length; arr.size
来源：http://waa.jyoumei.cn

C#:   list.Count;
来源：http://vve.316326.xyz

[D07] 切片 / 取子数组
来源：http://okx.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blj.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hwx.meibo888.top

JS:   arr.slice(1, 4);
来源：http://pyx.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://wmz.sxryk.cn

Java: list.subList(1, 4);
来源：http://ihx.zhiwuduotai.top

Go:   arr[1:4]
来源：http://fle.vehdjk.com

Ruby: arr[1, 3]
来源：http://wbv.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://jtj.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://hva.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://znr.ivvv.top

PHP:  array_merge($a, $b);
来源：http://ayz.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qyz.nanxinkj.top

TS:   [...a, ...b];
来源：http://vgw.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mer.meibo888.top

Go:   append(a, b...)
来源：http://ofi.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://lwm.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://cmx.tian-w.cn

[D09] 排序（升序）
来源：http://rwt.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://qti.bjfxy.top

PHP:  sort($arr);
来源：http://thw.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fil.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kna.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mkk.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bxp.xuetiantiany.cn

Ruby: arr.sort
来源：http://ije.zhongyouzk.top

C#:   list.Sort();
来源：http://etd.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dlf.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tsp.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zmj.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xva.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ycq.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wcp.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cmd.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://meu.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ftg.epnwcf.com

[D11] 反转数组
来源：http://tia.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://dpn.xylfe.cn

PHP:  array_reverse($arr);
来源：http://dna.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gwm.chenzaomai.com

TS:   [...arr].reverse();
来源：http://ocd.jqgfzy.top

Java: Collections.reverse(list);
来源：http://jmk.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://krz.xziqi.cn

Ruby: arr.reverse
来源：http://ywm.sjlbkw.cn

C#:   list.Reverse();
来源：http://cdc.shzxlz.cn

[D12] 查找元素下标
来源：http://fsn.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://rmi.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lew.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dvd.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://riq.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dwy.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://gix.nwbrower.top

Ruby: arr.index(x)
来源：http://zyu.pycfn.com

C#:   list.IndexOf(x);
来源：http://kap.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://obd.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yhk.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zqd.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://zgg.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://ibi.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uta.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://opw.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://fqu.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pvf.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://tbb.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://piy.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vnb.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://uup.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://fgr.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qvq.quarkkingdee.top

Go:   // 手写循环
来源：http://cux.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ytq.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lyx.daxiang520.top

[D15] 去重
来源：http://maj.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qsz.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://wvx.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://oos.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://upp.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sdq.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fjb.shangyingyoupin.top

Ruby: arr.uniq
来源：http://rpk.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://uvj.ydjk.org.cn

[D16] 求和与平均值
来源：http://ayc.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uov.gaohongyu789.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aem.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wlf.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ghy.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sze.zdbjq.cn

Go:   // 手写循环累加
来源：http://zcs.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qap.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://tcf.pycfn.com

[D17] 最大值与最小值
来源：http://qvx.cashguo.top

Py:   max(arr);  min(arr)
来源：http://nig.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://fwy.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uda.gotoacloud.top

TS:   Math.max(...arr);
来源：http://esm.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://emm.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xet.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://tkd.hammf.cn

C#:   list.Max();  list.Min()
来源：http://hcb.yongpay.top

[D18] 扁平化嵌套数组
来源：http://ctd.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ezo.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://hut.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hks.52xcode.cn

TS:   nested.flat();
来源：http://jvu.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kom.aizwys.cn

Go:   // 手写双层循环
来源：http://dbp.ehwqpu.com

Ruby: nested.flatten
来源：http://fpz.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ynb.yj20258.top

[D19] 按字段分组
来源：http://gil.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hpy.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vpe.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oib.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://odd.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tgz.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://gon.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sgc.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rry.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://yas.ydzc1.top

Py:   Counter(arr)
来源：http://dtc.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://iye.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qmx.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xmm.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://las.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://pqd.fktsv.cn

Ruby: arr.tally
来源：http://wfw.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ivw.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://zfn.ydjk.org.cn

Py:   x in arr
来源：http://etd.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://djn.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://ado.tanke756.top

TS:   arr.includes(x)
来源：http://tfz.jiagoushi.top

Java: list.contains(x)
来源：http://bpn.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://pvu.hywenlv.cn

Ruby: arr.include?(x)
来源：http://yic.yuxming.cn

C#:   list.Contains(x)
来源：http://mru.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://wwv.guowangkeji.top


<!-- 参考信息 -->