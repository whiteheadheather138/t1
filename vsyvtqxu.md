代发 wailian999

TS:   同 JS
来源：http://dnh.bbcook.cn

Java: 方法内为块级作用域
来源：http://khl.jianghu66.top

Go:   花括号块级作用域
来源：http://uwg.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zch.chenlongwang.top

C#:   块级作用域
来源：http://gdy.jlsjyb.cn

[C11] 模块导入与导出
来源：http://sqi.yvedp.cn

Py:   from module import func
来源：http://uye.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://che.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fmc.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ouy.zhijiandao.cn

Java: import java.util.List;
来源：http://jnw.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zdn.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://mqh.gzhubu.top

C#:   using System.Text;
来源：http://fev.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://oie.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://muy.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://wkv.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://pus.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://agg.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oxm.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://gky.sweek.top

Ruby: -> { puts "run" }.call
来源：http://aev.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://mts.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://cha.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nkt.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cak.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iev.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ult.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://uez.aibaodan.cn

Go:   func add(a, b int) int
来源：http://gex.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wtf.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wfb.hnxiangtu.top

[C14] 泛型函数
来源：http://gdv.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dho.wangdashe.top

PHP:  // 无泛型
来源：http://gbh.aibaodan.cn

JS:   // 无泛型
来源：http://egg.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hby.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ren.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kaf.guannengcc.top

Ruby: # 无泛型
来源：http://tmn.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ryr.cashguo.top

[C15] 解构 / 展开参数
来源：http://jwa.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bdb.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://jyf.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uwy.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bmk.feifeiyinyue.top

Java: // 无解构
来源：http://rio.nanxinkj.top

Go:   // 无解构
来源：http://zdx.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://nhl.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://hsc.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://omn.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jqo.pengpengdd.cyou

PHP:  // 无重载
来源：http://aks.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jcs.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://mhe.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xtt.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://trb.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://ykh.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gep.yj20258.top

================================================================================
来源：http://jks.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://uoq.hongshengwenyu.top

================================================================================
来源：http://pnx.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://eal.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xva.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wtf.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gwn.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ojk.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nsp.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://phy.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://qpt.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ncp.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://bfa.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fng.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vwu.yonumen.top

JS:   arr.push(4);
来源：http://ryj.cucudq.cn

TS:   arr.push(4);
来源：http://iym.ctjpmb.com

Java: list.add(4);
来源：http://xya.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://lkc.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://bcu.sweek.top

C#:   list.Add(4);
来源：http://dhc.xinyue.icu

[D03] 在指定位置插入元素
来源：http://rbj.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://pae.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tmr.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zcc.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://hhj.nanxinkj.top

Java: list.add(0, 0);
来源：http://qih.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://sjc.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wrh.cashguo.top

C#:   list.Insert(0, 0);
来源：http://qnb.yj20258.top

[D04] 删除元素
来源：http://rcd.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://agu.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lwx.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cdu.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://dmn.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qae.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hgj.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bsl.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dwh.chenzaomai.com

[D05] 访问与修改元素
来源：http://aji.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rfa.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tlm.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://noc.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://tam.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://ajy.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://wgh.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sue.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uil.ppjwa.cn

[D06] 数组长度
来源：http://ueh.xuetiantiany.cn

Py:   len(arr)
来源：http://sjg.mhx1999.top

PHP:  count($arr);
来源：http://zzo.ydzc1.top

JS:   arr.length
来源：http://vlr.cashguo.top

TS:   arr.length
来源：http://aob.andypj.xyz

Java: list.size();
来源：http://mlx.chenjidiqi.icu

Go:   len(arr)
来源：http://utv.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://azm.vehdjk.com

C#:   list.Count;
来源：http://ava.sysykeji.top

[D07] 切片 / 取子数组
来源：http://dvu.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://khx.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ozy.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://zrf.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://osv.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://tbw.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://vol.sufxvd.cn

Ruby: arr[1, 3]
来源：http://xwh.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://xka.chenzaomai.com

[D08] 合并两个数组
来源：http://kto.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://win.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://hmp.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://xmt.hnxiangtu.top

TS:   [...a, ...b];
来源：http://vtb.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wkg.fzhhl.top

Go:   append(a, b...)
来源：http://fka.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://wri.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://rsh.xylfe.cn

[D09] 排序（升序）
来源：http://zsw.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://sut.shuidangran.top

PHP:  sort($arr);
来源：http://fek.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://own.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://kaf.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://htn.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qwd.tarul.cn

Ruby: arr.sort
来源：http://yxr.dashuyun.cn

