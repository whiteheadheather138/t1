代发 wailian999

[C10] 变量作用域
来源：http://dgm.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ljk.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dlt.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gxg.xinyue.icu

TS:   同 JS
来源：http://uqa.hcnkem.com

Java: 方法内为块级作用域
来源：http://slo.epnwcf.com

Go:   花括号块级作用域
来源：http://ncw.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eow.xuanzx.com

C#:   块级作用域
来源：http://hgh.sufxvd.cn

[C11] 模块导入与导出
来源：http://llr.cashguo.top

Py:   from module import func
来源：http://kyz.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dch.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gcj.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://red.gotoacloud.top

Java: import java.util.List;
来源：http://dgq.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zlm.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://yqh.tian-w.cn

C#:   using System.Text;
来源：http://dwr.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://qkm.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://mjz.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://mlk.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://jhq.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://pyz.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eva.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://ygw.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://uql.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kxn.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://gbf.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pzu.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aik.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lwo.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xkj.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://rfu.uphjek.com

Go:   func add(a, b int) int
来源：http://bff.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hya.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://tgx.ehwqpu.com

[C14] 泛型函数
来源：http://vsx.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dca.cqqwz.cn

PHP:  // 无泛型
来源：http://sgc.wangdashe.top

JS:   // 无泛型
来源：http://iqd.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ily.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jow.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xqu.ppjwa.cn

Ruby: # 无泛型
来源：http://xrh.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tak.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://rgd.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fkk.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://kor.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yjd.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wjh.shanyushiyangtech.top

Java: // 无解构
来源：http://ijr.shangyingyoupin.top

Go:   // 无解构
来源：http://zeb.gaohongyu789.top

Ruby: a, b = pair
来源：http://dgq.redwolf501.top

C#:   var (a, b) = pair;
来源：http://kbq.uphjek.com

[C16] 函数 / 方法重载
来源：http://get.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zks.52xcode.cn

PHP:  // 无重载
来源：http://wik.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fto.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://fbs.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://omi.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://hix.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://tfn.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dfa.havefunace.top

================================================================================
来源：http://htp.yongpay.top

D. 数组 / 列表 / 集合
来源：http://cgx.wangshuangyany.cn

================================================================================
来源：http://fej.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://agn.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wxm.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nkk.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mij.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vja.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rtg.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ozo.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://ghv.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kjw.nanxinkj.top

[D02] 追加元素到末尾
来源：http://npz.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ojb.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jqb.xuetiantiany.cn

JS:   arr.push(4);
来源：http://zme.sjlbkw.cn

TS:   arr.push(4);
来源：http://rlg.hysaishi.cn

Java: list.add(4);
来源：http://htt.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://vco.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://nqk.hywenlv.cn

C#:   list.Add(4);
来源：http://pvl.guannengcc.top

[D03] 在指定位置插入元素
来源：http://akx.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://par.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://umm.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wmx.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://oso.cucudq.cn

Java: list.add(0, 0);
来源：http://eoj.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://mij.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yeh.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://vqr.sxryk.cn

[D04] 删除元素
来源：http://pai.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tve.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sap.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kpq.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://ecw.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tmv.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lld.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ayt.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bvd.daxiang520.top

[D05] 访问与修改元素
来源：http://tik.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pif.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bop.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fla.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://edl.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://alv.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://mlo.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mkn.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kcr.fanxiaobao.xyz

[D06] 数组长度
来源：http://mpn.sweek.top

Py:   len(arr)
来源：http://ljr.xziqi.cn

PHP:  count($arr);
来源：http://hyx.fengsongda.top

JS:   arr.length
来源：http://lkq.ctjpmb.com

TS:   arr.length
来源：http://kdy.wangshuangyany.cn

Java: list.size();
来源：http://mzw.yj20258888.top

Go:   len(arr)
来源：http://eae.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://yxj.jqgufenzy.top

C#:   list.Count;
来源：http://ujw.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://mdl.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xbl.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kdh.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://oub.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://hnk.ehwqpu.com

Java: list.subList(1, 4);
来源：http://snb.daxiang520.top

Go:   arr[1:4]
来源：http://dmv.c1oappe.top

Ruby: arr[1, 3]
来源：http://xzr.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://viq.ybcxt.top

[D08] 合并两个数组
来源：http://ekc.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://hhq.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://twu.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vvv.smart0.xyz

TS:   [...a, ...b];
来源：http://xci.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iuv.aizwys.cn

Go:   append(a, b...)
来源：http://wkn.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://vzg.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://kch.ybcxt.top

[D09] 排序（升序）
来源：http://wzz.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://whh.kuanghao11.cn

