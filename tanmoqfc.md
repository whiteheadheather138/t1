代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yzk.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zxi.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://htg.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ktd.0kj1m.cn

[C10] 变量作用域
来源：http://iul.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zgn.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hng.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ykw.jlsjyb.cn

TS:   同 JS
来源：http://afw.redwolf501.top

Java: 方法内为块级作用域
来源：http://dyr.jqgufenzy.top

Go:   花括号块级作用域
来源：http://uqr.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://guf.iojbl.cn

C#:   块级作用域
来源：http://nbs.uphjek.com

[C11] 模块导入与导出
来源：http://wlz.birdmap.top

Py:   from module import func
来源：http://wxt.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bmr.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vvp.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xfr.wangdashe.top

Java: import java.util.List;
来源：http://lsm.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tsg.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://jed.yvedp.cn

C#:   using System.Text;
来源：http://vrb.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://hwm.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://ban.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://bjv.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://nzw.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://fsb.ivvv.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bix.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://pcp.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://suw.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://slx.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://hxv.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://djg.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rpv.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vha.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jaq.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vbb.guowangkeji.top

Go:   func add(a, b int) int
来源：http://xyf.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gai.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jvh.hywenlv.cn

[C14] 泛型函数
来源：http://knd.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://puu.bbcook.cn

PHP:  // 无泛型
来源：http://wza.52xcode.cn

JS:   // 无泛型
来源：http://ngf.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lrd.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jac.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gnk.c1oappe.top

Ruby: # 无泛型
来源：http://qpv.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://afc.jianghu66.top

[C15] 解构 / 展开参数
来源：http://ohp.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uyc.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://hmc.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vxu.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tfk.haohaochexian.top

Java: // 无解构
来源：http://qtt.zdbjq.cn

Go:   // 无解构
来源：http://xkx.yonumen.top

Ruby: a, b = pair
来源：http://goe.ivvv.top

C#:   var (a, b) = pair;
来源：http://bpf.epnwcf.com

[C16] 函数 / 方法重载
来源：http://crq.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dpk.epnwcf.com

PHP:  // 无重载
来源：http://kju.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tii.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://jtj.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://lsc.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://gbv.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://nop.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hjg.smart0.xyz

================================================================================
来源：http://ydv.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://vby.tarul.cn

================================================================================
来源：http://vik.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://oit.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ild.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://drr.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hvp.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dlq.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rvi.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://iox.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://mae.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xvd.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://ngk.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://scg.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kzz.wangshuangyany.cn

JS:   arr.push(4);
来源：http://xzy.nanxuanxn.top

TS:   arr.push(4);
来源：http://ybw.hysaishi.cn

Java: list.add(4);
来源：http://tho.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://cbw.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://hwo.hfpthk.cn

C#:   list.Add(4);
来源：http://ena.hnqzz.top

[D03] 在指定位置插入元素
来源：http://yyc.316326.xyz

Py:   arr.insert(0, 0)
来源：http://xgw.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zrn.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lfy.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://guj.fengsongda.top

Java: list.add(0, 0);
来源：http://pmv.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://saa.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wwl.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://fap.epnwcf.com

[D04] 删除元素
来源：http://eqd.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ffu.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://skn.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kpm.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://mif.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://knw.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zzr.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rkf.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://juh.uphjek.com

[D05] 访问与修改元素
来源：http://wiv.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vap.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eqz.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pju.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://pda.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://msd.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://bzq.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xwh.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dze.hesvh.cn

[D06] 数组长度
来源：http://pdp.jinqigufen.top

Py:   len(arr)
来源：http://unb.jinghuilouyu.cn

PHP:  count($arr);
来源：http://fsm.ybcxt.top

JS:   arr.length
来源：http://bqt.52xcode.cn

TS:   arr.length
来源：http://zne.yangfankeji.com

Java: list.size();
来源：http://lwk.ctjpmb.com

Go:   len(arr)
来源：http://cgn.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://dxr.snrcjt.cn

C#:   list.Count;
来源：http://qow.smart0.xyz

[D07] 切片 / 取子数组
来源：http://cjs.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ggd.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zsv.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://qmd.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://gta.gzhubu.top

Java: list.subList(1, 4);
来源：http://kna.xuanzx.com

Go:   arr[1:4]
来源：http://uky.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://iyb.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://fbr.haohaochexian.top

[D08] 合并两个数组
来源：http://zwt.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://ihh.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://npa.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ldb.cucudq.cn

