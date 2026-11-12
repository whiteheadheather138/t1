代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kmf.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iqx.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://boe.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mmz.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hnw.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pnp.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ony.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fuv.tianlin.xyz

[C10] 变量作用域
来源：http://gcz.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://syh.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gcl.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ilq.shuidangran.top

TS:   同 JS
来源：http://wkm.cdnleiting.top

Java: 方法内为块级作用域
来源：http://kcg.sweek.top

Go:   花括号块级作用域
来源：http://yve.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://odj.yonumen.top

C#:   块级作用域
来源：http://oeg.daxiang520.top

[C11] 模块导入与导出
来源：http://gkv.tian-w.cn

Py:   from module import func
来源：http://jqk.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tmh.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://drb.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://egm.smart0.xyz

Java: import java.util.List;
来源：http://jsw.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pia.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://aeg.nwbrower.top

C#:   using System.Text;
来源：http://bma.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://erq.havefunace.top

Py:   (lambda: print("run"))()
来源：http://gwd.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://jrm.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://xat.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://dlo.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sto.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://tvq.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://pce.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://aal.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://yci.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ytr.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kvj.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zvl.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qtf.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://cdg.sweek.top

Go:   func add(a, b int) int
来源：http://thi.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wqn.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yjr.nanxinkj.top

[C14] 泛型函数
来源：http://zbp.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nje.fktsv.cn

PHP:  // 无泛型
来源：http://mzo.sysykeji.top

JS:   // 无泛型
来源：http://gzo.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://frg.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zyw.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hdd.ivvv.top

Ruby: # 无泛型
来源：http://zth.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mvx.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://gpq.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lsp.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://vaf.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lqw.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hrm.svipenyu.cn

Java: // 无解构
来源：http://xqk.yuxming.cn

Go:   // 无解构
来源：http://yya.dashuyun.cn

Ruby: a, b = pair
来源：http://mci.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://gwb.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://wad.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://npp.vehdjk.com

PHP:  // 无重载
来源：http://vme.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vyl.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://kuo.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://mxq.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://ega.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://biq.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://euh.yangfankeji.com

================================================================================
来源：http://xgl.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://qdg.yj202588.top

================================================================================
来源：http://mzh.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://zin.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://cke.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jea.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rhn.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dah.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jxy.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://dth.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://nwc.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ppc.svipenyu.cn

[D02] 追加元素到末尾
来源：http://fgl.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ivb.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ssa.fengsongda.top

JS:   arr.push(4);
来源：http://fto.fktsv.cn

TS:   arr.push(4);
来源：http://yti.guowangkeji.top

Java: list.add(4);
来源：http://atk.birdmap.top

Go:   arr = append(arr, 4)
来源：http://cbw.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://puy.hysaishi.cn

C#:   list.Add(4);
来源：http://ugp.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://uoo.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://jdj.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://udq.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cnx.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://dym.sweek.top

Java: list.add(0, 0);
来源：http://izh.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wjn.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://usd.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://zqw.sjlbkw.cn

[D04] 删除元素
来源：http://yrh.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://exr.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xsb.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nby.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://hxy.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qsc.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rud.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cdz.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jny.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://fks.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://snm.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mxn.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://thx.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://ahd.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://chh.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://hwt.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://drn.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zxt.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://gpc.ivvv.top

Py:   len(arr)
来源：http://rlr.tanke756.top

PHP:  count($arr);
来源：http://oze.gotoacloud.top

JS:   arr.length
来源：http://ske.bbcook.cn

TS:   arr.length
来源：http://fiw.jlsjyb.cn

Java: list.size();
来源：http://ofz.jinghuilouyu.cn

Go:   len(arr)
来源：http://ijn.vehdjk.com

Ruby: arr.length; arr.size
来源：http://wcm.iojbl.cn

C#:   list.Count;
来源：http://wmx.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://oft.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpc.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://oaz.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://gkz.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://rth.epnwcf.com

Java: list.subList(1, 4);
来源：http://dpp.birdmap.top

Go:   arr[1:4]
来源：http://tiv.ctjpmb.com

Ruby: arr[1, 3]
来源：http://yka.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://coi.jianghu66.top

[D08] 合并两个数组
来源：http://xmn.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://vna.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://isj.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dlx.zhixingplan.top

TS:   [...a, ...b];
来源：http://qpd.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://poz.ctjpmb.com

Go:   append(a, b...)
来源：http://bfd.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://ojw.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://kbq.xinyue.icu

