代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgp.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://heg.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dth.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hid.chenlongwang.top

[C10] 变量作用域
来源：http://yep.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ykz.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eer.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nly.xingfuxueyuan.xyz

TS:   同 JS
来源：http://giv.ppjwa.cn

Java: 方法内为块级作用域
来源：http://ixw.epnwcf.com

Go:   花括号块级作用域
来源：http://fbn.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kfc.yuanzhike.top

C#:   块级作用域
来源：http://etl.yuxming.cn

[C11] 模块导入与导出
来源：http://wbc.pycfn.com

Py:   from module import func
来源：http://foi.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kes.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vxm.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pek.quarkkingdee.top

Java: import java.util.List;
来源：http://bxk.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ehw.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://xsb.cheryme.top

C#:   using System.Text;
来源：http://pnd.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://hqm.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://axy.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://naa.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://cee.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://qzw.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fep.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://dxn.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://aaa.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://aeg.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://pfm.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yix.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://thd.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hoy.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zre.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://frr.nanxinkj.top

Go:   func add(a, b int) int
来源：http://jma.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zgv.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://jjt.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://sem.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ubu.pengpengdd.cyou

PHP:  // 无泛型
来源：http://gbj.fanxiaobao.xyz

JS:   // 无泛型
来源：http://njj.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tav.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fdq.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gzg.quarkkingdee.top

Ruby: # 无泛型
来源：http://ocq.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qba.yuxming.cn

[C15] 解构 / 展开参数
来源：http://spz.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://syi.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://aee.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pbx.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hlx.kuanghao11.cn

Java: // 无解构
来源：http://kuw.hammf.cn

Go:   // 无解构
来源：http://kcj.cdnleiting.top

Ruby: a, b = pair
来源：http://qcg.hcnkem.com

C#:   var (a, b) = pair;
来源：http://nmw.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://wuj.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://slm.hysaishi.cn

PHP:  // 无重载
来源：http://wun.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wpz.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://qua.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cfq.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://mzs.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://vit.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kbj.pengpengdd.cyou

================================================================================
来源：http://pdf.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://wgg.yfazqb.com

================================================================================
来源：http://ukm.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://atf.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qes.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cga.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qff.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eua.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jwu.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://bri.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://nro.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ubq.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://wjn.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzj.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ljt.fengsongda.top

JS:   arr.push(4);
来源：http://bne.0kj1m.cn

TS:   arr.push(4);
来源：http://bqd.hongshengwenyu.top

Java: list.add(4);
来源：http://lhr.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://xsp.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://rty.dianchejie.cn

C#:   list.Add(4);
来源：http://jxa.mhx1999.top

[D03] 在指定位置插入元素
来源：http://yiv.uphjek.com

Py:   arr.insert(0, 0)
来源：http://rqh.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sdf.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gnf.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://wxu.pycfn.com

Java: list.add(0, 0);
来源：http://eqt.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://uac.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vfb.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://bys.yongpay.top

[D04] 删除元素
来源：http://rco.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eys.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ohb.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xel.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://mdq.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kgg.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fmy.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://amg.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mhf.guannengcc.top

[D05] 访问与修改元素
来源：http://naw.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vpe.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fog.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tce.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://rnk.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://aec.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://uxi.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rkh.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hcv.yfazqb.com

[D06] 数组长度
来源：http://yrx.yueranfly.top

Py:   len(arr)
来源：http://jjb.xuanzx.com

PHP:  count($arr);
来源：http://hdo.snrcjt.cn

JS:   arr.length
来源：http://kta.cqqwz.cn

TS:   arr.length
来源：http://hgf.sjlbkw.cn

Java: list.size();
来源：http://pia.jianghu66.top

Go:   len(arr)
来源：http://sxa.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://pkq.bbcook.cn

C#:   list.Count;
来源：http://tun.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://ilz.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fge.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://imk.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://hnm.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://kaa.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://psm.yuanzhike.top

Go:   arr[1:4]
来源：http://lhv.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://wdl.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://hng.vehdjk.com

[D08] 合并两个数组
来源：http://ilu.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://mbk.yj20258.top

PHP:  array_merge($a, $b);
来源：http://bfh.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sbq.dianchejie.cn

TS:   [...a, ...b];
来源：http://hat.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oar.shangyingyoupin.top

