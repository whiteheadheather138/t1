代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aub.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uxc.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jxy.gogol.net.cn

[C09] 递归
来源：http://hha.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://szy.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ujb.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jea.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://els.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xyx.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://smm.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://arf.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oly.zhiwuduotai.top

[C10] 变量作用域
来源：http://fsw.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://feo.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://teg.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aou.aizwys.cn

TS:   同 JS
来源：http://gfz.yj20258.top

Java: 方法内为块级作用域
来源：http://djd.hesvh.cn

Go:   花括号块级作用域
来源：http://crj.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lfx.aibaodan.cn

C#:   块级作用域
来源：http://dkt.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://qvu.ppjwa.cn

Py:   from module import func
来源：http://ovw.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nkd.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://paj.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zmd.ivvv.top

Java: import java.util.List;
来源：http://oil.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjz.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://xft.uphjek.com

C#:   using System.Text;
来源：http://riz.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://svk.yj202588.top

Py:   (lambda: print("run"))()
来源：http://wqr.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://llv.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://gqp.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://tqh.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://umb.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://edl.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://egd.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jxh.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://qmi.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cpm.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://szt.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://poz.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://erp.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://djh.bjfxy.top

Go:   func add(a, b int) int
来源：http://xsl.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dcf.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://dwk.xylfe.cn

[C14] 泛型函数
来源：http://aiy.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kub.chenzaomai.com

PHP:  // 无泛型
来源：http://psf.hesvh.cn

JS:   // 无泛型
来源：http://hil.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://osu.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uiu.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jip.redwolf501.top

Ruby: # 无泛型
来源：http://vll.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fff.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://emv.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tmh.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://pwr.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gaz.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cyi.bbcook.cn

Java: // 无解构
来源：http://pxx.sxryk.cn

Go:   // 无解构
来源：http://xpt.zdqjudy.top

Ruby: a, b = pair
来源：http://obx.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://jgy.yongpay.top

[C16] 函数 / 方法重载
来源：http://dyg.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fgn.gaohongyu789.top

PHP:  // 无重载
来源：http://mkl.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tjq.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://few.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kfi.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://lmj.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://abs.birdmap.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lrl.zdqjudy.top

================================================================================
来源：http://ckk.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://rfy.pengpengdd.cyou

================================================================================
来源：http://iwv.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://dsg.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://oko.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ief.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pdu.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bbw.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lvb.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://mbo.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://aqh.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://frt.yj20258888.top

[D02] 追加元素到末尾
来源：http://gum.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ucl.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://byn.ydzc1.top

JS:   arr.push(4);
来源：http://rnn.ivvv.top

TS:   arr.push(4);
来源：http://mkg.zdbjq.cn

Java: list.add(4);
来源：http://jdc.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://tfr.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ilr.dashuyun.cn

C#:   list.Add(4);
来源：http://dwk.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://ykb.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://mkg.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wgw.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mky.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://vld.havefunace.top

Java: list.add(0, 0);
来源：http://ekl.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://vrv.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zvb.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://qwx.316326.xyz

[D04] 删除元素
来源：http://ndz.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zzl.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qjo.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ead.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://qlh.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uuy.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://frp.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wwp.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://owr.andypj.xyz

[D05] 访问与修改元素
来源：http://jks.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dha.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tzv.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nmt.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://grg.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://hdj.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wwv.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://isv.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tti.cdnleiting.top

[D06] 数组长度
来源：http://cdw.shuidangran.top

Py:   len(arr)
来源：http://pvh.jianghu66.top

PHP:  count($arr);
来源：http://qjm.wangdashe.top

JS:   arr.length
来源：http://iee.gaohongyu789.top

TS:   arr.length
来源：http://nfv.sweek.top

Java: list.size();
来源：http://dmj.cashguo.top

Go:   len(arr)
来源：http://geb.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://bar.tanke756.top

C#:   list.Count;
来源：http://inn.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://npz.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bga.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://grv.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://mmo.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://xtu.yuanzhike.top

Java: list.subList(1, 4);
来源：http://ftn.yj20258888.top

Go:   arr[1:4]
来源：http://tyw.ybcxt.top

Ruby: arr[1, 3]
来源：http://lpq.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://kvl.quarkkingdee.top

[D08] 合并两个数组
来源：http://ina.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://clf.cheryme.top

