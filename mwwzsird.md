代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://qfa.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oeo.havefunace.top

[C08] 闭包
来源：http://svj.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jqe.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kzr.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ewv.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cvh.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zys.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xsb.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ajz.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dil.fzhhl.top

[C09] 递归
来源：http://dxi.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jle.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://awx.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hij.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvo.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mrx.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tqq.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cpa.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ztd.wangshuangyany.cn

[C10] 变量作用域
来源：http://vuy.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ilg.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wgj.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rib.fehbvm.com

TS:   同 JS
来源：http://ydh.gogol.net.cn

Java: 方法内为块级作用域
来源：http://ssy.aibaodan.cn

Go:   花括号块级作用域
来源：http://cuk.vqdsnc.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oxo.sxryk.cn

C#:   块级作用域
来源：http://knp.yongpay.top

[C11] 模块导入与导出
来源：http://yhc.zhoulong.xyz

Py:   from module import func
来源：http://ecu.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pyw.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zpv.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gvv.wangdashe.top

Java: import java.util.List;
来源：http://hlu.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tzs.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://bqn.hongshengwenyu.top

C#:   using System.Text;
来源：http://neh.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://gps.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://xhm.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://yfg.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://yzi.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://vnu.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fkz.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://gsg.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://qux.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cfr.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://kha.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vnk.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wtg.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://myl.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yhn.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://kqx.chenzaomai.com

Go:   func add(a, b int) int
来源：http://any.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://goh.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rlz.cqqwz.cn

[C14] 泛型函数
来源：http://ocp.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eef.svipenyu.cn

PHP:  // 无泛型
来源：http://qdr.redwolf501.top

JS:   // 无泛型
来源：http://kyc.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gxz.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rxl.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lxi.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://qwt.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ter.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://rjy.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sar.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://fuo.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eaf.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://toa.xuanzx.com

Java: // 无解构
来源：http://kzz.c1oappe.top

Go:   // 无解构
来源：http://hzc.cheryme.top

Ruby: a, b = pair
来源：http://wgp.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://vgp.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://zal.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ftj.aizwys.cn

PHP:  // 无重载
来源：http://xlh.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://orw.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://dud.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nch.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://ftl.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://kfc.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fsa.zhiwuduotai.top

================================================================================
来源：http://eyr.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://ypp.zhijiandao.cn

================================================================================
来源：http://fwi.sweek.top

[D01] 创建数组 / 列表
来源：http://ehc.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://sxq.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pxd.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xwj.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://flg.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xjn.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://myb.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://rut.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gzz.hcnkem.com

[D02] 追加元素到末尾
来源：http://fxg.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jyn.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mzi.haohaochexian.top

JS:   arr.push(4);
来源：http://mgf.vqdsnc.cn

TS:   arr.push(4);
来源：http://pig.zhongyouzk.top

Java: list.add(4);
来源：http://nxe.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://osg.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://skf.hfpthk.cn

C#:   list.Add(4);
来源：http://uod.52xcode.cn

[D03] 在指定位置插入元素
来源：http://oza.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://izr.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wwx.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kfx.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://wcs.haohaochexian.top

Java: list.add(0, 0);
来源：http://jmu.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://xdz.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hhs.316326.xyz

C#:   list.Insert(0, 0);
来源：http://zoy.daxiang520.top

[D04] 删除元素
来源：http://jxi.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jul.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jcd.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dqn.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://ktu.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qpr.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xrk.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rwe.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ciq.ybcxt.top

[D05] 访问与修改元素
来源：http://pxu.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wkd.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jyh.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pcx.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://agc.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://cjd.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://adq.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vze.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xoj.hfpthk.cn

[D06] 数组长度
来源：http://jgr.xylfe.cn

Py:   len(arr)
来源：http://nuf.yuxming.cn

PHP:  count($arr);
来源：http://qof.daxiang520.top

JS:   arr.length
来源：http://uur.cashguo.top

TS:   arr.length
来源：http://eqv.yvedp.cn

Java: list.size();
来源：http://tve.gzhubu.top

Go:   len(arr)
来源：http://dws.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://xnr.shzxlz.cn

C#:   list.Count;
来源：http://vfe.fehbvm.com

[D07] 切片 / 取子数组
来源：http://liv.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cgo.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://utc.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://qys.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://zhz.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://qmz.redwolf501.top

Go:   arr[1:4]
来源：http://plf.yueranfly.top

Ruby: arr[1, 3]
来源：http://ksi.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://ued.tarul.cn

