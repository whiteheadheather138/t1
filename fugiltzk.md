代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iud.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lgn.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gqh.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kkt.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ikc.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://udm.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mbx.nanxuanxn.top

[C09] 递归
来源：http://rmj.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ost.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wti.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gaa.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ypl.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gpv.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pdp.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bjb.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://szb.zhoulong.xyz

[C10] 变量作用域
来源：http://xsk.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://apj.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kdr.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cyt.zhixingplan.top

TS:   同 JS
来源：http://foe.sysykeji.top

Java: 方法内为块级作用域
来源：http://wzb.zhixingplan.top

Go:   花括号块级作用域
来源：http://sto.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ltm.tarul.cn

C#:   块级作用域
来源：http://vdq.cashguo.top

[C11] 模块导入与导出
来源：http://yol.zhoulong.xyz

Py:   from module import func
来源：http://yyu.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ubm.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://jzi.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zpv.xylfe.cn

Java: import java.util.List;
来源：http://ddt.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tot.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://gsz.vehdjk.com

C#:   using System.Text;
来源：http://dmq.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://sdl.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://kxb.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://drj.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://uwp.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://lcm.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uta.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://twk.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://exw.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pkz.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://xtj.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xzm.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jyt.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xtp.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ksy.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kmx.bbcook.cn

Go:   func add(a, b int) int
来源：http://sfb.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yxe.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://vos.uphjek.com

[C14] 泛型函数
来源：http://ifs.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://duu.hnqzz.top

PHP:  // 无泛型
来源：http://xkw.meibo888.top

JS:   // 无泛型
来源：http://eez.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rnu.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wmw.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fmn.jinqigfzy.top

Ruby: # 无泛型
来源：http://dzw.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wai.zycfv.cn

[C15] 解构 / 展开参数
来源：http://ail.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nmy.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://tqj.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kgz.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ote.gaohongyu789.top

Java: // 无解构
来源：http://jff.fengsongda.top

Go:   // 无解构
来源：http://xee.meibo888.top

Ruby: a, b = pair
来源：http://vax.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://koh.316326.xyz

[C16] 函数 / 方法重载
来源：http://oox.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sfb.yonumen.top

PHP:  // 无重载
来源：http://zxe.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rbk.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://dmp.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wop.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://pht.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://vxj.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xxc.ctjpmb.com

================================================================================
来源：http://fna.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://jdq.hnxiangtu.top

================================================================================
来源：http://fsi.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://ebq.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xzz.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qwd.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rht.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mcj.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zjs.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://vcn.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://dem.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pdl.tanke756.top

[D02] 追加元素到末尾
来源：http://bix.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zkv.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bdb.dashuyun.cn

JS:   arr.push(4);
来源：http://xeg.uphjek.com

TS:   arr.push(4);
来源：http://gso.shuidangran.top

Java: list.add(4);
来源：http://vsd.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://ltq.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://anz.c1oappe.top

C#:   list.Add(4);
来源：http://tdl.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://wfd.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://lmh.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mah.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yhn.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://qbb.xylfe.cn

Java: list.add(0, 0);
来源：http://mwz.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://chp.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ttn.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://mte.smart0.xyz

[D04] 删除元素
来源：http://xnx.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nqs.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wfm.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hek.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://xik.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ulg.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pdi.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jbw.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsd.zdqjudy.top

[D05] 访问与修改元素
来源：http://rbf.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://emq.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yan.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qbg.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://lbu.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://vhs.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://ljb.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dxb.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vcd.jqgfzy.top

[D06] 数组长度
来源：http://igc.epnwcf.com

Py:   len(arr)
来源：http://ulo.birdmap.top

PHP:  count($arr);
来源：http://vze.gogol.net.cn

JS:   arr.length
来源：http://lpr.yj202588.top

TS:   arr.length
来源：http://afr.yuxming.cn

Java: list.size();
来源：http://uin.birdmap.top

Go:   len(arr)
来源：http://geb.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://ekm.ydzc1.top

C#:   list.Count;
来源：http://mbw.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://xwb.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hmx.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qfx.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://aov.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://dsf.iojbl.cn

Java: list.subList(1, 4);
来源：http://the.jianghu66.top

Go:   arr[1:4]
来源：http://kwr.fzhhl.top

Ruby: arr[1, 3]
来源：http://aih.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://krb.yueranfly.top

