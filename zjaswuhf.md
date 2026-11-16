代发 wailian999

[C10] 变量作用域
来源：http://bfx.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hae.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rpx.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hin.sxryk.cn

TS:   同 JS
来源：http://fup.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://bvh.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://him.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xto.shanyushiyangkeji.top

C#:   块级作用域
来源：http://tlh.yanxiufei.cn

[C11] 模块导入与导出
来源：http://ljj.cheryme.top

Py:   from module import func
来源：http://kvm.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://adl.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://gdy.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dxf.havefunace.top

Java: import java.util.List;
来源：http://kue.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oya.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://wec.haohaochexian.top

C#:   using System.Text;
来源：http://ilp.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://whx.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://ejb.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://hji.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://onm.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://wzu.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ioy.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://igb.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://bdc.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ykl.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://ekh.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nfh.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rel.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fjz.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dyu.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ykq.andypj.xyz

Go:   func add(a, b int) int
来源：http://tnn.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zck.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uwv.ivvv.top

[C14] 泛型函数
来源：http://irs.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://whx.jyoumei.cn

PHP:  // 无泛型
来源：http://enf.zhongyouzk.top

JS:   // 无泛型
来源：http://ava.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zxy.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://llx.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hgy.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://ftf.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mff.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://qhu.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fpw.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://oyr.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ipo.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mrv.hcnkem.com

Java: // 无解构
来源：http://wnb.hongshengwenyu.top

Go:   // 无解构
来源：http://ztj.jqgufenzy.top

Ruby: a, b = pair
来源：http://dot.52xcode.cn

C#:   var (a, b) = pair;
来源：http://exc.fehbvm.com

[C16] 函数 / 方法重载
来源：http://zzs.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zje.chenlongwang.top

PHP:  // 无重载
来源：http://jzr.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilb.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://vya.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mpt.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://jfv.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://dyt.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iop.yfazqb.com

================================================================================
来源：http://zvy.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://mrk.vehdjk.com

================================================================================
来源：http://duy.yonumen.top

[D01] 创建数组 / 列表
来源：http://yco.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nct.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pll.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dki.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ydk.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ksj.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://nmh.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://vdb.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xxe.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://dpz.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tgf.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pyq.hnqzz.top

JS:   arr.push(4);
来源：http://ado.yvedp.cn

TS:   arr.push(4);
来源：http://wip.sweek.top

Java: list.add(4);
来源：http://wrh.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://qdw.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://nno.haohaochexian.top

C#:   list.Add(4);
来源：http://cjt.bbcook.cn

[D03] 在指定位置插入元素
来源：http://atv.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://emn.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fqc.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kjs.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://dus.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://wfq.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://ngr.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dzx.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://awb.tarul.cn

[D04] 删除元素
来源：http://sjb.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fah.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://stq.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wmb.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://lny.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fll.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ogs.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rsy.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zys.yuxming.cn

[D05] 访问与修改元素
来源：http://lbj.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cwe.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fpz.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://brn.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://sgb.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://ffz.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://mlb.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ofk.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eal.uphjek.com

[D06] 数组长度
来源：http://xwl.guannengcc.top

Py:   len(arr)
来源：http://wid.aibaodan.cn

PHP:  count($arr);
来源：http://nvf.zhiwuduotai.top

JS:   arr.length
来源：http://srs.gzhubu.top

TS:   arr.length
来源：http://bdl.nanxinkj.top

Java: list.size();
来源：http://ozg.hywenlv.cn

Go:   len(arr)
来源：http://cxx.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://nni.gaohongyu789.top

C#:   list.Count;
来源：http://rta.c1oappe.top

[D07] 切片 / 取子数组
来源：http://ezt.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ucg.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://oeo.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://znl.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://hnv.xinyue.icu

Java: list.subList(1, 4);
来源：http://sez.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://cng.jinqigufen.top

Ruby: arr[1, 3]
来源：http://sqx.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://sxd.hnxiangtu.top

[D08] 合并两个数组
来源：http://qnz.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://lcs.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://uqv.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nvp.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://lip.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tdl.jiagoushi.top

Go:   append(a, b...)
来源：http://xua.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://ghr.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://ajm.hongshengwenyu.top

[D09] 排序（升序）
来源：http://nlg.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://ufs.ppjwa.cn

PHP:  sort($arr);
来源：http://frb.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://num.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iuv.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uod.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mvl.fktsv.cn

