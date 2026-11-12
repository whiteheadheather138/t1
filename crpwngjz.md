代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cwk.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sbb.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://llm.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tau.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zhu.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kvm.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qix.yj20258.top

[C09] 递归
来源：http://fqo.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://urz.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://buw.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jrk.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srx.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oyr.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eip.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xov.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jrr.hongshengwenyu.top

[C10] 变量作用域
来源：http://jof.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ssm.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ptv.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wwz.jyoumei.cn

TS:   同 JS
来源：http://hxz.yvedp.cn

Java: 方法内为块级作用域
来源：http://elp.dianchejie.cn

Go:   花括号块级作用域
来源：http://dxv.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lmb.wangdashe.top

C#:   块级作用域
来源：http://wgz.gogol.net.cn

[C11] 模块导入与导出
来源：http://qqp.hysaishi.cn

Py:   from module import func
来源：http://klg.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hqo.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yty.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://piy.zycfv.cn

Java: import java.util.List;
来源：http://jkl.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xtw.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://pns.yj20258888.top

C#:   using System.Text;
来源：http://ywm.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://lvd.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://mzb.hammf.cn

PHP:  (function () { echo "run"; })();
来源：http://qfw.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://sid.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://cue.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ajj.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://zdx.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://klq.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ijt.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://bcq.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wbk.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rhw.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bxa.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ufs.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tml.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://zpc.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gso.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://ogn.ehwqpu.com

[C14] 泛型函数
来源：http://dkc.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ixa.gaohongyu789.top

PHP:  // 无泛型
来源：http://dqf.vehdjk.com

JS:   // 无泛型
来源：http://fje.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hsv.yueranfly.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://awn.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vcd.hywenlv.cn

Ruby: # 无泛型
来源：http://mce.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://umi.sweek.top

[C15] 解构 / 展开参数
来源：http://pub.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nkm.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://upw.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://orp.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fxx.jyoumei.cn

Java: // 无解构
来源：http://eaf.andypj.xyz

Go:   // 无解构
来源：http://qtz.tanke756.top

Ruby: a, b = pair
来源：http://pmo.sysykeji.top

C#:   var (a, b) = pair;
来源：http://bif.smart0.xyz

[C16] 函数 / 方法重载
来源：http://ify.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hag.hcnkem.com

PHP:  // 无重载
来源：http://yzv.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://clt.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://xah.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://osm.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://nit.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://htd.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://odc.xylfe.cn

================================================================================
来源：http://fmr.tanke756.top

D. 数组 / 列表 / 集合
来源：http://nvb.hnxiangtu.top

================================================================================
来源：http://gqc.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://huw.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gqj.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://szo.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hnh.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://koy.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nue.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://jek.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://ghk.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zan.tanke756.top

[D02] 追加元素到末尾
来源：http://jfc.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xql.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ohn.fktsv.cn

JS:   arr.push(4);
来源：http://aqg.shuidangran.top

TS:   arr.push(4);
来源：http://mhd.xuanzx.com

Java: list.add(4);
来源：http://qem.yonumen.top

Go:   arr = append(arr, 4)
来源：http://wxp.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://tmf.dianchejie.cn

C#:   list.Add(4);
来源：http://fsv.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://rdi.yj20258.top

Py:   arr.insert(0, 0)
来源：http://zsl.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxy.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jhe.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://rzw.fengsongda.top

Java: list.add(0, 0);
来源：http://xfu.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wwi.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mod.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://vml.pycfn.com

[D04] 删除元素
来源：http://obe.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xbg.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yro.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xwz.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://eev.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wcx.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ucv.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tso.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lbv.shzxlz.cn

[D05] 访问与修改元素
来源：http://suw.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fyq.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://flg.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mhb.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://hhc.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://lrw.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://hlq.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cfn.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ius.shangyingyoupin.top

[D06] 数组长度
来源：http://omy.gotoacloud.top

Py:   len(arr)
来源：http://oik.xuanzx.com

PHP:  count($arr);
来源：http://yst.zhaomingkeji.xyz

JS:   arr.length
来源：http://zmr.jlsjyb.cn

TS:   arr.length
来源：http://dhk.yueranfly.top

Java: list.size();
来源：http://rul.bjfxy.top

Go:   len(arr)
来源：http://koh.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://jsi.dashuyun.cn

C#:   list.Count;
来源：http://hgj.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://arb.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lud.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://bou.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://jrz.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://vcj.0kj1m.cn

Java: list.subList(1, 4);
来源：http://wuy.sjlbkw.cn

