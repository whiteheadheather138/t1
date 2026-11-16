代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tbe.ydjk.org.cn

TS:   arr.map(String)
来源：http://ghj.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://exu.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rlc.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://tgb.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wjc.cashguo.top

[C08] 闭包
来源：http://fcz.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hvs.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xpt.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ggz.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cwg.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ynw.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bpv.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iiu.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dae.hesvh.cn

[C09] 递归
来源：http://wae.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uzh.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kyd.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://faq.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xjx.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://trx.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nxc.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bpv.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://guk.fanxiaobao.xyz

[C10] 变量作用域
来源：http://fla.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mjw.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cii.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zmg.aibaodan.cn

TS:   同 JS
来源：http://gwn.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://die.yueranfly.top

Go:   花括号块级作用域
来源：http://wjx.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ngf.redwolf501.top

C#:   块级作用域
来源：http://enk.hfpthk.cn

[C11] 模块导入与导出
来源：http://yir.hcnkem.com

Py:   from module import func
来源：http://qgv.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vrc.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jwr.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfw.dianchejie.cn

Java: import java.util.List;
来源：http://wlc.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://adz.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://jne.kuanghao11.cn

C#:   using System.Text;
来源：http://uis.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://dci.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://bkf.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://lrj.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://gvw.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://hsa.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wwa.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://ecf.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://rgw.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ccp.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://rvn.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lqp.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxs.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qyd.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pgd.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ebc.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://tpl.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vnm.haohaochexian.top

C#:   int Add(int a, int b) => a + b;
来源：http://ksa.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://lfx.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://czm.vehdjk.com

PHP:  // 无泛型
来源：http://ziw.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://dxb.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fgd.yueranfly.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dpk.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://shc.zhengqikj.top

Ruby: # 无泛型
来源：http://rau.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mex.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://wdi.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hvr.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://jgz.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azq.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rdk.hfpthk.cn

Java: // 无解构
来源：http://zzl.xuetiantiany.cn

Go:   // 无解构
来源：http://czt.shzxlz.cn

Ruby: a, b = pair
来源：http://oid.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://ezs.yuxming.cn

[C16] 函数 / 方法重载
来源：http://zlf.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qty.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://hzt.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hdo.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://wtw.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uyl.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://xfm.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://fsn.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://nqk.daxiang520.top

================================================================================
来源：http://qit.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://knb.uphjek.com

================================================================================
来源：http://wfb.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://yiq.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pvj.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://diy.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fmy.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://adm.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yei.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://rqt.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://siw.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eug.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://awr.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sdc.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qij.zhijiandao.cn

JS:   arr.push(4);
来源：http://mmy.pycfn.com

TS:   arr.push(4);
来源：http://aoa.vehdjk.com

Java: list.add(4);
来源：http://rtg.birdmap.top

Go:   arr = append(arr, 4)
来源：http://tnq.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://ygd.jianghu66.top

C#:   list.Add(4);
来源：http://vxd.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://csg.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://uyu.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vao.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qxy.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://ezu.gogol.net.cn

Java: list.add(0, 0);
来源：http://jhg.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aif.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vsy.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://vag.zhaomingkeji.xyz

[D04] 删除元素
来源：http://fqs.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zfo.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jqk.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oep.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://znh.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lwm.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gnt.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mjg.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xgu.zdqjudy.top

[D05] 访问与修改元素
来源：http://oqs.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zwh.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xdu.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aho.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://vhw.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://bvn.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://trt.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vzk.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uzz.pycfn.com

[D06] 数组长度
来源：http://ghb.ehwqpu.com

Py:   len(arr)
来源：http://aqv.xuetiantiany.cn

PHP:  count($arr);
来源：http://yha.xziqi.cn

JS:   arr.length
来源：http://cdd.jinqigufen.top

TS:   arr.length
来源：http://hnv.meibo888.top

Java: list.size();
来源：http://ary.yj202588.top

Go:   len(arr)
来源：http://eoz.cashguo.top

Ruby: arr.length; arr.size
来源：http://wcg.cashguo.top

C#:   list.Count;
来源：http://ejc.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://mpq.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qbo.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://ocm.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://cvo.birdmap.top

TS:   arr.slice(1, 4);
来源：http://ujt.hcnkem.com

Java: list.subList(1, 4);
来源：http://wme.ppjwa.cn

