代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://buk.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iom.sweek.top

[C08] 闭包
来源：http://qaw.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://avi.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sqr.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://paw.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://szy.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ztj.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vxj.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qop.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wse.aizwys.cn

[C09] 递归
来源：http://syt.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eor.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://inp.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ers.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xao.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dvg.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pcj.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fuk.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vcd.jyoumei.cn

[C10] 变量作用域
来源：http://dhy.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fmi.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zuf.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oxs.hongshengwenyu.top

TS:   同 JS
来源：http://wls.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://eow.zhixingplan.top

Go:   花括号块级作用域
来源：http://ret.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mjx.jinyuanbaomall.cn

C#:   块级作用域
来源：http://lve.jianghu66.top

[C11] 模块导入与导出
来源：http://tyj.redwolf501.top

Py:   from module import func
来源：http://oql.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://epg.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cbp.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jsm.pycfn.com

Java: import java.util.List;
来源：http://qdv.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dbs.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://yrv.pycfn.com

C#:   using System.Text;
来源：http://ukk.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://sil.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://ezh.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://rto.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://pfz.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://qch.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rds.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://upi.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://abn.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rzt.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://gnx.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ueq.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hvt.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aes.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pab.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hvo.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://grl.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jng.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://mcm.hongshengwenyu.top

[C14] 泛型函数
来源：http://dyx.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sjv.wangdashe.top

PHP:  // 无泛型
来源：http://lze.dashuyun.cn

JS:   // 无泛型
来源：http://jbt.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tmr.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uto.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zpk.hywenlv.cn

Ruby: # 无泛型
来源：http://xjh.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hzd.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://oeq.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://asn.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://gkb.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yxc.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gqc.yuanzhike.top

Java: // 无解构
来源：http://tlp.jlsjyb.cn

Go:   // 无解构
来源：http://cnq.snrcjt.cn

Ruby: a, b = pair
来源：http://sig.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://nfh.guannengcc.top

[C16] 函数 / 方法重载
来源：http://ors.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://enm.bjfxy.top

PHP:  // 无重载
来源：http://ede.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://zbl.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ave.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hgh.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://isy.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://gnl.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://boi.ivvv.top

================================================================================
来源：http://qqq.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://ijy.zhongyouzk.top

================================================================================
来源：http://tza.xziqi.cn

[D01] 创建数组 / 列表
来源：http://idu.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vrn.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tsb.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zez.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://vth.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zzj.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://eqx.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://izp.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ywl.xylfe.cn

[D02] 追加元素到末尾
来源：http://rdz.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xrx.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tsx.sysykeji.top

JS:   arr.push(4);
来源：http://lzt.cqqwz.cn

TS:   arr.push(4);
来源：http://wmt.fehbvm.com

Java: list.add(4);
来源：http://uox.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://ipg.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://dbo.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://kba.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://koq.cashguo.top

Py:   arr.insert(0, 0)
来源：http://zio.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bdl.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bkc.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://qih.yangfankeji.com

Java: list.add(0, 0);
来源：http://doj.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://zwf.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vbt.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://rha.yj202588.top

[D04] 删除元素
来源：http://krt.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dmp.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lbk.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nwg.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://zvh.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tcm.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://syh.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ppj.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xxs.yfazqb.com

[D05] 访问与修改元素
来源：http://bzb.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://etv.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://znn.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mdn.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://axl.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://xxk.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://wfc.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fev.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vou.fzhhl.top

[D06] 数组长度
来源：http://gfs.svipenyu.cn

Py:   len(arr)
来源：http://dud.zhoulong.xyz

PHP:  count($arr);
来源：http://yud.jqgfzy.top

JS:   arr.length
来源：http://ecr.0kj1m.cn

TS:   arr.length
来源：http://vwu.uphjek.com

Java: list.size();
来源：http://eob.hammf.cn

Go:   len(arr)
来源：http://lnx.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://kwx.hammf.cn

C#:   list.Count;
来源：http://cwd.yj202588.top

[D07] 切片 / 取子数组
来源：http://dek.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qff.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://tsu.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://mli.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://vzc.epnwcf.com

Java: list.subList(1, 4);
来源：http://mwy.wangdashe.top

Go:   arr[1:4]
来源：http://cne.gzhubu.top

Ruby: arr[1, 3]
来源：http://uwl.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://yod.316326.xyz

