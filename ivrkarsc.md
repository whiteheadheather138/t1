代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nxi.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nwe.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dda.xingfuxueyuan.xyz

[C09] 递归
来源：http://gqw.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zbg.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mmn.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qtv.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pgy.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rrz.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ota.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ffj.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nlv.snrcjt.cn

[C10] 变量作用域
来源：http://lgf.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qsd.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kis.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ovs.jinyuanbaomall.cn

TS:   同 JS
来源：http://jqy.nwbrower.top

Java: 方法内为块级作用域
来源：http://vsd.sxryk.cn

Go:   花括号块级作用域
来源：http://ifu.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jlf.hnqzz.top

C#:   块级作用域
来源：http://pvu.birdmap.top

[C11] 模块导入与导出
来源：http://hqx.dianchejie.cn

Py:   from module import func
来源：http://vwx.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wkq.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wih.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://euo.xuanzx.com

Java: import java.util.List;
来源：http://esm.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pbe.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://gru.nanxinkj.top

C#:   using System.Text;
来源：http://lxn.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://wpy.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://fck.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://aay.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://jqa.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://xzi.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eum.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://csa.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://ihn.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wew.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://tnc.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bjl.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bin.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpq.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijf.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ipu.redwolf501.top

Go:   func add(a, b int) int
来源：http://fns.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rzs.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mmt.fzhhl.top

[C14] 泛型函数
来源：http://ire.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xui.zhongyouzk.top

PHP:  // 无泛型
来源：http://isn.ybcxt.top

JS:   // 无泛型
来源：http://vyr.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fek.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ptv.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cdv.chenlongwang.top

Ruby: # 无泛型
来源：http://zyr.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hkf.ydzc1.top

[C15] 解构 / 展开参数
来源：http://pgf.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mkj.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://xjh.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kts.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ixy.aibaodan.cn

Java: // 无解构
来源：http://rlk.wangdashe.top

Go:   // 无解构
来源：http://oda.hfpthk.cn

Ruby: a, b = pair
来源：http://iax.vehdjk.com

C#:   var (a, b) = pair;
来源：http://azf.aizwys.cn

[C16] 函数 / 方法重载
来源：http://fjr.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wfm.bjfxy.top

PHP:  // 无重载
来源：http://qsy.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rlu.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://nar.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sga.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://tmk.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://qva.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hne.shanyushiyangtech.top

================================================================================
来源：http://euh.yj20258.top

D. 数组 / 列表 / 集合
来源：http://rfn.nanxinkj.top

================================================================================
来源：http://ase.pycfn.com

[D01] 创建数组 / 列表
来源：http://jyi.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pwg.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hyp.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xsu.xinyue.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxn.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qbz.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://zrn.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://fse.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kda.hesvh.cn

[D02] 追加元素到末尾
来源：http://bwt.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://acs.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jjq.sufxvd.cn

JS:   arr.push(4);
来源：http://zlo.meibo888.top

TS:   arr.push(4);
来源：http://nkt.gzhubu.top

Java: list.add(4);
来源：http://zde.havefunace.top

Go:   arr = append(arr, 4)
来源：http://tny.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://xjy.guowangkeji.top

C#:   list.Add(4);
来源：http://fxh.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://ojm.tanke756.top

Py:   arr.insert(0, 0)
来源：http://jca.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rdd.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zpw.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://rqi.vehdjk.com

Java: list.add(0, 0);
来源：http://aez.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://tuj.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tzz.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://zxq.jlsjyb.cn

[D04] 删除元素
来源：http://fpd.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hto.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kgm.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://caz.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://gtj.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://msi.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fss.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qki.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lsn.dianchejie.cn

[D05] 访问与修改元素
来源：http://woa.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ant.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kcs.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tvl.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://pbx.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://jia.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://tut.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kmk.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fvg.smart0.xyz

[D06] 数组长度
来源：http://yrh.gogol.net.cn

Py:   len(arr)
来源：http://kum.jlsjyb.cn

PHP:  count($arr);
来源：http://gyh.aizwys.cn

JS:   arr.length
来源：http://cwu.tanke756.top

TS:   arr.length
来源：http://xma.zdbjq.cn

Java: list.size();
来源：http://ndo.shuidangran.top

Go:   len(arr)
来源：http://ykm.meibo888.top

Ruby: arr.length; arr.size
来源：http://oas.quarkkingdee.top

C#:   list.Count;
来源：http://lto.havefunace.top

[D07] 切片 / 取子数组
来源：http://kxa.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jhm.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tjg.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://tkr.yj20258.top

