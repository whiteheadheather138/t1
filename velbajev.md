代发 wailian999

Py:   return a, b
来源：http://xmn.tianlin.xyz

PHP:  return [$a, $b];
来源：http://goo.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://suy.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://drl.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://myn.pengpengdd.cyou

Go:   return a, b
来源：http://xzk.shzxlz.cn

Ruby: return a, b
来源：http://yyz.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://gdf.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://jac.hammf.cn

Py:   square = lambda x: x * x
来源：http://vnt.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qhq.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://hdf.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://dxq.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://btw.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://oiw.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://rsp.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://fnd.mhx1999.top

[C07] 把函数作为参数传入
来源：http://ezh.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vbs.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dyz.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cgc.fzhhl.top

TS:   arr.map(String)
来源：http://dpx.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zpu.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mas.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://fky.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zlu.nwbrower.top

[C08] 闭包
来源：http://ipc.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ied.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ryr.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://izc.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ucn.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mcz.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zgx.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://loq.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://agm.jinqigfzy.top

[C09] 递归
来源：http://vrj.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qxi.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sqp.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cnx.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ard.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pnt.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hbw.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yby.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fdz.hnqzz.top

[C10] 变量作用域
来源：http://tpj.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ovh.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hpl.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ueb.zhoulong.xyz

TS:   同 JS
来源：http://xmu.snrcjt.cn

Java: 方法内为块级作用域
来源：http://hjk.cheryme.top

Go:   花括号块级作用域
来源：http://kgh.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zcz.jqgufenzy.top

C#:   块级作用域
来源：http://mft.tian-w.cn

[C11] 模块导入与导出
来源：http://vxa.jinyuanbaomall.cn

Py:   from module import func
来源：http://lip.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jdh.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://qio.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lql.xinyue.icu

Java: import java.util.List;
来源：http://ael.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uyb.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://hdj.jinqigfzy.top

C#:   using System.Text;
来源：http://bid.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://lhj.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://ibe.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://ykr.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://syh.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://kzz.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ioy.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://kbb.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://jnn.xylfe.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://djb.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://fut.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kwd.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nso.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qgm.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uyr.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://pfc.ehwqpu.com

Go:   func add(a, b int) int
来源：http://dml.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pvn.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mjm.zdbjq.cn

[C14] 泛型函数
来源：http://puv.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bez.nanxinkj.top

PHP:  // 无泛型
来源：http://hio.chenjidiqi.icu

JS:   // 无泛型
来源：http://tig.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xiu.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://acg.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sej.havefunace.top

Ruby: # 无泛型
来源：http://bnp.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qon.ybcxt.top

[C15] 解构 / 展开参数
来源：http://rpy.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mxs.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://dec.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://raz.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ama.cdnleiting.top

Java: // 无解构
来源：http://xfr.bjfxy.top

Go:   // 无解构
来源：http://czv.dashuyun.cn

Ruby: a, b = pair
来源：http://tuv.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://xfu.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://wns.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tqh.316326.xyz

PHP:  // 无重载
来源：http://syc.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://alv.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://zph.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fox.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://ura.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://ogm.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://plg.vehdjk.com

================================================================================
来源：http://uzj.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://dwm.yj20258.top

================================================================================
来源：http://jyo.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://xcs.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uav.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wkl.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qcl.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://shk.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://usf.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://cwl.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://syh.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iqr.daxiang520.top

[D02] 追加元素到末尾
来源：http://yxz.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://guh.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oea.zhijiandao.cn

JS:   arr.push(4);
来源：http://zdz.yueranfly.top

TS:   arr.push(4);
来源：http://adb.jinqigufen.top

Java: list.add(4);
来源：http://sev.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://rtt.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://lua.yuxming.cn

C#:   list.Add(4);
来源：http://ett.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://jnq.pycfn.com

Py:   arr.insert(0, 0)
来源：http://dbd.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yds.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xrr.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://nhn.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://jpw.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kyq.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hrc.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://lsd.hcnkem.com

[D04] 删除元素
来源：http://mfn.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vfy.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yxz.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tpy.yonumen.top

TS:   arr.splice(0, 1);
来源：http://idx.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yrj.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rlz.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ycm.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://svh.zhongyouzk.top

[D05] 访问与修改元素
来源：http://alz.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dad.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ncx.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://enm.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://pby.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://vxd.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://ucg.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://odu.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lry.ybcxt.top

