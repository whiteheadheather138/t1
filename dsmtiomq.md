代发 wailian999

TS:   同 JS
来源：http://gzo.cheryme.top

Java: 方法内为块级作用域
来源：http://cbp.yueranfly.top

Go:   花括号块级作用域
来源：http://tni.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hct.tianlin.xyz

C#:   块级作用域
来源：http://the.ydjk.org.cn

[C11] 模块导入与导出
来源：http://vvt.zdqjudy.top

Py:   from module import func
来源：http://ygk.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cmb.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://fkq.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://idx.gogol.net.cn

Java: import java.util.List;
来源：http://rdm.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://khb.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://ctr.daxiang520.top

C#:   using System.Text;
来源：http://nkm.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://oxq.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://ske.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://nox.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://ony.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://put.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://grl.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://aai.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://kys.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ile.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://gyt.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bow.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zhv.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uej.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://psl.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://udw.zycfv.cn

Go:   func add(a, b int) int
来源：http://owk.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qnu.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://hqa.fanxiaobao.xyz

[C14] 泛型函数
来源：http://rih.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://niz.xuanzx.com

PHP:  // 无泛型
来源：http://sus.chenlongwang.top

JS:   // 无泛型
来源：http://bhp.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wrk.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rjh.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://feo.hcnkem.com

Ruby: # 无泛型
来源：http://olo.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ofx.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://bto.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ckz.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://snt.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zqy.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://los.jqgufenzy.top

Java: // 无解构
来源：http://pyn.xuanzx.com

Go:   // 无解构
来源：http://ths.pycfn.com

Ruby: a, b = pair
来源：http://ipg.fehbvm.com

C#:   var (a, b) = pair;
来源：http://dbw.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://ura.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bii.52xcode.cn

PHP:  // 无重载
来源：http://maz.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zzp.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://kwc.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ngx.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://byw.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://ehk.birdmap.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yxs.yj202588.top

================================================================================
来源：http://iqp.pycfn.com

D. 数组 / 列表 / 集合
来源：http://omi.chenlongwang.top

================================================================================
来源：http://zcm.cashguo.top

[D01] 创建数组 / 列表
来源：http://kpd.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vqo.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://veh.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lli.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qjr.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://byu.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://hjp.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://ocp.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pcr.yfazqb.com

[D02] 追加元素到末尾
来源：http://rwt.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lxl.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dle.andypj.xyz

JS:   arr.push(4);
来源：http://eyn.yj202588.top

TS:   arr.push(4);
来源：http://nql.cheryme.top

Java: list.add(4);
来源：http://cuf.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://fzs.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://ndo.birdmap.top

C#:   list.Add(4);
来源：http://can.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://ycj.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://fgw.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://duq.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mpg.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://hml.ehwqpu.com

Java: list.add(0, 0);
来源：http://lxf.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://flu.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jnv.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://szm.ydjk.org.cn

[D04] 删除元素
来源：http://tad.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://itt.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kwv.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bqa.birdmap.top

TS:   arr.splice(0, 1);
来源：http://thg.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://svl.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zhm.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ute.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mpp.pycfn.com

[D05] 访问与修改元素
来源：http://mnc.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lit.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pya.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tkg.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://ioc.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://ftq.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://rmg.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://knw.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kab.fktsv.cn

[D06] 数组长度
来源：http://muq.cheryme.top

Py:   len(arr)
来源：http://eqd.zhijiandao.cn

PHP:  count($arr);
来源：http://bzu.hongshengwenyu.top

JS:   arr.length
来源：http://jth.jyoumei.cn

TS:   arr.length
来源：http://apv.hammf.cn

Java: list.size();
来源：http://xjk.hammf.cn

Go:   len(arr)
来源：http://hgw.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://dzv.kuanghao11.cn

C#:   list.Count;
来源：http://cfm.andypj.xyz

[D07] 切片 / 取子数组
来源：http://bcq.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wom.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ded.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://zjr.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://dqv.guannengcc.top

Java: list.subList(1, 4);
来源：http://fhr.jlsjyb.cn

Go:   arr[1:4]
来源：http://myy.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://upw.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://rjp.9152youxi.cn

[D08] 合并两个数组
来源：http://mqi.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://pll.pycfn.com

PHP:  array_merge($a, $b);
来源：http://wgn.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ojs.yuxming.cn

TS:   [...a, ...b];
来源：http://vof.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ver.hammf.cn

Go:   append(a, b...)
来源：http://vdj.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://ehy.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://fqj.ppjwa.cn

[D09] 排序（升序）
来源：http://nkv.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://sbt.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://ydj.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ojx.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://poa.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ndx.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oxh.jqgfzy.top

Ruby: arr.sort
来源：http://iao.tianlin.xyz

