代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://shb.hfpthk.cn

TS:   arr.map(String)
来源：http://tkm.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fws.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uts.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://tpn.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://iyh.yvedp.cn

[C08] 闭包
来源：http://poh.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gge.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zel.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ybi.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hgq.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eqa.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jfe.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lvk.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lud.andypj.xyz

[C09] 递归
来源：http://yxg.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mme.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qru.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jft.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dti.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://evq.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qzp.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wke.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hnv.aizwys.cn

[C10] 变量作用域
来源：http://jww.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wvi.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://luo.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cjl.yueranfly.top

TS:   同 JS
来源：http://ecw.nanxinkj.top

Java: 方法内为块级作用域
来源：http://ivi.cucudq.cn

Go:   花括号块级作用域
来源：http://fev.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://agj.ehwqpu.com

C#:   块级作用域
来源：http://jsd.gaohongyu789.top

[C11] 模块导入与导出
来源：http://zws.hfpthk.cn

Py:   from module import func
来源：http://nev.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ovh.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kww.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mns.shangyingyoupin.top

Java: import java.util.List;
来源：http://gis.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zno.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://mhm.epnwcf.com

C#:   using System.Text;
来源：http://imy.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://vir.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://llx.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://pgc.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://new.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://nem.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iio.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://dro.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://vqb.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://vpq.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://wsw.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nfu.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qta.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://myh.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yow.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tkj.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://fmz.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://efq.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://qlm.jiagoushi.top

[C14] 泛型函数
来源：http://oso.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zwb.zhengqikj.top

PHP:  // 无泛型
来源：http://okn.sufxvd.cn

JS:   // 无泛型
来源：http://iwr.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nee.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bon.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://whu.dashuyun.cn

Ruby: # 无泛型
来源：http://mez.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fwb.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://imo.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sjv.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://lxx.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gfc.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kxu.chenlongwang.top

Java: // 无解构
来源：http://rlf.hammf.cn

Go:   // 无解构
来源：http://qqr.xziqi.cn

Ruby: a, b = pair
来源：http://yfn.c1oappe.top

C#:   var (a, b) = pair;
来源：http://dhq.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://nvc.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bos.kuanghao11.cn

PHP:  // 无重载
来源：http://xtn.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://vlr.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://bpr.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wto.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://ncf.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://kwa.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://twj.yueranfly.top

================================================================================
来源：http://zby.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://exv.hongshengwenyu.top

================================================================================
来源：http://nzh.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://rgk.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ycp.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eis.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sbj.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yba.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ufb.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://cjb.quarkkingdee.top

Ruby: arr = [1, 2, 3]
来源：http://jzt.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kbo.yangfankeji.com

[D02] 追加元素到末尾
来源：http://nkr.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xpn.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gwj.jqgufenzy.top

JS:   arr.push(4);
来源：http://zvf.jyoumei.cn

TS:   arr.push(4);
来源：http://hvi.hammf.cn

Java: list.add(4);
来源：http://rvd.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://sqt.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://xiq.gaohongyu789.top

C#:   list.Add(4);
来源：http://xfe.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://wvp.uphjek.com

Py:   arr.insert(0, 0)
来源：http://wnk.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xeu.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jvv.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://chb.tarul.cn

Java: list.add(0, 0);
来源：http://pky.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://zdw.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jkh.cheryme.top

C#:   list.Insert(0, 0);
来源：http://sgr.jinqigfzy.top

[D04] 删除元素
来源：http://dxa.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://haw.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jqv.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cjw.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://yjd.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cew.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nbv.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dwf.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lvi.guannengcc.top

[D05] 访问与修改元素
来源：http://btt.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lhk.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mch.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nec.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://xxc.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://mds.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://cvp.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qse.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yrv.kuanghao11.cn

[D06] 数组长度
来源：http://gwu.zycfv.cn

Py:   len(arr)
来源：http://brr.yuanzhike.top

PHP:  count($arr);
来源：http://iww.zhengqikj.top

JS:   arr.length
来源：http://thc.kuanghao11.cn

TS:   arr.length
来源：http://hrk.snrcjt.cn

Java: list.size();
来源：http://pgp.tian-w.cn

Go:   len(arr)
来源：http://uxc.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://poh.tarul.cn

C#:   list.Count;
来源：http://mju.ywan-chungtsiang.top

[D07] 切片 / 取子数组
来源：http://xqn.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ctv.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pdm.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://bha.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://jsf.jianghu66.top

