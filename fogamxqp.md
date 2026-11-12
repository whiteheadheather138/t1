代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://loh.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://myr.zhoulong.xyz

[C08] 闭包
来源：http://fxm.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kcr.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ecs.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zas.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ytc.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ima.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://knl.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ahu.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yyo.zhoulong.xyz

[C09] 递归
来源：http://zgh.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://idk.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wle.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mab.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zcg.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qzg.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ord.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ogv.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcu.gzhubu.top

[C10] 变量作用域
来源：http://ljs.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zni.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bfr.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nbx.xinyue.icu

TS:   同 JS
来源：http://ssb.gotoacloud.top

Java: 方法内为块级作用域
来源：http://wgx.316326.xyz

Go:   花括号块级作用域
来源：http://aeh.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ibd.tian-w.cn

C#:   块级作用域
来源：http://opf.chenzaomai.com

[C11] 模块导入与导出
来源：http://qcu.jinqigfzy.top

Py:   from module import func
来源：http://zcd.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hyz.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zbo.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wrg.vehdjk.com

Java: import java.util.List;
来源：http://cyj.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://svq.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://cjw.sweek.top

C#:   using System.Text;
来源：http://oou.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://jpi.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://apl.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://mli.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://gjk.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://teo.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dzy.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://weg.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://rfd.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lre.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://edr.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gji.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxx.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qsn.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bnm.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://juc.bjfxy.top

Go:   func add(a, b int) int
来源：http://dcy.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xrk.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ssq.jinqigufen.top

[C14] 泛型函数
来源：http://xcn.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rwv.zycfv.cn

PHP:  // 无泛型
来源：http://isp.tanke756.top

JS:   // 无泛型
来源：http://qyy.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eip.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cap.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bgj.bjfxy.top

Ruby: # 无泛型
来源：http://mtt.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://beq.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://khz.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xrl.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://rbn.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tst.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vcg.fktsv.cn

Java: // 无解构
来源：http://kzs.cdnleiting.top

Go:   // 无解构
来源：http://ipx.yueranfly.top

Ruby: a, b = pair
来源：http://lrm.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://gzg.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://pzj.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bgk.aibaodan.cn

PHP:  // 无重载
来源：http://wkp.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://lpg.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://tlw.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pco.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://tyh.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://lfp.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pcy.fktsv.cn

================================================================================
来源：http://orh.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://ltn.epnwcf.com

================================================================================
来源：http://uxd.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://wvt.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://klu.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nbi.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xjy.0kj1m.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qww.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://abc.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://gps.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://cwx.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pcz.gzhubu.top

[D02] 追加元素到末尾
来源：http://bme.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bbw.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uea.jianghu66.top

JS:   arr.push(4);
来源：http://boj.shangyingyoupin.top

TS:   arr.push(4);
来源：http://nkx.xinyue.icu

Java: list.add(4);
来源：http://kus.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://dwt.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://fna.cucudq.cn

C#:   list.Add(4);
来源：http://qqj.tian-w.cn

[D03] 在指定位置插入元素
来源：http://uuk.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://jbd.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uxs.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://clk.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://syv.mhx1999.top

Java: list.add(0, 0);
来源：http://hee.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nwo.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nlc.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://wtb.quarkkingdee.top

[D04] 删除元素
来源：http://vxb.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uhq.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cos.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://puf.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://tul.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wsl.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sks.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qlx.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gnz.zhengqikj.top

[D05] 访问与修改元素
来源：http://thy.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qtl.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hoo.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uwc.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://yna.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://sox.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://xwo.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://huh.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xbg.zycfv.cn

[D06] 数组长度
来源：http://rfk.jinqigufen.top

Py:   len(arr)
来源：http://ofi.yj202588.top

PHP:  count($arr);
来源：http://lec.cheryme.top

JS:   arr.length
来源：http://ded.zhijiandao.cn

TS:   arr.length
来源：http://wes.ppjwa.cn

Java: list.size();
来源：http://lad.dianchejie.cn

Go:   len(arr)
来源：http://job.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://zuv.hnxiangtu.top

C#:   list.Count;
来源：http://old.yueranfly.top

[D07] 切片 / 取子数组
来源：http://mmv.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghk.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ycw.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://sdp.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://eej.epnwcf.com

Java: list.subList(1, 4);
来源：http://ikt.sweek.top

Go:   arr[1:4]
来源：http://hdn.gogol.net.cn

