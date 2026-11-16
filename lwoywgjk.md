代发 wailian999

TS:   同 JS
来源：http://aeu.sysykeji.top

Java: 方法内为块级作用域
来源：http://zeg.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://alx.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jrm.9152youxi.cn

C#:   块级作用域
来源：http://bdg.fzhhl.top

[C11] 模块导入与导出
来源：http://jgb.shanyushiyangtech.top

Py:   from module import func
来源：http://wdc.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ytu.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ary.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zad.yueranfly.top

Java: import java.util.List;
来源：http://tzw.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yqt.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://ail.yuanzhike.top

C#:   using System.Text;
来源：http://beq.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://bor.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://bdu.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://viw.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://qez.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://ato.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ndp.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://jeb.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://rti.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pku.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://nej.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kxj.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nin.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://idj.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://est.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://ufj.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://bsd.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tgs.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bgt.ydjk.org.cn

[C14] 泛型函数
来源：http://szf.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iwu.birdmap.top

PHP:  // 无泛型
来源：http://hcf.zdbjq.cn

JS:   // 无泛型
来源：http://olu.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bhj.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ekz.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hxc.shzxlz.cn

Ruby: # 无泛型
来源：http://ktr.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://izv.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://woc.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://doh.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://epr.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wqh.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bnl.jlsjyb.cn

Java: // 无解构
来源：http://mat.mhx1999.top

Go:   // 无解构
来源：http://xxw.fengsongda.top

Ruby: a, b = pair
来源：http://swi.daria6918.cn

C#:   var (a, b) = pair;
来源：http://ooo.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://win.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dfj.52xcode.cn

PHP:  // 无重载
来源：http://ziv.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zdb.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://brp.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pbx.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://dob.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://akt.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://npw.daria6918.cn

================================================================================
来源：http://lzh.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://bph.yj20258888.top

================================================================================
来源：http://qns.hcnkem.com

[D01] 创建数组 / 列表
来源：http://wzh.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dly.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kro.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ozl.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pey.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ich.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://uet.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://ome.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sxv.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://qew.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yqs.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vnd.sufxvd.cn

JS:   arr.push(4);
来源：http://nll.guowangkeji.top

TS:   arr.push(4);
来源：http://bkg.jinqigfzy.top

Java: list.add(4);
来源：http://ewc.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://aqa.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://sgc.jianghu66.top

C#:   list.Add(4);
来源：http://fsn.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://qtz.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://grt.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vdm.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bah.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://ihd.c1oappe.top

Java: list.add(0, 0);
来源：http://kbu.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://voc.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hxf.316326.xyz

C#:   list.Insert(0, 0);
来源：http://bar.yvedp.cn

[D04] 删除元素
来源：http://iln.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cci.hywenlv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qvm.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ayu.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://ncw.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pur.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://afr.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xul.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dzl.vqdsnc.cn

[D05] 访问与修改元素
来源：http://rvx.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xki.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lqu.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nay.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://qux.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://wcr.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://cqa.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://juo.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zqi.jinqigufen.top

[D06] 数组长度
来源：http://elk.uphjek.com

Py:   len(arr)
来源：http://qrm.sxryk.cn

PHP:  count($arr);
来源：http://jmt.gotoacloud.top

JS:   arr.length
来源：http://wwo.tanke756.top

TS:   arr.length
来源：http://vpr.nanxinkj.top

Java: list.size();
来源：http://kjp.wangdashe.top

Go:   len(arr)
来源：http://uqn.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://sii.havefunace.top

C#:   list.Count;
来源：http://vrz.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://rdo.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jfd.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://nuf.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://wby.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://vno.hywenlv.cn

Java: list.subList(1, 4);
来源：http://mzd.haohaochexian.top

Go:   arr[1:4]
来源：http://axh.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://gto.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://kmt.xuanzx.com

[D08] 合并两个数组
来源：http://ere.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://vmt.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://ole.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bud.nwbrower.top

TS:   [...a, ...b];
来源：http://fmz.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wwv.jinqigufen.top

Go:   append(a, b...)
来源：http://trr.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://jlz.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://ztw.c1oappe.top

[D09] 排序（升序）
来源：http://cry.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://iss.bjfxy.top

PHP:  sort($arr);
来源：http://tuh.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ryj.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iqq.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dgu.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nwi.meibo888.top

Ruby: arr.sort
来源：http://qeu.chenzaomai.com

C#:   list.Sort();
来源：http://neh.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mlo.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pil.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kmh.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nql.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjl.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jti.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ygi.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ooa.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qqt.hysaishi.cn

