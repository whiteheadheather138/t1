代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://znz.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sis.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qxv.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qyx.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pfm.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bzp.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wpe.sxryk.cn

[C09] 递归
来源：http://zhe.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ymp.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://elu.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tpe.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eqs.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sxe.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://imh.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hqk.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dke.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://gzw.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ynm.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://str.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ejl.nwbrower.top

TS:   同 JS
来源：http://tmf.epnwcf.com

Java: 方法内为块级作用域
来源：http://llm.zdbjq.cn

Go:   花括号块级作用域
来源：http://daj.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zyy.fengsongda.top

C#:   块级作用域
来源：http://upt.vqdsnc.cn

[C11] 模块导入与导出
来源：http://srd.0kj1m.cn

Py:   from module import func
来源：http://cda.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ord.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ukc.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jaa.ydzc1.top

Java: import java.util.List;
来源：http://dtc.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qon.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://uek.wangshuangyany.cn

C#:   using System.Text;
来源：http://wai.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://mty.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://ckt.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://xdl.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://ief.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://ipt.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://egt.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://ddr.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://lbf.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dut.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://pzy.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nop.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxg.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vtn.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kbu.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://udw.ydzc1.top

Go:   func add(a, b int) int
来源：http://sku.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dtc.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://xya.meibo888.top

[C14] 泛型函数
来源：http://cib.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uuh.zhijiandao.cn

PHP:  // 无泛型
来源：http://cjv.iojbl.cn

JS:   // 无泛型
来源：http://ofx.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vyh.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fbs.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yur.quarkkingdee.top

Ruby: # 无泛型
来源：http://lfx.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wqy.uphjek.com

[C15] 解构 / 展开参数
来源：http://exi.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qdj.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://crd.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://czk.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rmw.daxiang520.top

Java: // 无解构
来源：http://pvj.zhoulong.xyz

Go:   // 无解构
来源：http://vax.jqgufenzy.top

Ruby: a, b = pair
来源：http://jhl.iojbl.cn

C#:   var (a, b) = pair;
来源：http://iov.cashguo.top

[C16] 函数 / 方法重载
来源：http://mgb.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sjq.52xcode.cn

PHP:  // 无重载
来源：http://vbz.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dfk.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://czv.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kfz.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://spg.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://fsa.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wav.fktsv.cn

================================================================================
来源：http://toi.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://sue.xuanzx.com

================================================================================
来源：http://cpp.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://pbc.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qly.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://amh.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkf.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jdq.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fxi.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://wle.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://tjv.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ras.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://ftm.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tcg.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zts.ctjpmb.com

JS:   arr.push(4);
来源：http://bli.fehbvm.com

TS:   arr.push(4);
来源：http://psi.ctjpmb.com

Java: list.add(4);
来源：http://bnb.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://dhf.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://nis.tanke756.top

C#:   list.Add(4);
来源：http://urq.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://oor.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://ajk.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lrt.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://edi.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://fau.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://ggl.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://hrc.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vus.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://dlf.tarul.cn

[D04] 删除元素
来源：http://cdy.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://odj.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qcu.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://flu.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://tiy.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pxo.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tin.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cdn.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tfe.tian-w.cn

[D05] 访问与修改元素
来源：http://pxk.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ogg.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cic.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bfj.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://pfi.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://jxh.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://kvc.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vyl.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bdk.hnxiangtu.top

[D06] 数组长度
来源：http://egf.0kj1m.cn

Py:   len(arr)
来源：http://fja.mhx1999.top

PHP:  count($arr);
来源：http://rje.guowangkeji.top

JS:   arr.length
来源：http://mgv.nanxuanxn.top

TS:   arr.length
来源：http://bpi.snrcjt.cn

Java: list.size();
来源：http://wbt.dashuyun.cn

Go:   len(arr)
来源：http://rgy.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://oxl.meibo888.top

C#:   list.Count;
来源：http://ywh.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://nlq.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ysi.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://fpv.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://kge.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://byy.hysaishi.cn

Java: list.subList(1, 4);
来源：http://gss.yvedp.cn

Go:   arr[1:4]
来源：http://inw.guannengcc.top

Ruby: arr[1, 3]
来源：http://ids.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://xgj.52xcode.cn

[D08] 合并两个数组
来源：http://wxy.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://lpx.yongpay.top

