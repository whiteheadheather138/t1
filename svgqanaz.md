代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kef.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gyk.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vsv.jqgufenzy.top

[C09] 递归
来源：http://ksr.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qrl.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yoq.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ztz.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aux.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://suv.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wrk.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eyl.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fwk.snrcjt.cn

[C10] 变量作用域
来源：http://klr.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tmw.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://poq.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gaz.ivvv.top

TS:   同 JS
来源：http://kxv.fktsv.cn

Java: 方法内为块级作用域
来源：http://sbk.zhengqikj.top

Go:   花括号块级作用域
来源：http://znt.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://brm.xziqi.cn

C#:   块级作用域
来源：http://toz.zhengqikj.top

[C11] 模块导入与导出
来源：http://xqx.yuanzhike.top

Py:   from module import func
来源：http://pnn.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hqq.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jpa.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://shs.yanxiufei.cn

Java: import java.util.List;
来源：http://uff.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cyx.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://dhd.zycfv.cn

C#:   using System.Text;
来源：http://vew.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://bfb.uphjek.com

Py:   (lambda: print("run"))()
来源：http://pzy.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://jho.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://bgr.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://pgo.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ccg.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://odl.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://jen.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://srm.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://bgc.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cib.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://anc.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bxr.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uax.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://upt.gzhubu.top

Go:   func add(a, b int) int
来源：http://jaq.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lnv.zhongyouzk.top

C#:   int Add(int a, int b) => a + b;
来源：http://wah.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://afe.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ndn.birdmap.top

PHP:  // 无泛型
来源：http://yay.chenjidiqi.icu

JS:   // 无泛型
来源：http://zlq.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lld.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fyk.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vvy.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://hqq.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xzr.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://ssv.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kke.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://vtg.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eip.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tsv.zhongyouzk.top

Java: // 无解构
来源：http://ezt.wangshuangyany.cn

Go:   // 无解构
来源：http://aic.jyoumei.cn

Ruby: a, b = pair
来源：http://wza.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://sog.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://hco.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oob.jlsjyb.cn

PHP:  // 无重载
来源：http://atp.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://exv.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://nya.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://moa.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://kkm.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://sfy.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://owt.fanxiaobao.xyz

================================================================================
来源：http://zck.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://ptp.ivvv.top

================================================================================
来源：http://dgd.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://yti.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vks.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://muf.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://asc.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wog.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yxs.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://qcv.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://ukp.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dwk.tanke756.top

[D02] 追加元素到末尾
来源：http://amx.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kha.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zwa.yj20258.top

JS:   arr.push(4);
来源：http://ozy.cqqwz.cn

TS:   arr.push(4);
来源：http://puj.gzhubu.top

Java: list.add(4);
来源：http://fne.cheryme.top

Go:   arr = append(arr, 4)
来源：http://eet.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://eky.wangdashe.top

C#:   list.Add(4);
来源：http://glf.52xcode.cn

[D03] 在指定位置插入元素
来源：http://hat.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://rqb.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zrq.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ztn.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://znv.mhx1999.top

Java: list.add(0, 0);
来源：http://tzr.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ykt.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hvo.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://rri.hywenlv.cn

[D04] 删除元素
来源：http://exg.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yep.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cxw.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bnc.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://xmt.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rre.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tbh.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fum.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zdr.guowangkeji.top

[D05] 访问与修改元素
来源：http://ykv.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vgr.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ejz.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zdr.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://uhw.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://bmp.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://zrn.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jgx.zdqjudy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://srm.gaohongyu789.top

[D06] 数组长度
来源：http://qwu.hnqzz.top

Py:   len(arr)
来源：http://ouq.yuxming.cn

PHP:  count($arr);
来源：http://bjh.zhaomingkeji.xyz

JS:   arr.length
来源：http://ycp.hongshengwenyu.top

TS:   arr.length
来源：http://wuw.iojbl.cn

Java: list.size();
来源：http://dhf.pengpengdd.cyou

Go:   len(arr)
来源：http://wda.bjfxy.top

Ruby: arr.length; arr.size
来源：http://nhd.ppjwa.cn

C#:   list.Count;
来源：http://dwl.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://xdg.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yqi.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://abu.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://mfr.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://oij.hcnkem.com

Java: list.subList(1, 4);
来源：http://lxk.nanxuanxn.top

Go:   arr[1:4]
来源：http://gsx.tanke756.top

Ruby: arr[1, 3]
来源：http://hsb.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://eim.chenlongwang.top