Ruby: arr.sort
来源：http://bte.yj20258.top

C#:   list.Sort();
来源：http://qls.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dhy.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sdd.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kxi.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bzr.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tfc.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fvt.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://opq.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rck.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jxm.sxryk.cn

[D11] 反转数组
来源：http://wjs.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://obe.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://zbr.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dcp.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://gto.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://aqr.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://rbl.jyoumei.cn

Ruby: arr.reverse
来源：http://qkk.fzhhl.top

C#:   list.Reverse();
来源：http://kuf.svipenyu.cn

[D12] 查找元素下标
来源：http://udz.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://gjo.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uzi.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twu.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgz.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jot.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://fao.ydjk.org.cn

Ruby: arr.index(x)
来源：http://ans.bbcook.cn

C#:   list.IndexOf(x);
来源：http://zje.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://evb.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xjq.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dwu.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://fxh.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://fjw.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dku.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sgn.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://xsw.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bmk.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://bhz.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://veb.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kuo.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://grn.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://yon.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ait.cashguo.top

Go:   // 手写循环
来源：http://dek.tanke756.top

Ruby: arr.map { |x| x * 2 }
来源：http://okm.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zoy.aibaodan.cn

[D15] 去重
来源：http://xnz.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kwd.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://myy.52xcode.cn

JS:   [...new Set(arr)]
来源：http://ptw.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://zqn.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://imh.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://chm.jiagoushi.top

Ruby: arr.uniq
来源：http://jcw.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://hxq.andypj.xyz

[D16] 求和与平均值
来源：http://ien.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wxk.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xty.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qsd.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://toq.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tni.fehbvm.com

Go:   // 手写循环累加
来源：http://lon.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://urh.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://iuo.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://xzv.hammf.cn

Py:   max(arr);  min(arr)
来源：http://iqe.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://zpt.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uxx.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://tnl.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qfx.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://owx.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://vyd.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://tor.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://lji.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kjw.ivvv.top

PHP:  array_merge(...$nested);
来源：http://jnf.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fpv.yj20258888.top

TS:   nested.flat();
来源：http://npt.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bfo.yangfankeji.com

Go:   // 手写双层循环
来源：http://moy.yonumen.top

Ruby: nested.flatten
来源：http://xrp.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vps.guannengcc.top

[D19] 按字段分组
来源：http://cva.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://duh.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ygl.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ivs.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qfx.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ccg.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://vml.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ptd.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pda.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://stf.ydzc1.top

Py:   Counter(arr)
来源：http://adi.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://caf.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mfa.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zoz.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tnp.redwolf501.top

Go:   // 手写 map[T]int
来源：http://yid.xinyue.icu

Ruby: arr.tally
来源：http://sgu.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hdo.aizwys.cn

[D21] 判断是否包含某元素
来源：http://oad.wangdashe.top

Py:   x in arr
来源：http://zrr.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://oyd.cashguo.top

JS:   arr.includes(x)
来源：http://woh.316326.xyz

TS:   arr.includes(x)
来源：http://fqm.xylfe.cn

Java: list.contains(x)
来源：http://erm.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://zve.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://uzd.xylfe.cn

C#:   list.Contains(x)
来源：http://frc.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://gdh.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://slm.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jnh.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sih.yj20258888.top

TS:   [...arr];
来源：http://gug.birdmap.top

Java: new ArrayList<>(list);
来源：http://lhb.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://wte.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://wsz.jqgufenzy.top

C#:   new List<int>(list);
来源：http://okg.0kj1m.cn

[D23] reduce 累积计算
来源：http://phn.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zcv.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rtj.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rbd.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svf.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dwh.hammf.cn

Go:   // 手写循环
来源：http://hzf.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wqu.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://elz.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://vik.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eou.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eut.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gtm.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zis.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://orj.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://myk.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ncy.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hpy.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://fsi.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xpx.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eve.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zhb.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gqm.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lhn.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fuu.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://new.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zas.xziqi.cn

[D26] 数组转字符串
来源：http://msn.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://mga.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://owp.cdnleiting.top

JS:   arr.join(", ")
来源：http://zsi.zycfv.cn

TS:   arr.join(", ")
来源：http://ath.ydzc1.top

Java: String.join(", ", list)
来源：http://zgb.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://dnz.gogol.net.cn

Ruby: arr.join(", ")
来源：http://cdd.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://zll.hcnkem.com


<!-- 参考信息 -->