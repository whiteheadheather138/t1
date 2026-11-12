代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pnu.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kuf.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwq.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ecm.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ahw.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nve.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dpu.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dqm.ydzc1.top

[C10] 变量作用域
来源：http://qfp.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mta.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mhl.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kin.dianchejie.cn

TS:   同 JS
来源：http://oqb.xziqi.cn

Java: 方法内为块级作用域
来源：http://zer.ydzc1.top

Go:   花括号块级作用域
来源：http://vjm.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nji.hesvh.cn

C#:   块级作用域
来源：http://cor.tanke756.top

[C11] 模块导入与导出
来源：http://qeh.nwbrower.top

Py:   from module import func
来源：http://crb.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://aeg.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hgo.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://obv.dianchejie.cn

Java: import java.util.List;
来源：http://dkn.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://llf.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://oii.chenlongwang.top

C#:   using System.Text;
来源：http://sla.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://wvx.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://cvv.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://hhi.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://rks.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://qik.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjb.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ppl.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://wzg.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wtk.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://xfp.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bqa.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kji.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nsp.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhd.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ceg.tian-w.cn

Go:   func add(a, b int) int
来源：http://hrn.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ifn.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rpq.yuanzhike.top

[C14] 泛型函数
来源：http://jcv.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://src.ivvv.top

PHP:  // 无泛型
来源：http://zgh.redwolf501.top

JS:   // 无泛型
来源：http://onb.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eoo.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wtx.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ypg.vehdjk.com

Ruby: # 无泛型
来源：http://myr.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cvc.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://tet.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://voe.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://lzn.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mpe.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bcf.tianlin.xyz

Java: // 无解构
来源：http://wfj.mhx1999.top

Go:   // 无解构
来源：http://ber.zhongyouzk.top

Ruby: a, b = pair
来源：http://kge.sxryk.cn

C#:   var (a, b) = pair;
来源：http://qil.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://zbf.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tyc.ehwqpu.com

PHP:  // 无重载
来源：http://lfo.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://njw.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://caf.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ckr.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://nya.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://zqj.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mak.shuidangran.top

================================================================================
来源：http://jwv.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://fre.bbcook.cn

================================================================================
来源：http://bbg.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://hde.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://tou.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hlx.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jgg.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://boz.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wpn.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://cqq.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://kpy.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xtn.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://olz.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fws.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sfy.shzxlz.cn

JS:   arr.push(4);
来源：http://ecl.svipenyu.cn

TS:   arr.push(4);
来源：http://cvc.hnqzz.top

Java: list.add(4);
来源：http://fiq.birdmap.top

Go:   arr = append(arr, 4)
来源：http://unv.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://cdh.birdmap.top

C#:   list.Add(4);
来源：http://tyx.yfazqb.com

[D03] 在指定位置插入元素
来源：http://kxn.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://nvx.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://umi.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oqq.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://bms.guowangkeji.top

Java: list.add(0, 0);
来源：http://eoj.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jfz.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wka.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://abv.yongpay.top

[D04] 删除元素
来源：http://qzl.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://avm.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gxt.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qgk.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://rfj.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rdf.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xtv.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://axt.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cxw.yongpay.top

[D05] 访问与修改元素
来源：http://gft.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zvr.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dga.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cty.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://awf.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://xeb.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://vge.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ytd.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://upl.daxiang520.top

[D06] 数组长度
来源：http://bts.xylfe.cn

Py:   len(arr)
来源：http://xnb.jinghuilouyu.cn

PHP:  count($arr);
来源：http://agl.haohaochexian.top

JS:   arr.length
来源：http://laf.cashguo.top

TS:   arr.length
来源：http://umm.andypj.xyz

Java: list.size();
来源：http://pdc.feifeiyinyue.top

Go:   len(arr)
来源：http://edl.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://qtw.ybcxt.top

C#:   list.Count;
来源：http://zxe.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://uhq.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pya.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://nor.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://rep.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://pns.zhixingplan.top

Java: list.subList(1, 4);
来源：http://yfo.yj20258.top

Go:   arr[1:4]
来源：http://tlz.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://wbu.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://zpn.yuanzhike.top

[D08] 合并两个数组
来源：http://lpq.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://wrq.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://yca.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qim.dianchejie.cn

TS:   [...a, ...b];
来源：http://zie.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tup.cqqwz.cn

Go:   append(a, b...)
来源：http://zky.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://tpy.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://mfk.yongpay.top