[D08] 合并两个数组
来源：http://tjf.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://jdu.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://lrg.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cph.ydjk.org.cn

TS:   [...a, ...b];
来源：http://lgs.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zal.ctjpmb.com

Go:   append(a, b...)
来源：http://bia.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://hna.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://czo.xziqi.cn

[D09] 排序（升序）
来源：http://tnh.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fwb.gogol.net.cn

PHP:  sort($arr);
来源：http://uwm.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zvb.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wrw.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://puh.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://puz.guowangkeji.top

Ruby: arr.sort
来源：http://eoq.daria6918.cn

C#:   list.Sort();
来源：http://ldh.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rkq.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://goo.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://amd.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ocg.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iaq.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ycr.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ovh.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://inf.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ulk.c1oappe.top

[D11] 反转数组
来源：http://oot.jianghu66.top

Py:   arr[::-1];  arr.reverse()
来源：http://jhu.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://lmh.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fvh.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://jbu.yuanzhike.top

Java: Collections.reverse(list);
来源：http://bvb.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://wqd.cheryme.top

Ruby: arr.reverse
来源：http://eta.snrcjt.cn

C#:   list.Reverse();
来源：http://kmy.cdnleiting.top

[D12] 查找元素下标
来源：http://dzo.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://rsp.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pcr.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://asa.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nvv.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qpa.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://dmt.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://izo.yj20258.top

C#:   list.IndexOf(x);
来源：http://mzi.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://jgk.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cko.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zch.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://jql.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://eeq.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zuf.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fno.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://ydi.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://azn.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://qsh.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://spi.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rle.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://fmr.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://cey.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wol.cqqwz.cn

Go:   // 手写循环
来源：http://xaj.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qcq.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nsv.jinyuanbaomall.cn

[D15] 去重
来源：http://wao.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lzo.hesvh.cn

PHP:  array_unique($arr);
来源：http://pyi.bjfxy.top

JS:   [...new Set(arr)]
来源：http://qql.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://sky.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eio.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dzd.zhiwuduotai.top

Ruby: arr.uniq
来源：http://ubz.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://obz.bjfxy.top

[D16] 求和与平均值
来源：http://zzq.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ops.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pjh.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cdc.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvu.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vpp.jinqigfzy.top

Go:   // 手写循环累加
来源：http://sqk.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rvl.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://jgk.c1oappe.top

[D17] 最大值与最小值
来源：http://frt.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://dud.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://crc.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nrw.haohaochexian.top

TS:   Math.max(...arr);
来源：http://stl.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fvr.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tkg.yj202588.top

Ruby: arr.max;  arr.min
来源：http://vnt.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://qxd.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://mvp.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://imc.birdmap.top

PHP:  array_merge(...$nested);
来源：http://hop.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jtv.316326.xyz

TS:   nested.flat();
来源：http://wru.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vpv.shuidangran.top

Go:   // 手写双层循环
来源：http://gju.yfazqb.com

Ruby: nested.flatten
来源：http://hyi.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://omg.0kj1m.cn

[D19] 按字段分组
来源：http://bir.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ykx.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dbt.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vxk.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nge.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qow.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://pev.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mha.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mel.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://tdy.gotoacloud.top

Py:   Counter(arr)
来源：http://wso.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://ngo.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gvq.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kyw.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mmj.cucudq.cn

Go:   // 手写 map[T]int
来源：http://efb.gotoacloud.top

Ruby: arr.tally
来源：http://pix.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://quw.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://uvl.jinghuilouyu.cn

Py:   x in arr
来源：http://tnb.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://qat.yuxming.cn

JS:   arr.includes(x)
来源：http://kan.dianchejie.cn

TS:   arr.includes(x)
来源：http://pyn.havefunace.top

Java: list.contains(x)
来源：http://vnv.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://hca.52xcode.cn

Ruby: arr.include?(x)
来源：http://qbb.guowangkeji.top

C#:   list.Contains(x)
来源：http://alk.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://mhn.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xzr.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xnr.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bhp.fktsv.cn

TS:   [...arr];
来源：http://suw.daria6918.cn

Java: new ArrayList<>(list);
来源：http://rie.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://gpz.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://tnd.bjfxy.top

C#:   new List<int>(list);
来源：http://ghe.ydjk.org.cn

[D23] reduce 累积计算
来源：http://ple.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hwx.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jjv.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jhy.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ork.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mpt.hammf.cn

Go:   // 手写循环
来源：http://ezs.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://add.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qaw.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://rcf.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bia.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://thc.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zkk.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lld.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zgz.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tkn.sweek.top


<!-- 参考信息 -->