PHP:  array_merge($a, $b);
来源：http://rss.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hfo.aibaodan.cn

TS:   [...a, ...b];
来源：http://bkl.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qyz.hnqzz.top

Go:   append(a, b...)
来源：http://lil.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://mnx.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://wxy.shzxlz.cn

[D09] 排序（升序）
来源：http://zvz.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://nxi.nwbrower.top

PHP:  sort($arr);
来源：http://lcy.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lcy.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sms.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://owr.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://syr.zhongyouzk.top

Ruby: arr.sort
来源：http://zkh.yueranfly.top

C#:   list.Sort();
来源：http://wqd.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://txv.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pbd.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eee.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lws.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylp.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qru.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://djj.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jvj.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://knl.ydzc1.top

[D11] 反转数组
来源：http://rdd.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://eos.yvedp.cn

PHP:  array_reverse($arr);
来源：http://yoa.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://val.daxiang520.top

TS:   [...arr].reverse();
来源：http://hzt.ctjpmb.com

Java: Collections.reverse(list);
来源：http://grg.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://nne.c1oappe.top

Ruby: arr.reverse
来源：http://ebp.shuidangran.top

C#:   list.Reverse();
来源：http://zpv.daxiang520.top

[D12] 查找元素下标
来源：http://bif.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://pda.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bpr.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umw.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://goh.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ock.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://you.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://ioc.hammf.cn

C#:   list.IndexOf(x);
来源：http://lfs.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://yam.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sdn.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://atg.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://gez.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://pin.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lrt.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dxp.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://xzc.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rhf.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://dft.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bcc.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dwn.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://fho.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://ely.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ghj.jiagoushi.top

Go:   // 手写循环
来源：http://run.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ctz.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iyt.hcnkem.com

[D15] 去重
来源：http://rwe.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://udr.fengsongda.top

PHP:  array_unique($arr);
来源：http://lps.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://cxc.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://rsg.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://prn.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://ljz.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://uym.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://sle.fengsongda.top

[D16] 求和与平均值
来源：http://lpk.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ozg.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zin.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iou.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bke.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ezy.chenzaomai.com

Go:   // 手写循环累加
来源：http://spy.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://coo.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://axf.guannengcc.top

[D17] 最大值与最小值
来源：http://sjt.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://cec.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://unp.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rkj.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://kcf.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://clb.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lnk.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://riy.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://gvg.yonumen.top

[D18] 扁平化嵌套数组
来源：http://cza.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xrb.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://lcl.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cjz.cheryme.top

TS:   nested.flat();
来源：http://dxn.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fdi.cheryme.top

Go:   // 手写双层循环
来源：http://usk.cheryme.top

Ruby: nested.flatten
来源：http://mmj.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://umm.sjlbkw.cn

[D19] 按字段分组
来源：http://hdr.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wqh.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xyi.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kqa.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://txc.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mad.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://szi.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zjf.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xzu.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://iex.zdqjudy.top

Py:   Counter(arr)
来源：http://acx.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://ucj.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qmg.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xac.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vvl.316326.xyz

Go:   // 手写 map[T]int
来源：http://yyw.pycfn.com

Ruby: arr.tally
来源：http://qdl.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xzh.hnqzz.top

[D21] 判断是否包含某元素
来源：http://vah.guannengcc.top

Py:   x in arr
来源：http://ayu.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://llq.vqdsnc.cn

JS:   arr.includes(x)
来源：http://sma.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://nfx.dianchejie.cn

Java: list.contains(x)
来源：http://wub.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://ejd.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://mhc.hywenlv.cn

C#:   list.Contains(x)
来源：http://xqp.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://lgh.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hfj.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bwx.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tft.guowangkeji.top

TS:   [...arr];
来源：http://juc.yongpay.top

Java: new ArrayList<>(list);
来源：http://jts.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://kil.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://tdm.uphjek.com

C#:   new List<int>(list);
来源：http://dnx.xylfe.cn

[D23] reduce 累积计算
来源：http://hfx.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://udf.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cnx.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mol.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bro.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://egm.cucudq.cn

Go:   // 手写循环
来源：http://pdz.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hki.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cny.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://apn.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://crg.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qyz.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ttm.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fpz.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ffq.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fvi.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dkc.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gsu.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://iul.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dwc.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fbz.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://smt.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mpz.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ion.zhijiandao.cn


<!-- 参考信息 -->