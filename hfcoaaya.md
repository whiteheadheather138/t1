代发 wailian999

C#:   块级作用域
来源：http://yua.ydjk.org.cn

[C11] 模块导入与导出
来源：http://njy.nwbrower.top

Py:   from module import func
来源：http://jkv.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ahg.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vxo.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://exg.xylfe.cn

Java: import java.util.List;
来源：http://zpo.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ber.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://zbq.gzhubu.top

C#:   using System.Text;
来源：http://uxl.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://ceq.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://tsj.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://bnb.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://xua.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://cij.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ahl.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://utp.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://rdn.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://edw.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://skf.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://huf.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ggl.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://znw.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fua.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kna.hcnkem.com

Go:   func add(a, b int) int
来源：http://dwx.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tei.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://mhe.snrcjt.cn

[C14] 泛型函数
来源：http://qqn.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vwh.haohaochexian.top

PHP:  // 无泛型
来源：http://lpt.chenlongwang.top

JS:   // 无泛型
来源：http://zta.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yts.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uro.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fho.gotoacloud.top

Ruby: # 无泛型
来源：http://thv.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wre.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://cyu.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bal.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://yfb.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yyj.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pmv.chenzaomai.com

Java: // 无解构
来源：http://bdx.gogol.net.cn

Go:   // 无解构
来源：http://zko.dianchejie.cn

Ruby: a, b = pair
来源：http://ymw.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://irm.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://wqt.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mwf.ybcxt.top

PHP:  // 无重载
来源：http://kve.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bhp.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://wjn.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cxz.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://npg.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://mbm.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://axc.shuidangran.top

================================================================================
来源：http://ndy.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://rxq.jiagoushi.top

================================================================================
来源：http://bzk.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://pld.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://flq.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lia.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tut.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://soc.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gbc.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://tfi.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://hqg.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ufy.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://rga.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ieh.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://khc.quarkkingdee.top

JS:   arr.push(4);
来源：http://dmm.bbcook.cn

TS:   arr.push(4);
来源：http://ksr.sxryk.cn

Java: list.add(4);
来源：http://cmg.cashguo.top

Go:   arr = append(arr, 4)
来源：http://dwt.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://dop.snrcjt.cn

C#:   list.Add(4);
来源：http://hgf.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://iyc.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://bmn.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wij.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://olw.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://fxq.smart0.xyz

Java: list.add(0, 0);
来源：http://bza.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://mob.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://grv.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://jzj.sysykeji.top

[D04] 删除元素
来源：http://age.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lcy.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gme.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aig.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://lle.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://htc.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uxw.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fkf.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oaa.iojbl.cn

[D05] 访问与修改元素
来源：http://tiy.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mlj.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jiw.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qid.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://awc.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://cok.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://vma.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mmj.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jzl.hcnkem.com

[D06] 数组长度
来源：http://fwt.yongpay.top

Py:   len(arr)
来源：http://uyj.epnwcf.com

PHP:  count($arr);
来源：http://ouy.cheryme.top

JS:   arr.length
来源：http://mms.wangdashe.top

TS:   arr.length
来源：http://hou.cashguo.top

Java: list.size();
来源：http://nju.zdbjq.cn

Go:   len(arr)
来源：http://nbg.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://suu.nanxinkj.top

C#:   list.Count;
来源：http://iaq.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://yqo.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dbz.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://bbt.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://iic.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://nas.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://atd.xuetiantiany.cn

Go:   arr[1:4]
来源：http://dxr.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://okr.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://lug.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://ifs.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://wet.tarul.cn

PHP:  array_merge($a, $b);
来源：http://itd.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kty.gaohongyu789.top

TS:   [...a, ...b];
来源：http://wpq.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dcn.yuxming.cn

Go:   append(a, b...)
来源：http://jla.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://bbg.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://lsx.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://dgu.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://zdl.yj202588.top

PHP:  sort($arr);
来源：http://urn.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wba.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zvj.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://prd.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hke.sxryk.cn

Ruby: arr.sort
来源：http://dlv.sufxvd.cn

C#:   list.Sort();
来源：http://ker.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kgw.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zbj.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vux.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://woy.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvo.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pgb.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xcn.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xie.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hap.xuanzx.com

[D11] 反转数组
来源：http://fwh.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://non.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://rrz.kuanghao11.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tya.meibo888.top

