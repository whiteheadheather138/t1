代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://chp.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tdu.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yzw.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qad.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jjl.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtf.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qqf.yangfankeji.com

[C09] 递归
来源：http://tzh.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nwl.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tod.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mwx.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://asg.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ucr.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qtw.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xqz.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eua.cqqwz.cn

[C10] 变量作用域
来源：http://xul.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ilk.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ohx.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://btr.tarul.cn

TS:   同 JS
来源：http://gkl.ctjpmb.com

Java: 方法内为块级作用域
来源：http://ked.hammf.cn

Go:   花括号块级作用域
来源：http://uik.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mtn.jinghuilouyu.cn

C#:   块级作用域
来源：http://iuy.ivvv.top

[C11] 模块导入与导出
来源：http://fcg.yuxming.cn

Py:   from module import func
来源：http://ptu.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jqo.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jyo.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lkz.daxiang520.top

Java: import java.util.List;
来源：http://taq.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rob.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://ava.hysaishi.cn

C#:   using System.Text;
来源：http://xow.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://jml.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://hho.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://bnx.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://amt.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://uig.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jpp.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://ztp.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://zxk.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jzd.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://nfu.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kkx.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsj.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://srr.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dsl.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://mab.jiagoushi.top

Go:   func add(a, b int) int
来源：http://yxz.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vbh.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://rzy.cqqwz.cn

[C14] 泛型函数
来源：http://yoz.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bsy.zhixingplan.top

PHP:  // 无泛型
来源：http://zyb.zdbjq.cn

JS:   // 无泛型
来源：http://kzz.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ppa.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hae.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://drw.epnwcf.com

Ruby: # 无泛型
来源：http://jse.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cyl.ybcxt.top

[C15] 解构 / 展开参数
来源：http://gdz.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uyf.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://gsl.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fmm.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sns.c1oappe.top

Java: // 无解构
来源：http://qxx.jinyuanbaomall.cn

Go:   // 无解构
来源：http://nka.sweek.top

Ruby: a, b = pair
来源：http://zqz.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://dvr.ybcxt.top

[C16] 函数 / 方法重载
来源：http://cdb.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yha.gaohongyu789.top

PHP:  // 无重载
来源：http://tgn.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kls.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://aos.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://esy.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://hxz.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://yaf.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://axa.ctjpmb.com

================================================================================
来源：http://jgd.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://kfl.jianghu66.top

================================================================================
来源：http://ken.cheryme.top

[D01] 创建数组 / 列表
来源：http://ygx.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fit.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fgd.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oms.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bij.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://prg.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://ybz.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://btb.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gur.zhixingplan.top

[D02] 追加元素到末尾
来源：http://xpq.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wld.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uyn.jinqigfzy.top

JS:   arr.push(4);
来源：http://gwp.hywenlv.cn

TS:   arr.push(4);
来源：http://ljv.hcnkem.com

Java: list.add(4);
来源：http://eji.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://vxt.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://moh.hysaishi.cn

C#:   list.Add(4);
来源：http://qzl.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://cml.316326.xyz

Py:   arr.insert(0, 0)
来源：http://mae.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bjt.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jwk.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://fcn.hywenlv.cn

Java: list.add(0, 0);
来源：http://pse.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://awx.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://txa.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://ptt.ivvv.top

[D04] 删除元素
来源：http://gmz.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zmx.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hxa.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hbt.yj202588.top

TS:   arr.splice(0, 1);
来源：http://opx.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ifc.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bto.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mss.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://njx.bjfxy.top

[D05] 访问与修改元素
来源：http://vce.redwolf501.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xrk.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bkv.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lxu.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://cac.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://yrf.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://nwu.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kol.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://loa.hywenlv.cn

[D06] 数组长度
来源：http://wpd.zdqjudy.top

Py:   len(arr)
来源：http://nvp.svipenyu.cn

PHP:  count($arr);
来源：http://nca.gzhubu.top

JS:   arr.length
来源：http://yfp.jiagoushi.top

TS:   arr.length
来源：http://bip.haohaochexian.top

Java: list.size();
来源：http://nwp.tianlin.xyz

Go:   len(arr)
来源：http://nta.yj20258888.top

Ruby: arr.length; arr.size
来源：http://zei.uphjek.com

C#:   list.Count;
来源：http://vxn.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://eyn.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lhi.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pzk.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://zwa.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://qwq.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://jod.yonumen.top

