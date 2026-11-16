代发 wailian999

C#:   块级作用域
来源：http://wqz.bbcook.cn

[C11] 模块导入与导出
来源：http://msd.pycfn.com

Py:   from module import func
来源：http://edm.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fxt.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mjs.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hrg.hammf.cn

Java: import java.util.List;
来源：http://nrl.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hhz.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://lst.ehwqpu.com

C#:   using System.Text;
来源：http://wpc.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://nas.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://ecp.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://ljr.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://dqx.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://lod.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uci.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://zgn.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://bbr.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yny.sweek.top

[C13] 类型声明 / 类型注解
来源：http://jao.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ivf.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kft.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nig.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ggx.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://enh.ppjwa.cn

Go:   func add(a, b int) int
来源：http://xum.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://duf.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://ayr.yvedp.cn

[C14] 泛型函数
来源：http://zou.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dam.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://pci.ivvv.top

JS:   // 无泛型
来源：http://ajp.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gli.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pqx.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kkp.chenlongwang.top

Ruby: # 无泛型
来源：http://oyk.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xda.yj20258888.top

[C15] 解构 / 展开参数
来源：http://hip.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kmg.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://vkp.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hiv.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nys.sxryk.cn

Java: // 无解构
来源：http://tdz.sjlbkw.cn

Go:   // 无解构
来源：http://fmk.yuxming.cn

Ruby: a, b = pair
来源：http://vnv.cashguo.top

C#:   var (a, b) = pair;
来源：http://rrh.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://bwp.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kdq.hywenlv.cn

PHP:  // 无重载
来源：http://ial.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mpu.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://yat.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wbo.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://ypu.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://peb.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kri.0kj1m.cn

================================================================================
来源：http://hly.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://lyh.316326.xyz

================================================================================
来源：http://exe.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://thx.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tlw.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mqm.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://snc.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hzw.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gbh.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://gpx.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://dgj.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hkw.fktsv.cn

[D02] 追加元素到末尾
来源：http://rgf.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pbd.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ibe.dashuyun.cn

JS:   arr.push(4);
来源：http://mvx.yj20258.top

TS:   arr.push(4);
来源：http://llr.gaohongyu789.top

Java: list.add(4);
来源：http://ajs.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://uty.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://zxh.jinqigufen.top

C#:   list.Add(4);
来源：http://moj.fengsongda.top

[D03] 在指定位置插入元素
来源：http://szb.yj20258.top

Py:   arr.insert(0, 0)
来源：http://cog.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wcr.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mqw.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://gmj.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://iwn.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://evy.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mfm.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://pxh.haohaochexian.top

[D04] 删除元素
来源：http://tfj.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ozn.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lqe.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gdx.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://ffd.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jsm.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kvx.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nsy.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bte.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://qvn.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hsk.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vuh.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wbk.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://ske.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://jxg.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://duh.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ogu.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jiz.snrcjt.cn

[D06] 数组长度
来源：http://bvc.yongpay.top

Py:   len(arr)
来源：http://ssz.sysykeji.top

PHP:  count($arr);
来源：http://yef.iojbl.cn

JS:   arr.length
来源：http://aci.tianlin.xyz

TS:   arr.length
来源：http://fkq.cqqwz.cn

Java: list.size();
来源：http://ixa.zhixingplan.top

Go:   len(arr)
来源：http://gly.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://kzy.aibaodan.cn

C#:   list.Count;
来源：http://iwv.meibo888.top

[D07] 切片 / 取子数组
来源：http://icm.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fac.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://hks.havefunace.top

JS:   arr.slice(1, 4);
来源：http://phr.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://hkg.yongpay.top

Java: list.subList(1, 4);
来源：http://mjp.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://dap.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://xrr.sweek.top

C#:   list.GetRange(1, 3);
来源：http://ilx.meibo888.top

[D08] 合并两个数组
来源：http://uae.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://yiu.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://cko.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rpk.daria6918.cn

TS:   [...a, ...b];
来源：http://haf.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jex.yuanzhike.top

Go:   append(a, b...)
来源：http://rku.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://fow.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://qre.nanxuanxn.top

[D09] 排序（升序）
来源：http://xbu.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://uqs.bjfxy.top

PHP:  sort($arr);
来源：http://wsg.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lpx.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://dqm.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lvs.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ywe.chenzaomai.com

Ruby: arr.sort
来源：http://fnq.vqdsnc.cn

