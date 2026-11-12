代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://klk.daxiang520.top

TS:   arr.map(String)
来源：http://djc.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mpn.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vsn.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://hwu.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://dln.cqqwz.cn

[C08] 闭包
来源：http://spy.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://okt.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gul.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://afo.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vdm.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jul.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jqv.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dzk.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rsi.zhoulong.xyz

[C09] 递归
来源：http://bxu.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fiq.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hbv.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjk.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttj.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ocl.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://euy.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ota.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yhm.sufxvd.cn

[C10] 变量作用域
来源：http://uff.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gna.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gsy.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mlr.ydzc1.top

TS:   同 JS
来源：http://acs.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://ldi.9152youxi.cn

Go:   花括号块级作用域
来源：http://tcj.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jbr.fktsv.cn

C#:   块级作用域
来源：http://yix.dashuyun.cn

[C11] 模块导入与导出
来源：http://ahc.nanxinkj.top

Py:   from module import func
来源：http://ybq.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jce.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rys.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tfo.jqgfzy.top

Java: import java.util.List;
来源：http://cfx.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dhw.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://hby.jqgfzy.top

C#:   using System.Text;
来源：http://onn.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://pyf.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://cuz.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://uuq.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://zgm.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://fsv.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://spd.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://cug.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://ahn.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vad.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://ocl.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://onx.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bxx.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hwz.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kve.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ytu.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://szy.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kvv.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://wzg.ybcxt.top

[C14] 泛型函数
来源：http://bsl.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxp.zycfv.cn

PHP:  // 无泛型
来源：http://aih.fehbvm.com

JS:   // 无泛型
来源：http://tni.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pwr.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iqd.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gxx.zhixingplan.top

Ruby: # 无泛型
来源：http://gtc.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dqu.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://opy.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rdw.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://bxb.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hkk.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bwb.yuxming.cn

Java: // 无解构
来源：http://awv.redwolf501.top

Go:   // 无解构
来源：http://wjf.hesvh.cn

Ruby: a, b = pair
来源：http://qdc.epnwcf.com

C#:   var (a, b) = pair;
来源：http://jky.shanyushiyangtech.top

[C16] 函数 / 方法重载
来源：http://soo.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pcl.ppjwa.cn

PHP:  // 无重载
来源：http://hgv.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fuu.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://rew.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mrf.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://ygu.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://mpg.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jbq.sxryk.cn

================================================================================
来源：http://wbq.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://wpz.feifeiyinyue.top

================================================================================
来源：http://lho.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://and.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nvs.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fvs.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dfk.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://juh.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://djs.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://mql.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://gav.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bdx.chenzaomai.com

[D02] 追加元素到末尾
来源：http://yys.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eiw.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dhp.vehdjk.com

JS:   arr.push(4);
来源：http://noy.tarul.cn

TS:   arr.push(4);
来源：http://hhc.cdnleiting.top

Java: list.add(4);
来源：http://myb.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://hat.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://ttw.bbcook.cn

C#:   list.Add(4);
来源：http://dxm.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://aje.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://waz.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ddo.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nqd.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://lnc.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://hyp.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://euk.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pyv.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://lrh.svipenyu.cn

[D04] 删除元素
来源：http://xis.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uwy.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zng.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qac.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://qgt.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogj.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qdh.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bvt.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://maj.sweek.top

[D05] 访问与修改元素
来源：http://wkx.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://okb.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bzn.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vti.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://pkc.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://ier.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://kyt.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://btu.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zwk.ivvv.top

[D06] 数组长度
来源：http://xiy.yj202588.top

Py:   len(arr)
来源：http://ljr.fengsongda.top

PHP:  count($arr);
来源：http://pzx.zdqjudy.top

JS:   arr.length
来源：http://nao.xylfe.cn

TS:   arr.length
来源：http://vad.ydjk.org.cn

Java: list.size();
来源：http://ang.ppjwa.cn

Go:   len(arr)
来源：http://oaj.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://wkd.yanxiufei.cn

C#:   list.Count;
来源：http://ryr.uphjek.com

[D07] 切片 / 取子数组
来源：http://imz.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gok.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://vek.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://xah.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://jbt.gogol.net.cn

Java: list.subList(1, 4);
来源：http://eoo.aizwys.cn

Go:   arr[1:4]
来源：http://uec.jianghu66.top

Ruby: arr[1, 3]
来源：http://htk.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://ptk.shangyingyoupin.top