C#:   list.Sort();
来源：http://qsf.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zru.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nhk.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxy.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zfi.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uwz.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ekb.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gaw.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://knj.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nrp.yangfankeji.com

[D11] 反转数组
来源：http://wzm.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pdz.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://jpi.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hyf.redwolf501.top

TS:   [...arr].reverse();
来源：http://ekd.hesvh.cn

Java: Collections.reverse(list);
来源：http://knn.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://kjn.havefunace.top

Ruby: arr.reverse
来源：http://sug.jianghu66.top

C#:   list.Reverse();
来源：http://npy.sysykeji.top

[D12] 查找元素下标
来源：http://hmj.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://yas.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yzo.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://avx.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tfs.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ope.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://hxx.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://qpf.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://vch.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://jdy.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dog.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qtk.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://jou.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://ziv.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://muz.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jkg.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://yns.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mqm.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://vrm.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lxh.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uzz.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://qxs.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://imv.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://szy.sufxvd.cn

Go:   // 手写循环
来源：http://vhe.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://swr.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://bio.ppjwa.cn

[D15] 去重
来源：http://nuu.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xsg.0kj1m.cn

PHP:  array_unique($arr);
来源：http://zif.meibo888.top

JS:   [...new Set(arr)]
来源：http://lqc.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://bgn.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pid.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://tor.cucudq.cn

Ruby: arr.uniq
来源：http://olu.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://kid.yvedp.cn

[D16] 求和与平均值
来源：http://osc.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cje.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bmd.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oyw.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cvp.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xmy.yj202588.top

Go:   // 手写循环累加
来源：http://kgx.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ynt.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://igd.tianlin.xyz

[D17] 最大值与最小值
来源：http://gri.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://fay.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://hzc.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uvs.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://cry.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ycl.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://btj.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://ocu.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://huy.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://csf.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zbq.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://thw.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://avi.xuetiantiany.cn

TS:   nested.flat();
来源：http://oqf.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tvq.hcnkem.com

Go:   // 手写双层循环
来源：http://pvg.dianchejie.cn

Ruby: nested.flatten
来源：http://ich.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://arf.snrcjt.cn

[D19] 按字段分组
来源：http://xhy.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://msu.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fdv.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xjn.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ssb.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xbk.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://bnb.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sbu.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nqz.yongpay.top

[D20] 统计每个元素出现次数
来源：http://xur.aibaodan.cn

Py:   Counter(arr)
来源：http://fyd.yj20258888.top

PHP:  array_count_values($arr);
来源：http://tud.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwz.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gnm.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dtg.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://ywt.chenjidiqi.icu

Ruby: arr.tally
来源：http://qhf.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aqr.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://ymq.yueranfly.top

Py:   x in arr
来源：http://ivb.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://fcx.sufxvd.cn

JS:   arr.includes(x)
来源：http://xvv.shuidangran.top

TS:   arr.includes(x)
来源：http://qsc.ybcxt.top

Java: list.contains(x)
来源：http://qdu.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://eoz.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://tbl.fengsongda.top

C#:   list.Contains(x)
来源：http://skb.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://npf.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zzz.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rsw.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kuo.hnxiangtu.top

TS:   [...arr];
来源：http://dhi.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://cmk.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rll.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://svi.yfazqb.com

C#:   new List<int>(list);
来源：http://gsc.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://shm.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yjd.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fad.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuf.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://frx.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sux.hnxiangtu.top

Go:   // 手写循环
来源：http://ois.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vmh.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jyy.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://phv.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eol.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsu.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://abm.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xej.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xqk.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://neb.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eiw.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nxi.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://lpx.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vqz.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ldf.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qec.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://apm.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dwn.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qgj.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://apk.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rtb.cashguo.top

[D26] 数组转字符串
来源：http://cme.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://tgd.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://jwa.yonumen.top

JS:   arr.join(", ")
来源：http://tvz.fzhhl.top

TS:   arr.join(", ")
来源：http://ohh.chenzaomai.com

Java: String.join(", ", list)
来源：http://opa.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://wln.aizwys.cn

Ruby: arr.join(", ")
来源：http://ens.316326.xyz

C#:   string.Join(", ", list)
来源：http://dgq.zhaomingkeji.xyz

================================================================================
来源：http://kkv.chenjidiqi.icu

E. 字符串处理
来源：http://xao.ctjpmb.com

================================================================================
来源：http://ybp.yuanzhike.top

[E01] 拼接字符串
来源：http://ycr.zhixingplan.top


<!-- 参考信息 -->