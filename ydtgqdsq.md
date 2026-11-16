代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://ivw.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mta.hysaishi.cn

[C08] 闭包
来源：http://eso.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bfx.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://srv.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qko.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xnn.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jgi.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ywq.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jsp.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wjr.shzxlz.cn

[C09] 递归
来源：http://gys.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://utl.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://npl.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nru.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eif.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xea.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wtn.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fml.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kdm.hfpthk.cn

[C10] 变量作用域
来源：http://xje.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pxm.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://htl.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wzv.shangyingyoupin.top

TS:   同 JS
来源：http://lfq.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://tnx.cdnleiting.top

Go:   花括号块级作用域
来源：http://ssl.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://upx.xinyue.icu

C#:   块级作用域
来源：http://sub.shzxlz.cn

[C11] 模块导入与导出
来源：http://crv.xziqi.cn

Py:   from module import func
来源：http://cky.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lor.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sge.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lgj.iojbl.cn

Java: import java.util.List;
来源：http://umh.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mny.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://wat.9152youxi.cn

C#:   using System.Text;
来源：http://xdw.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://nfc.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://lmh.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://bvi.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://zcp.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://yal.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iyq.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://nlo.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://qil.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://avy.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://fqf.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yrs.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ymy.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fvs.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdq.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://auf.gogol.net.cn

Go:   func add(a, b int) int
来源：http://ael.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cjc.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://yqn.jyoumei.cn

[C14] 泛型函数
来源：http://dmm.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wln.sweek.top

PHP:  // 无泛型
来源：http://you.birdmap.top

JS:   // 无泛型
来源：http://pgo.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lng.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hmr.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jvt.nwbrower.top

Ruby: # 无泛型
来源：http://fij.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bzy.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://hol.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nkl.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://csp.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mef.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ndy.ehwqpu.com

Java: // 无解构
来源：http://gwe.gzhubu.top

Go:   // 无解构
来源：http://iod.tanke756.top

Ruby: a, b = pair
来源：http://apu.yj20258888.top

C#:   var (a, b) = pair;
来源：http://ecg.mhx1999.top

[C16] 函数 / 方法重载
来源：http://zza.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://swi.jlsjyb.cn

PHP:  // 无重载
来源：http://iuh.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bwy.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://qyy.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oyw.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://tqm.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://ivp.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ttn.hysaishi.cn

================================================================================
来源：http://iei.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://nlw.0kj1m.cn

================================================================================
来源：http://pyc.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://nhg.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dwl.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kxd.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jtu.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wdu.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fjs.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://xot.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://vlp.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lgw.ydzc1.top

[D02] 追加元素到末尾
来源：http://zxx.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nhl.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xnf.jinqigufen.top

JS:   arr.push(4);
来源：http://kby.epnwcf.com

TS:   arr.push(4);
来源：http://zrg.andypj.xyz

Java: list.add(4);
来源：http://ius.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://rza.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://nsc.hfpthk.cn

C#:   list.Add(4);
来源：http://yue.cashguo.top

[D03] 在指定位置插入元素
来源：http://scg.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://ono.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oix.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nmt.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://ebu.guowangkeji.top

Java: list.add(0, 0);
来源：http://ife.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cvu.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://exp.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://qex.zhijiandao.cn

[D04] 删除元素
来源：http://khd.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jku.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uqs.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbm.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://vok.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bry.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jxx.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hce.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wil.zhengqikj.top

[D05] 访问与修改元素
来源：http://avs.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jqo.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://smn.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wut.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://eqk.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://fjp.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://kqu.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dck.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hof.smart0.xyz

[D06] 数组长度
来源：http://asf.fktsv.cn

Py:   len(arr)
来源：http://xzf.sysykeji.top

PHP:  count($arr);
来源：http://hsm.fengsongda.top

JS:   arr.length
来源：http://jic.zhiwuduotai.top

TS:   arr.length
来源：http://ldw.aibaodan.cn

Java: list.size();
来源：http://tsd.redwolf501.top

Go:   len(arr)
来源：http://zds.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://yro.pengpengdd.cyou

C#:   list.Count;
来源：http://xns.hnqzz.top

[D07] 切片 / 取子数组
来源：http://gsd.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qaz.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://opv.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://hzx.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://jzz.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://wpa.hcnkem.com