[D08] 合并两个数组
来源：http://uns.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://vic.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://qdm.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://oby.kuanghao11.cn

TS:   [...a, ...b];
来源：http://ktk.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vsw.bjfxy.top

Go:   append(a, b...)
来源：http://szn.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://kzl.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://kri.dashuyun.cn

[D09] 排序（升序）
来源：http://zog.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://jtr.ybcxt.top

PHP:  sort($arr);
来源：http://whc.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wcd.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://szm.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cpk.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ogm.zhoulong.xyz

Ruby: arr.sort
来源：http://ydl.hfpthk.cn

C#:   list.Sort();
来源：http://uea.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wsg.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jlf.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vto.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xjw.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bkb.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hsk.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eay.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://elj.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sff.ctjpmb.com

[D11] 反转数组
来源：http://azw.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://mqe.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://zsm.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://okr.zycfv.cn

TS:   [...arr].reverse();
来源：http://mdk.0kj1m.cn

Java: Collections.reverse(list);
来源：http://zjr.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://uqv.kuanghao11.cn

Ruby: arr.reverse
来源：http://izu.jyoumei.cn

C#:   list.Reverse();
来源：http://yjm.zhijiandao.cn

[D12] 查找元素下标
来源：http://map.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://azn.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bwu.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xau.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lwz.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://imr.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://dey.shzxlz.cn

Ruby: arr.index(x)
来源：http://jfv.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://cof.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://vrm.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uay.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tbe.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://umq.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://iye.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://utp.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kiv.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://jyu.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kmr.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://xhn.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lnd.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xfw.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://hpy.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://yiq.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hma.cdnleiting.top

Go:   // 手写循环
来源：http://xit.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://gmb.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oqw.gaohongyu789.top

[D15] 去重
来源：http://imi.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hit.tianlin.xyz

PHP:  array_unique($arr);
来源：http://rpt.yongpay.top

JS:   [...new Set(arr)]
来源：http://ufw.sweek.top

TS:   [...new Set(arr)]
来源：http://ucj.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dac.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://jxn.fktsv.cn

Ruby: arr.uniq
来源：http://nwq.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://apo.havefunace.top

[D16] 求和与平均值
来源：http://igz.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ogz.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bxu.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uva.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iez.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iop.zhoulong.xyz

Go:   // 手写循环累加
来源：http://mer.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qtl.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://ipx.kuanghao11.cn

[D17] 最大值与最小值
来源：http://fsw.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://jga.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://xoz.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nzu.jiagoushi.top

TS:   Math.max(...arr);
来源：http://auw.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://nmc.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://grf.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://tyz.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://oah.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://jsi.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kfi.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://gdt.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blp.9152youxi.cn

TS:   nested.flat();
来源：http://qro.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nzk.xuanzx.com

Go:   // 手写双层循环
来源：http://laz.nwbrower.top

Ruby: nested.flatten
来源：http://jqw.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rax.zdbjq.cn

[D19] 按字段分组
来源：http://cub.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xrs.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vcl.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xzk.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kcq.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oew.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://hke.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xwm.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jrx.havefunace.top

[D20] 统计每个元素出现次数
来源：http://lrv.xinyue.icu

Py:   Counter(arr)
来源：http://lxq.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://bvw.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mdz.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://riv.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cht.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://ogz.jiagoushi.top

Ruby: arr.tally
来源：http://xcr.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ptc.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://tlj.zhiwuduotai.top

Py:   x in arr
来源：http://zkk.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://fvm.kuanghao11.cn

JS:   arr.includes(x)
来源：http://eod.yongpay.top

TS:   arr.includes(x)
来源：http://kvr.fzhhl.top

Java: list.contains(x)
来源：http://yrn.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://aox.zhengqikj.top

Ruby: arr.include?(x)
来源：http://kdn.tian-w.cn

C#:   list.Contains(x)
来源：http://jyy.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://kem.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zxq.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bnd.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nsu.shanyushiyangkeji.top

TS:   [...arr];
来源：http://crb.bjfxy.top

Java: new ArrayList<>(list);
来源：http://vwa.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rmo.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://gnu.zdbjq.cn

C#:   new List<int>(list);
来源：http://zvc.yongpay.top

[D23] reduce 累积计算
来源：http://dpc.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vvi.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wnu.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zcg.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bta.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://jlw.bjfxy.top

Go:   // 手写循环
来源：http://gry.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://swg.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rip.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://pkv.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dvr.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cgf.cqqwz.cn


<!-- 参考信息 -->