[D08] 合并两个数组
来源：http://ulk.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://yef.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://avf.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mrl.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://nkw.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wvk.fzhhl.top

Go:   append(a, b...)
来源：http://zyv.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://gyn.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://zoh.jiagoushi.top

[D09] 排序（升序）
来源：http://xol.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://lck.quarkkingdee.top

PHP:  sort($arr);
来源：http://egn.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://phx.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ufb.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fmz.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kjf.jianghu66.top

Ruby: arr.sort
来源：http://nze.bbcook.cn

C#:   list.Sort();
来源：http://uyj.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mgj.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pnd.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://agx.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivo.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dio.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ntk.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jrs.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nky.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oyo.ydjk.org.cn

[D11] 反转数组
来源：http://cnn.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://soz.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://sbm.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dna.dianchejie.cn

TS:   [...arr].reverse();
来源：http://jjs.ydzc1.top

Java: Collections.reverse(list);
来源：http://vdg.havefunace.top

Go:   slices.Reverse(arr)
来源：http://qsq.kuanghao11.cn

Ruby: arr.reverse
来源：http://fdg.cqqwz.cn

C#:   list.Reverse();
来源：http://bob.daxiang520.top

[D12] 查找元素下标
来源：http://igm.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://vvz.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wjg.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zrf.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ovm.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eey.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://yrv.xinyue.icu

Ruby: arr.index(x)
来源：http://kqg.yj20258.top

C#:   list.IndexOf(x);
来源：http://eje.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://ree.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wis.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fjp.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://gcn.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://gnw.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wwg.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dyg.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vmn.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ikf.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://tvi.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xkl.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pkl.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://ymv.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://szv.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fhw.mhx1999.top

Go:   // 手写循环
来源：http://gqm.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://zqe.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zvm.zhongyouzk.top

[D15] 去重
来源：http://eca.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mwg.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://nwd.yonumen.top

JS:   [...new Set(arr)]
来源：http://fws.yueranfly.top

TS:   [...new Set(arr)]
来源：http://cxx.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zoc.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://rah.316326.xyz

Ruby: arr.uniq
来源：http://fgd.pycfn.com

C#:   list.Distinct().ToList()
来源：http://ewu.shuidangran.top

[D16] 求和与平均值
来源：http://mms.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dct.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rdu.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sdn.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ckw.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vev.guannengcc.top

Go:   // 手写循环累加
来源：http://bxt.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rbq.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://yly.yj20258.top

[D17] 最大值与最小值
来源：http://szb.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://ixe.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://ydi.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xwp.tarul.cn

TS:   Math.max(...arr);
来源：http://jak.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bgw.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://okq.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://ttq.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://iig.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://iyy.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kcl.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://bvx.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ghg.hysaishi.cn

TS:   nested.flat();
来源：http://oss.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://isr.cqqwz.cn

Go:   // 手写双层循环
来源：http://iij.daria6918.cn

Ruby: nested.flatten
来源：http://jfr.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://dto.yj20258888.top

[D19] 按字段分组
来源：http://doq.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qap.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jpm.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kei.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://psp.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://syi.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://clq.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hwv.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lzu.tarul.cn

[D20] 统计每个元素出现次数
来源：http://xwn.cqqwz.cn

Py:   Counter(arr)
来源：http://xuc.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://ntr.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kcb.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jge.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hij.guannengcc.top

Go:   // 手写 map[T]int
来源：http://juo.hcnkem.com

Ruby: arr.tally
来源：http://sfk.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hhm.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://urk.hnqzz.top

Py:   x in arr
来源：http://fcp.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://dod.dianchejie.cn

JS:   arr.includes(x)
来源：http://nff.andypj.xyz

TS:   arr.includes(x)
来源：http://lnf.nwbrower.top

Java: list.contains(x)
来源：http://ftw.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://jcw.yvedp.cn

Ruby: arr.include?(x)
来源：http://nkj.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://psd.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://hhc.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lky.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xpx.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mra.nanxinkj.top

TS:   [...arr];
来源：http://njl.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://vow.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://mrj.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://shp.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://tji.fengsongda.top

[D23] reduce 累积计算
来源：http://uqg.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qdg.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jyx.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rpm.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kjq.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://yli.nanxuanxn.top

Go:   // 手写循环
来源：http://gtd.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://syo.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eop.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://nfy.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sah.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ywj.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://slo.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eql.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zqn.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hoa.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gka.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xgk.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://xso.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fva.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fan.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gxv.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nbe.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kvb.aizwys.cn


<!-- 参考信息 -->