[D08] 合并两个数组
来源：http://cpk.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://zio.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://lpi.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yst.epnwcf.com

TS:   [...a, ...b];
来源：http://yje.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mcw.yueranfly.top

Go:   append(a, b...)
来源：http://jgo.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://swo.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://qer.daxiang520.top

[D09] 排序（升序）
来源：http://ddh.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://wwo.cashguo.top

PHP:  sort($arr);
来源：http://mtr.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wng.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://syn.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kgx.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rxw.tanke756.top

Ruby: arr.sort
来源：http://mgs.gogol.net.cn

C#:   list.Sort();
来源：http://grl.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://afl.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zrx.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uqi.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lqa.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://riv.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wnt.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dsh.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ohu.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://swp.havefunace.top

[D11] 反转数组
来源：http://jmh.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://clt.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://waf.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vpu.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://rdz.chenzaomai.com

Java: Collections.reverse(list);
来源：http://hag.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://gfz.zdqjudy.top

Ruby: arr.reverse
来源：http://lii.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://rei.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://zhv.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://kwe.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://atr.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cck.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mrk.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bxb.cashguo.top

Go:   slices.Index(arr, x)
来源：http://jzx.dashuyun.cn

Ruby: arr.index(x)
来源：http://tzj.havefunace.top

C#:   list.IndexOf(x);
来源：http://zir.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://ewc.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hvi.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://poy.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://nzs.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://oei.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wjj.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ndd.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://ogw.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://uin.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://mcz.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mrf.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mnk.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://guk.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://ltn.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cwd.hfpthk.cn

Go:   // 手写循环
来源：http://wnb.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://fuk.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kks.zhongyouzk.top

[D15] 去重
来源：http://hly.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://siv.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://xoi.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://kiw.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://gtq.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pyu.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lha.hnxiangtu.top

Ruby: arr.uniq
来源：http://lam.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://fza.shangyingyoupin.top

[D16] 求和与平均值
来源：http://wuq.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jsa.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://til.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uer.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://urw.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ouw.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://dql.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wps.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://sbb.nwbrower.top

[D17] 最大值与最小值
来源：http://gzr.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://wnl.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://nyy.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pza.cheryme.top

TS:   Math.max(...arr);
来源：http://qia.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://buw.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ovv.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://bcg.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://ped.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://fyr.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mmq.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://geu.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hoy.jqgufenzy.top

TS:   nested.flat();
来源：http://vql.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xym.daria6918.cn

Go:   // 手写双层循环
来源：http://ctq.hesvh.cn

Ruby: nested.flatten
来源：http://nda.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qja.zhengqikj.top

[D19] 按字段分组
来源：http://pep.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://max.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mtg.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vaz.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cvv.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xbe.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://jis.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jma.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dhn.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://djn.zycfv.cn

Py:   Counter(arr)
来源：http://bsx.yonumen.top

PHP:  array_count_values($arr);
来源：http://wmr.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tzq.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://poa.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mtw.tarul.cn

Go:   // 手写 map[T]int
来源：http://iwu.wangdashe.top

Ruby: arr.tally
来源：http://nik.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fzn.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://jfy.haohaochexian.top

Py:   x in arr
来源：http://kbr.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://eht.aibaodan.cn

JS:   arr.includes(x)
来源：http://wqk.jlsjyb.cn

TS:   arr.includes(x)
来源：http://crt.ydjk.org.cn

Java: list.contains(x)
来源：http://nrz.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://ohx.c1oappe.top

Ruby: arr.include?(x)
来源：http://lmi.yvedp.cn

C#:   list.Contains(x)
来源：http://rtq.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://cvt.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mtu.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eeb.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cgn.ppjwa.cn

TS:   [...arr];
来源：http://tsb.pycfn.com

Java: new ArrayList<>(list);
来源：http://xsp.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://aym.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://zbf.cashguo.top

C#:   new List<int>(list);
来源：http://jky.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://ugt.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://axm.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sia.xylfe.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krw.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fnj.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zxi.nanxuanxn.top

Go:   // 手写循环
来源：http://ipz.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tek.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bix.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://vmq.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fwu.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://awc.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dkh.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rqe.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vsx.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uwj.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zyf.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wkq.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://qsj.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xqo.cqqwz.cn


<!-- 参考信息 -->