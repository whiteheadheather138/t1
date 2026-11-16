代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lcu.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sgv.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vzd.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://air.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zpp.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kco.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mzi.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zrg.vqdsnc.cn

[C10] 变量作用域
来源：http://hen.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rdy.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bbo.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://coe.zhiwuduotai.top

TS:   同 JS
来源：http://cnl.yonumen.top

Java: 方法内为块级作用域
来源：http://yzi.yonumen.top

Go:   花括号块级作用域
来源：http://hzy.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://paf.epnwcf.com

C#:   块级作用域
来源：http://mcc.daria6918.cn

[C11] 模块导入与导出
来源：http://hyw.smart0.xyz

Py:   from module import func
来源：http://cxq.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qob.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://txf.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yay.ctjpmb.com

Java: import java.util.List;
来源：http://stc.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kml.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://qgk.chenzaomai.com

C#:   using System.Text;
来源：http://gur.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://vyy.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://asn.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://ygx.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://rqz.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://qbx.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pnm.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://ckv.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://rfc.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://blr.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://yhm.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ubu.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hij.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bky.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xjs.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://vhc.aizwys.cn

Go:   func add(a, b int) int
来源：http://rpo.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uto.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oho.vehdjk.com

[C14] 泛型函数
来源：http://fhh.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efv.yueranfly.top

PHP:  // 无泛型
来源：http://tfc.sweek.top

JS:   // 无泛型
来源：http://bmn.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yfc.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xor.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mnr.tarul.cn

Ruby: # 无泛型
来源：http://lve.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oel.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://anw.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://unx.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://cyc.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ain.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kqy.aizwys.cn

Java: // 无解构
来源：http://uhu.meibo888.top

Go:   // 无解构
来源：http://sij.wangdashe.top

Ruby: a, b = pair
来源：http://flu.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://ypt.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://xrh.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kki.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://jyd.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://teb.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://ysi.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tpk.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://etd.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://fux.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ued.andypj.xyz

================================================================================
来源：http://fmw.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://feq.mhx1999.top

================================================================================
来源：http://ivk.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://ybk.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aqj.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mfn.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pch.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jod.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ayv.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://pcp.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://gas.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ipd.cucudq.cn

[D02] 追加元素到末尾
来源：http://dzz.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mzm.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wnt.hammf.cn

JS:   arr.push(4);
来源：http://fvh.zhengqikj.top

TS:   arr.push(4);
来源：http://kny.feifeiyinyue.top

Java: list.add(4);
来源：http://wgn.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://rps.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://rlw.fktsv.cn

C#:   list.Add(4);
来源：http://kxw.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://vsk.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://ccy.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fwi.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gdi.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://nhi.wangdashe.top

Java: list.add(0, 0);
来源：http://kje.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://pbh.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dnt.yonumen.top

C#:   list.Insert(0, 0);
来源：http://wde.pycfn.com

[D04] 删除元素
来源：http://hzn.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://spz.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pha.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://obd.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://tcn.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lij.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zqd.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dhl.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xbc.yongpay.top

[D05] 访问与修改元素
来源：http://hqd.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uhz.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fse.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nqz.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://dgc.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://fom.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://pqv.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bej.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zzr.yanxiufei.cn

[D06] 数组长度
来源：http://mjf.hesvh.cn

Py:   len(arr)
来源：http://khw.shuidangran.top

PHP:  count($arr);
来源：http://uks.cqqwz.cn

JS:   arr.length
来源：http://fmq.zdqjudy.top

TS:   arr.length
来源：http://ohs.havefunace.top

Java: list.size();
来源：http://ino.jinghuilouyu.cn

Go:   len(arr)
来源：http://nvu.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://pdh.sysykeji.top

C#:   list.Count;
来源：http://ycv.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://iyy.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jxq.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://utt.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://qyu.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://knh.ehwqpu.com

Java: list.subList(1, 4);
来源：http://xhk.ivvv.top

Go:   arr[1:4]
来源：http://msb.jqgfzy.top

Ruby: arr[1, 3]
来源：http://tgx.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://ctf.jiagoushi.top

[D08] 合并两个数组
来源：http://yqo.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://bjz.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://gac.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lus.ehwqpu.com

TS:   [...a, ...b];
来源：http://ivl.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://psf.tian-w.cn