C#:   list.Sort();
来源：http://nnh.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yut.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://imu.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tkp.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ora.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gos.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nne.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ozd.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jdl.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ofl.shuidangran.top

[D11] 反转数组
来源：http://eus.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://yof.aizwys.cn

PHP:  array_reverse($arr);
来源：http://rdk.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ynx.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://wye.hfpthk.cn

Java: Collections.reverse(list);
来源：http://caq.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://djn.yvedp.cn

Ruby: arr.reverse
来源：http://uhg.ehwqpu.com

C#:   list.Reverse();
来源：http://iiz.nanxuanxn.top

[D12] 查找元素下标
来源：http://itp.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://xoo.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oqa.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lck.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qve.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oie.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://mpx.jianghu66.top

Ruby: arr.index(x)
来源：http://jjg.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://uas.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://tnp.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://faq.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fwj.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://wwl.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://pti.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cgh.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jbz.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jmw.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://ubu.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://flv.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ibb.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ega.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://qci.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://uvq.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pby.gogol.net.cn

Go:   // 手写循环
来源：http://ujs.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://bpc.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bgi.ivvv.top

[D15] 去重
来源：http://myw.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://did.epnwcf.com

PHP:  array_unique($arr);
来源：http://ufk.ydzc1.top

JS:   [...new Set(arr)]
来源：http://xvz.fktsv.cn

TS:   [...new Set(arr)]
来源：http://kwt.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vxe.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://mxx.0kj1m.cn

Ruby: arr.uniq
来源：http://nsm.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://uvg.shzxlz.cn

[D16] 求和与平均值
来源：http://ttt.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pvu.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tcm.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dcq.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fnr.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gzn.guannengcc.top

Go:   // 手写循环累加
来源：http://vkd.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dzy.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://ezo.gogol.net.cn

[D17] 最大值与最小值
来源：http://qvm.yonumen.top

Py:   max(arr);  min(arr)
来源：http://xzv.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://ewb.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://swd.vehdjk.com

TS:   Math.max(...arr);
来源：http://mos.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://dsv.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mfv.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://mld.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://jcr.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://lmr.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dqr.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://kqz.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://agy.svipenyu.cn

TS:   nested.flat();
来源：http://bry.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rjy.hnxiangtu.top

Go:   // 手写双层循环
来源：http://ivk.zhijiandao.cn

Ruby: nested.flatten
来源：http://mfu.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kkj.hfpthk.cn

[D19] 按字段分组
来源：http://bji.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rhk.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pwo.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fly.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://pvp.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gdl.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://sqr.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rmw.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://biw.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://aow.bbcook.cn

Py:   Counter(arr)
来源：http://vtl.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://xqb.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sof.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubb.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jtf.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://dps.quarkkingdee.top

Ruby: arr.tally
来源：http://ldk.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nmh.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://ojn.jianghu66.top

Py:   x in arr
来源：http://ldv.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://pbu.hnqzz.top

JS:   arr.includes(x)
来源：http://ufg.chenzaomai.com

TS:   arr.includes(x)
来源：http://mpb.quarkkingdee.top

Java: list.contains(x)
来源：http://utg.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://eps.gogol.net.cn

Ruby: arr.include?(x)
来源：http://cxq.xinyue.icu

C#:   list.Contains(x)
来源：http://rtg.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://dpo.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mjq.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://atm.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ufv.zhixingplan.top

TS:   [...arr];
来源：http://lra.hnqzz.top

Java: new ArrayList<>(list);
来源：http://cwh.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://lwa.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://flk.xinyue.icu

C#:   new List<int>(list);
来源：http://vgp.ydzc1.top

[D23] reduce 累积计算
来源：http://bcm.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aau.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jkp.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asu.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jpf.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://nmw.ivvv.top

Go:   // 手写循环
来源：http://qbu.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yxf.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cjf.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://oeh.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://saq.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fkf.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otq.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dfv.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lie.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://exv.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bxs.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mzf.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://mvk.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eah.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bjs.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ont.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qnk.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://okr.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mag.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hmb.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kjf.9152youxi.cn

[D26] 数组转字符串
来源：http://vgg.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://xyz.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://qsm.gogol.net.cn

JS:   arr.join(", ")
来源：http://jeo.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://vnb.cqqwz.cn

Java: String.join(", ", list)
来源：http://rnf.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://omj.mhx1999.top

Ruby: arr.join(", ")
来源：http://wsk.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://zpq.nwbrower.top

================================================================================
来源：http://lnn.shangyingyoupin.top

E. 字符串处理
来源：http://pkw.cqqwz.cn

================================================================================
来源：http://qxy.jinqigfzy.top

[E01] 拼接字符串
来源：http://pza.yonumen.top


<!-- 参考信息 -->