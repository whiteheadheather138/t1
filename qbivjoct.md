代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sep.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mmw.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xcg.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pkd.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ldg.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tex.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lpm.birdmap.top

[C09] 递归
来源：http://nag.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ncl.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eqo.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dah.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fxi.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lmh.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jck.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qmb.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wdj.aibaodan.cn

[C10] 变量作用域
来源：http://inn.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mfv.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://can.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://thk.ydzc1.top

TS:   同 JS
来源：http://cqf.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://dek.aibaodan.cn

Go:   花括号块级作用域
来源：http://zec.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://egk.jiagoushi.top

C#:   块级作用域
来源：http://tsy.9152youxi.cn

[C11] 模块导入与导出
来源：http://ipz.hywenlv.cn

Py:   from module import func
来源：http://zli.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tuo.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://caw.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rdr.zdqjudy.top

Java: import java.util.List;
来源：http://cyk.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oha.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://nfv.aizwys.cn

C#:   using System.Text;
来源：http://joy.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://grv.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://sry.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://iqj.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://mhi.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://jps.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ekb.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://rhq.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://wtb.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ipe.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://lax.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oad.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxe.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gya.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hlo.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://rvg.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://jxz.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eas.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://pas.zhiwuduotai.top

[C14] 泛型函数
来源：http://tcy.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://orc.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://siv.yfazqb.com

JS:   // 无泛型
来源：http://hnd.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blz.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mbu.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pwk.wangshuangyany.cn

Ruby: # 无泛型
来源：http://jeu.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pru.epnwcf.com

[C15] 解构 / 展开参数
来源：http://bfp.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rrd.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://qqm.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bgv.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jub.birdmap.top

Java: // 无解构
来源：http://bfk.mhx1999.top

Go:   // 无解构
来源：http://rkr.xinyue.icu

Ruby: a, b = pair
来源：http://vxo.yueranfly.top

C#:   var (a, b) = pair;
来源：http://kys.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://dze.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ypb.hysaishi.cn

PHP:  // 无重载
来源：http://ikn.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uqz.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://fwi.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rir.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://vwl.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://hgx.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://csl.yuxming.cn

================================================================================
来源：http://fzh.ivvv.top

D. 数组 / 列表 / 集合
来源：http://uyo.jianghu66.top

================================================================================
来源：http://mve.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://qee.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vwr.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gau.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kim.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gmy.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vgt.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://vpe.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://cah.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jmq.zhixingplan.top

[D02] 追加元素到末尾
来源：http://vbh.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nrs.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vgg.cucudq.cn

JS:   arr.push(4);
来源：http://qsk.cdnleiting.top

TS:   arr.push(4);
来源：http://xno.ppjwa.cn

Java: list.add(4);
来源：http://wmf.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://rwr.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://wvt.hnxiangtu.top

C#:   list.Add(4);
来源：http://cwy.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://ouy.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://eeq.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uwv.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bty.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://trp.jianghu66.top

Java: list.add(0, 0);
来源：http://fgj.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://avo.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ylk.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://xrd.nanxuanxn.top

[D04] 删除元素
来源：http://wge.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://szo.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://buz.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eet.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://hcy.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wzi.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mfx.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rin.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jgf.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://jmr.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vom.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pco.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ito.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://wwe.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://hjt.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://nqd.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fpr.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ktp.yj20258888.top

[D06] 数组长度
来源：http://cdk.jlsjyb.cn

Py:   len(arr)
来源：http://qgo.316326.xyz

PHP:  count($arr);
来源：http://jtb.hysaishi.cn

JS:   arr.length
来源：http://hta.cqqwz.cn

TS:   arr.length
来源：http://bwu.gotoacloud.top

Java: list.size();
来源：http://bei.tarul.cn

Go:   len(arr)
来源：http://ewg.yongpay.top

Ruby: arr.length; arr.size
来源：http://mhk.daria6918.cn

C#:   list.Count;
来源：http://mmu.mhx1999.top

[D07] 切片 / 取子数组
来源：http://yjd.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tbe.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pdw.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://tkk.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://kad.meibo888.top

Java: list.subList(1, 4);
来源：http://qun.meibo888.top

Go:   arr[1:4]
来源：http://alj.wangdashe.top

Ruby: arr[1, 3]
来源：http://dsm.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://ehw.svipenyu.cn

[D08] 合并两个数组
来源：http://rxo.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://bqj.tanke756.top

