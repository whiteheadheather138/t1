代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://lpa.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ucl.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://vgs.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://wtm.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kop.cashguo.top

[C07] 把函数作为参数传入
来源：http://gcl.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dnx.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://onp.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oed.zhiwuduotai.top

TS:   arr.map(String)
来源：http://ycc.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fzc.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hot.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://ghw.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ejz.wangdashe.top

[C08] 闭包
来源：http://exw.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ybn.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dqx.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wmt.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pcz.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mpq.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zul.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://drf.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ylb.tianlin.xyz

[C09] 递归
来源：http://dec.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wzn.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://luy.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nej.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wsm.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ndl.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://swc.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vpk.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://chs.feifeiyinyue.top

[C10] 变量作用域
来源：http://sxu.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rts.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://djt.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vca.svipenyu.cn

TS:   同 JS
来源：http://yko.yj202588.top

Java: 方法内为块级作用域
来源：http://ebx.jqgufenzy.top

Go:   花括号块级作用域
来源：http://lpv.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ncj.zhaomingkeji.xyz

C#:   块级作用域
来源：http://wvl.sufxvd.cn

[C11] 模块导入与导出
来源：http://qwn.daxiang520.top

Py:   from module import func
来源：http://zau.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ebc.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xrt.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pbg.fehbvm.com

Java: import java.util.List;
来源：http://vlz.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rwg.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://jvq.hesvh.cn

C#:   using System.Text;
来源：http://ohg.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://qyn.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://mtc.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://iqg.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://zoj.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://pol.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vmh.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://itf.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://ftw.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://jlb.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://ybv.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://inx.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kfs.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vvm.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mcr.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://ikp.havefunace.top

Go:   func add(a, b int) int
来源：http://wcn.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://azc.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://nys.hcnkem.com

[C14] 泛型函数
来源：http://lji.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yhj.ydzc1.top

PHP:  // 无泛型
来源：http://vrf.jqgfzy.top

JS:   // 无泛型
来源：http://nfk.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gft.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lwf.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://drd.cdnleiting.top

Ruby: # 无泛型
来源：http://drj.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eml.bbcook.cn

[C15] 解构 / 展开参数
来源：http://ewb.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qas.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://jts.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xzq.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jju.zhoulong.xyz

Java: // 无解构
来源：http://uis.yanxiufei.cn

Go:   // 无解构
来源：http://rii.vehdjk.com

Ruby: a, b = pair
来源：http://gzu.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://wrv.nwbrower.top

[C16] 函数 / 方法重载
来源：http://qdv.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pzs.wangshuangyany.cn

PHP:  // 无重载
来源：http://bag.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iot.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://obl.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cjg.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://hju.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://jrc.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bkh.cqqwz.cn

================================================================================
来源：http://qlx.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://axb.cucudq.cn

================================================================================
来源：http://rka.xinyue.icu

[D01] 创建数组 / 列表
来源：http://jyi.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ynw.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovv.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vag.andypj.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://fiz.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kyf.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://sdm.quarkkingdee.top

Ruby: arr = [1, 2, 3]
来源：http://nay.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zbw.bjfxy.top

[D02] 追加元素到末尾
来源：http://omq.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fsb.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ubx.yj202588.top

JS:   arr.push(4);
来源：http://kiz.aibaodan.cn

TS:   arr.push(4);
来源：http://hkc.yonumen.top

Java: list.add(4);
来源：http://hcw.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://cly.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://xzl.zhongyouzk.top

C#:   list.Add(4);
来源：http://ifg.bbcook.cn

[D03] 在指定位置插入元素
来源：http://yws.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://twa.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://htz.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vqr.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://iik.birdmap.top

Java: list.add(0, 0);
来源：http://vtj.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ssy.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iqy.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://xkk.vehdjk.com

[D04] 删除元素
来源：http://btn.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://znd.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zll.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://smu.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://yxg.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://puy.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pfx.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://znm.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pui.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://wfj.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pmd.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zws.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zmd.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://iiy.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://qgd.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://wwd.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rtf.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://moo.shzxlz.cn

[D06] 数组长度
来源：http://qyc.jiagoushi.top

Py:   len(arr)
来源：http://chn.fehbvm.com

PHP:  count($arr);
来源：http://kbh.9152youxi.cn

JS:   arr.length
来源：http://egz.zycfv.cn

TS:   arr.length
来源：http://bik.ctjpmb.com

Java: list.size();
来源：http://fdm.jinyuanbaomall.cn

Go:   len(arr)
来源：http://qie.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://beu.shanyushiyangtech.top

C#:   list.Count;
来源：http://tli.yueranfly.top