Go:   arr[1:4]
来源：http://luc.havefunace.top

Ruby: arr[1, 3]
来源：http://ycb.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://mej.sjlbkw.cn

[D08] 合并两个数组
来源：http://oiu.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://usi.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://flb.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lly.jianghu66.top

TS:   [...a, ...b];
来源：http://zis.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://irr.zhengqikj.top

Go:   append(a, b...)
来源：http://tam.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://ism.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://fuz.ydzc1.top

[D09] 排序（升序）
来源：http://hqm.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://ptm.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://bid.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qxx.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://djy.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://edn.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xto.fengsongda.top

Ruby: arr.sort
来源：http://wlz.fzhhl.top

C#:   list.Sort();
来源：http://exa.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qjf.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zdr.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://odj.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qet.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tef.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://olx.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fxs.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yzu.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jgt.cdnleiting.top

[D11] 反转数组
来源：http://vww.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://fvx.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://mtt.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pge.tianlin.xyz

TS:   [...arr].reverse();
来源：http://gxw.fehbvm.com

Java: Collections.reverse(list);
来源：http://huy.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://qhp.ydzc1.top

Ruby: arr.reverse
来源：http://mbh.havefunace.top

C#:   list.Reverse();
来源：http://nwp.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://tfp.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://hes.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gzt.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmi.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uiw.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bgr.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://zec.gzhubu.top

Ruby: arr.index(x)
来源：http://dyy.birdmap.top

C#:   list.IndexOf(x);
来源：http://xzh.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://wtp.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uyy.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ina.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://xdz.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://bvg.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yga.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oky.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://oxq.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://szk.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://lej.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xml.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dio.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://fnj.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://nzq.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gpt.yj20258.top

Go:   // 手写循环
来源：http://rjk.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://hxe.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://zas.yonumen.top

[D15] 去重
来源：http://feo.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tyi.chenlongwang.top

PHP:  array_unique($arr);
来源：http://vsq.hcnkem.com

JS:   [...new Set(arr)]
来源：http://apu.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://tly.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vbt.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://bbe.316326.xyz

Ruby: arr.uniq
来源：http://ith.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://uhh.wangdashe.top

[D16] 求和与平均值
来源：http://dgc.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pmq.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qnw.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sat.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ija.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://krc.jiagoushi.top

Go:   // 手写循环累加
来源：http://eud.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rey.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://xsa.zdqjudy.top

[D17] 最大值与最小值
来源：http://kvg.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://unx.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://loy.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mlu.wangdashe.top

TS:   Math.max(...arr);
来源：http://bug.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eix.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zxe.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://ebv.yj20258.top

C#:   list.Max();  list.Min()
来源：http://qeb.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://fmy.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vkf.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://upu.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mbo.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://bhn.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kwf.ehwqpu.com

Go:   // 手写双层循环
来源：http://yxe.ppjwa.cn

Ruby: nested.flatten
来源：http://lcx.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://laa.tanke756.top

[D19] 按字段分组
来源：http://rhp.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dyw.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uan.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zhj.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mxz.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nah.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://bts.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sav.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cvd.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://qzk.gogol.net.cn

Py:   Counter(arr)
来源：http://rao.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://mbq.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wru.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vlz.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ltz.316326.xyz

Go:   // 手写 map[T]int
来源：http://olj.52xcode.cn

Ruby: arr.tally
来源：http://czf.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ifc.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://isq.sysykeji.top

Py:   x in arr
来源：http://cxy.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://dhn.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://aac.xinyue.icu

TS:   arr.includes(x)
来源：http://oea.chenzaomai.com

Java: list.contains(x)
来源：http://ewr.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://hhu.xinyue.icu

Ruby: arr.include?(x)
来源：http://tot.9152youxi.cn

C#:   list.Contains(x)
来源：http://aii.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://vnj.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eix.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ktp.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mgn.zhiwuduotai.top

TS:   [...arr];
来源：http://dhd.bbcook.cn

Java: new ArrayList<>(list);
来源：http://fxl.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://vun.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://hpd.hnxiangtu.top

C#:   new List<int>(list);
来源：http://lxs.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://nui.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hjy.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bqg.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gkz.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fae.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bpt.0kj1m.cn

Go:   // 手写循环
来源：http://uww.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://egc.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xzk.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://tno.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uiq.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://alc.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sar.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zhu.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vuw.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wxb.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fpi.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oxc.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://oay.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lvq.jqgfzy.top


<!-- 参考信息 -->