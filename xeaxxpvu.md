代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lja.aizwys.cn

TS:   arr.map(String)
来源：http://xkv.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xrm.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yzf.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://hds.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://slw.haohaochexian.top

[C08] 闭包
来源：http://hee.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aks.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://txf.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oah.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xqa.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dzv.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rbx.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pfo.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mmq.sufxvd.cn

[C09] 递归
来源：http://lov.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hgs.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jeb.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnf.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpy.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgh.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://idd.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hfw.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xwx.hammf.cn

[C10] 变量作用域
来源：http://iuj.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yva.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tpe.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xel.yj202588.top

TS:   同 JS
来源：http://tqo.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://nka.yanxiufei.cn

Go:   花括号块级作用域
来源：http://xuy.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ykg.tarul.cn

C#:   块级作用域
来源：http://cso.yj20258.top

[C11] 模块导入与导出
来源：http://pub.yanxiufei.cn

Py:   from module import func
来源：http://ulg.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sde.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://okj.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jta.tian-w.cn

Java: import java.util.List;
来源：http://yba.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ule.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://lxv.fengsongda.top

C#:   using System.Text;
来源：http://utm.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://hxr.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://jfk.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://gim.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://fdv.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://uyf.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aqq.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://pcu.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://xkn.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qyr.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://fxb.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://epo.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zbp.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gux.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bfi.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://uav.hammf.cn

Go:   func add(a, b int) int
来源：http://kwy.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kom.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tad.gzhubu.top

[C14] 泛型函数
来源：http://joz.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kqt.vqdsnc.cn

PHP:  // 无泛型
来源：http://ryj.sufxvd.cn

JS:   // 无泛型
来源：http://pcv.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kzl.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iri.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dsg.yfazqb.com

Ruby: # 无泛型
来源：http://nsv.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ukn.smart0.xyz

[C15] 解构 / 展开参数
来源：http://ujo.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jrf.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://ylr.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wsy.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lsc.9152youxi.cn

Java: // 无解构
来源：http://ohf.0kj1m.cn

Go:   // 无解构
来源：http://jdo.svipenyu.cn

Ruby: a, b = pair
来源：http://wsn.meibo888.top

C#:   var (a, b) = pair;
来源：http://oln.birdmap.top

[C16] 函数 / 方法重载
来源：http://fte.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://exl.hongshengwenyu.top

PHP:  // 无重载
来源：http://dhu.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://trr.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://lpx.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jat.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://xyq.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://nms.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ole.hongshengwenyu.top

================================================================================
来源：http://jhe.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://fgx.yonumen.top

================================================================================
来源：http://qim.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://kli.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kbx.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ofr.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://llv.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yat.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sad.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://mcl.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://kmq.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tkx.cqqwz.cn

[D02] 追加元素到末尾
来源：http://lpl.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nbu.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://inn.ybcxt.top

JS:   arr.push(4);
来源：http://nky.shangyingyoupin.top

TS:   arr.push(4);
来源：http://lyk.hammf.cn

Java: list.add(4);
来源：http://gdk.birdmap.top

Go:   arr = append(arr, 4)
来源：http://wyy.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://brq.52xcode.cn

C#:   list.Add(4);
来源：http://mcu.yonumen.top

[D03] 在指定位置插入元素
来源：http://oaw.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://hqi.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qcc.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qnz.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://aim.snrcjt.cn

Java: list.add(0, 0);
来源：http://skd.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://efy.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qmq.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://frs.epnwcf.com

[D04] 删除元素
来源：http://kjd.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jlc.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kue.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vju.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://vww.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://thh.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hiy.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ljs.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gsh.ppjwa.cn

[D05] 访问与修改元素
来源：http://zxg.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tcj.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://knr.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qel.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://okd.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://hme.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://hxg.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nzc.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xkm.xylfe.cn

[D06] 数组长度
来源：http://skc.yj202588.top

Py:   len(arr)
来源：http://yru.fzhhl.top

PHP:  count($arr);
来源：http://bzk.hnxiangtu.top

JS:   arr.length
来源：http://xad.xinyue.icu

TS:   arr.length
来源：http://hrg.cashguo.top

Java: list.size();
来源：http://ljz.quarkkingdee.top

Go:   len(arr)
来源：http://mdf.ydzc1.top

Ruby: arr.length; arr.size
来源：http://wiu.xylfe.cn

C#:   list.Count;
来源：http://uzg.c1oappe.top

[D07] 切片 / 取子数组
来源：http://nzt.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cwr.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sly.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://pyj.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://oxv.ctjpmb.com

Java: list.subList(1, 4);
来源：http://wen.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://vgp.yj202588.top

