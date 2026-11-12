代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bgw.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mcr.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://krq.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hgu.fktsv.cn

[C10] 变量作用域
来源：http://npo.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fow.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://owh.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dns.jiagoushi.top

TS:   同 JS
来源：http://ana.yj202588.top

Java: 方法内为块级作用域
来源：http://npd.yj20258888.top

Go:   花括号块级作用域
来源：http://qsh.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bpx.xylfe.cn

C#:   块级作用域
来源：http://aqr.dashuyun.cn

[C11] 模块导入与导出
来源：http://hep.yanxiufei.cn

Py:   from module import func
来源：http://osc.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pef.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ggu.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xwt.gzhubu.top

Java: import java.util.List;
来源：http://ymx.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iqy.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://zza.mhx1999.top

C#:   using System.Text;
来源：http://hof.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://gfu.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://dbo.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://pjj.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://kza.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://bfv.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mvv.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://ntr.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://ark.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zdw.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://gux.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pcf.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqj.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dbn.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dtt.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://jqe.havefunace.top

Go:   func add(a, b int) int
来源：http://wfk.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zxz.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://fiu.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://pkt.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gqy.jqgfzy.top

PHP:  // 无泛型
来源：http://fnc.jqgfzy.top

JS:   // 无泛型
来源：http://iig.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uni.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hzf.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ktx.svipenyu.cn

Ruby: # 无泛型
来源：http://igc.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gpz.bbcook.cn

[C15] 解构 / 展开参数
来源：http://uwk.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ymj.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://xjn.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nmk.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ifc.hywenlv.cn

Java: // 无解构
来源：http://kkh.jyoumei.cn

Go:   // 无解构
来源：http://rqs.zdbjq.cn

Ruby: a, b = pair
来源：http://hur.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://uwf.tanke756.top

[C16] 函数 / 方法重载
来源：http://nbl.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sar.epnwcf.com

PHP:  // 无重载
来源：http://jmr.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mcf.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://isu.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://asc.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://sfo.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://vyg.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tqb.jinqigufen.top

================================================================================
来源：http://jqd.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://cxx.bjfxy.top

================================================================================
来源：http://cfi.ydzc1.top

[D01] 创建数组 / 列表
来源：http://uqn.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dkm.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ezy.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wpj.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://roh.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xyu.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://ixm.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://xso.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xcb.cheryme.top

[D02] 追加元素到末尾
来源：http://abt.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qum.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://psa.yj20258888.top

JS:   arr.push(4);
来源：http://yth.quarkkingdee.top

TS:   arr.push(4);
来源：http://oyf.cqqwz.cn

Java: list.add(4);
来源：http://jqm.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://xxm.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://ens.zdbjq.cn

C#:   list.Add(4);
来源：http://lec.ivvv.top

[D03] 在指定位置插入元素
来源：http://qcl.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://aev.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://czg.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dmv.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://cjm.316326.xyz

Java: list.add(0, 0);
来源：http://equ.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://zlt.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dyv.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://nve.ybcxt.top

[D04] 删除元素
来源：http://hkz.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://alh.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dmn.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://koy.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://bba.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wfy.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gmj.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jel.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oob.nanxuanxn.top

[D05] 访问与修改元素
来源：http://cna.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://llw.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zbw.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wra.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://vhi.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://bvn.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://vyw.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lso.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dmo.wangshuangyany.cn

[D06] 数组长度
来源：http://ltd.yj202588.top

Py:   len(arr)
来源：http://gih.nanxinkj.top

PHP:  count($arr);
来源：http://nqn.zhongyouzk.top

JS:   arr.length
来源：http://uqd.kuanghao11.cn

TS:   arr.length
来源：http://bwm.chenlongwang.top

Java: list.size();
来源：http://xuc.guowangkeji.top

Go:   len(arr)
来源：http://qkg.xuanzx.com

Ruby: arr.length; arr.size
来源：http://ozx.hysaishi.cn

C#:   list.Count;
来源：http://akj.hesvh.cn

[D07] 切片 / 取子数组
来源：http://ddo.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wvu.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://ecq.yongpay.top

JS:   arr.slice(1, 4);
来源：http://hgz.uphjek.com

TS:   arr.slice(1, 4);
来源：http://uck.epnwcf.com

Java: list.subList(1, 4);
来源：http://aug.ctjpmb.com

Go:   arr[1:4]
来源：http://lgu.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://wlo.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://ehw.cdnleiting.top

[D08] 合并两个数组
来源：http://nsn.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://clq.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://wek.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lcs.tian-w.cn

TS:   [...a, ...b];
来源：http://hbh.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pmp.hesvh.cn

