代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://izz.316326.xyz

TS:   arr.map(String)
来源：http://pko.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hbc.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nnd.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://lge.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://igx.wangdashe.top

[C08] 闭包
来源：http://tzt.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kxr.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sug.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pjr.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://atw.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rqt.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pqz.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zdh.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qfm.aizwys.cn

[C09] 递归
来源：http://gsd.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vue.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wzj.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gha.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mge.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://krl.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vxg.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rxn.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tio.sufxvd.cn

[C10] 变量作用域
来源：http://qtk.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wdp.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bsy.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hvc.316326.xyz

TS:   同 JS
来源：http://ukt.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://bfb.yuxming.cn

Go:   花括号块级作用域
来源：http://sah.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://csj.ehwqpu.com

C#:   块级作用域
来源：http://sbh.tanke756.top

[C11] 模块导入与导出
来源：http://vmp.meibo888.top

Py:   from module import func
来源：http://oyz.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://arc.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://zpz.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jau.chenlongwang.top

Java: import java.util.List;
来源：http://vab.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lny.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://qpv.bbcook.cn

C#:   using System.Text;
来源：http://nts.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://imh.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://spl.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://tly.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://oez.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://ges.jinqigufen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://euu.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://fis.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://rqp.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hyd.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://jwh.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qvf.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vjt.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mfb.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mve.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://yjf.uphjek.com

Go:   func add(a, b int) int
来源：http://xzq.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qza.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://urf.dashuyun.cn

[C14] 泛型函数
来源：http://uyr.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aao.xziqi.cn

PHP:  // 无泛型
来源：http://lkr.shanyushiyangtech.top

JS:   // 无泛型
来源：http://abi.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eva.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vkj.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bct.gzhubu.top

Ruby: # 无泛型
来源：http://wjf.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hgs.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://nxk.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rfq.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://pzy.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kmr.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bmp.jinqigfzy.top

Java: // 无解构
来源：http://arz.zhaomingkeji.xyz

Go:   // 无解构
来源：http://cjc.sweek.top

Ruby: a, b = pair
来源：http://inv.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://bks.iojbl.cn

[C16] 函数 / 方法重载
来源：http://sbw.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hqj.vehdjk.com

PHP:  // 无重载
来源：http://veu.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://skq.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://sxv.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pex.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://fcy.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://oqz.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://auc.yfazqb.com

================================================================================
来源：http://cjq.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://wyh.jinqigfzy.top

================================================================================
来源：http://cff.xziqi.cn

[D01] 创建数组 / 列表
来源：http://xfe.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://buq.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rwn.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wdr.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://azx.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rjq.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://rfa.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://hzb.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nlb.jyoumei.cn

[D02] 追加元素到末尾
来源：http://isr.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hmb.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wec.jlsjyb.cn

JS:   arr.push(4);
来源：http://nwa.pengpengdd.cyou

TS:   arr.push(4);
来源：http://mfb.zdbjq.cn

Java: list.add(4);
来源：http://otu.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://xvp.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://txa.aizwys.cn

C#:   list.Add(4);
来源：http://pyi.fzhhl.top

[D03] 在指定位置插入元素
来源：http://mwm.yongpay.top

Py:   arr.insert(0, 0)
来源：http://ubq.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bab.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jdk.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://zei.kuanghao11.cn

Java: list.add(0, 0);
来源：http://hap.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uqt.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cko.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://ldz.fktsv.cn

[D04] 删除元素
来源：http://oxp.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ycs.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rxa.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ptk.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://cgj.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xzb.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://twg.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://spo.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yut.chenzaomai.com

[D05] 访问与修改元素
来源：http://orj.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ppt.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wuh.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tpy.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://vhm.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://lpd.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://hbq.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uoo.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pqd.c1oappe.top

[D06] 数组长度
来源：http://iow.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://hnm.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://lwq.zhoulong.xyz

JS:   arr.length
来源：http://arh.chenzaomai.com

TS:   arr.length
来源：http://smv.nanxinkj.top

Java: list.size();
来源：http://pvz.birdmap.top

Go:   len(arr)
来源：http://usu.tian-w.cn

Ruby: arr.length; arr.size
来源：http://jkc.sufxvd.cn

C#:   list.Count;
来源：http://piz.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://cyt.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ivc.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://ony.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://jiv.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://dyd.pycfn.com

Java: list.subList(1, 4);
来源：http://dhl.gzhubu.top

Go:   arr[1:4]
来源：http://tui.tanke756.top