Go:   arr[1:4]
来源：http://gpg.wangdashe.top

Ruby: arr[1, 3]
来源：http://dnx.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://fgp.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://dza.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://dqw.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://fzh.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jhg.haohaochexian.top

TS:   [...a, ...b];
来源：http://dzs.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jpd.fktsv.cn

Go:   append(a, b...)
来源：http://fhs.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://xmd.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://zvz.tarul.cn

[D09] 排序（升序）
来源：http://bjo.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://sty.zhengqikj.top

PHP:  sort($arr);
来源：http://kbd.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uui.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ysk.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jdr.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wly.nwbrower.top

Ruby: arr.sort
来源：http://ztq.c1oappe.top

C#:   list.Sort();
来源：http://yzp.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yjw.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ezm.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tft.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jli.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yww.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://otl.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ujo.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://whw.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mks.fengsongda.top

[D11] 反转数组
来源：http://igx.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://cgl.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://myz.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nyk.haohaochexian.top

TS:   [...arr].reverse();
来源：http://fqo.cqqwz.cn

Java: Collections.reverse(list);
来源：http://dxr.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://upp.9152youxi.cn

Ruby: arr.reverse
来源：http://zms.xziqi.cn

C#:   list.Reverse();
来源：http://lvt.fengsongda.top

[D12] 查找元素下标
来源：http://pcc.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://eir.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hpn.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrc.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mld.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://naw.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://xgh.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://dgn.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://lzt.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://oac.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ugr.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uax.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://scw.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://tdf.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://erh.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://myh.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tyk.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zsw.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://jmb.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tpm.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gsa.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://rfx.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://ddc.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ifz.hysaishi.cn

Go:   // 手写循环
来源：http://pko.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jps.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hqy.zdqjudy.top

[D15] 去重
来源：http://scu.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zae.cdnleiting.top

PHP:  array_unique($arr);
来源：http://odj.sysykeji.top

JS:   [...new Set(arr)]
来源：http://mru.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://wzk.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zjg.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://uth.xylfe.cn

Ruby: arr.uniq
来源：http://zui.cashguo.top

C#:   list.Distinct().ToList()
来源：http://udo.birdmap.top

[D16] 求和与平均值
来源：http://znu.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zrm.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyv.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://api.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyl.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bha.meibo888.top

Go:   // 手写循环累加
来源：http://mwl.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ngy.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://hpx.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://ikr.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://cas.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://owz.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ycf.sweek.top

TS:   Math.max(...arr);
来源：http://xee.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://uaw.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nuj.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://qho.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://jxg.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://rzr.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dis.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://sws.ivvv.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yxd.meibo888.top

TS:   nested.flat();
来源：http://dal.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://onk.shuidangran.top

Go:   // 手写双层循环
来源：http://rvs.snrcjt.cn

Ruby: nested.flatten
来源：http://jek.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pja.gaohongyu789.top

[D19] 按字段分组
来源：http://xfv.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://avz.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://htr.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sva.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lpu.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uto.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://knw.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xof.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wwq.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://cjr.zhoulong.xyz

Py:   Counter(arr)
来源：http://lmm.bbcook.cn

PHP:  array_count_values($arr);
来源：http://ogj.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ssj.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tps.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dvv.hesvh.cn

Go:   // 手写 map[T]int
来源：http://sil.ybcxt.top

Ruby: arr.tally
来源：http://xuq.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://izq.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://bcf.bjfxy.top

Py:   x in arr
来源：http://fwz.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://ouc.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://nvp.xylfe.cn

TS:   arr.includes(x)
来源：http://hzu.pycfn.com

Java: list.contains(x)
来源：http://whh.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://nrd.shuidangran.top

Ruby: arr.include?(x)
来源：http://pjs.redwolf501.top

C#:   list.Contains(x)
来源：http://ftu.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://kql.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yhu.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qjv.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eep.havefunace.top

TS:   [...arr];
来源：http://ykp.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://dut.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dat.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://ekp.fengsongda.top

C#:   new List<int>(list);
来源：http://ikw.zhixingplan.top

[D23] reduce 累积计算
来源：http://zwb.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ajy.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hdu.xylfe.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpt.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omz.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://imh.yj202588.top

Go:   // 手写循环
来源：http://zbk.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gas.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pxf.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://tie.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jyt.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://loy.smart0.xyz


<!-- 参考信息 -->