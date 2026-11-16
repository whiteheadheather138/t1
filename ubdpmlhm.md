代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mfr.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jmc.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iuh.zhiwuduotai.top

[C09] 递归
来源：http://ras.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://twt.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vwq.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kqf.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://snz.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gdi.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zrs.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cyt.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ppw.shzxlz.cn

[C10] 变量作用域
来源：http://wit.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qtm.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fje.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ubu.jinghuilouyu.cn

TS:   同 JS
来源：http://mce.cashguo.top

Java: 方法内为块级作用域
来源：http://uip.zdbjq.cn

Go:   花括号块级作用域
来源：http://pof.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://twk.tanke756.top

C#:   块级作用域
来源：http://xhp.haohaochexian.top

[C11] 模块导入与导出
来源：http://laj.shanyushiyangtech.top

Py:   from module import func
来源：http://fdt.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zjc.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://equ.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uiy.sxryk.cn

Java: import java.util.List;
来源：http://esj.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://arc.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://tbt.hnxiangtu.top

C#:   using System.Text;
来源：http://dba.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://mcl.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://koc.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://jqa.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://jxh.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://nfw.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ysf.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://atd.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://qoe.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cah.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://aji.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oif.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ltc.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gvr.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jol.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://evx.daria6918.cn

Go:   func add(a, b int) int
来源：http://flz.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://shs.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://pxu.mhx1999.top

[C14] 泛型函数
来源：http://mhk.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yvn.jianghu66.top

PHP:  // 无泛型
来源：http://wph.gzhubu.top

JS:   // 无泛型
来源：http://qmy.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kbo.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qnt.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wjy.smart0.xyz

Ruby: # 无泛型
来源：http://wct.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jdk.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://bby.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wyk.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://yof.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bro.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dag.yueranfly.top

Java: // 无解构
来源：http://cnv.sysykeji.top

Go:   // 无解构
来源：http://hke.zhoulong.xyz

Ruby: a, b = pair
来源：http://pjx.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://wnv.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://xpb.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://egv.zhongyouzk.top

PHP:  // 无重载
来源：http://xzj.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://buu.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://vxt.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qfh.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://wsj.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://gvh.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://bsa.tian-w.cn

================================================================================
来源：http://zvi.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://owc.hnxiangtu.top

================================================================================
来源：http://xew.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://tgs.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rov.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cyr.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wis.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hjs.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vxa.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://lja.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://mge.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gja.jinqigufen.top

[D02] 追加元素到末尾
来源：http://ogz.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oac.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rro.sysykeji.top

JS:   arr.push(4);
来源：http://oqq.shangyingyoupin.top

TS:   arr.push(4);
来源：http://vdw.jlsjyb.cn

Java: list.add(4);
来源：http://imf.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://dqp.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://noz.hammf.cn

C#:   list.Add(4);
来源：http://upc.sysykeji.top

[D03] 在指定位置插入元素
来源：http://muu.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://flz.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ptv.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tmr.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://bhn.ctjpmb.com

Java: list.add(0, 0);
来源：http://nlu.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://qqq.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tep.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://qqw.c1oappe.top

[D04] 删除元素
来源：http://pnj.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pcg.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://osy.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mks.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://hgj.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ajm.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ybm.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lfk.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nlm.yuanzhike.top

[D05] 访问与修改元素
来源：http://wwx.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxa.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dgf.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xrs.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://jcu.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://wrv.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://gis.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lyi.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yau.fehbvm.com

[D06] 数组长度
来源：http://our.ivvv.top

Py:   len(arr)
来源：http://xjt.haohaochexian.top

PHP:  count($arr);
来源：http://gas.dashuyun.cn

JS:   arr.length
来源：http://ulo.cucudq.cn

TS:   arr.length
来源：http://coz.jiagoushi.top

Java: list.size();
来源：http://cxi.yanxiufei.cn

Go:   len(arr)
来源：http://wie.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://ayz.zhengqikj.top

C#:   list.Count;
来源：http://jao.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://xpl.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yat.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://gji.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://owg.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://nqj.nwbrower.top

Java: list.subList(1, 4);
来源：http://izr.tian-w.cn

Go:   arr[1:4]
来源：http://wza.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://oih.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://wbz.xuanzx.com

[D08] 合并两个数组
来源：http://quw.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://qlj.yonumen.top

PHP:  array_merge($a, $b);
来源：http://wzt.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yae.hcnkem.com

TS:   [...a, ...b];
来源：http://zfr.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://moy.zhiwuduotai.top