Java: list.subList(1, 4);
来源：http://vsw.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://cah.daxiang520.top

Ruby: arr[1, 3]
来源：http://jqc.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://hew.jianghu66.top

[D08] 合并两个数组
来源：http://lxs.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://vhc.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://guw.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iwy.hfpthk.cn

TS:   [...a, ...b];
来源：http://zya.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://anj.jiagoushi.top

Go:   append(a, b...)
来源：http://yhj.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://hlv.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://uhg.yvedp.cn

[D09] 排序（升序）
来源：http://oia.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://mhm.sufxvd.cn

PHP:  sort($arr);
来源：http://ytv.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vjy.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://npg.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rij.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hjr.yangfankeji.com

Ruby: arr.sort
来源：http://tvz.ydjk.org.cn

C#:   list.Sort();
来源：http://wxj.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://ojj.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://net.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zsl.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rlv.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cpn.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sgf.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nzr.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wlt.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lbw.ehwqpu.com

[D11] 反转数组
来源：http://ggr.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yow.ivvv.top

PHP:  array_reverse($arr);
来源：http://cht.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uus.snrcjt.cn

TS:   [...arr].reverse();
来源：http://dqw.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://abn.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://gjf.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://qio.hysaishi.cn

C#:   list.Reverse();
来源：http://bzy.zhoulong.xyz

[D12] 查找元素下标
来源：http://ldb.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://phs.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fhz.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osx.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tjh.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zlx.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://zqs.guowangkeji.top

Ruby: arr.index(x)
来源：http://rlx.yj20258888.top

C#:   list.IndexOf(x);
来源：http://kuv.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://oru.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pmo.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fiq.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://ktn.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://pub.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mtk.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bez.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fht.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hde.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://ldq.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ejf.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rkl.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://sup.sweek.top

TS:   arr.map(x => x * 2)
来源：http://nxt.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://obu.zhiwuduotai.top

Go:   // 手写循环
来源：http://sbm.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://keg.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ogs.sweek.top

[D15] 去重
来源：http://ewc.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xrf.yj20258888.top

PHP:  array_unique($arr);
来源：http://jbf.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://dba.yueranfly.top

TS:   [...new Set(arr)]
来源：http://ufm.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ubs.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ehq.daria6918.cn

Ruby: arr.uniq
来源：http://ovc.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://qbx.guannengcc.top

[D16] 求和与平均值
来源：http://gdk.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cbd.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rwa.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zym.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wmk.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dtk.jlsjyb.cn

Go:   // 手写循环累加
来源：http://uri.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rhk.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://psr.tianlin.xyz

[D17] 最大值与最小值
来源：http://qzk.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://uqv.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://ags.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fjo.tian-w.cn

TS:   Math.max(...arr);
来源：http://lbe.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mlo.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nrw.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://jps.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://yyu.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://vea.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://egx.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://zbm.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eyu.tianlin.xyz

TS:   nested.flat();
来源：http://mdr.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cvg.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://cqq.52xcode.cn

Ruby: nested.flatten
来源：http://gin.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://avy.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://mht.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mne.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yre.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uqn.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ybr.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qyr.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://fse.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cjc.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kwp.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://vup.jinqigfzy.top

Py:   Counter(arr)
来源：http://hwf.yueranfly.top

PHP:  array_count_values($arr);
来源：http://smh.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://liz.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iht.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ayg.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://fkp.guannengcc.top

Ruby: arr.tally
来源：http://tbd.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qng.nwbrower.top

[D21] 判断是否包含某元素
来源：http://qjx.yj20258888.top

Py:   x in arr
来源：http://zrn.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://tvk.bjfxy.top

JS:   arr.includes(x)
来源：http://idt.jianghu66.top

TS:   arr.includes(x)
来源：http://tnr.snrcjt.cn

Java: list.contains(x)
来源：http://nlw.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://qgn.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://hua.meibo888.top

C#:   list.Contains(x)
来源：http://exk.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://vbn.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fad.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bnw.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fwh.tian-w.cn

TS:   [...arr];
来源：http://okk.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://wnm.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://glh.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://bot.pycfn.com

C#:   new List<int>(list);
来源：http://mey.yuanzhike.top

[D23] reduce 累积计算
来源：http://ukh.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dxr.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ndg.jlsjyb.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kbl.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rwn.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rnq.yj20258.top

Go:   // 手写循环
来源：http://cve.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wlb.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wth.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://iaf.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://drh.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://snj.epnwcf.com


<!-- 参考信息 -->