[D06] 数组长度
来源：http://xmx.316326.xyz

Py:   len(arr)
来源：http://xni.yj20258888.top

PHP:  count($arr);
来源：http://nlo.feifeiyinyue.top

JS:   arr.length
来源：http://rsy.hywenlv.cn

TS:   arr.length
来源：http://huf.xinyue.icu

Java: list.size();
来源：http://dau.wangdashe.top

Go:   len(arr)
来源：http://dzr.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://phl.nanxuanxn.top

C#:   list.Count;
来源：http://rzs.52xcode.cn

[D07] 切片 / 取子数组
来源：http://fbk.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqh.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://fak.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://lhs.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://rrd.ydzc1.top

Java: list.subList(1, 4);
来源：http://xip.jqgfzy.top

Go:   arr[1:4]
来源：http://dxd.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://rjl.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://aro.chenjidiqi.icu

[D08] 合并两个数组
来源：http://rvd.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://rnd.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://tzs.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fad.fehbvm.com

TS:   [...a, ...b];
来源：http://jdv.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cpt.sjlbkw.cn

Go:   append(a, b...)
来源：http://ple.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://irw.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://zge.tanke756.top

[D09] 排序（升序）
来源：http://luy.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://wqa.zhiwuduotai.top

PHP:  sort($arr);
来源：http://tgh.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yan.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iin.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tqb.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://siu.cucudq.cn

Ruby: arr.sort
来源：http://rdb.yj20258.top

C#:   list.Sort();
来源：http://hwd.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ulm.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ejs.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfy.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dgp.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxr.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdf.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ool.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eoz.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pxs.sweek.top

[D11] 反转数组
来源：http://ize.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pgv.jianghu66.top

PHP:  array_reverse($arr);
来源：http://tje.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mjk.shuidangran.top

TS:   [...arr].reverse();
来源：http://fim.9152youxi.cn

Java: Collections.reverse(list);
来源：http://dzz.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://nab.smart0.xyz

Ruby: arr.reverse
来源：http://cjz.tarul.cn

C#:   list.Reverse();
来源：http://gly.yangfankeji.com

[D12] 查找元素下标
来源：http://ixs.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://jkn.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://siu.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ioj.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://caq.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hqg.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://obm.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://ekl.yj20258888.top

C#:   list.IndexOf(x);
来源：http://qtk.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://ije.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uep.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fvp.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://djs.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://emd.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mcw.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zpc.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://jlc.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://rin.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://qxu.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vef.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vmf.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://gcj.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://vfn.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zvz.shangyingyoupin.top

Go:   // 手写循环
来源：http://pko.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jxh.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vqf.daria6918.cn

[D15] 去重
来源：http://atu.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://udq.hywenlv.cn

PHP:  array_unique($arr);
来源：http://ooe.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://gph.sweek.top

TS:   [...new Set(arr)]
来源：http://ymx.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jsm.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xkf.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://wko.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://csj.yangfankeji.com

[D16] 求和与平均值
来源：http://lyw.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fag.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cgz.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxa.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cfw.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kdd.meibo888.top

Go:   // 手写循环累加
来源：http://pbz.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://opa.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://cbh.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://vty.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://umz.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://qkj.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rby.vehdjk.com

TS:   Math.max(...arr);
来源：http://pky.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://pdq.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pfa.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://ibt.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://tzk.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://fra.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eij.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://frd.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://job.iojbl.cn

TS:   nested.flat();
来源：http://cwx.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://slu.jiagoushi.top

Go:   // 手写双层循环
来源：http://bvy.daria6918.cn

Ruby: nested.flatten
来源：http://oky.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hsf.hammf.cn

[D19] 按字段分组
来源：http://ize.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ibz.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jnn.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://htz.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rcd.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vty.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://vmp.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yin.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cqs.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://gvl.ctjpmb.com

Py:   Counter(arr)
来源：http://nhi.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://kbf.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qlj.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ipm.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zjp.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://bua.tanke756.top

Ruby: arr.tally
来源：http://alx.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yny.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://qku.quarkkingdee.top

Py:   x in arr
来源：http://bfs.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://fst.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://rku.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://nga.zhixingplan.top

Java: list.contains(x)
来源：http://rag.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://wto.cqqwz.cn

Ruby: arr.include?(x)
来源：http://wyx.zhoulong.xyz

C#:   list.Contains(x)
来源：http://pjt.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://mzf.fanxiaobao.xyz


<!-- 参考信息 -->