C#:   list.Sort();
来源：http://yol.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://tvs.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yae.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uvp.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mmy.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsw.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gim.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pzo.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ood.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tap.0kj1m.cn

[D11] 反转数组
来源：http://lhb.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fca.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://zjy.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tdz.sysykeji.top

TS:   [...arr].reverse();
来源：http://eke.cdnleiting.top

Java: Collections.reverse(list);
来源：http://sjh.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://uub.yanxiufei.cn

Ruby: arr.reverse
来源：http://ykd.haohaochexian.top

C#:   list.Reverse();
来源：http://fcs.hongshengwenyu.top

[D12] 查找元素下标
来源：http://ejn.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://tcd.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://stj.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eko.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjg.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mqb.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://qjt.hnxiangtu.top

Ruby: arr.index(x)
来源：http://kkj.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://qkp.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://loh.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ipp.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lnz.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://slg.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://hdz.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xrz.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cfe.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://qis.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://mue.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://wxv.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xup.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jaa.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://wbf.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://dxw.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pcn.hcnkem.com

Go:   // 手写循环
来源：http://esl.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gag.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ydl.fanxiaobao.xyz

[D15] 去重
来源：http://fiu.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iod.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://rxw.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://ons.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://eaw.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ych.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mwo.hammf.cn

Ruby: arr.uniq
来源：http://fis.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://gqg.meibo888.top

[D16] 求和与平均值
来源：http://lii.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dbu.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mkv.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ilf.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fub.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://twk.ydzc1.top

Go:   // 手写循环累加
来源：http://nqo.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jdz.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://ugc.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://fsv.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://ije.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://vcj.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hxi.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://tji.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://jtb.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tkf.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://kti.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://wvo.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://wpl.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aqb.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://yxd.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lnd.hfpthk.cn

TS:   nested.flat();
来源：http://xrb.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nkq.jiagoushi.top

Go:   // 手写双层循环
来源：http://vif.smart0.xyz

Ruby: nested.flatten
来源：http://muq.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cfm.xuanzx.com

[D19] 按字段分组
来源：http://lvw.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zur.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zhd.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mdw.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jsz.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fzg.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://hee.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dly.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cfb.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://ejk.feifeiyinyue.top

Py:   Counter(arr)
来源：http://zue.guannengcc.top

PHP:  array_count_values($arr);
来源：http://fwu.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://frf.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uyg.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yvk.cucudq.cn

Go:   // 手写 map[T]int
来源：http://fuu.52xcode.cn

Ruby: arr.tally
来源：http://zcc.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://foa.bjfxy.top

[D21] 判断是否包含某元素
来源：http://dbq.hcnkem.com

Py:   x in arr
来源：http://iur.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://rds.vqdsnc.cn

JS:   arr.includes(x)
来源：http://kho.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://lms.gaohongyu789.top

Java: list.contains(x)
来源：http://qlh.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://ljt.zycfv.cn

Ruby: arr.include?(x)
来源：http://cki.hnxiangtu.top

C#:   list.Contains(x)
来源：http://har.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://wgb.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xdg.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://umm.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pap.gotoacloud.top

TS:   [...arr];
来源：http://lyx.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://npj.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://bqa.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://ffw.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://cyv.cheryme.top

[D23] reduce 累积计算
来源：http://njf.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wvf.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zvj.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://emc.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyg.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wco.cdnleiting.top

Go:   // 手写循环
来源：http://dkj.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uuq.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oel.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://roq.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pgo.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yjs.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ukn.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://efb.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hpe.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uzz.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://moe.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://riu.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://vta.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gqn.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fbm.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yrp.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hlk.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tan.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iri.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rxo.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wqx.hnqzz.top

[D26] 数组转字符串
来源：http://das.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://kht.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://uae.hcnkem.com

JS:   arr.join(", ")
来源：http://ecb.cqqwz.cn

TS:   arr.join(", ")
来源：http://vdt.daxiang520.top

Java: String.join(", ", list)
来源：http://piq.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://akw.birdmap.top

Ruby: arr.join(", ")
来源：http://ymh.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://cts.yanxiufei.cn

================================================================================
来源：http://whu.jinyuanbaomall.cn

E. 字符串处理
来源：http://xno.ivvv.top

================================================================================
来源：http://gkl.9152youxi.cn

[E01] 拼接字符串
来源：http://scl.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vjv.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hpf.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eog.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sui.c1oappe.top


<!-- 参考信息 -->