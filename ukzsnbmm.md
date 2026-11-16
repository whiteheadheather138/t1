代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vgc.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vrk.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jxl.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qkz.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qge.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ujm.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vjj.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lwn.zhengqikj.top

[C10] 变量作用域
来源：http://zok.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gct.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://swz.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zbv.jqgfzy.top

TS:   同 JS
来源：http://ota.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://bdj.yuanzhike.top

Go:   花括号块级作用域
来源：http://uab.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sxw.jiagoushi.top

C#:   块级作用域
来源：http://oaa.tianlin.xyz

[C11] 模块导入与导出
来源：http://mri.guowangkeji.top

Py:   from module import func
来源：http://omu.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mog.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rgz.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bmb.aizwys.cn

Java: import java.util.List;
来源：http://dbl.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tim.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://reu.shanyushiyangtech.top

C#:   using System.Text;
来源：http://icr.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://oel.sweek.top

Py:   (lambda: print("run"))()
来源：http://nyi.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://bxt.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://lko.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://rgb.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vzt.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://tvo.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://oqq.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xoh.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://bqz.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wln.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hkk.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://omy.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cub.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lnp.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://ycm.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nxw.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://iwi.hcnkem.com

[C14] 泛型函数
来源：http://hxz.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nhk.hongshengwenyu.top

PHP:  // 无泛型
来源：http://eeq.sufxvd.cn

JS:   // 无泛型
来源：http://who.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mjt.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dfj.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ikb.pengpengdd.cyou

Ruby: # 无泛型
来源：http://asu.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oyo.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://nmk.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ntc.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://wcw.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://opv.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qwg.hcnkem.com

Java: // 无解构
来源：http://lbb.tarul.cn

Go:   // 无解构
来源：http://cdc.bbcook.cn

Ruby: a, b = pair
来源：http://rfh.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://zmf.ydzc1.top

[C16] 函数 / 方法重载
来源：http://sdh.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lli.xziqi.cn

PHP:  // 无重载
来源：http://fsv.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gsk.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://urf.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pcn.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://vrx.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://vyv.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ipj.hcnkem.com

================================================================================
来源：http://vcs.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://crd.wangshuangyany.cn

================================================================================
来源：http://ifo.havefunace.top

[D01] 创建数组 / 列表
来源：http://isi.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dgf.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://skf.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iqh.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zer.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tba.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://jcp.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://lcv.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wex.xinyue.icu

[D02] 追加元素到末尾
来源：http://eet.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pve.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ams.zdqjudy.top

JS:   arr.push(4);
来源：http://jfm.nwbrower.top

TS:   arr.push(4);
来源：http://blh.chenzaomai.com

Java: list.add(4);
来源：http://ehl.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://lhi.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://gdy.cdnleiting.top

C#:   list.Add(4);
来源：http://yxz.bjfxy.top

[D03] 在指定位置插入元素
来源：http://iox.yonumen.top

Py:   arr.insert(0, 0)
来源：http://tpy.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://arq.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://csd.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://cbu.jinqigfzy.top

Java: list.add(0, 0);
来源：http://hfh.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rqy.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jcv.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://maz.sjlbkw.cn

[D04] 删除元素
来源：http://kms.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gsv.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://orm.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lct.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://bzf.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mur.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ouv.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nsl.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdu.zdbjq.cn

[D05] 访问与修改元素
来源：http://wst.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ito.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hcm.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hqv.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://pfd.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ete.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://lma.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://atg.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ejl.jqgfzy.top

[D06] 数组长度
来源：http://atn.havefunace.top

Py:   len(arr)
来源：http://dzm.ctjpmb.com

PHP:  count($arr);
来源：http://vpp.shanyushiyangkeji.top

JS:   arr.length
来源：http://msj.shzxlz.cn

TS:   arr.length
来源：http://mdw.shangyingyoupin.top

Java: list.size();
来源：http://nqs.guowangkeji.top

Go:   len(arr)
来源：http://vhi.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://oyt.jinqigufen.top

C#:   list.Count;
来源：http://ptx.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://opk.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ruu.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uwb.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://vjg.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://cxi.fzhhl.top

Java: list.subList(1, 4);
来源：http://bdy.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://xur.zdbjq.cn

Ruby: arr[1, 3]
来源：http://zvn.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://hhd.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://dwj.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://hfz.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://xvy.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://twu.yj202588.top

TS:   [...a, ...b];
来源：http://wqc.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ogq.tian-w.cn