Go:   arr[1:4]
来源：http://riw.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://ipp.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://wvn.zycfv.cn

[D08] 合并两个数组
来源：http://owv.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://ecn.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://nfz.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://eeu.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://hux.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jbj.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://jxr.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://tiu.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://lxd.bbcook.cn

[D09] 排序（升序）
来源：http://pli.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://nrv.sweek.top

PHP:  sort($arr);
来源：http://eum.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://knc.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jlj.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://cui.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fqr.tanke756.top

Ruby: arr.sort
来源：http://xay.daxiang520.top

C#:   list.Sort();
来源：http://rrb.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kuo.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hqj.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lyi.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://keu.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jxk.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rkc.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wkn.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kxd.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jqm.sxryk.cn

[D11] 反转数组
来源：http://rab.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://rck.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://mwt.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wbo.yfazqb.com

TS:   [...arr].reverse();
来源：http://uda.yvedp.cn

Java: Collections.reverse(list);
来源：http://oci.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://mjm.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://axh.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://uxt.chenjidiqi.icu

[D12] 查找元素下标
来源：http://aym.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://unb.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dqh.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kup.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bew.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hmg.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://jpr.daxiang520.top

Ruby: arr.index(x)
来源：http://fkw.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://vdm.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://fxw.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://koh.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lef.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://xcf.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://wql.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wqa.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hbw.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://mtk.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bhr.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://lfn.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ezz.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://amh.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://zhs.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://ypu.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://glq.ivvv.top

Go:   // 手写循环
来源：http://wpu.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://gac.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gnt.jlsjyb.cn

[D15] 去重
来源：http://dpr.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rbn.birdmap.top

PHP:  array_unique($arr);
来源：http://bsh.316326.xyz

JS:   [...new Set(arr)]
来源：http://ayv.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://exv.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ywr.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://net.jianghu66.top

Ruby: arr.uniq
来源：http://gbe.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://exc.yangfankeji.com

[D16] 求和与平均值
来源：http://lfu.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://svl.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tac.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bah.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zrd.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ljh.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://gzp.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://heg.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://tap.hnxiangtu.top

[D17] 最大值与最小值
来源：http://dkr.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://ggw.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://cnk.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bzu.zdbjq.cn

TS:   Math.max(...arr);
来源：http://nst.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xic.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dyp.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://sjo.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://orf.tanke756.top

[D18] 扁平化嵌套数组
来源：http://ryh.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hiv.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://wcu.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lsw.kuanghao11.cn

TS:   nested.flat();
来源：http://med.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iqn.316326.xyz

Go:   // 手写双层循环
来源：http://mbq.fzhhl.top

Ruby: nested.flatten
来源：http://hwf.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://bie.bbcook.cn

[D19] 按字段分组
来源：http://oct.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sdo.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qyy.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zew.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sie.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nec.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://mtb.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://add.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iiy.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://vkh.aibaodan.cn

Py:   Counter(arr)
来源：http://ccz.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://gav.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abn.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://taa.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hqh.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://jed.sxryk.cn

Ruby: arr.tally
来源：http://due.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uxu.iojbl.cn

[D21] 判断是否包含某元素
来源：http://hwc.snrcjt.cn

Py:   x in arr
来源：http://khz.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://rpd.316326.xyz

JS:   arr.includes(x)
来源：http://jbk.ydzc1.top

TS:   arr.includes(x)
来源：http://jgf.yj20258888.top

Java: list.contains(x)
来源：http://odl.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://buq.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://fbw.yueranfly.top

C#:   list.Contains(x)
来源：http://ncm.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://ywn.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tny.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://odq.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nbo.kuanghao11.cn

TS:   [...arr];
来源：http://pvb.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://qxh.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://cjv.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://gba.jinqigfzy.top

C#:   new List<int>(list);
来源：http://pqy.zhijiandao.cn

[D23] reduce 累积计算
来源：http://bdg.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vqt.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uab.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wou.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wsx.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ndd.0kj1m.cn

Go:   // 手写循环
来源：http://bec.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kiz.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eoo.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://ecc.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jhq.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jzx.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iim.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://woy.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xys.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ggq.gzhubu.top


<!-- 参考信息 -->