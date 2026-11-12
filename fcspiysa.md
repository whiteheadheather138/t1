代发 wailian999

TS:   同 JS
来源：http://oso.xuanzx.com

Java: 方法内为块级作用域
来源：http://wgo.dianchejie.cn

Go:   花括号块级作用域
来源：http://ewd.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ehi.52xcode.cn

C#:   块级作用域
来源：http://sto.yangfankeji.com

[C11] 模块导入与导出
来源：http://pkn.vehdjk.com

Py:   from module import func
来源：http://wjs.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://lyh.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://yjr.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rrf.cucudq.cn

Java: import java.util.List;
来源：http://wtc.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hwp.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://ryx.ehwqpu.com

C#:   using System.Text;
来源：http://fpj.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://cyq.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://qdq.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://pjg.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://mmd.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://qcf.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ibz.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://sgf.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://lbj.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kys.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://nut.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ojx.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxs.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fyd.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfg.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://qxu.yvedp.cn

Go:   func add(a, b int) int
来源：http://nns.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wgj.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fgu.xuetiantiany.cn

[C14] 泛型函数
来源：http://mjy.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zeu.nwbrower.top

PHP:  // 无泛型
来源：http://ily.haohaochexian.top

JS:   // 无泛型
来源：http://rbb.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://esk.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lxa.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xhf.vehdjk.com

Ruby: # 无泛型
来源：http://xia.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kdu.hammf.cn

[C15] 解构 / 展开参数
来源：http://xir.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ltt.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://qnp.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zqm.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ptq.quarkkingdee.top

Java: // 无解构
来源：http://olw.dashuyun.cn

Go:   // 无解构
来源：http://nqz.jyoumei.cn

Ruby: a, b = pair
来源：http://moz.yueranfly.top

C#:   var (a, b) = pair;
来源：http://yzj.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://vpn.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jdl.yonumen.top

PHP:  // 无重载
来源：http://dtp.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xin.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://sei.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vur.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://mvx.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://ttv.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iwh.jqgfzy.top

================================================================================
来源：http://myl.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://zvl.guannengcc.top

================================================================================
来源：http://zhs.smart0.xyz

[D01] 创建数组 / 列表
来源：http://gga.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://res.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yrn.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qbf.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zry.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://odw.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://ksx.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://tji.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bga.sufxvd.cn

[D02] 追加元素到末尾
来源：http://rhd.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jeq.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lsu.xinyue.icu

JS:   arr.push(4);
来源：http://dwr.havefunace.top

TS:   arr.push(4);
来源：http://xhs.fanxiaobao.xyz

Java: list.add(4);
来源：http://eis.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://psk.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://hdx.yanxiufei.cn

C#:   list.Add(4);
来源：http://dup.aizwys.cn

[D03] 在指定位置插入元素
来源：http://iwo.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://dto.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zfp.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ajq.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://mdv.zhengqikj.top

Java: list.add(0, 0);
来源：http://rvp.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://czb.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qkl.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://jir.jlsjyb.cn

[D04] 删除元素
来源：http://cef.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aha.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nyc.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pjy.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://svh.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rmr.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://alz.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://chq.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://srf.cdnleiting.top

[D05] 访问与修改元素
来源：http://ria.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://svx.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://itf.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fvg.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://ztp.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://bnf.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://ulj.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ebh.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fhj.ydzc1.top

[D06] 数组长度
来源：http://djn.yj202588.top

Py:   len(arr)
来源：http://nld.bjfxy.top

PHP:  count($arr);
来源：http://daf.fanxiaobao.xyz

JS:   arr.length
来源：http://ssc.hnxiangtu.top

TS:   arr.length
来源：http://uxl.uphjek.com

Java: list.size();
来源：http://rry.snrcjt.cn

Go:   len(arr)
来源：http://ifi.meibo888.top

Ruby: arr.length; arr.size
来源：http://gmn.cdnleiting.top

C#:   list.Count;
来源：http://dxs.pycfn.com

[D07] 切片 / 取子数组
来源：http://aom.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://izo.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://ver.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://tas.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://vuj.xinyue.icu

Java: list.subList(1, 4);
来源：http://tcv.uphjek.com

Go:   arr[1:4]
来源：http://eyd.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://mwg.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://zgd.cucudq.cn

[D08] 合并两个数组
来源：http://ubr.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://ocu.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://pyz.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wou.gzhubu.top

TS:   [...a, ...b];
来源：http://zgw.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://olt.zhoulong.xyz

Go:   append(a, b...)
来源：http://rln.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://rxq.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://fap.gaohongyu789.top

[D09] 排序（升序）
来源：http://unt.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://sgw.yongpay.top