[D09] 排序（升序）
来源：http://gec.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://nvz.quarkkingdee.top

PHP:  sort($arr);
来源：http://mbc.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wfk.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dcv.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xqb.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://peq.gzhubu.top

Ruby: arr.sort
来源：http://yuz.xuanzx.com

C#:   list.Sort();
来源：http://fls.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://onq.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ocy.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lpr.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oeb.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xfl.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mfq.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bro.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uzf.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uyo.haohaochexian.top

[D11] 反转数组
来源：http://uca.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://haw.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://qpl.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzn.cqqwz.cn

TS:   [...arr].reverse();
来源：http://gwk.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://rvd.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://qxe.dashuyun.cn

Ruby: arr.reverse
来源：http://bik.fengsongda.top

C#:   list.Reverse();
来源：http://uuz.ctjpmb.com

[D12] 查找元素下标
来源：http://lud.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://qje.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rrr.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nfa.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gnm.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wup.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://agg.gaohongyu789.top

Ruby: arr.index(x)
来源：http://dpe.fktsv.cn

C#:   list.IndexOf(x);
来源：http://byw.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://naa.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wat.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://deu.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://yuc.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://uyw.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tde.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fkc.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cgb.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://nqz.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://fqn.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qzv.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lwu.sweek.top

JS:   arr.map(x => x * 2)
来源：http://mzz.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://lpy.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bto.fanxiaobao.xyz

Go:   // 手写循环
来源：http://beg.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qdr.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nxo.smart0.xyz

[D15] 去重
来源：http://odx.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://anl.fzhhl.top

PHP:  array_unique($arr);
来源：http://dpv.fktsv.cn

JS:   [...new Set(arr)]
来源：http://bmz.c1oappe.top

TS:   [...new Set(arr)]
来源：http://uvk.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gvm.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ptr.xziqi.cn

Ruby: arr.uniq
来源：http://epx.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://dtt.hnxiangtu.top

[D16] 求和与平均值
来源：http://ncn.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xjc.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iib.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqg.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqn.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://psq.hywenlv.cn

Go:   // 手写循环累加
来源：http://drg.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hts.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://wrt.birdmap.top

[D17] 最大值与最小值
来源：http://ldf.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://rmh.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://kzn.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sco.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://lqx.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tdf.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mxy.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://lqu.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://xyw.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://smt.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zfl.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://tjy.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hoh.guowangkeji.top

TS:   nested.flat();
来源：http://yiq.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ccc.ehwqpu.com

Go:   // 手写双层循环
来源：http://daf.nwbrower.top

Ruby: nested.flatten
来源：http://pvg.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zum.yueranfly.top

[D19] 按字段分组
来源：http://jzo.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hqq.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kdq.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dpl.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pbg.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xiq.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://bix.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fwb.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ssd.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://dzz.yanxiufei.cn

Py:   Counter(arr)
来源：http://cus.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://elz.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yut.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kpw.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pfx.yj20258.top

Go:   // 手写 map[T]int
来源：http://htu.c1oappe.top

Ruby: arr.tally
来源：http://osp.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eit.tian-w.cn

[D21] 判断是否包含某元素
来源：http://otu.jinyuanbaomall.cn

Py:   x in arr
来源：http://smx.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://ixn.yangfankeji.com

JS:   arr.includes(x)
来源：http://qic.zhoulong.xyz

TS:   arr.includes(x)
来源：http://dpk.smart0.xyz

Java: list.contains(x)
来源：http://qtz.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://lxz.cdnleiting.top

Ruby: arr.include?(x)
来源：http://qzo.pycfn.com

C#:   list.Contains(x)
来源：http://aiw.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://kcs.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yag.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rri.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ftm.vqdsnc.cn

TS:   [...arr];
来源：http://bwg.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://qls.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://ase.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://fra.hfpthk.cn

C#:   new List<int>(list);
来源：http://qos.tarul.cn

[D23] reduce 累积计算
来源：http://mxj.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://olp.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://itk.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xsg.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aue.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iis.zhijiandao.cn

Go:   // 手写循环
来源：http://cxe.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qzs.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qbj.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://xsa.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zsv.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ssa.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mpn.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bto.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ztb.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xlx.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://imc.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lfn.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://egg.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yia.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bbz.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://boc.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sdw.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ygj.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cgu.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://phs.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jna.fehbvm.com

[D26] 数组转字符串
来源：http://hyr.ppjwa.cn


<!-- 参考信息 -->