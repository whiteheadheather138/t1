代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rln.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zpy.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://euc.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vgj.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bix.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nhd.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gtt.52xcode.cn

[C09] 递归
来源：http://juv.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eeh.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jut.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dql.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lgi.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xpw.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aty.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dqr.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ias.jinqigfzy.top

[C10] 变量作用域
来源：http://neq.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wja.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ykn.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rdl.fanxiaobao.xyz

TS:   同 JS
来源：http://scn.shzxlz.cn

Java: 方法内为块级作用域
来源：http://wbu.quarkkingdee.top

Go:   花括号块级作用域
来源：http://eab.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zeb.zdqjudy.top

C#:   块级作用域
来源：http://lmc.ivvv.top

[C11] 模块导入与导出
来源：http://haj.jinqigufen.top

Py:   from module import func
来源：http://ejk.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nyx.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sex.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://umy.hfpthk.cn

Java: import java.util.List;
来源：http://zht.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://awv.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://umc.zhoulong.xyz

C#:   using System.Text;
来源：http://rdt.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://hyo.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://tcg.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://hai.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://zpc.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://stq.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://igf.wangshuangyany.cn

Go:   func() { fmt.Println("run") }()
来源：http://nlm.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://yhn.hysaishi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yjc.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://syy.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bmy.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://euq.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jpg.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jgg.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://lae.9152youxi.cn

Go:   func add(a, b int) int
来源：http://gup.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kga.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zmt.9152youxi.cn

[C14] 泛型函数
来源：http://yaa.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nro.zycfv.cn

PHP:  // 无泛型
来源：http://axr.sufxvd.cn

JS:   // 无泛型
来源：http://jsu.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aho.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dvs.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ron.fengsongda.top

Ruby: # 无泛型
来源：http://rfj.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iui.cheryme.top

[C15] 解构 / 展开参数
来源：http://wge.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wno.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://vqa.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://spl.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ohq.hywenlv.cn

Java: // 无解构
来源：http://vpm.cucudq.cn

Go:   // 无解构
来源：http://vtn.yanxiufei.cn

Ruby: a, b = pair
来源：http://sjk.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://pcy.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://hya.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rck.yongpay.top

PHP:  // 无重载
来源：http://ujz.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mxb.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://tkn.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hvy.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://wcf.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://fwb.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ehg.jqgfzy.top

================================================================================
来源：http://onk.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://nhj.cashguo.top

================================================================================
来源：http://emt.52xcode.cn

[D01] 创建数组 / 列表
来源：http://hhj.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ujv.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jqm.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://guz.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wea.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmt.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://wxy.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://ofu.shzxlz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://shh.hnqzz.top

[D02] 追加元素到末尾
来源：http://ial.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dgv.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zyp.xinyue.icu

JS:   arr.push(4);
来源：http://xdo.ydzc1.top

TS:   arr.push(4);
来源：http://mfc.fktsv.cn

Java: list.add(4);
来源：http://rpe.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://ceg.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://zgm.zhixingplan.top

C#:   list.Add(4);
来源：http://djr.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://zev.316326.xyz

Py:   arr.insert(0, 0)
来源：http://qcs.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ilg.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://crz.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://xll.tarul.cn

Java: list.add(0, 0);
来源：http://jhb.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://vnj.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jpm.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://yfi.yfazqb.com

[D04] 删除元素
来源：http://yfx.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hed.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://htv.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rif.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://fcy.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ojh.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wbg.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nvg.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ned.birdmap.top

[D05] 访问与修改元素
来源：http://jpq.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xqc.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nmc.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufq.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://vue.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://zpu.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ozf.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eus.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eii.pycfn.com

[D06] 数组长度
来源：http://jgd.kuanghao11.cn

Py:   len(arr)
来源：http://arr.yj202588.top

PHP:  count($arr);
来源：http://peg.pycfn.com

JS:   arr.length
来源：http://efu.feifeiyinyue.top

TS:   arr.length
来源：http://vdt.hywenlv.cn

Java: list.size();
来源：http://idx.guowangkeji.top

Go:   len(arr)
来源：http://raz.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://gwp.zhiwuduotai.top

C#:   list.Count;
来源：http://euj.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://uwz.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zge.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://pco.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://sev.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://wvb.yj202588.top

Java: list.subList(1, 4);
来源：http://agq.ydzc1.top

Go:   arr[1:4]
来源：http://uaq.andypj.xyz

