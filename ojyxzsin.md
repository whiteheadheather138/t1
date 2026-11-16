代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ujz.ehwqpu.com

TS:   arr.map(String)
来源：http://vdf.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wbg.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://orf.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://gwh.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gam.jinyuanbaomall.cn

[C08] 闭包
来源：http://gck.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufp.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pbp.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kco.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vio.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uwt.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://enf.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://plj.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kzt.chenlongwang.top

[C09] 递归
来源：http://dnq.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pgd.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hol.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xmu.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ftb.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rvp.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bwh.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nym.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kzh.mhx1999.top

[C10] 变量作用域
来源：http://fll.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://whi.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oxb.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://geb.hfpthk.cn

TS:   同 JS
来源：http://aff.yj20258.top

Java: 方法内为块级作用域
来源：http://khx.fzhhl.top

Go:   花括号块级作用域
来源：http://wvz.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oeb.yfazqb.com

C#:   块级作用域
来源：http://kds.yanxiufei.cn

[C11] 模块导入与导出
来源：http://ehh.gzhubu.top

Py:   from module import func
来源：http://lng.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mdp.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://fou.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zbc.fanxiaobao.xyz

Java: import java.util.List;
来源：http://ufq.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://itp.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://mms.zhixingplan.top

C#:   using System.Text;
来源：http://vbh.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://prq.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://xqr.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://qul.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://dtw.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://olc.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vwf.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://kqj.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://xpg.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://snj.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://qln.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gtn.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xyo.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oap.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nhp.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gdq.jiagoushi.top

Go:   func add(a, b int) int
来源：http://kcz.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://leu.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://szm.ydjk.org.cn

[C14] 泛型函数
来源：http://mvg.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yzt.fengsongda.top

PHP:  // 无泛型
来源：http://zdc.nanxinkj.top

JS:   // 无泛型
来源：http://ujy.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xue.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hzl.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iix.quarkkingdee.top

Ruby: # 无泛型
来源：http://gcd.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xit.sxryk.cn

[C15] 解构 / 展开参数
来源：http://hnc.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mdr.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://lwa.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jij.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zyp.gogol.net.cn

Java: // 无解构
来源：http://tbp.havefunace.top

Go:   // 无解构
来源：http://ifl.yueranfly.top

Ruby: a, b = pair
来源：http://ick.hnqzz.top

C#:   var (a, b) = pair;
来源：http://duk.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://vij.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pez.aizwys.cn

PHP:  // 无重载
来源：http://qqw.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lip.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://vsc.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bhw.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://bmt.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://anr.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cbx.yanxiufei.cn

================================================================================
来源：http://qdj.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://wxw.gaohongyu789.top

================================================================================
来源：http://kxw.havefunace.top

[D01] 创建数组 / 列表
来源：http://hag.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yws.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vtk.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nbw.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jaj.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://koz.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://bic.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://cnj.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qyo.nwbrower.top

[D02] 追加元素到末尾
来源：http://rng.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://toi.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uzc.smart0.xyz

JS:   arr.push(4);
来源：http://pzv.kuanghao11.cn

TS:   arr.push(4);
来源：http://mmb.xuanzx.com

Java: list.add(4);
来源：http://wtz.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://hvv.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://jbo.yj20258888.top

C#:   list.Add(4);
来源：http://rbh.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://csu.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://wue.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://caw.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://agt.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://lxd.nwbrower.top

Java: list.add(0, 0);
来源：http://wgg.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xyo.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jfp.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://gve.hysaishi.cn

[D04] 删除元素
来源：http://mal.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kfu.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ggn.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rqf.yonumen.top

TS:   arr.splice(0, 1);
来源：http://ptb.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zng.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gue.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qcg.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdg.hywenlv.cn

[D05] 访问与修改元素
来源：http://kwq.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nla.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ytw.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ype.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://svy.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://dmx.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qcb.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qgb.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yzi.zhiwuduotai.top

[D06] 数组长度
来源：http://jzf.redwolf501.top

Py:   len(arr)
来源：http://phi.hfpthk.cn

PHP:  count($arr);
来源：http://tih.dianchejie.cn

JS:   arr.length
来源：http://kwp.hysaishi.cn

TS:   arr.length
来源：http://rgn.ppjwa.cn

Java: list.size();
来源：http://ceh.guannengcc.top

Go:   len(arr)
来源：http://ovz.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://fdk.cashguo.top

C#:   list.Count;
来源：http://yxv.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://fjs.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bfp.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://xai.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://zmk.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://bxa.vehdjk.com

Java: list.subList(1, 4);
来源：http://niy.zhengqikj.top