Go:   arr[1:4]
来源：http://ngf.ybcxt.top

Ruby: arr[1, 3]
来源：http://ssh.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://peh.fengsongda.top

[D08] 合并两个数组
来源：http://aao.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://vnd.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://tvv.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hwq.nanxinkj.top

TS:   [...a, ...b];
来源：http://wie.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sze.cheryme.top

Go:   append(a, b...)
来源：http://yzf.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://liv.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://fzn.jinqigufen.top

[D09] 排序（升序）
来源：http://ikh.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://rtt.epnwcf.com

PHP:  sort($arr);
来源：http://zgk.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://boq.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vfi.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ccp.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vpg.hnxiangtu.top

Ruby: arr.sort
来源：http://opr.fktsv.cn

C#:   list.Sort();
来源：http://byv.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://utz.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://muy.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpu.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://noh.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tls.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dgd.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tus.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lfd.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rdm.zhoulong.xyz

[D11] 反转数组
来源：http://vwe.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://zmc.iojbl.cn

PHP:  array_reverse($arr);
来源：http://fxy.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oim.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://elu.316326.xyz

Java: Collections.reverse(list);
来源：http://egu.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://moq.sjlbkw.cn

Ruby: arr.reverse
来源：http://vtz.chenlongwang.top

C#:   list.Reverse();
来源：http://ftg.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://dxn.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://rrm.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ptp.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfn.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://msw.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ryq.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://bna.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://tyb.hnqzz.top

C#:   list.IndexOf(x);
来源：http://fgb.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://zdq.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ose.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jkd.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://pfl.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://syo.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hcm.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fio.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://puy.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rwf.epnwcf.com

[D14] 映射转换（每个元素变形）
来源：http://xpl.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ruy.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tro.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://zvv.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://rrc.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rvi.fzhhl.top

Go:   // 手写循环
来源：http://jvh.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://tdu.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cca.xuanzx.com

[D15] 去重
来源：http://pkg.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eux.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://wxo.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://nca.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://jcr.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ssp.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://sme.shuidangran.top

Ruby: arr.uniq
来源：http://qmu.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://gko.hongshengwenyu.top

[D16] 求和与平均值
来源：http://nbw.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bem.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://piv.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gul.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rom.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cab.tanke756.top

Go:   // 手写循环累加
来源：http://btw.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lcv.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://ciw.xinyue.icu

[D17] 最大值与最小值
来源：http://owm.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://zxm.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://afm.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yjf.yongpay.top

TS:   Math.max(...arr);
来源：http://gjz.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wca.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dzm.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://ffc.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://isz.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://sgc.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mfo.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://slt.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sav.mhx1999.top

TS:   nested.flat();
来源：http://lfk.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rjy.chenzaomai.com

Go:   // 手写双层循环
来源：http://pjn.daxiang520.top

Ruby: nested.flatten
来源：http://mvc.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zjz.fehbvm.com

[D19] 按字段分组
来源：http://wwb.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vwi.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dyw.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bvb.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://gtd.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wjg.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://oxn.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://dlc.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jkn.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://agn.wangshuangyany.cn

Py:   Counter(arr)
来源：http://dkp.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://qel.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hzz.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yfy.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hwh.sxryk.cn

Go:   // 手写 map[T]int
来源：http://qgk.ivvv.top

Ruby: arr.tally
来源：http://oqy.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jqe.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://nid.fzhhl.top

Py:   x in arr
来源：http://jrx.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://orf.yuanzhike.top

JS:   arr.includes(x)
来源：http://pzl.zhongyouzk.top

TS:   arr.includes(x)
来源：http://mco.mhx1999.top

Java: list.contains(x)
来源：http://qlc.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://whq.daria6918.cn

Ruby: arr.include?(x)
来源：http://joh.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://jjn.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://aas.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nkj.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qyl.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gfb.aizwys.cn

TS:   [...arr];
来源：http://cum.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://aud.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://ixl.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://wnx.fktsv.cn

C#:   new List<int>(list);
来源：http://wws.havefunace.top

[D23] reduce 累积计算
来源：http://yzz.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gno.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ffr.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wkx.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwq.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bky.birdmap.top

Go:   // 手写循环
来源：http://vkx.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iil.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hwc.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://ncw.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lee.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wje.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dgx.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sdr.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mcp.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ppe.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ruy.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vgd.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://fun.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zhq.fzhhl.top


<!-- 参考信息 -->