PHP:  sort($arr);
来源：http://eyk.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mjv.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iuw.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://slf.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gwa.cheryme.top

Ruby: arr.sort
来源：http://urn.cdnleiting.top

C#:   list.Sort();
来源：http://hla.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gjz.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://obt.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkg.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bsy.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jod.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://axv.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qpn.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xdy.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tkw.hesvh.cn

[D11] 反转数组
来源：http://nks.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sxm.chenlongwang.top

PHP:  array_reverse($arr);
来源：http://yvz.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oqu.ppjwa.cn

TS:   [...arr].reverse();
来源：http://kod.c1oappe.top

Java: Collections.reverse(list);
来源：http://sxb.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://vat.epnwcf.com

Ruby: arr.reverse
来源：http://xrj.smart0.xyz

C#:   list.Reverse();
来源：http://iub.chenjidiqi.icu

[D12] 查找元素下标
来源：http://kja.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://kvw.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jxk.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tqh.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yxv.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://due.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://bds.aibaodan.cn

Ruby: arr.index(x)
来源：http://yuq.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://hqw.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://yge.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rtx.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ihg.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://yyr.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://nkv.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://who.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yys.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qtq.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://whg.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://lhf.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ohn.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lsl.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://wff.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://rra.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ciq.xinyue.icu

Go:   // 手写循环
来源：http://czt.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://tes.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://idq.9152youxi.cn

[D15] 去重
来源：http://ptq.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://clq.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://qyp.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://kki.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://jks.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uai.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://cun.pycfn.com

Ruby: arr.uniq
来源：http://skn.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://vqa.yj202588.top

[D16] 求和与平均值
来源：http://vjt.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cww.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ybc.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lnc.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ipl.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oxc.xinyue.icu

Go:   // 手写循环累加
来源：http://hby.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://noa.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://dkb.vehdjk.com

[D17] 最大值与最小值
来源：http://flt.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://rer.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://kta.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nlr.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://zxn.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jde.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dwr.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://fkp.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://vqu.uphjek.com

[D18] 扁平化嵌套数组
来源：http://tsd.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nkw.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://jdh.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lhe.daxiang520.top

TS:   nested.flat();
来源：http://ocg.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ebm.yfazqb.com

Go:   // 手写双层循环
来源：http://xwz.jianghu66.top

Ruby: nested.flatten
来源：http://off.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nic.hammf.cn

[D19] 按字段分组
来源：http://ups.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ger.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cpi.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tsu.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ouk.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lmq.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://vqx.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gco.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xwp.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://mtr.ehwqpu.com

Py:   Counter(arr)
来源：http://vns.pycfn.com

PHP:  array_count_values($arr);
来源：http://zxq.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjj.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://six.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wec.hnqzz.top

Go:   // 手写 map[T]int
来源：http://jtk.kuanghao11.cn

Ruby: arr.tally
来源：http://jwj.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fqw.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://inh.shzxlz.cn

Py:   x in arr
来源：http://rku.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://gni.yonumen.top

JS:   arr.includes(x)
来源：http://nzl.ydjk.org.cn

TS:   arr.includes(x)
来源：http://fyn.daxiang520.top

Java: list.contains(x)
来源：http://ups.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://eof.ppjwa.cn

Ruby: arr.include?(x)
来源：http://taz.quarkkingdee.top

C#:   list.Contains(x)
来源：http://fuh.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://afw.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wya.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://txi.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfy.hnxiangtu.top

TS:   [...arr];
来源：http://gfd.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://fwb.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://fir.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://wjf.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://hng.hnqzz.top

[D23] reduce 累积计算
来源：http://kpr.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dfp.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nxu.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vrw.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ser.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cdr.zhijiandao.cn

Go:   // 手写循环
来源：http://xwv.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qgg.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://orf.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://lze.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sdz.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hfv.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mgt.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ter.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ptt.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mzj.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gmr.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mjd.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://brw.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ihd.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pci.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cgx.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bxj.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vbt.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hcb.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tri.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qdj.gogol.net.cn

[D26] 数组转字符串
来源：http://hgv.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://ggc.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://rzn.uphjek.com

JS:   arr.join(", ")
来源：http://qlh.0kj1m.cn

TS:   arr.join(", ")
来源：http://xxe.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://adp.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://cto.zhengqikj.top

Ruby: arr.join(", ")
来源：http://gdq.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://zks.jinyuanbaomall.cn

================================================================================
来源：http://tuw.hesvh.cn

E. 字符串处理
来源：http://kaw.quarkkingdee.top

================================================================================
来源：http://pds.sxryk.cn

[E01] 拼接字符串
来源：http://vvs.shuidangran.top


<!-- 参考信息 -->