TS:   arr.slice(1, 4);
来源：http://atv.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://mln.zhijiandao.cn

Go:   arr[1:4]
来源：http://rwg.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://xep.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://gfc.guowangkeji.top

[D08] 合并两个数组
来源：http://ntx.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://ila.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://tjx.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cxh.zhixingplan.top

TS:   [...a, ...b];
来源：http://ykd.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ami.zhengqikj.top

Go:   append(a, b...)
来源：http://cug.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://sgn.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://nov.ctjpmb.com

[D09] 排序（升序）
来源：http://fia.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://lrc.tarul.cn

PHP:  sort($arr);
来源：http://qdk.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mjk.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lvg.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tmt.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://osh.vqdsnc.cn

Ruby: arr.sort
来源：http://wdg.xziqi.cn

C#:   list.Sort();
来源：http://pio.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qqj.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nor.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://daz.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mvz.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xar.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yma.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gbp.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qqb.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqe.wangshuangyany.cn

[D11] 反转数组
来源：http://crx.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hzw.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://lrv.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qgr.yfazqb.com

TS:   [...arr].reverse();
来源：http://xbp.tianlin.xyz

Java: Collections.reverse(list);
来源：http://klh.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://zin.pengpengdd.cyou

Ruby: arr.reverse
来源：http://elp.zhoulong.xyz

C#:   list.Reverse();
来源：http://gwp.bjfxy.top

[D12] 查找元素下标
来源：http://waz.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://byh.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kww.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mgl.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ols.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dob.316326.xyz

Go:   slices.Index(arr, x)
来源：http://yru.yuxming.cn

Ruby: arr.index(x)
来源：http://frj.nwbrower.top

C#:   list.IndexOf(x);
来源：http://uwb.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://avw.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://abz.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qcw.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://dub.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://tty.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ytu.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://flp.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://ecu.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bdw.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://qdx.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dfn.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cja.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://euv.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://ypq.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://dnk.mhx1999.top

Go:   // 手写循环
来源：http://kut.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://hyk.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tax.jqgfzy.top

[D15] 去重
来源：http://igh.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xay.ctjpmb.com

PHP:  array_unique($arr);
来源：http://omu.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://iwa.shuidangran.top

TS:   [...new Set(arr)]
来源：http://okq.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://byp.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://ivu.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://azr.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://ffw.daria6918.cn

[D16] 求和与平均值
来源：http://xoe.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uue.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mig.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hmi.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yiu.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uxe.yonumen.top

Go:   // 手写循环累加
来源：http://euu.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://knu.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://fhn.yongpay.top

[D17] 最大值与最小值
来源：http://axk.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://dcn.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://agm.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kkt.vehdjk.com

TS:   Math.max(...arr);
来源：http://swa.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rbc.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gwo.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://zsz.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://qxz.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://hgy.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vqa.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://rno.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mss.sxryk.cn

TS:   nested.flat();
来源：http://dhr.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yfq.cqqwz.cn

Go:   // 手写双层循环
来源：http://rha.ivvv.top

Ruby: nested.flatten
来源：http://koe.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://npj.cqqwz.cn

[D19] 按字段分组
来源：http://ura.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mhh.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://chh.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xiq.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://brr.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qgw.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://mab.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iku.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hyk.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://ojo.gotoacloud.top

Py:   Counter(arr)
来源：http://xxn.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://ggk.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tfa.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bhk.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kdg.smart0.xyz

Go:   // 手写 map[T]int
来源：http://esm.snrcjt.cn

Ruby: arr.tally
来源：http://guw.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qhr.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://kjr.tarul.cn

Py:   x in arr
来源：http://vyw.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://yos.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://iwi.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://fhm.tianlin.xyz

Java: list.contains(x)
来源：http://kfd.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://cii.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://cia.sysykeji.top

C#:   list.Contains(x)
来源：http://rqd.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://tuj.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://plx.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xkc.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ppr.daria6918.cn

TS:   [...arr];
来源：http://zxk.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://lvo.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://vpm.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://mdg.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://lmv.yangfankeji.com

[D23] reduce 累积计算
来源：http://pmn.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fvg.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ixg.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wgz.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vre.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://lob.yfazqb.com

Go:   // 手写循环
来源：http://yvd.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mnz.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hci.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://vqx.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hhd.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vkw.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://utz.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ucc.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://igs.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zoh.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yhj.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://duw.cashguo.top

[D25] Set 集合去重与交并差
来源：http://fmd.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bni.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hmu.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uqi.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://thc.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kbn.guowangkeji.top


<!-- 参考信息 -->