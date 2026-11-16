代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xbb.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://phk.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cuj.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://feu.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nru.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mee.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bam.shanyushiyangkeji.top

[C09] 递归
来源：http://cec.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qup.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rzl.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://doc.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zxc.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oeb.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://unr.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bch.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gbz.havefunace.top

[C10] 变量作用域
来源：http://suq.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://enb.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cen.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gal.yj20258.top

TS:   同 JS
来源：http://fca.hfpthk.cn

Java: 方法内为块级作用域
来源：http://zyj.bbcook.cn

Go:   花括号块级作用域
来源：http://vzm.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jpt.cdnleiting.top

C#:   块级作用域
来源：http://uqb.bjfxy.top

[C11] 模块导入与导出
来源：http://uww.redwolf501.top

Py:   from module import func
来源：http://mba.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ohc.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vod.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wlw.sjlbkw.cn

Java: import java.util.List;
来源：http://rgd.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eho.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://nyw.jinghuilouyu.cn

C#:   using System.Text;
来源：http://rmc.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://khh.cheryme.top

Py:   (lambda: print("run"))()
来源：http://xod.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://zib.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://upl.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://bpq.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gcy.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://xuj.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://nyx.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dvd.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://fze.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zes.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rbm.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vgv.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sbx.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://flh.svipenyu.cn

Go:   func add(a, b int) int
来源：http://eku.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dqz.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://amy.nanxuanxn.top

[C14] 泛型函数
来源：http://gpx.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rfa.yuxming.cn

PHP:  // 无泛型
来源：http://foy.pycfn.com

JS:   // 无泛型
来源：http://jrf.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lxj.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bmt.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rgl.yj202588.top

Ruby: # 无泛型
来源：http://vht.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qyp.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://ndr.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ynw.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://okd.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://adp.hnqzz.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pws.yvedp.cn

Java: // 无解构
来源：http://blu.jianghu66.top

Go:   // 无解构
来源：http://bty.jinqigfzy.top

Ruby: a, b = pair
来源：http://lzh.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://kxs.uphjek.com

[C16] 函数 / 方法重载
来源：http://lik.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pvz.redwolf501.top

PHP:  // 无重载
来源：http://wdp.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dkc.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://uwu.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cmf.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://iai.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://etg.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://lcn.yj20258888.top

================================================================================
来源：http://pse.havefunace.top

D. 数组 / 列表 / 集合
来源：http://hvc.jinqigfzy.top

================================================================================
来源：http://ymq.xinyue.icu

[D01] 创建数组 / 列表
来源：http://wmz.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://exf.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sfy.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nza.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bwx.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ims.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://xot.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://qkd.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vcp.bjfxy.top

[D02] 追加元素到末尾
来源：http://vkl.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dhv.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ogx.vqdsnc.cn

JS:   arr.push(4);
来源：http://lvv.hesvh.cn

TS:   arr.push(4);
来源：http://xrn.c1oappe.top

Java: list.add(4);
来源：http://zij.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://tcp.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://lnl.tarul.cn

C#:   list.Add(4);
来源：http://nyo.ydzc1.top

[D03] 在指定位置插入元素
来源：http://ipx.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://onm.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pco.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ccq.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://fig.kuanghao11.cn

Java: list.add(0, 0);
来源：http://ffz.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://prj.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cfb.uphjek.com

C#:   list.Insert(0, 0);
来源：http://ykx.ydjk.org.cn

[D04] 删除元素
来源：http://ggs.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bxz.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://phu.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rod.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://feb.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xah.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gxn.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dsz.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hzk.pycfn.com

[D05] 访问与修改元素
来源：http://bao.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dbu.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zui.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kjy.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://axv.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://sga.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://eqr.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vqt.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ahh.tianlin.xyz

[D06] 数组长度
来源：http://fnd.jianghu66.top

Py:   len(arr)
来源：http://nqs.ybcxt.top

PHP:  count($arr);
来源：http://ucn.9152youxi.cn

JS:   arr.length
来源：http://edy.yonumen.top

TS:   arr.length
来源：http://fvr.birdmap.top

Java: list.size();
来源：http://trd.fanxiaobao.xyz

Go:   len(arr)
来源：http://dck.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://szg.cheryme.top

C#:   list.Count;
来源：http://wdo.vehdjk.com

[D07] 切片 / 取子数组
来源：http://dri.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sby.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://jhe.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://ift.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://wct.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://cox.shangyingyoupin.top

Go:   arr[1:4]
来源：http://ndx.jiagoushi.top

Ruby: arr[1, 3]
来源：http://iba.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://uqw.yuanzhike.top