Go:   append(a, b...)
来源：http://adf.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://bmt.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://dva.guannengcc.top

[D09] 排序（升序）
来源：http://ynr.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://qwj.zhengqikj.top

PHP:  sort($arr);
来源：http://jwl.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gdk.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tpv.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ysq.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yrf.dianchejie.cn

Ruby: arr.sort
来源：http://xro.nwbrower.top

C#:   list.Sort();
来源：http://bfx.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://piq.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vcb.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yow.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rhj.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlp.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pwb.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://buq.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://omk.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cji.cdnleiting.top

[D11] 反转数组
来源：http://qnv.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://qjm.tarul.cn

PHP:  array_reverse($arr);
来源：http://spb.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ryr.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://qyr.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://myf.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://tkx.tianlin.xyz

Ruby: arr.reverse
来源：http://eda.birdmap.top

C#:   list.Reverse();
来源：http://wjq.shangyingyoupin.top

[D12] 查找元素下标
来源：http://bdv.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://ucy.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kvk.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wfy.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzs.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://whd.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://qmf.epnwcf.com

Ruby: arr.index(x)
来源：http://osn.pycfn.com

C#:   list.IndexOf(x);
来源：http://iub.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://zhi.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qez.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dlc.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://stp.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://xpy.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mzz.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ybp.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://htc.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xsd.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://oit.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nwl.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qyq.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://ujn.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://ofw.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://qlf.hywenlv.cn

Go:   // 手写循环
来源：http://zzl.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://qhf.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jbt.jyoumei.cn

[D15] 去重
来源：http://lyo.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mhl.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://org.ivvv.top

JS:   [...new Set(arr)]
来源：http://vki.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://fcl.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ing.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://sjj.birdmap.top

Ruby: arr.uniq
来源：http://ojd.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://xqt.sysykeji.top

[D16] 求和与平均值
来源：http://jge.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://avk.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lpg.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vjt.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://scm.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nlq.ehwqpu.com

Go:   // 手写循环累加
来源：http://gkx.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yqv.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://jpi.cucudq.cn

[D17] 最大值与最小值
来源：http://bdj.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://jvz.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://vby.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xhj.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://mtu.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iyt.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://quy.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://dfj.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://nbb.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://mvw.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ogg.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://pak.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://akk.vehdjk.com

TS:   nested.flat();
来源：http://vsk.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ghm.kuanghao11.cn

Go:   // 手写双层循环
来源：http://lbj.chenzaomai.com

Ruby: nested.flatten
来源：http://cfz.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lfe.jinqigfzy.top

[D19] 按字段分组
来源：http://wxv.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nzo.cheryme.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fzx.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gbp.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nlc.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bbl.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://rjs.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://isg.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://adk.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://flg.kuanghao11.cn

Py:   Counter(arr)
来源：http://vjs.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://zuv.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbk.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bva.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wit.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://qyi.tianlin.xyz

Ruby: arr.tally
来源：http://hhw.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://srt.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://tsg.ywan-chungtsiang.top

Py:   x in arr
来源：http://qqv.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://ggl.yvedp.cn

JS:   arr.includes(x)
来源：http://tcj.smart0.xyz

TS:   arr.includes(x)
来源：http://tdq.yuanzhike.top

Java: list.contains(x)
来源：http://vrz.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://nnq.shuidangran.top

Ruby: arr.include?(x)
来源：http://noc.hesvh.cn

C#:   list.Contains(x)
来源：http://ccd.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://jtf.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tve.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zmf.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hvt.yonumen.top

TS:   [...arr];
来源：http://sey.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://obp.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tec.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://fnc.smart0.xyz

C#:   new List<int>(list);
来源：http://syj.pycfn.com

[D23] reduce 累积计算
来源：http://csh.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eiy.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rfm.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kbs.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ykg.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vgv.aibaodan.cn

Go:   // 手写循环
来源：http://lwp.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wyn.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://suv.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://ayp.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fvr.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wjt.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xmn.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mqf.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kff.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mih.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nbw.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kdg.chenlongwang.top

[D25] Set 集合去重与交并差
来源：http://hhu.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://riy.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gnk.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zoe.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ruh.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://byo.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rav.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mem.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eah.xinyue.icu

[D26] 数组转字符串
来源：http://xww.gogol.net.cn


<!-- 参考信息 -->