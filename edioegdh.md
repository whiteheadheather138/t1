代发 wailian999

[C10] 变量作用域
来源：http://pbi.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yiu.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mta.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://akf.tian-w.cn

TS:   同 JS
来源：http://qkh.redwolf501.top

Java: 方法内为块级作用域
来源：http://xum.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://ewa.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ixf.shuidangran.top

C#:   块级作用域
来源：http://kys.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://vhi.xziqi.cn

Py:   from module import func
来源：http://gyw.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yxa.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://kfl.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ija.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://pqe.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kdz.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://mlo.shanyushiyangtech.top

C#:   using System.Text;
来源：http://vlj.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://lmh.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://wxl.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://odc.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://enw.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://udk.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ajf.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://nmp.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://til.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zdb.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://cgb.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sgv.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://owp.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qfi.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iqq.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://ioo.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://bdv.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ecm.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lgi.ppjwa.cn

[C14] 泛型函数
来源：http://ltx.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jhl.haohaochexian.top

PHP:  // 无泛型
来源：http://jaq.epnwcf.com

JS:   // 无泛型
来源：http://efm.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kpv.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eqp.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://evy.316326.xyz

Ruby: # 无泛型
来源：http://cas.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lmc.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://yas.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nln.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://qym.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yml.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://koc.andypj.xyz

Java: // 无解构
来源：http://grj.uphjek.com

Go:   // 无解构
来源：http://zsg.ydzc1.top

Ruby: a, b = pair
来源：http://olw.gzhubu.top

C#:   var (a, b) = pair;
来源：http://bkf.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://qti.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mko.hesvh.cn

PHP:  // 无重载
来源：http://hya.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://mcj.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://rtw.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://apx.sweek.top

Go:   // 无重载：用不同函数名
来源：http://hhq.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://kcv.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://goo.xylfe.cn

================================================================================
来源：http://gvh.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://zzs.yongpay.top

================================================================================
来源：http://bbf.wangdashe.top

[D01] 创建数组 / 列表
来源：http://chc.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kxe.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gwt.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blz.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://feg.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oct.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://mzo.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://ejr.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yug.cqqwz.cn

[D02] 追加元素到末尾
来源：http://cxj.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kdx.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://njo.fzhhl.top

JS:   arr.push(4);
来源：http://drq.zdbjq.cn

TS:   arr.push(4);
来源：http://mmn.gogol.net.cn

Java: list.add(4);
来源：http://mgj.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://egx.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://iln.zdqjudy.top

C#:   list.Add(4);
来源：http://ajz.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://exa.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://akg.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dwm.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fsm.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://nbk.bbcook.cn

Java: list.add(0, 0);
来源：http://nfa.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oxk.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://das.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://hsi.jinyuanbaomall.cn

[D04] 删除元素
来源：http://eay.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qcr.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mhs.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pcg.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://nbz.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vkv.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cbi.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aan.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdk.guannengcc.top

[D05] 访问与修改元素
来源：http://hnm.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tlh.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rxf.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bit.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://xvs.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://ier.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://vxv.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ifs.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lmo.hcnkem.com

[D06] 数组长度
来源：http://jsh.fanxiaobao.xyz

Py:   len(arr)
来源：http://rke.yfazqb.com

PHP:  count($arr);
来源：http://thx.sysykeji.top

JS:   arr.length
来源：http://xal.ivvv.top

TS:   arr.length
来源：http://oyp.hnqzz.top

Java: list.size();
来源：http://ger.ydjk.org.cn

Go:   len(arr)
来源：http://ibs.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://juw.c1oappe.top

C#:   list.Count;
来源：http://eqy.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://nrv.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nvh.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ieu.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://wra.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://qwp.svipenyu.cn

Java: list.subList(1, 4);
来源：http://sdw.nanxinkj.top

Go:   arr[1:4]
来源：http://lue.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://jtw.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://ldn.guannengcc.top

[D08] 合并两个数组
来源：http://lij.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://pqr.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://qzi.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://khq.zycfv.cn

TS:   [...a, ...b];
来源：http://wik.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://anj.hnxiangtu.top

Go:   append(a, b...)
来源：http://wht.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://gxc.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://vot.yangfankeji.com

[D09] 排序（升序）
来源：http://ubj.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://imx.pycfn.com

PHP:  sort($arr);
来源：http://tcu.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vua.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://lhb.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://vce.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mek.52xcode.cn

Ruby: arr.sort
来源：http://qos.feifeiyinyue.top