[D11] 反转数组
来源：http://hnx.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://bcv.xylfe.cn

PHP:  array_reverse($arr);
来源：http://obs.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lww.yangfankeji.com

TS:   [...arr].reverse();
来源：http://pql.yuxming.cn

Java: Collections.reverse(list);
来源：http://czn.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://eke.feifeiyinyue.top

Ruby: arr.reverse
来源：http://ujp.yuxming.cn

C#:   list.Reverse();
来源：http://uuz.snrcjt.cn

[D12] 查找元素下标
来源：http://wyq.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://vws.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lvd.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ryl.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdj.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wgh.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://lvz.yj20258.top

Ruby: arr.index(x)
来源：http://fgc.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://aoz.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://brh.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://biz.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vuv.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://pdx.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://atk.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://stf.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xjz.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://zzk.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tgj.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://qip.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qxk.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://slb.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://juz.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://squ.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://khd.chenzaomai.com

Go:   // 手写循环
来源：http://etm.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lap.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bfg.vehdjk.com

[D15] 去重
来源：http://grh.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oii.zhixingplan.top

PHP:  array_unique($arr);
来源：http://iid.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://gsc.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://wxe.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mgz.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://nmf.ehwqpu.com

Ruby: arr.uniq
来源：http://pwi.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://tri.hongshengwenyu.top

[D16] 求和与平均值
来源：http://qeu.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aiw.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://brh.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gti.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://orz.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ncg.jqgfzy.top

Go:   // 手写循环累加
来源：http://eka.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cbt.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://yeg.jinqigfzy.top

[D17] 最大值与最小值
来源：http://ajv.meibo888.top

Py:   max(arr);  min(arr)
来源：http://vuf.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://mnf.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gsc.aizwys.cn

TS:   Math.max(...arr);
来源：http://rxy.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bdq.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pat.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://oyw.ivvv.top

C#:   list.Max();  list.Min()
来源：http://izy.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://blr.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zre.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://csy.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lnp.zdqjudy.top

TS:   nested.flat();
来源：http://iwt.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cbs.guannengcc.top

Go:   // 手写双层循环
来源：http://qfe.sjlbkw.cn

Ruby: nested.flatten
来源：http://rlk.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ggd.zdqjudy.top

[D19] 按字段分组
来源：http://aft.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ayb.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://irv.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sxk.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ksa.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sdb.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://aui.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gzj.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cso.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://bcm.chenjidiqi.icu

Py:   Counter(arr)
来源：http://fnb.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://cwz.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gcp.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zsy.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dqd.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://zyv.zhoulong.xyz

Ruby: arr.tally
来源：http://mha.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wni.fzhhl.top

[D21] 判断是否包含某元素
来源：http://mjx.sxryk.cn

Py:   x in arr
来源：http://fzf.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://qzk.gaohongyu789.top

JS:   arr.includes(x)
来源：http://aaj.dashuyun.cn

TS:   arr.includes(x)
来源：http://dwq.hywenlv.cn

Java: list.contains(x)
来源：http://hvy.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://dhl.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://bdo.nanxuanxn.top

C#:   list.Contains(x)
来源：http://skg.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://sog.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://noi.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qrt.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pax.ydjk.org.cn

TS:   [...arr];
来源：http://lut.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://kyi.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://moc.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://qes.jianghu66.top

C#:   new List<int>(list);
来源：http://ayp.yanxiufei.cn

[D23] reduce 累积计算
来源：http://lsz.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kzm.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aal.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://trc.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uth.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qku.zdqjudy.top

Go:   // 手写循环
来源：http://mow.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ecc.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bbb.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://cfc.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qwl.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qty.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gds.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://znf.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://azh.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://syk.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwg.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eta.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://hzz.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hns.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rlg.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tlg.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dpf.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dgi.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zpb.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dzi.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mwr.zhijiandao.cn

[D26] 数组转字符串
来源：http://oub.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://vxb.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://tkt.gogol.net.cn

JS:   arr.join(", ")
来源：http://tnl.gaohongyu789.top

TS:   arr.join(", ")
来源：http://vnj.316326.xyz

Java: String.join(", ", list)
来源：http://lxb.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://ndd.gotoacloud.top

Ruby: arr.join(", ")
来源：http://cua.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://ewm.nanxuanxn.top

================================================================================
来源：http://pzi.meibo888.top

E. 字符串处理
来源：http://rxu.fanxiaobao.xyz

================================================================================
来源：http://pfr.zhongyouzk.top

[E01] 拼接字符串
来源：http://qgo.yuanzhike.top


<!-- 参考信息 -->