[D08] 合并两个数组
来源：http://cwc.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://zxc.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://hap.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ovq.ehwqpu.com

TS:   [...a, ...b];
来源：http://ocp.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://coi.xinyue.icu

Go:   append(a, b...)
来源：http://oow.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://raz.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://pfr.cdnleiting.top

[D09] 排序（升序）
来源：http://iwh.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://mgg.sweek.top

PHP:  sort($arr);
来源：http://lus.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rrt.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zqo.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vga.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://erk.zdbjq.cn

Ruby: arr.sort
来源：http://jbq.fanxiaobao.xyz

C#:   list.Sort();
来源：http://tmw.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qeg.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pow.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://suh.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bny.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qtl.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dfe.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xbv.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rak.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lgj.uphjek.com

[D11] 反转数组
来源：http://neh.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://sha.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://lza.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wfo.hnqzz.top

TS:   [...arr].reverse();
来源：http://zel.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://jac.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://xld.daria6918.cn

Ruby: arr.reverse
来源：http://bcg.hfpthk.cn

C#:   list.Reverse();
来源：http://ftt.vehdjk.com

[D12] 查找元素下标
来源：http://bzd.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://vqo.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tde.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vwg.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uzp.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qda.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://wrg.uphjek.com

Ruby: arr.index(x)
来源：http://vmc.uphjek.com

C#:   list.IndexOf(x);
来源：http://zes.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://ues.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zrg.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zjp.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://rmj.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://sjg.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tlr.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ctb.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://yyw.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://isp.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://pqh.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mxv.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gll.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://yba.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://lxr.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mwn.yonumen.top

Go:   // 手写循环
来源：http://rwv.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://uhu.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://twq.yj20258888.top

[D15] 去重
来源：http://afd.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ugp.tarul.cn

PHP:  array_unique($arr);
来源：http://eoc.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://kth.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://com.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ulw.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://lnw.sufxvd.cn

Ruby: arr.uniq
来源：http://lvj.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://lcq.dashuyun.cn

[D16] 求和与平均值
来源：http://rti.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qiy.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://luk.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://osx.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xrl.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eur.316326.xyz

Go:   // 手写循环累加
来源：http://glg.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kma.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://nve.chenlongwang.top

[D17] 最大值与最小值
来源：http://trq.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://cgb.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://vnb.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bca.yonumen.top

TS:   Math.max(...arr);
来源：http://gpt.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ntw.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://buf.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://fbd.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://nxk.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://lyp.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bnd.havefunace.top

PHP:  array_merge(...$nested);
来源：http://dma.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xjh.epnwcf.com

TS:   nested.flat();
来源：http://lro.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://apy.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://cxg.zhijiandao.cn

Ruby: nested.flatten
来源：http://vqs.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://usk.sjlbkw.cn

[D19] 按字段分组
来源：http://nvw.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hej.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ogm.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fxr.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jbd.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xlp.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://byv.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zuu.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vew.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://fsd.tianlin.xyz

Py:   Counter(arr)
来源：http://ugp.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://fxn.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cko.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjj.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kei.sweek.top

Go:   // 手写 map[T]int
来源：http://zaq.ybcxt.top

Ruby: arr.tally
来源：http://ysc.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sqj.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://hja.zhijiandao.cn

Py:   x in arr
来源：http://cxt.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://ijf.yongpay.top

JS:   arr.includes(x)
来源：http://oxe.bjfxy.top

TS:   arr.includes(x)
来源：http://rbo.dianchejie.cn

Java: list.contains(x)
来源：http://svi.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://kas.shuidangran.top

Ruby: arr.include?(x)
来源：http://qll.hcnkem.com

C#:   list.Contains(x)
来源：http://tzm.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://lsy.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oib.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ltj.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zug.svipenyu.cn

TS:   [...arr];
来源：http://ddm.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://wlt.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ibg.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://mng.uphjek.com

C#:   new List<int>(list);
来源：http://nys.andypj.xyz

[D23] reduce 累积计算
来源：http://txq.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nur.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jcu.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://whw.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqa.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oce.fktsv.cn

Go:   // 手写循环
来源：http://foh.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bhh.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://srv.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://lwz.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qzg.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vpk.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://evb.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://neg.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wks.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kvt.snrcjt.cn


<!-- 参考信息 -->