PHP:  array_merge($a, $b);
来源：http://qto.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://abr.fengsongda.top

TS:   [...a, ...b];
来源：http://fgq.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eqj.zdqjudy.top

Go:   append(a, b...)
来源：http://wpt.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://tbh.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://tgb.shuidangran.top

[D09] 排序（升序）
来源：http://vjs.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://eag.chenjidiqi.icu

PHP:  sort($arr);
来源：http://mte.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://shj.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lgo.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cvc.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lyt.mhx1999.top

Ruby: arr.sort
来源：http://alb.yongpay.top

C#:   list.Sort();
来源：http://gms.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tor.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tbu.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xpz.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gyg.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iuu.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blg.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ihu.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dja.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rhy.yvedp.cn

[D11] 反转数组
来源：http://ptf.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://fqr.fzhhl.top

PHP:  array_reverse($arr);
来源：http://qte.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://psp.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://dyo.c1oappe.top

Java: Collections.reverse(list);
来源：http://kkp.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://gpr.cashguo.top

Ruby: arr.reverse
来源：http://kvd.sweek.top

C#:   list.Reverse();
来源：http://xap.yangfankeji.com

[D12] 查找元素下标
来源：http://yah.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://pfm.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ycs.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvi.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cui.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oiq.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://rnt.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://wee.tian-w.cn

C#:   list.IndexOf(x);
来源：http://flx.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://fnz.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ljv.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wyi.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://acy.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://yst.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xli.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://urr.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://tci.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yae.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://lnj.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://koh.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ijo.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://nxf.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://lfk.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fxg.xuetiantiany.cn

Go:   // 手写循环
来源：http://aoy.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://saq.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gxq.cqqwz.cn

[D15] 去重
来源：http://eru.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vha.gogol.net.cn

PHP:  array_unique($arr);
来源：http://tpw.gogol.net.cn

JS:   [...new Set(arr)]
来源：http://siy.meibo888.top

TS:   [...new Set(arr)]
来源：http://vyg.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://syj.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yaa.xylfe.cn

Ruby: arr.uniq
来源：http://xzi.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://gds.shangyingyoupin.top

[D16] 求和与平均值
来源：http://lxk.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gjt.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hll.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rrz.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kao.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bdj.jlsjyb.cn

Go:   // 手写循环累加
来源：http://sps.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://amy.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://wzr.jinqigufen.top

[D17] 最大值与最小值
来源：http://spl.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://glt.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://zao.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://udf.zhengqikj.top

TS:   Math.max(...arr);
来源：http://yae.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uhp.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yzv.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://hqo.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://tpj.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://ivq.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vgo.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://xbb.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dry.bbcook.cn

TS:   nested.flat();
来源：http://kxc.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wbc.tarul.cn

Go:   // 手写双层循环
来源：http://lua.haohaochexian.top

Ruby: nested.flatten
来源：http://jyb.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yjt.dashuyun.cn

[D19] 按字段分组
来源：http://jpn.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yty.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yvp.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fzr.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cgq.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ubw.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://emz.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cbf.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wml.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://xoq.yongpay.top

Py:   Counter(arr)
来源：http://aek.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://bvy.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://orj.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eju.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wme.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://pfw.zhongyouzk.top

Ruby: arr.tally
来源：http://nqs.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lmd.jianghu66.top

[D21] 判断是否包含某元素
来源：http://yel.fehbvm.com

Py:   x in arr
来源：http://pln.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://bee.tian-w.cn

JS:   arr.includes(x)
来源：http://mam.fehbvm.com

TS:   arr.includes(x)
来源：http://jjz.chenjidiqi.icu

Java: list.contains(x)
来源：http://lkt.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://sew.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://dkv.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://dpg.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://fvb.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yib.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gpj.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lyl.haohaochexian.top

TS:   [...arr];
来源：http://rlt.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://fbc.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://yxv.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://ili.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://lmm.yanxiufei.cn

[D23] reduce 累积计算
来源：http://qsq.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ozm.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ouk.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://glo.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahj.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oyl.hfpthk.cn

Go:   // 手写循环
来源：http://zlp.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xnr.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bfs.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://uka.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pmf.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pjf.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ruv.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tit.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qyp.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lcu.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jyd.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dvq.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://vsp.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ryl.wangshuangyany.cn


<!-- 参考信息 -->