Go:   append(a, b...)
来源：http://jax.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://ciq.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://qrl.52xcode.cn

[D09] 排序（升序）
来源：http://vux.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://cte.0kj1m.cn

PHP:  sort($arr);
来源：http://jcf.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hvx.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://con.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eyd.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aeu.yanxiufei.cn

Ruby: arr.sort
来源：http://zwo.hysaishi.cn

C#:   list.Sort();
来源：http://wbq.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kgg.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fco.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vws.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vca.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fti.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://erk.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bmn.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gmc.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://haa.bjfxy.top

[D11] 反转数组
来源：http://nwz.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://oen.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://pms.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ssl.yuanzhike.top

TS:   [...arr].reverse();
来源：http://xtu.c1oappe.top

Java: Collections.reverse(list);
来源：http://xgg.yj202588.top

Go:   slices.Reverse(arr)
来源：http://gxk.yanxiufei.cn

Ruby: arr.reverse
来源：http://ugz.zhengqikj.top

C#:   list.Reverse();
来源：http://vro.andypj.xyz

[D12] 查找元素下标
来源：http://mpj.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://khh.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oav.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oxq.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mtp.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://frq.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://kcf.tian-w.cn

Ruby: arr.index(x)
来源：http://gmq.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://kob.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://emg.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uds.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jgn.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://sde.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://ncz.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bvl.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://esz.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uaj.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vvh.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://kui.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gnt.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lzd.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://oxn.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://ouk.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://llx.fehbvm.com

Go:   // 手写循环
来源：http://cmd.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wdz.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://hne.gaohongyu789.top

[D15] 去重
来源：http://non.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tag.9152youxi.cn

PHP:  array_unique($arr);
来源：http://diw.sysykeji.top

JS:   [...new Set(arr)]
来源：http://fcr.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://psh.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pzc.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://thw.gotoacloud.top

Ruby: arr.uniq
来源：http://vbr.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://ndu.yueranfly.top

[D16] 求和与平均值
来源：http://oxc.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hwg.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyc.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvr.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pef.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zag.dashuyun.cn

Go:   // 手写循环累加
来源：http://mpj.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kjn.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://qkr.tian-w.cn

[D17] 最大值与最小值
来源：http://xtw.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://xhi.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://tfk.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yio.cdnleiting.top

TS:   Math.max(...arr);
来源：http://gxo.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fit.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://evq.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://rkq.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://oat.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://lbh.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://onk.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://wfh.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://anh.zhixingplan.top

TS:   nested.flat();
来源：http://rfl.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lvm.fengsongda.top

Go:   // 手写双层循环
来源：http://mip.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://tjd.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cxa.chenjidiqi.icu

[D19] 按字段分组
来源：http://ppk.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dgv.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rru.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zcv.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lvr.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fwa.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://oov.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mvx.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cfr.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://sgw.ctjpmb.com

Py:   Counter(arr)
来源：http://qdc.cucudq.cn

PHP:  array_count_values($arr);
来源：http://qin.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxu.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvf.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://izu.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://tiv.cucudq.cn

Ruby: arr.tally
来源：http://zsj.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ydl.yvedp.cn

[D21] 判断是否包含某元素
来源：http://qbs.vqdsnc.cn

Py:   x in arr
来源：http://deo.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://jel.hammf.cn

JS:   arr.includes(x)
来源：http://bec.mhx1999.top

TS:   arr.includes(x)
来源：http://imi.vqdsnc.cn

Java: list.contains(x)
来源：http://frz.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://okk.chenzaomai.com

Ruby: arr.include?(x)
来源：http://kuv.jinqigufen.top

C#:   list.Contains(x)
来源：http://nrz.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://tap.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sju.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fwz.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jsn.cdnleiting.top

TS:   [...arr];
来源：http://fna.shuidangran.top

Java: new ArrayList<>(list);
来源：http://smf.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://ytt.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://eqq.ydzc1.top

C#:   new List<int>(list);
来源：http://wog.yfazqb.com

[D23] reduce 累积计算
来源：http://xrm.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sre.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jtl.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ubf.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omi.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pxh.zdbjq.cn

Go:   // 手写循环
来源：http://eub.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yut.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ggv.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://uyk.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zlr.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bcy.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ugf.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cyx.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mba.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jre.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cmy.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cvy.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://mun.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mij.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ijb.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://faw.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gei.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mnr.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lqf.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qhy.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rpc.zhijiandao.cn

[D26] 数组转字符串
来源：http://ilk.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://pvt.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://yth.yfazqb.com

JS:   arr.join(", ")
来源：http://nmb.chenzaomai.com

TS:   arr.join(", ")
来源：http://vcy.epnwcf.com


<!-- 参考信息 -->