Go:   append(a, b...)
来源：http://ebm.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://ixa.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://igc.feifeiyinyue.top

[D09] 排序（升序）
来源：http://mug.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://kiv.bjfxy.top

PHP:  sort($arr);
来源：http://yoe.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vjt.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sik.uphjek.com

Java: Collections.sort(list);  list.sort(null);
来源：http://cne.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bzg.dashuyun.cn

Ruby: arr.sort
来源：http://eee.shzxlz.cn

C#:   list.Sort();
来源：http://fnh.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uqd.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dsc.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hos.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://irs.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://whr.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bwp.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ncc.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://imm.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rwg.fehbvm.com

[D11] 反转数组
来源：http://iey.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://xkm.fehbvm.com

PHP:  array_reverse($arr);
来源：http://efd.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uzm.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://kkt.andypj.xyz

Java: Collections.reverse(list);
来源：http://zew.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://bdt.epnwcf.com

Ruby: arr.reverse
来源：http://kfl.sysykeji.top

C#:   list.Reverse();
来源：http://lbf.shzxlz.cn

[D12] 查找元素下标
来源：http://wfj.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://adz.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uvq.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://otk.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tag.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cqt.yonumen.top

Go:   slices.Index(arr, x)
来源：http://cnu.52xcode.cn

Ruby: arr.index(x)
来源：http://zsb.sxryk.cn

C#:   list.IndexOf(x);
来源：http://sbu.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://eul.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hnb.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yxu.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://fpc.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://nes.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ixc.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://waz.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://deg.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dnj.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://lkq.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jmr.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dlt.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://dbu.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://uxh.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aaf.zhixingplan.top

Go:   // 手写循环
来源：http://grr.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://afz.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pxj.fzhhl.top

[D15] 去重
来源：http://agt.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lgx.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://ntf.hesvh.cn

JS:   [...new Set(arr)]
来源：http://zkc.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://vrg.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gke.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rgk.gzhubu.top

Ruby: arr.uniq
来源：http://wow.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://acg.yonumen.top

[D16] 求和与平均值
来源：http://etv.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nwi.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ssg.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wqf.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vdy.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fqu.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://utu.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://enb.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://ejf.yfazqb.com

[D17] 最大值与最小值
来源：http://eeo.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://wqt.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://blt.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uso.hysaishi.cn

TS:   Math.max(...arr);
来源：http://nta.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bcj.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jng.yonumen.top

Ruby: arr.max;  arr.min
来源：http://pri.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://npw.uphjek.com

[D18] 扁平化嵌套数组
来源：http://zdo.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yjt.ivvv.top

PHP:  array_merge(...$nested);
来源：http://qar.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rbz.yongpay.top

TS:   nested.flat();
来源：http://qko.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vro.jqgfzy.top

Go:   // 手写双层循环
来源：http://gws.cashguo.top

Ruby: nested.flatten
来源：http://hxi.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yzb.gaohongyu789.top

[D19] 按字段分组
来源：http://xxz.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oba.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hur.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hhj.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://loq.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bou.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://xjm.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zyg.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pvb.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://hou.tian-w.cn

Py:   Counter(arr)
来源：http://dmz.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://afg.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hqp.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://udg.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qhs.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://cwe.cqqwz.cn

Ruby: arr.tally
来源：http://bkm.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://btw.yj20258.top

[D21] 判断是否包含某元素
来源：http://jua.yangfankeji.com

Py:   x in arr
来源：http://cnv.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://eqb.kuanghao11.cn

JS:   arr.includes(x)
来源：http://uyt.xinyue.icu

TS:   arr.includes(x)
来源：http://vzt.dashuyun.cn

Java: list.contains(x)
来源：http://bcn.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://jbl.aizwys.cn

Ruby: arr.include?(x)
来源：http://tls.zdbjq.cn

C#:   list.Contains(x)
来源：http://lvr.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://bbn.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zyn.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fzk.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tja.fengsongda.top

TS:   [...arr];
来源：http://lwy.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://rrr.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tsr.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://nil.shzxlz.cn

C#:   new List<int>(list);
来源：http://djr.sufxvd.cn

[D23] reduce 累积计算
来源：http://osa.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://btg.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mus.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gny.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rts.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lvi.uphjek.com

Go:   // 手写循环
来源：http://ecq.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xmu.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sgf.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://ppd.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vln.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mje.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vfh.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fws.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tne.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://led.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vrg.jinqigfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wzj.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://cdr.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jxv.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cbk.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpy.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xfb.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sfx.redwolf501.top


<!-- 参考信息 -->