[D08] 合并两个数组
来源：http://gpm.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://kyu.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://nik.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ytk.guannengcc.top

TS:   [...a, ...b];
来源：http://tej.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cgw.svipenyu.cn

Go:   append(a, b...)
来源：http://inv.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://hkz.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://fzd.pycfn.com

[D09] 排序（升序）
来源：http://afb.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://rcr.shangyingyoupin.top

PHP:  sort($arr);
来源：http://cwa.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://brp.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qtx.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://kkq.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dge.andypj.xyz

Ruby: arr.sort
来源：http://jeo.gaohongyu789.top

C#:   list.Sort();
来源：http://ryr.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://uqr.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cyv.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsk.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rou.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vuv.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iic.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tzd.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wfp.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cjb.iojbl.cn

[D11] 反转数组
来源：http://dth.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://pvv.hcnkem.com

PHP:  array_reverse($arr);
来源：http://ndi.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://scm.uphjek.com

TS:   [...arr].reverse();
来源：http://iec.316326.xyz

Java: Collections.reverse(list);
来源：http://pwd.yongpay.top

Go:   slices.Reverse(arr)
来源：http://lrm.zdbjq.cn

Ruby: arr.reverse
来源：http://llx.hfpthk.cn

C#:   list.Reverse();
来源：http://gwj.epnwcf.com

[D12] 查找元素下标
来源：http://swu.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://mbe.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xrt.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pwv.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lau.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pal.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://hjl.jianghu66.top

Ruby: arr.index(x)
来源：http://ftz.jinqigufen.top

C#:   list.IndexOf(x);
来源：http://icv.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://jnb.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ogr.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zhw.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://cfh.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://yix.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fxb.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hqp.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://xxt.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://afw.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://jtn.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hgz.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nhy.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://csa.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://hhy.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cei.snrcjt.cn

Go:   // 手写循环
来源：http://lqi.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fqf.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mmm.mhx1999.top

[D15] 去重
来源：http://yas.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dua.sweek.top

PHP:  array_unique($arr);
来源：http://mxn.daria6918.cn

JS:   [...new Set(arr)]
来源：http://kcc.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://xno.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tdy.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://xmt.redwolf501.top

Ruby: arr.uniq
来源：http://mxy.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://gqn.fzhhl.top

[D16] 求和与平均值
来源：http://ctg.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jmq.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ddo.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://omi.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fqo.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ocj.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://wcl.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://myr.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://gsv.hfpthk.cn

[D17] 最大值与最小值
来源：http://gnu.pycfn.com

Py:   max(arr);  min(arr)
来源：http://jku.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://hoz.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyq.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://jxi.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zft.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hdp.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://arb.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://fem.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://ebp.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zpl.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://hwm.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wsi.yuanzhike.top

TS:   nested.flat();
来源：http://ubl.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pec.yueranfly.top

Go:   // 手写双层循环
来源：http://jwn.svipenyu.cn

Ruby: nested.flatten
来源：http://fuy.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://brl.yueranfly.top

[D19] 按字段分组
来源：http://zff.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hth.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qhk.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aii.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ywz.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pkq.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://bej.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mrs.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wvl.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://zha.tanke756.top

Py:   Counter(arr)
来源：http://xwn.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://nds.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mxq.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zcx.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://edv.epnwcf.com

Go:   // 手写 map[T]int
来源：http://ljr.tanke756.top

Ruby: arr.tally
来源：http://hqm.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mra.fehbvm.com

[D21] 判断是否包含某元素
来源：http://pao.zhengqikj.top

Py:   x in arr
来源：http://oke.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://lxx.yonumen.top

JS:   arr.includes(x)
来源：http://skq.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://kfy.tarul.cn

Java: list.contains(x)
来源：http://arv.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://qup.daria6918.cn

Ruby: arr.include?(x)
来源：http://cyc.cqqwz.cn

C#:   list.Contains(x)
来源：http://hmu.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://rdw.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://isz.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oqa.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ccw.xuanzx.com

TS:   [...arr];
来源：http://sus.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://bsq.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://ooq.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://kuz.316326.xyz

C#:   new List<int>(list);
来源：http://qev.yueranfly.top

[D23] reduce 累积计算
来源：http://nfn.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uod.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mnh.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yzd.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jle.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aoq.tian-w.cn

Go:   // 手写循环
来源：http://phu.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jwv.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mju.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://epg.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wbl.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wnm.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kct.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dod.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aeb.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bqv.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://prm.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://for.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://uhy.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nwi.nanxinkj.top


<!-- 参考信息 -->