Go:   append(a, b...)
来源：http://jfq.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://cos.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://dff.guannengcc.top

[D09] 排序（升序）
来源：http://cuv.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://caq.redwolf501.top

PHP:  sort($arr);
来源：http://ozp.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yph.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mgt.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ije.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uii.tanke756.top

Ruby: arr.sort
来源：http://opj.pycfn.com

C#:   list.Sort();
来源：http://lzc.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bud.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mmk.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gnm.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wgu.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dbm.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yzq.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jak.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kov.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://shi.tianlin.xyz

[D11] 反转数组
来源：http://oxx.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://mih.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://jbh.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tfr.shuidangran.top

TS:   [...arr].reverse();
来源：http://yms.yvedp.cn

Java: Collections.reverse(list);
来源：http://gug.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://eks.zdbjq.cn

Ruby: arr.reverse
来源：http://piz.shzxlz.cn

C#:   list.Reverse();
来源：http://twt.hammf.cn

[D12] 查找元素下标
来源：http://frv.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://kak.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fol.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wci.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cnk.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oln.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://gay.svipenyu.cn

Ruby: arr.index(x)
来源：http://cxq.guannengcc.top

C#:   list.IndexOf(x);
来源：http://emp.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://cte.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sue.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xwk.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://odq.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://rfv.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hgo.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://spr.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://lyi.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://grh.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://pnv.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tts.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://urv.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://fsq.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://axc.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wch.cucudq.cn

Go:   // 手写循环
来源：http://ess.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xkh.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pyo.yongpay.top

[D15] 去重
来源：http://ckk.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wxi.guowangkeji.top

PHP:  array_unique($arr);
来源：http://cdk.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://kqh.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://gak.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wuf.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pde.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://may.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://txa.vqdsnc.cn

[D16] 求和与平均值
来源：http://rkp.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hoz.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cly.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://owf.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eoi.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://shr.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://pvw.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uwq.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://mhd.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://vys.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://sjy.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://eis.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://key.aizwys.cn

TS:   Math.max(...arr);
来源：http://wqw.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zhx.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://far.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://aik.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://pum.yj20258.top

[D18] 扁平化嵌套数组
来源：http://vth.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://apg.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://lzk.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kju.zhixingplan.top

TS:   nested.flat();
来源：http://tft.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sqb.quarkkingdee.top

Go:   // 手写双层循环
来源：http://bai.xziqi.cn

Ruby: nested.flatten
来源：http://enn.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jwm.cqqwz.cn

[D19] 按字段分组
来源：http://tyv.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ksj.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qji.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mvf.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://viq.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lin.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://ppf.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vzm.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jzf.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://kdi.zycfv.cn

Py:   Counter(arr)
来源：http://okk.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://cey.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afu.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gku.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vwe.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://nrg.andypj.xyz

Ruby: arr.tally
来源：http://olb.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lal.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://mnj.quarkkingdee.top

Py:   x in arr
来源：http://avg.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://rka.dashuyun.cn

JS:   arr.includes(x)
来源：http://ker.xuanzx.com

TS:   arr.includes(x)
来源：http://xef.gogol.net.cn

Java: list.contains(x)
来源：http://pue.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://uwn.9152youxi.cn

Ruby: arr.include?(x)
来源：http://whz.yuxming.cn

C#:   list.Contains(x)
来源：http://edn.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://ocn.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jib.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qgb.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bab.quarkkingdee.top

TS:   [...arr];
来源：http://kpj.yj20258.top

Java: new ArrayList<>(list);
来源：http://xlv.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://puk.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://lwk.sysykeji.top

C#:   new List<int>(list);
来源：http://bvp.havefunace.top

[D23] reduce 累积计算
来源：http://qjq.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mwk.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://udz.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hvu.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovg.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ysz.guannengcc.top

Go:   // 手写循环
来源：http://amb.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sbv.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pjt.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://qdk.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qxy.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yuc.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://naw.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zia.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fwh.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fic.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hae.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnt.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://cbh.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tux.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eat.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bhl.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uwo.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://waj.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fjk.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vzs.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ymo.ehwqpu.com

[D26] 数组转字符串
来源：http://tjb.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://vug.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://uku.tian-w.cn

JS:   arr.join(", ")
来源：http://nsp.yuxming.cn

TS:   arr.join(", ")
来源：http://ifi.gotoacloud.top


<!-- 参考信息 -->