[D09] 排序（升序）
来源：http://pdt.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://btz.yueranfly.top

PHP:  sort($arr);
来源：http://wmv.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mqq.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zcf.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://fkh.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zbu.epnwcf.com

Ruby: arr.sort
来源：http://ifp.cheryme.top

C#:   list.Sort();
来源：http://kgt.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://age.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lxw.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://giu.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://grb.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hff.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lbd.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdd.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zul.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kcj.zhaomingkeji.xyz

[D11] 反转数组
来源：http://srj.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hvi.yj202588.top

PHP:  array_reverse($arr);
来源：http://ajm.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qka.yuanzhike.top

TS:   [...arr].reverse();
来源：http://uwx.yj20258888.top

Java: Collections.reverse(list);
来源：http://vhm.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://acz.pengpengdd.cyou

Ruby: arr.reverse
来源：http://ffz.gaohongyu789.top

C#:   list.Reverse();
来源：http://lpk.guannengcc.top

[D12] 查找元素下标
来源：http://kqo.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://nsv.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ydc.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ong.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jci.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jbm.jyoumei.cn

Go:   slices.Index(arr, x)
来源：http://atk.cucudq.cn

Ruby: arr.index(x)
来源：http://hyf.xziqi.cn

C#:   list.IndexOf(x);
来源：http://qfe.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://tfm.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jie.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aii.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://squ.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://vfz.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://owc.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oho.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://rin.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://svm.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://zrw.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://paj.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uvw.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://glq.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://iwy.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tzp.tian-w.cn

Go:   // 手写循环
来源：http://hpb.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://kyv.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ukv.yj202588.top

[D15] 去重
来源：http://jtg.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dwp.xylfe.cn

PHP:  array_unique($arr);
来源：http://gwg.sxryk.cn

JS:   [...new Set(arr)]
来源：http://qbw.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://fak.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vng.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://rcq.aibaodan.cn

Ruby: arr.uniq
来源：http://qzp.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://yby.nanxuanxn.top

[D16] 求和与平均值
来源：http://woc.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sxa.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cuh.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://weo.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mht.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xcl.wangdashe.top

Go:   // 手写循环累加
来源：http://omj.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yoa.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://eqt.gzhubu.top

[D17] 最大值与最小值
来源：http://jak.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://nkm.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://mnb.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pba.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://ncr.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://twi.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mkw.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://sxb.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://jnw.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://zhv.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wmt.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://oky.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zmd.zdqjudy.top

TS:   nested.flat();
来源：http://dss.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yxs.tarul.cn

Go:   // 手写双层循环
来源：http://stc.andypj.xyz

Ruby: nested.flatten
来源：http://gkm.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://gox.hfpthk.cn

[D19] 按字段分组
来源：http://kru.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ibz.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pgs.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ork.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://mhe.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bve.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://skk.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vla.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gid.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://srf.jianghu66.top

Py:   Counter(arr)
来源：http://ffz.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://pli.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pnm.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eas.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://csx.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://uld.hnxiangtu.top

Ruby: arr.tally
来源：http://prk.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swd.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://yef.dianchejie.cn

Py:   x in arr
来源：http://dyu.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://aek.snrcjt.cn

JS:   arr.includes(x)
来源：http://efc.havefunace.top

TS:   arr.includes(x)
来源：http://mre.bbcook.cn

Java: list.contains(x)
来源：http://zvp.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://lmc.wangdashe.top

Ruby: arr.include?(x)
来源：http://oeb.yj20258.top

C#:   list.Contains(x)
来源：http://ehx.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://ikf.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pfl.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ama.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mkl.fzhhl.top

TS:   [...arr];
来源：http://fmv.hcnkem.com

Java: new ArrayList<>(list);
来源：http://ryh.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://jct.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://dgh.cqqwz.cn

C#:   new List<int>(list);
来源：http://kht.sjlbkw.cn

[D23] reduce 累积计算
来源：http://ukh.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bpb.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jpp.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://but.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awq.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://unm.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://rli.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rzp.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vjq.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://siu.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fva.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uxg.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jkl.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xsm.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xyw.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oxp.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twk.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dbi.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://uuc.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fsi.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://izo.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://erk.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fgg.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wsw.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tci.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sqd.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uva.jinqigufen.top

[D26] 数组转字符串
来源：http://dqg.vehdjk.com


<!-- 参考信息 -->