Ruby: arr[1, 3]
来源：http://rkg.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://rhv.yj202588.top

[D08] 合并两个数组
来源：http://rbq.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://ulp.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://qwm.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://wng.tian-w.cn

TS:   [...a, ...b];
来源：http://azz.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lnz.aibaodan.cn

Go:   append(a, b...)
来源：http://rbm.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://tgw.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://uao.vqdsnc.cn

[D09] 排序（升序）
来源：http://pdg.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://vym.316326.xyz

PHP:  sort($arr);
来源：http://vtg.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dhe.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qvp.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mnf.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ahl.redwolf501.top

Ruby: arr.sort
来源：http://nje.vqdsnc.cn

C#:   list.Sort();
来源：http://vaq.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yeo.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://faj.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eiz.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uqy.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yyz.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kkm.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tvv.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ntf.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://emc.mhx1999.top

[D11] 反转数组
来源：http://frg.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://liv.yj202588.top

PHP:  array_reverse($arr);
来源：http://app.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://foh.iojbl.cn

TS:   [...arr].reverse();
来源：http://wlu.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://pgk.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://myj.quarkkingdee.top

Ruby: arr.reverse
来源：http://gtt.sxryk.cn

C#:   list.Reverse();
来源：http://vcr.shangyingyoupin.top

[D12] 查找元素下标
来源：http://pub.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://twy.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ttz.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ewp.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bmu.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nic.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://sop.jyoumei.cn

Ruby: arr.index(x)
来源：http://xol.sysykeji.top

C#:   list.IndexOf(x);
来源：http://pcn.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://vtz.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qnu.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://akh.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://igk.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://vru.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bxw.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://npb.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qph.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nxz.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://lpf.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fih.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wdm.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://gon.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://hdv.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qyp.epnwcf.com

Go:   // 手写循环
来源：http://csn.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://nje.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://xtf.zdbjq.cn

[D15] 去重
来源：http://nmh.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rqp.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://znd.fktsv.cn

JS:   [...new Set(arr)]
来源：http://hlu.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://hzq.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sbf.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://duq.uphjek.com

Ruby: arr.uniq
来源：http://lfz.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://hbv.kuanghao11.cn

[D16] 求和与平均值
来源：http://erq.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rnm.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sxp.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ham.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xss.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gah.zhengqikj.top

Go:   // 手写循环累加
来源：http://sjm.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sdd.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://hkq.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://jmb.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://hrf.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://upp.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rvx.gogol.net.cn

TS:   Math.max(...arr);
来源：http://cpc.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ugg.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zoh.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://xqy.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://tcg.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://yeu.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zog.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://mpd.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://axr.zdqjudy.top

TS:   nested.flat();
来源：http://jkt.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jzw.cashguo.top

Go:   // 手写双层循环
来源：http://qeq.jyoumei.cn

Ruby: nested.flatten
来源：http://dgz.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lqf.jqgfzy.top

[D19] 按字段分组
来源：http://hcy.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mzr.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ktr.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gxs.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://wis.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uob.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://fkd.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bsx.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oel.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://bdw.havefunace.top

Py:   Counter(arr)
来源：http://mgl.fengsongda.top

PHP:  array_count_values($arr);
来源：http://zqv.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mes.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nlj.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zed.yj202588.top

Go:   // 手写 map[T]int
来源：http://ezg.gaohongyu789.top

Ruby: arr.tally
来源：http://zmf.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nci.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://ahy.hammf.cn

Py:   x in arr
来源：http://uox.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://qcm.tian-w.cn

JS:   arr.includes(x)
来源：http://keu.jinqigfzy.top

TS:   arr.includes(x)
来源：http://wjx.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://ojt.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://hfp.tanke756.top

Ruby: arr.include?(x)
来源：http://fip.yvedp.cn

C#:   list.Contains(x)
来源：http://oxu.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://jpd.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aws.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dnn.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kzl.cheryme.top

TS:   [...arr];
来源：http://oly.shuidangran.top

Java: new ArrayList<>(list);
来源：http://bpm.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tkc.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://lxk.316326.xyz

C#:   new List<int>(list);
来源：http://kle.sxryk.cn

[D23] reduce 累积计算
来源：http://evw.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fqk.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gad.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gde.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eog.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ktx.quarkkingdee.top

Go:   // 手写循环
来源：http://lvb.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ijq.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xul.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://ghp.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zkd.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zut.daxiang520.top


<!-- 参考信息 -->