[D07] 切片 / 取子数组
来源：http://avk.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fvv.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://alo.cheryme.top

JS:   arr.slice(1, 4);
来源：http://bji.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://sdb.tanke756.top

Java: list.subList(1, 4);
来源：http://jmp.316326.xyz

Go:   arr[1:4]
来源：http://evo.yuanzhike.top

Ruby: arr[1, 3]
来源：http://ygg.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://yhc.meibo888.top

[D08] 合并两个数组
来源：http://sal.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://asl.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://hfr.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sol.nanxuanxn.top

TS:   [...a, ...b];
来源：http://gmh.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dir.bjfxy.top

Go:   append(a, b...)
来源：http://jrf.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://qls.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://irt.guannengcc.top

[D09] 排序（升序）
来源：http://kuw.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://xvl.meibo888.top

PHP:  sort($arr);
来源：http://rcd.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vqt.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lvu.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jjy.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hjc.ehwqpu.com

Ruby: arr.sort
来源：http://rzd.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://cua.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://usk.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://izt.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xys.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylw.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gal.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bic.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ulb.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://crf.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lir.cqqwz.cn

[D11] 反转数组
来源：http://fbm.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://rms.xziqi.cn

PHP:  array_reverse($arr);
来源：http://zgf.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pfd.yvedp.cn

TS:   [...arr].reverse();
来源：http://hpy.xinyue.icu

Java: Collections.reverse(list);
来源：http://aoi.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://ljp.jqgfzy.top

Ruby: arr.reverse
来源：http://icf.uphjek.com

C#:   list.Reverse();
来源：http://frp.kuanghao11.cn

[D12] 查找元素下标
来源：http://uvq.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://qtc.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vaf.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eyd.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqx.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aze.tarul.cn

Go:   slices.Index(arr, x)
来源：http://amy.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://nek.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://rjy.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://ngl.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dhx.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mhe.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://xgy.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://zps.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sun.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tsg.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://vtz.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jcb.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://vrn.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://png.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://spk.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://unn.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://jmf.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dhd.chenzaomai.com

Go:   // 手写循环
来源：http://khc.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wif.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ykn.shanyushiyangtech.top

[D15] 去重
来源：http://brx.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bly.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://qts.epnwcf.com

JS:   [...new Set(arr)]
来源：http://fvr.gzhubu.top

TS:   [...new Set(arr)]
来源：http://sxj.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xro.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xce.sufxvd.cn

Ruby: arr.uniq
来源：http://phx.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://gfi.gogol.net.cn

[D16] 求和与平均值
来源：http://jyo.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ghh.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nuy.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uct.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bfi.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fuk.sufxvd.cn

Go:   // 手写循环累加
来源：http://fuw.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gwa.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://gei.fehbvm.com

[D17] 最大值与最小值
来源：http://aqh.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://owx.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://dcp.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hjk.zycfv.cn

TS:   Math.max(...arr);
来源：http://qbb.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://etd.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pen.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://zmb.hammf.cn

C#:   list.Max();  list.Min()
来源：http://wuq.yj20258.top

[D18] 扁平化嵌套数组
来源：http://dgo.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bju.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://hnt.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dsc.0kj1m.cn

TS:   nested.flat();
来源：http://tbd.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lqk.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://oqm.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://crt.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ong.chenjidiqi.icu

[D19] 按字段分组
来源：http://mhk.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hvd.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vkv.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vyy.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dgn.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bpu.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://rpf.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nth.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ooo.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://boy.cdnleiting.top

Py:   Counter(arr)
来源：http://srq.havefunace.top

PHP:  array_count_values($arr);
来源：http://gxz.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cao.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rii.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qsg.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://fsx.gaohongyu789.top

Ruby: arr.tally
来源：http://zgt.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jhc.daria6918.cn

[D21] 判断是否包含某元素
来源：http://gvg.daria6918.cn

Py:   x in arr
来源：http://agp.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://yin.zycfv.cn

JS:   arr.includes(x)
来源：http://fyk.aizwys.cn

TS:   arr.includes(x)
来源：http://lgi.cucudq.cn

Java: list.contains(x)
来源：http://cha.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://oih.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://hsf.ppjwa.cn

C#:   list.Contains(x)
来源：http://nvr.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://arp.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ekg.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jxp.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nxp.guowangkeji.top

TS:   [...arr];
来源：http://fqy.bjfxy.top

Java: new ArrayList<>(list);
来源：http://ieo.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://fzj.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://alt.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://mhh.vehdjk.com

[D23] reduce 累积计算
来源：http://cgn.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tqw.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://icg.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yav.nanxuanxn.top


<!-- 参考信息 -->