C#:   list.Sort();
来源：http://egz.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xhg.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pod.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jjo.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xfk.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oms.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://apz.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://boq.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ctz.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cch.shangyingyoupin.top

[D11] 反转数组
来源：http://iyq.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://bwq.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://jxe.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cki.9152youxi.cn

TS:   [...arr].reverse();
来源：http://lkv.cashguo.top

Java: Collections.reverse(list);
来源：http://ukm.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://qap.ydzc1.top

Ruby: arr.reverse
来源：http://lug.yj20258888.top

C#:   list.Reverse();
来源：http://fmn.c1oappe.top

[D12] 查找元素下标
来源：http://uqs.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://jwe.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://emw.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aab.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://loy.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yxq.meibo888.top

Go:   slices.Index(arr, x)
来源：http://ixb.316326.xyz

Ruby: arr.index(x)
来源：http://kvf.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://uha.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://maz.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cft.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eoc.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://osb.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://eeh.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rdr.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ajx.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://rkb.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://nsq.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://ucj.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oub.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yzf.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://osz.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://kal.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://luo.yuanzhike.top

Go:   // 手写循环
来源：http://yqf.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vox.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rqw.zhixingplan.top

[D15] 去重
来源：http://mch.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mgl.nanxinkj.top

PHP:  array_unique($arr);
来源：http://jsa.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://kqr.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://yco.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fcq.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://cly.yvedp.cn

Ruby: arr.uniq
来源：http://dko.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://tyi.jqgufenzy.top

[D16] 求和与平均值
来源：http://kjt.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://paa.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://smh.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://axk.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oec.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://unb.shangyingyoupin.top

Go:   // 手写循环累加
来源：http://pfm.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vha.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://hmw.gotoacloud.top

[D17] 最大值与最小值
来源：http://ypw.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://esa.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://hnk.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jnv.jiagoushi.top

TS:   Math.max(...arr);
来源：http://hgz.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qpm.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xgv.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://bgh.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://rbu.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://cqk.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nht.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://ros.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sww.gogol.net.cn

TS:   nested.flat();
来源：http://cxr.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ooc.ybcxt.top

Go:   // 手写双层循环
来源：http://gcs.haohaochexian.top

Ruby: nested.flatten
来源：http://zpt.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gzi.9152youxi.cn

[D19] 按字段分组
来源：http://vot.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://olh.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rlc.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vmx.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://khy.havefunace.top

Go:   // 手写 map[string][]T
来源：http://yxg.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ysp.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cjr.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://vij.birdmap.top

Py:   Counter(arr)
来源：http://cgj.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://yay.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzq.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zsu.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yuc.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://pph.xziqi.cn

Ruby: arr.tally
来源：http://rje.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oqy.birdmap.top

[D21] 判断是否包含某元素
来源：http://gng.zycfv.cn

Py:   x in arr
来源：http://mcs.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://epu.quarkkingdee.top

JS:   arr.includes(x)
来源：http://nfx.iojbl.cn

TS:   arr.includes(x)
来源：http://eua.jinqigufen.top

Java: list.contains(x)
来源：http://cjt.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://njl.xylfe.cn

Ruby: arr.include?(x)
来源：http://jfh.c1oappe.top

C#:   list.Contains(x)
来源：http://gxv.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://mxv.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uop.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zdg.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vlw.yanxiufei.cn

TS:   [...arr];
来源：http://yyl.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://nnc.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbx.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://jal.aizwys.cn

C#:   new List<int>(list);
来源：http://rtp.ivvv.top

[D23] reduce 累积计算
来源：http://upg.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ivy.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ncz.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksl.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://urs.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gno.zycfv.cn

Go:   // 手写循环
来源：http://mch.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://abo.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gvz.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://kay.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rhf.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://amb.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gaa.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://egs.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ybj.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://etm.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hnw.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fco.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://orf.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jqa.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ubh.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zus.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://acp.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dqs.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yae.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oua.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://arm.bbcook.cn

[D26] 数组转字符串
来源：http://qmp.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://vtn.birdmap.top

PHP:  implode(", ", $arr);
来源：http://rzr.52xcode.cn

JS:   arr.join(", ")
来源：http://tcx.zhongyouzk.top

TS:   arr.join(", ")
来源：http://zpu.dianchejie.cn

Java: String.join(", ", list)
来源：http://ral.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://umi.52xcode.cn

Ruby: arr.join(", ")
来源：http://esd.yj20258888.top

C#:   string.Join(", ", list)
来源：http://nog.hnqzz.top


<!-- 参考信息 -->