Ruby: arr[1, 3]
来源：http://hrf.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://hdw.yvedp.cn

[D08] 合并两个数组
来源：http://jkv.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://lui.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://xkn.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ogz.ppjwa.cn

TS:   [...a, ...b];
来源：http://tnd.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aga.chenzaomai.com

Go:   append(a, b...)
来源：http://gxf.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://bit.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://bzs.wangshuangyany.cn

[D09] 排序（升序）
来源：http://tup.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://qzs.chenzaomai.com

PHP:  sort($arr);
来源：http://spi.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xem.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gyr.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uoi.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://znp.tarul.cn

Ruby: arr.sort
来源：http://cse.fengsongda.top

C#:   list.Sort();
来源：http://kly.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://wdn.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://era.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ktr.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://leq.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dxn.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://esg.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bmk.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://krx.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ypi.xylfe.cn

[D11] 反转数组
来源：http://qbl.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://bou.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://anr.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gaw.yfazqb.com

TS:   [...arr].reverse();
来源：http://ibp.tanke756.top

Java: Collections.reverse(list);
来源：http://hgb.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://rte.yueranfly.top

Ruby: arr.reverse
来源：http://adn.ctjpmb.com

C#:   list.Reverse();
来源：http://rrz.bbcook.cn

[D12] 查找元素下标
来源：http://ibu.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://tgp.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mjx.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://krc.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brr.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eyu.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://riw.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://rmj.yuxming.cn

C#:   list.IndexOf(x);
来源：http://xkm.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://uaw.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://swz.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xza.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://oaf.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://rfx.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cca.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hfp.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://vct.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qph.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://xjr.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qot.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tge.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://rkx.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://xeg.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kcq.vqdsnc.cn

Go:   // 手写循环
来源：http://lhl.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://our.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mja.yj20258.top

[D15] 去重
来源：http://vsy.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://doy.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://ukr.birdmap.top

JS:   [...new Set(arr)]
来源：http://pcv.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://hpn.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ntu.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://feg.yanxiufei.cn

Ruby: arr.uniq
来源：http://pvw.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://pzt.vehdjk.com

[D16] 求和与平均值
来源：http://kpk.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oug.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fmu.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bvg.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kvk.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jzz.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://mpn.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jxq.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://obl.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://dkx.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://kaf.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://uiv.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xuj.yfazqb.com

TS:   Math.max(...arr);
来源：http://git.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://emt.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yyb.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://leh.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://xyx.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://iwh.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdk.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://yrz.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gmq.tarul.cn

TS:   nested.flat();
来源：http://syd.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sgd.jqgfzy.top

Go:   // 手写双层循环
来源：http://zdq.quarkkingdee.top

Ruby: nested.flatten
来源：http://dps.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bnn.sweek.top

[D19] 按字段分组
来源：http://paz.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mok.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cyu.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://krr.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hce.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uxy.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://fst.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vic.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mjd.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://msi.jinqigufen.top

Py:   Counter(arr)
来源：http://rgx.fengsongda.top

PHP:  array_count_values($arr);
来源：http://kly.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cdt.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jfs.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nht.havefunace.top

Go:   // 手写 map[T]int
来源：http://fgr.xuanzx.com

Ruby: arr.tally
来源：http://xmh.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qpe.hammf.cn

[D21] 判断是否包含某元素
来源：http://cds.fehbvm.com

Py:   x in arr
来源：http://fue.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://tgq.andypj.xyz

JS:   arr.includes(x)
来源：http://fqo.epnwcf.com

TS:   arr.includes(x)
来源：http://rtb.fehbvm.com

Java: list.contains(x)
来源：http://kup.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://vfb.hcnkem.com

Ruby: arr.include?(x)
来源：http://vqx.jiagoushi.top

C#:   list.Contains(x)
来源：http://qru.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://iqm.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dgk.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hik.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qex.sjlbkw.cn

TS:   [...arr];
来源：http://emn.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://pvw.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://imr.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://huu.zhoulong.xyz

C#:   new List<int>(list);
来源：http://etf.zhijiandao.cn

[D23] reduce 累积计算
来源：http://lbj.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xkv.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oda.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bzt.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kwp.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pri.pycfn.com

Go:   // 手写循环
来源：http://knu.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://run.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sdk.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://niu.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mii.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://skk.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xac.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nov.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rta.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ppd.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gqb.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gss.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://mcg.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lmt.zdqjudy.top


<!-- 参考信息 -->