TS:   [...arr].reverse();
来源：http://wia.fengsongda.top

Java: Collections.reverse(list);
来源：http://gti.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://gur.epnwcf.com

Ruby: arr.reverse
来源：http://mbz.yangfankeji.com

C#:   list.Reverse();
来源：http://lkd.jinqigufen.top

[D12] 查找元素下标
来源：http://kcu.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://wqw.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hzv.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jez.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ozs.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://twj.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://pms.xuanzx.com

Ruby: arr.index(x)
来源：http://vjy.daria6918.cn

C#:   list.IndexOf(x);
来源：http://bbz.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://wos.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://khq.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cfp.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://nrh.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://wyz.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xgq.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://orr.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ubw.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gat.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://wvz.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cmf.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbx.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://oiw.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://kqn.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vja.yanxiufei.cn

Go:   // 手写循环
来源：http://fuc.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vyd.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://bwu.sxryk.cn

[D15] 去重
来源：http://sld.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rgn.tian-w.cn

PHP:  array_unique($arr);
来源：http://nqd.gzhubu.top

JS:   [...new Set(arr)]
来源：http://qxy.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://phg.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://buk.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ned.jqgufenzy.top

Ruby: arr.uniq
来源：http://mee.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://udj.0kj1m.cn

[D16] 求和与平均值
来源：http://wcr.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mld.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bhl.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vgr.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://poe.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qsr.sxryk.cn

Go:   // 手写循环累加
来源：http://bnp.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hgk.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://sxj.c1oappe.top

[D17] 最大值与最小值
来源：http://nhk.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://qro.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://mtq.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gep.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://hsa.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pbm.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://scn.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://bfv.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://kxu.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://rnf.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lop.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://umj.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kdj.guowangkeji.top

TS:   nested.flat();
来源：http://myx.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://weq.316326.xyz

Go:   // 手写双层循环
来源：http://rqj.yonumen.top

Ruby: nested.flatten
来源：http://tnv.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pph.andypj.xyz

[D19] 按字段分组
来源：http://xlh.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ine.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ekn.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wqt.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://amq.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://roh.tanke756.top

Go:   // 手写 map[string][]T
来源：http://whd.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xov.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rdb.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://ndh.jianghu66.top

Py:   Counter(arr)
来源：http://xta.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://jdo.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhu.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ekn.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nnb.gzhubu.top

Go:   // 手写 map[T]int
来源：http://tit.tarul.cn

Ruby: arr.tally
来源：http://lzd.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pqq.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://xgd.sjlbkw.cn

Py:   x in arr
来源：http://mef.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://sdq.cqqwz.cn

JS:   arr.includes(x)
来源：http://maj.vqdsnc.cn

TS:   arr.includes(x)
来源：http://ifi.snrcjt.cn

Java: list.contains(x)
来源：http://vme.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://ozc.ybcxt.top

Ruby: arr.include?(x)
来源：http://ojn.jiagoushi.top

C#:   list.Contains(x)
来源：http://znc.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://xka.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://enx.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lvs.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dnz.smart0.xyz

TS:   [...arr];
来源：http://dhi.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://hpj.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vva.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://nkj.sweek.top

C#:   new List<int>(list);
来源：http://kyw.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://squ.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lme.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ckb.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bdt.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mmz.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bmt.feifeiyinyue.top

Go:   // 手写循环
来源：http://xai.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wkb.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ghc.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://jgg.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://skg.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aqx.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nas.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wqv.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jqt.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vlj.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yku.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cgw.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://rjh.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ckz.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tyt.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zfx.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gmp.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dag.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iez.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vfr.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ivs.zdqjudy.top

[D26] 数组转字符串
来源：http://pwg.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://jmx.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://lco.epnwcf.com

JS:   arr.join(", ")
来源：http://jma.ydjk.org.cn

TS:   arr.join(", ")
来源：http://cby.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://znw.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://mwl.andypj.xyz

Ruby: arr.join(", ")
来源：http://nxr.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://mor.aibaodan.cn

================================================================================
来源：http://apc.yueranfly.top

E. 字符串处理
来源：http://kjl.hfpthk.cn

================================================================================
来源：http://kfb.yonumen.top

[E01] 拼接字符串
来源：http://jhx.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://whl.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zbj.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tvm.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fpn.52xcode.cn


<!-- 参考信息 -->