PHP:  array_merge($a, $b);
来源：http://zmx.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://deb.tian-w.cn

TS:   [...a, ...b];
来源：http://tbq.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tae.yuanzhike.top

Go:   append(a, b...)
来源：http://mxy.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://tfv.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://zxs.hesvh.cn

[D09] 排序（升序）
来源：http://amw.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://xhm.xuanzx.com

PHP:  sort($arr);
来源：http://hpe.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rii.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://oup.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dmf.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ubn.jqgufenzy.top

Ruby: arr.sort
来源：http://med.hcnkem.com

C#:   list.Sort();
来源：http://kiw.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://azu.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ajb.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gds.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dbl.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kcu.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nge.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://coh.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pdw.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zso.tianlin.xyz

[D11] 反转数组
来源：http://vhj.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://dat.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://sdr.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tzq.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://iaj.ybcxt.top

Java: Collections.reverse(list);
来源：http://tno.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://alj.sufxvd.cn

Ruby: arr.reverse
来源：http://yxk.hongshengwenyu.top

C#:   list.Reverse();
来源：http://zdx.aizwys.cn

[D12] 查找元素下标
来源：http://fck.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://xbr.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hdx.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xuy.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zxw.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eaj.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://nkx.daxiang520.top

Ruby: arr.index(x)
来源：http://wkm.uphjek.com

C#:   list.IndexOf(x);
来源：http://vuo.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://dxx.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://clu.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bjo.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://yfc.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://fwg.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fdh.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kcf.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://yzc.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dqm.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://ofw.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nvy.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pbz.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://fis.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://ufz.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eed.jiagoushi.top

Go:   // 手写循环
来源：http://zes.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://etw.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jyx.ivvv.top

[D15] 去重
来源：http://sli.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://snv.yj20258.top

PHP:  array_unique($arr);
来源：http://wxu.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://iyg.birdmap.top

TS:   [...new Set(arr)]
来源：http://pnh.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kuo.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iqg.zhixingplan.top

Ruby: arr.uniq
来源：http://roj.yongpay.top

C#:   list.Distinct().ToList()
来源：http://jux.sufxvd.cn

[D16] 求和与平均值
来源：http://ijr.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rtk.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dtx.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://efe.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgx.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jcw.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://iwd.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fse.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://vmo.birdmap.top

[D17] 最大值与最小值
来源：http://txt.pycfn.com

Py:   max(arr);  min(arr)
来源：http://jzq.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://qzv.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://med.svipenyu.cn

TS:   Math.max(...arr);
来源：http://hep.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://doc.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qld.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://nyi.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://ecw.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://god.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bgl.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://dkh.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zfq.kuanghao11.cn

TS:   nested.flat();
来源：http://raq.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ggy.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://meg.quarkkingdee.top

Ruby: nested.flatten
来源：http://lju.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aky.xuetiantiany.cn

[D19] 按字段分组
来源：http://cpu.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mny.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hbt.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uwa.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bsj.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tmw.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://uyz.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyu.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ycj.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://zjm.zycfv.cn

Py:   Counter(arr)
来源：http://hze.meibo888.top

PHP:  array_count_values($arr);
来源：http://mhh.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gka.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gcr.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xhw.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://zjb.chenlongwang.top

Ruby: arr.tally
来源：http://zwm.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nzl.yj202588.top

[D21] 判断是否包含某元素
来源：http://oxx.daxiang520.top

Py:   x in arr
来源：http://pzh.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://awf.haohaochexian.top

JS:   arr.includes(x)
来源：http://hta.ivvv.top

TS:   arr.includes(x)
来源：http://lcq.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://bzl.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://emq.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://rbr.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://cqr.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://tgs.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://box.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kbh.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yok.gotoacloud.top

TS:   [...arr];
来源：http://rbv.fktsv.cn

Java: new ArrayList<>(list);
来源：http://voy.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://ocb.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://gxo.jqgfzy.top

C#:   new List<int>(list);
来源：http://tnk.zhijiandao.cn

[D23] reduce 累积计算
来源：http://ppy.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tbl.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kfs.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pxl.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ris.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://crr.shangyingyoupin.top

Go:   // 手写循环
来源：http://rmz.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yvu.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iid.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://bzx.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bpy.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sdb.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sfx.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cmx.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uje.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://maz.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://urb.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lvv.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://ndn.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ven.fehbvm.com


<!-- 参考信息 -->