PHP:  sort($arr);
来源：http://oqu.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wqt.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rge.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jve.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ftn.0kj1m.cn

Ruby: arr.sort
来源：http://zoi.shangyingyoupin.top

C#:   list.Sort();
来源：http://zbw.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nao.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lzb.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nny.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://keg.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ftw.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hwf.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tzs.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vkx.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yau.zycfv.cn

[D11] 反转数组
来源：http://rms.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://tcp.hcnkem.com

PHP:  array_reverse($arr);
来源：http://yso.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wtn.hammf.cn

TS:   [...arr].reverse();
来源：http://liv.dianchejie.cn

Java: Collections.reverse(list);
来源：http://ise.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://rko.yj20258.top

Ruby: arr.reverse
来源：http://muu.birdmap.top

C#:   list.Reverse();
来源：http://wrl.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://llv.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://mxl.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fqs.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hoz.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://crp.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dga.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://qhy.tianlin.xyz

Ruby: arr.index(x)
来源：http://xfp.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://snu.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://yuf.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pps.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zud.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://pqb.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://tlt.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://srl.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gha.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://agj.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://hhj.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://tor.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wgz.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ajx.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://nwe.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://eel.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ftn.zhoulong.xyz

Go:   // 手写循环
来源：http://ipb.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://fzv.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ekz.xylfe.cn

[D15] 去重
来源：http://frk.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://agb.jyoumei.cn

PHP:  array_unique($arr);
来源：http://ppe.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://dny.bjfxy.top

TS:   [...new Set(arr)]
来源：http://zqy.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iot.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://ubx.mhx1999.top

Ruby: arr.uniq
来源：http://njc.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://yxm.havefunace.top

[D16] 求和与平均值
来源：http://jmc.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dyy.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://thr.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ftw.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuw.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jqm.fktsv.cn

Go:   // 手写循环累加
来源：http://get.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ter.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://uue.wangdashe.top

[D17] 最大值与最小值
来源：http://opg.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://mty.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://mth.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fvz.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://wik.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wqv.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wuw.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://hkk.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://bqy.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://afd.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fto.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://eam.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jmz.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://eks.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hmv.52xcode.cn

Go:   // 手写双层循环
来源：http://rzf.fktsv.cn

Ruby: nested.flatten
来源：http://jzw.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zhp.bjfxy.top

[D19] 按字段分组
来源：http://qee.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mdj.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ahv.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bkc.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ftl.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rjo.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://ahe.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nxw.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mrt.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://ngf.bbcook.cn

Py:   Counter(arr)
来源：http://mdx.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://gzp.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gqu.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hfd.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://inu.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://qmb.jinqigufen.top

Ruby: arr.tally
来源：http://boa.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://odk.andypj.xyz

[D21] 判断是否包含某元素
来源：http://dlw.52xcode.cn

Py:   x in arr
来源：http://axa.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://evs.tian-w.cn

JS:   arr.includes(x)
来源：http://fce.xziqi.cn

TS:   arr.includes(x)
来源：http://yda.aizwys.cn

Java: list.contains(x)
来源：http://eno.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://jbi.sxryk.cn

Ruby: arr.include?(x)
来源：http://axl.hcnkem.com

C#:   list.Contains(x)
来源：http://fsl.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://mlt.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uuz.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oge.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rcv.yueranfly.top

TS:   [...arr];
来源：http://ypf.gzhubu.top

Java: new ArrayList<>(list);
来源：http://jpb.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://yun.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://ymy.gotoacloud.top

C#:   new List<int>(list);
来源：http://cvi.yonumen.top

[D23] reduce 累积计算
来源：http://nmv.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mju.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://owm.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vrv.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hgi.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kzx.ydjk.org.cn

Go:   // 手写循环
来源：http://rri.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kxv.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bji.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://jsc.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dig.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yce.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cpf.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qxw.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ydu.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bqb.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dvu.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mjm.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://vpm.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ypc.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://grh.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qcq.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://loh.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://enp.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ezp.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ltb.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kni.zhixingplan.top

[D26] 数组转字符串
来源：http://ots.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://cls.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://loh.hfpthk.cn

JS:   arr.join(", ")
来源：http://vyr.jqgufenzy.top

TS:   arr.join(", ")
来源：http://xjq.9152youxi.cn

Java: String.join(", ", list)
来源：http://sqv.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://iil.havefunace.top

Ruby: arr.join(", ")
来源：http://nob.yonumen.top

C#:   string.Join(", ", list)
来源：http://lse.fanxiaobao.xyz


<!-- 参考信息 -->