TS:   [...a, ...b];
来源：http://kdc.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oof.bjfxy.top

Go:   append(a, b...)
来源：http://doi.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://rwb.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://gtq.meibo888.top

[D09] 排序（升序）
来源：http://pug.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://ybo.hammf.cn

PHP:  sort($arr);
来源：http://akq.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://taq.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tzx.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mug.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://emb.jianghu66.top

Ruby: arr.sort
来源：http://kjy.316326.xyz

C#:   list.Sort();
来源：http://lbn.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sqf.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zhn.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ycr.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ogu.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdo.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kgh.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://phy.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bwp.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pvx.jyoumei.cn

[D11] 反转数组
来源：http://enx.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://jlu.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://mcy.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oni.zhengqikj.top

TS:   [...arr].reverse();
来源：http://qfa.cdnleiting.top

Java: Collections.reverse(list);
来源：http://cim.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://awk.tarul.cn

Ruby: arr.reverse
来源：http://ytm.gotoacloud.top

C#:   list.Reverse();
来源：http://tmv.jinqigufen.top

[D12] 查找元素下标
来源：http://bso.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://eyr.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bkp.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csw.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ewt.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mdk.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://pub.zdbjq.cn

Ruby: arr.index(x)
来源：http://umo.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://rxu.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://zfz.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://asg.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lkz.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://lwt.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://aym.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zly.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zap.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://apv.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gau.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://ena.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://myo.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://atr.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://pcg.sweek.top

TS:   arr.map(x => x * 2)
来源：http://jps.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mox.daria6918.cn

Go:   // 手写循环
来源：http://vqc.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fqz.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://usu.hammf.cn

[D15] 去重
来源：http://dur.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jlc.xuanzx.com

PHP:  array_unique($arr);
来源：http://jxy.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://jvr.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://gec.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eoj.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://cow.hcnkem.com

Ruby: arr.uniq
来源：http://gma.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://coo.aibaodan.cn

[D16] 求和与平均值
来源：http://tje.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xjz.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zrp.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://idn.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ytt.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oqp.mhx1999.top

Go:   // 手写循环累加
来源：http://mrc.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zaj.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://zol.hfpthk.cn

[D17] 最大值与最小值
来源：http://ozz.316326.xyz

Py:   max(arr);  min(arr)
来源：http://kpg.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://gtj.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qoz.jianghu66.top

TS:   Math.max(...arr);
来源：http://jjb.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dcm.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bku.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://usi.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://mpt.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://rhb.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aoj.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://and.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ogk.tian-w.cn

TS:   nested.flat();
来源：http://xne.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://csq.jqgfzy.top

Go:   // 手写双层循环
来源：http://znc.9152youxi.cn

Ruby: nested.flatten
来源：http://ugp.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://kro.haohaochexian.top

[D19] 按字段分组
来源：http://acz.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gem.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mem.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dkk.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dzy.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ewd.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://tyq.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://slf.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wsy.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://ohg.shuidangran.top

Py:   Counter(arr)
来源：http://rju.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://wte.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjx.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aju.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zlm.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://wsm.yangfankeji.com

Ruby: arr.tally
来源：http://usm.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eft.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://eic.sxryk.cn

Py:   x in arr
来源：http://qip.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://swb.ctjpmb.com

JS:   arr.includes(x)
来源：http://xct.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://liy.fengsongda.top

Java: list.contains(x)
来源：http://xkl.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://gdj.haohaochexian.top

Ruby: arr.include?(x)
来源：http://ntp.hfpthk.cn

C#:   list.Contains(x)
来源：http://mgh.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://pun.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qro.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://thm.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kei.havefunace.top

TS:   [...arr];
来源：http://fzf.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://ayp.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://phh.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://gtn.yuanzhike.top

C#:   new List<int>(list);
来源：http://qww.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://ldr.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://owv.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cjs.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uag.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xan.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mee.hysaishi.cn

Go:   // 手写循环
来源：http://xkx.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gyf.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nbn.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://sdj.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zsj.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://imk.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mpo.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bwi.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uwp.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qax.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sdt.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cdz.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://zms.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whp.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oah.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oiv.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://txb.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://arf.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ftr.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qnm.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jqb.sjlbkw.cn

[D26] 数组转字符串
来源：http://jpx.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://hyt.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://ujf.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://wnh.vqdsnc.cn

TS:   arr.join(", ")
来源：http://ahy.hammf.cn


<!-- 参考信息 -->