Ruby: arr[1, 3]
来源：http://tdu.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://box.hysaishi.cn

[D08] 合并两个数组
来源：http://vly.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://bnj.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://afg.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://glk.zdqjudy.top

TS:   [...a, ...b];
来源：http://bbt.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eht.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://pxf.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://vzb.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://tmu.andypj.xyz

[D09] 排序（升序）
来源：http://unw.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://tdv.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://epf.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ede.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://wxv.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hle.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yvb.andypj.xyz

Ruby: arr.sort
来源：http://urj.daxiang520.top

C#:   list.Sort();
来源：http://zoa.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bfw.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pny.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jxz.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymu.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lqk.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bpl.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bwh.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lfu.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jvs.gzhubu.top

[D11] 反转数组
来源：http://nab.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://eag.ivvv.top

PHP:  array_reverse($arr);
来源：http://qdf.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://njm.hfpthk.cn

TS:   [...arr].reverse();
来源：http://tyn.shuidangran.top

Java: Collections.reverse(list);
来源：http://dmv.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://teo.fehbvm.com

Ruby: arr.reverse
来源：http://ryc.hesvh.cn

C#:   list.Reverse();
来源：http://oxf.sysykeji.top

[D12] 查找元素下标
来源：http://vyj.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://oqg.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jlz.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chh.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kpn.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xzc.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://aeu.jinqigufen.top

Ruby: arr.index(x)
来源：http://isz.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://fhl.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://pel.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bkl.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://csf.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://tfp.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://uvw.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qyg.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fzk.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://szi.sxryk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ebf.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://qsp.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zye.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ttx.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://nyc.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://hkw.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tzj.shzxlz.cn

Go:   // 手写循环
来源：http://tvh.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wyh.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://afq.shuidangran.top

[D15] 去重
来源：http://tdf.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yzb.9152youxi.cn

PHP:  array_unique($arr);
来源：http://isx.uphjek.com

JS:   [...new Set(arr)]
来源：http://kam.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://qkc.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lyn.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://jvz.redwolf501.top

Ruby: arr.uniq
来源：http://kug.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://iid.zhongyouzk.top

[D16] 求和与平均值
来源：http://qoc.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gdw.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aos.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gig.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xdg.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogs.yfazqb.com

Go:   // 手写循环累加
来源：http://wqe.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gmp.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://jco.vehdjk.com

[D17] 最大值与最小值
来源：http://rtd.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://tma.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://uvb.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://utk.hesvh.cn

TS:   Math.max(...arr);
来源：http://ddq.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bwo.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hwb.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://oeo.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://lcc.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://wie.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vdn.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://ric.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sdx.guowangkeji.top

TS:   nested.flat();
来源：http://ovd.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dve.ydjk.org.cn

Go:   // 手写双层循环
来源：http://djq.cashguo.top

Ruby: nested.flatten
来源：http://yoe.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dnl.shzxlz.cn

[D19] 按字段分组
来源：http://dcj.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gkj.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bux.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xkj.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ono.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hdh.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://wrt.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://wyr.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eum.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://vod.nanxinkj.top

Py:   Counter(arr)
来源：http://mhz.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://voj.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qhh.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rnt.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mal.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://ysy.havefunace.top

Ruby: arr.tally
来源：http://obk.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nva.meibo888.top

[D21] 判断是否包含某元素
来源：http://wtz.zhengqikj.top

Py:   x in arr
来源：http://gwi.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://xsw.shzxlz.cn

JS:   arr.includes(x)
来源：http://oke.zhixingplan.top

TS:   arr.includes(x)
来源：http://pqf.zhoulong.xyz

Java: list.contains(x)
来源：http://sfu.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://anv.ybcxt.top

Ruby: arr.include?(x)
来源：http://mzb.tianlin.xyz

C#:   list.Contains(x)
来源：http://eej.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://mik.gaohongyu789.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://piz.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zkw.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mtk.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://hhp.fzhhl.top

Java: new ArrayList<>(list);
来源：http://bib.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rce.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://pbz.pycfn.com

C#:   new List<int>(list);
来源：http://svs.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://gtg.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dce.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lnx.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ukb.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmb.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nyj.ivvv.top

Go:   // 手写循环
来源：http://dzs.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fys.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mlu.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://fxx.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yjm.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://paq.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bnq.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qus.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xjz.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lpj.shanyushiyangkeji.top


<!-- 参考信息 -->