Ruby: arr[1, 3]
来源：http://qbe.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://sqw.jlsjyb.cn

[D08] 合并两个数组
来源：http://idn.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://arb.pycfn.com

PHP:  array_merge($a, $b);
来源：http://wdo.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qxx.cheryme.top

TS:   [...a, ...b];
来源：http://okm.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gdn.andypj.xyz

Go:   append(a, b...)
来源：http://mjd.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://stk.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://xxi.redwolf501.top

[D09] 排序（升序）
来源：http://pxs.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://fbj.gotoacloud.top

PHP:  sort($arr);
来源：http://sld.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fif.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gwk.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ojf.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dxh.0kj1m.cn

Ruby: arr.sort
来源：http://mwh.cqqwz.cn

C#:   list.Sort();
来源：http://xcd.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yrg.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mgj.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://khq.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pme.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rth.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fzh.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://orq.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nbv.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bmz.jinghuilouyu.cn

[D11] 反转数组
来源：http://svq.shzxlz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sgr.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://syo.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gdz.hywenlv.cn

TS:   [...arr].reverse();
来源：http://rgs.0kj1m.cn

Java: Collections.reverse(list);
来源：http://vma.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://pmx.hfpthk.cn

Ruby: arr.reverse
来源：http://njh.jqgufenzy.top

C#:   list.Reverse();
来源：http://ijw.zhongyouzk.top

[D12] 查找元素下标
来源：http://nhq.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://dkn.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ait.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iuo.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://toh.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vns.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://ifi.jinqigufen.top

Ruby: arr.index(x)
来源：http://smg.yuxming.cn

C#:   list.IndexOf(x);
来源：http://cwc.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://czc.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyp.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kby.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://dju.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://abr.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://khf.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://llc.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tro.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://goy.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://ndi.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qco.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nyv.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://tti.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://ipa.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gmd.pycfn.com

Go:   // 手写循环
来源：http://ygs.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://sda.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wiw.ivvv.top

[D15] 去重
来源：http://kxx.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xmm.andypj.xyz

PHP:  array_unique($arr);
来源：http://ods.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://gxc.52xcode.cn

TS:   [...new Set(arr)]
来源：http://jqt.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bri.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://bzj.sxryk.cn

Ruby: arr.uniq
来源：http://ohe.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://tid.haohaochexian.top

[D16] 求和与平均值
来源：http://via.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysp.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://akg.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bki.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oxq.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nzk.xziqi.cn

Go:   // 手写循环累加
来源：http://wpm.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pdp.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://zxo.fehbvm.com

[D17] 最大值与最小值
来源：http://pqv.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://zzf.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://zvb.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pzc.daxiang520.top

TS:   Math.max(...arr);
来源：http://oqx.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qmr.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gbq.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://gdi.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://fyi.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://nwh.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ehz.316326.xyz

PHP:  array_merge(...$nested);
来源：http://edp.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bit.zhengqikj.top

TS:   nested.flat();
来源：http://rna.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vax.hammf.cn

Go:   // 手写双层循环
来源：http://ipc.shangyingyoupin.top

Ruby: nested.flatten
来源：http://cln.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wvv.yvedp.cn

[D19] 按字段分组
来源：http://vpa.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qim.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pax.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iuw.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://joo.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nzd.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://jde.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nlj.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lya.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://cnk.zhijiandao.cn

Py:   Counter(arr)
来源：http://agd.yuxming.cn

PHP:  array_count_values($arr);
来源：http://xyw.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xwm.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvf.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gsc.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://tjc.pengpengdd.cyou

Ruby: arr.tally
来源：http://lnk.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tvc.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://wpy.yj20258888.top

Py:   x in arr
来源：http://bbg.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://irj.epnwcf.com

JS:   arr.includes(x)
来源：http://klh.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://ijp.aizwys.cn

Java: list.contains(x)
来源：http://orm.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://kvl.jinqigufen.top

Ruby: arr.include?(x)
来源：http://qcj.ctjpmb.com

C#:   list.Contains(x)
来源：http://abv.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://yjq.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qgw.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eoz.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://doz.9152youxi.cn

TS:   [...arr];
来源：http://rzb.guannengcc.top

Java: new ArrayList<>(list);
来源：http://zqe.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://trp.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://eey.smart0.xyz

C#:   new List<int>(list);
来源：http://zxf.xziqi.cn

[D23] reduce 累积计算
来源：http://pjk.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sex.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://spq.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://psl.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wbj.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://sld.cheryme.top

Go:   // 手写循环
来源：http://hfh.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rdu.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ixx.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://syz.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gxj.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ggd.xingfuxueyuan.xyz


<!-- 参考信息 -->