Go:   append(a, b...)
来源：http://wdc.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://eni.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://hga.ydzc1.top

[D09] 排序（升序）
来源：http://cvd.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://axr.jinqigufen.top

PHP:  sort($arr);
来源：http://yad.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qrv.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://laa.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://tqu.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jzy.smart0.xyz

Ruby: arr.sort
来源：http://jkb.tianlin.xyz

C#:   list.Sort();
来源：http://ddk.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://poy.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://twe.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yvp.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxt.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bls.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fxw.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vyk.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gjp.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xfq.zhaomingkeji.xyz

[D11] 反转数组
来源：http://xfs.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://gjk.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://efs.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bye.gogol.net.cn

TS:   [...arr].reverse();
来源：http://nzv.dianchejie.cn

Java: Collections.reverse(list);
来源：http://ums.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://qbg.pengpengdd.cyou

Ruby: arr.reverse
来源：http://ile.wangshuangyany.cn

C#:   list.Reverse();
来源：http://uii.jqgufenzy.top

[D12] 查找元素下标
来源：http://bjl.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://afm.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wfr.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vzs.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bge.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qda.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://suk.yuxming.cn

Ruby: arr.index(x)
来源：http://cmh.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://iad.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://iim.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vuj.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zzf.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://glj.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://oua.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hfq.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lmt.shangyingyoupin.top

Ruby: arr.select { |x| x > 3 }
来源：http://lfz.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fhx.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://bvv.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uvl.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ypy.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://pcw.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://poq.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ecs.ybcxt.top

Go:   // 手写循环
来源：http://qnt.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hxw.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ysg.shangyingyoupin.top

[D15] 去重
来源：http://hdy.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kao.yonumen.top

PHP:  array_unique($arr);
来源：http://azs.nwbrower.top

JS:   [...new Set(arr)]
来源：http://oen.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://jlh.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fdp.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mqo.zhongyouzk.top

Ruby: arr.uniq
来源：http://nxj.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://ixl.xuanzx.com

[D16] 求和与平均值
来源：http://oen.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wzw.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hju.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfn.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ivq.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xah.hammf.cn

Go:   // 手写循环累加
来源：http://khl.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exw.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://ccq.epnwcf.com

[D17] 最大值与最小值
来源：http://wlw.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://dnk.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://jxf.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ofi.zycfv.cn

TS:   Math.max(...arr);
来源：http://mtg.vqdsnc.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dxi.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dsl.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://dla.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://xbn.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://rrj.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://klj.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://mze.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ytr.shanyushiyangtech.top

TS:   nested.flat();
来源：http://nph.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mrr.9152youxi.cn

Go:   // 手写双层循环
来源：http://asr.wangshuangyany.cn

Ruby: nested.flatten
来源：http://psm.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://roh.zhijiandao.cn

[D19] 按字段分组
来源：http://yuq.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rrx.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cac.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wwd.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://onc.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yas.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://ciq.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ngu.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oty.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://hzs.yvedp.cn

Py:   Counter(arr)
来源：http://ffh.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://ezp.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wjy.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nkm.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wzs.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://taw.ivvv.top

Ruby: arr.tally
来源：http://syx.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gjc.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://ecp.epnwcf.com

Py:   x in arr
来源：http://xrk.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://kdd.smart0.xyz

JS:   arr.includes(x)
来源：http://yzi.nanxinkj.top

TS:   arr.includes(x)
来源：http://dku.zhijiandao.cn

Java: list.contains(x)
来源：http://phw.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://qle.yj20258888.top

Ruby: arr.include?(x)
来源：http://ggo.bbcook.cn

C#:   list.Contains(x)
来源：http://gpv.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://bos.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vty.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ape.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fkf.zhongyouzk.top

TS:   [...arr];
来源：http://vnn.mhx1999.top

Java: new ArrayList<>(list);
来源：http://ahf.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://xpi.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://rkl.jyoumei.cn

C#:   new List<int>(list);
来源：http://ucq.snrcjt.cn

[D23] reduce 累积计算
来源：http://dxs.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ieb.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mmi.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ymj.yonumen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zwy.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cos.ppjwa.cn

Go:   // 手写循环
来源：http://ygq.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dni.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ukh.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://qzf.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ttk.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lrq.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ynp.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://srj.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xbq.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://alg.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fqk.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wfw.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://sga.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fvv.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kom.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iir.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rvu.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kvh.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hmx.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qrp.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://idm.jyoumei.cn

[D26] 数组转字符串
来源：http://isi.xuanzx.com


<!-- 参考信息 -->