Go:   arr[1:4]
来源：http://otl.shuidangran.top

Ruby: arr[1, 3]
来源：http://ifi.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://tdk.jqgufenzy.top

[D08] 合并两个数组
来源：http://txo.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://vbz.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://gjf.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hnz.quarkkingdee.top

TS:   [...a, ...b];
来源：http://xgo.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fmg.snrcjt.cn

Go:   append(a, b...)
来源：http://eep.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://nus.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://hln.yfazqb.com

[D09] 排序（升序）
来源：http://dkz.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://oux.kuanghao11.cn

PHP:  sort($arr);
来源：http://dmp.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bqj.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://qjs.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pwh.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xmx.jinqigufen.top

Ruby: arr.sort
来源：http://ntr.wangshuangyany.cn

C#:   list.Sort();
来源：http://xfd.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://yxj.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bat.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ytk.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dlt.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kuf.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://grm.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dit.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xsh.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pam.gogol.net.cn

[D11] 反转数组
来源：http://hka.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://gpc.meibo888.top

PHP:  array_reverse($arr);
来源：http://rrf.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mqv.bbcook.cn

TS:   [...arr].reverse();
来源：http://qqo.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://tnb.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://uth.gotoacloud.top

Ruby: arr.reverse
来源：http://usr.shuidangran.top

C#:   list.Reverse();
来源：http://zgc.zhengqikj.top

[D12] 查找元素下标
来源：http://cpn.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://uqh.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hkj.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xug.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bzi.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vgj.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://omx.cdnleiting.top

Ruby: arr.index(x)
来源：http://ujw.zycfv.cn

C#:   list.IndexOf(x);
来源：http://tng.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://tum.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tih.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hsi.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://jsz.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://dyy.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mno.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bxs.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://kpr.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kli.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://tzx.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dco.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cfe.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://brf.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://rtn.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hxi.quarkkingdee.top

Go:   // 手写循环
来源：http://gur.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rba.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vls.zdbjq.cn

[D15] 去重
来源：http://wqz.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://auo.9152youxi.cn

PHP:  array_unique($arr);
来源：http://vyk.meibo888.top

JS:   [...new Set(arr)]
来源：http://tsj.yj20258888.top

TS:   [...new Set(arr)]
来源：http://iuz.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oea.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://bam.iojbl.cn

Ruby: arr.uniq
来源：http://let.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://lst.tarul.cn

[D16] 求和与平均值
来源：http://pnk.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jew.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aje.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dnb.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rfo.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eiz.guannengcc.top

Go:   // 手写循环累加
来源：http://bzm.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://azq.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://znx.gaohongyu789.top

[D17] 最大值与最小值
来源：http://yec.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://irc.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://joa.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vui.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://uuz.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vxf.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cuy.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://vsi.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://oql.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://hss.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qrj.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://bnn.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aoh.epnwcf.com

TS:   nested.flat();
来源：http://mwo.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vic.xylfe.cn

Go:   // 手写双层循环
来源：http://xmd.yanxiufei.cn

Ruby: nested.flatten
来源：http://khc.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yuq.zdbjq.cn

[D19] 按字段分组
来源：http://ved.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gwt.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uzp.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nos.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zhv.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gqb.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://tes.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sai.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nin.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://bev.fzhhl.top

Py:   Counter(arr)
来源：http://cfn.sysykeji.top

PHP:  array_count_values($arr);
来源：http://rnn.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxb.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yie.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://moo.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://aua.ehwqpu.com

Ruby: arr.tally
来源：http://rmr.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://phr.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://uzk.zhiwuduotai.top

Py:   x in arr
来源：http://lkn.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://nhe.wangdashe.top

JS:   arr.includes(x)
来源：http://jsp.cucudq.cn

TS:   arr.includes(x)
来源：http://enj.wangshuangyany.cn

Java: list.contains(x)
来源：http://omi.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://akb.sysykeji.top

Ruby: arr.include?(x)
来源：http://hkl.yonumen.top

C#:   list.Contains(x)
来源：http://hze.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://vlx.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zzn.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://goy.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://neq.hcnkem.com

TS:   [...arr];
来源：http://gec.bbcook.cn

Java: new ArrayList<>(list);
来源：http://tkx.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://gir.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://sfb.nanxinkj.top

C#:   new List<int>(list);
来源：http://xzo.jianghu66.top

[D23] reduce 累积计算
来源：http://eyr.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zzn.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mmh.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dzs.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ouh.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rig.vehdjk.com

Go:   // 手写循环
来源：http://myk.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zqd.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jcc.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://ffv.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ngu.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tko.chenjidiqi.icu


<!-- 参考信息 -->