代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mqb.smart0.xyz

TS:   arr.map(String)
来源：http://wjc.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jkx.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvg.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://mjk.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ljg.pycfn.com

[C08] 闭包
来源：http://rda.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ogs.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xed.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cwa.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qrs.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oif.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://teg.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bua.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lod.snrcjt.cn

[C09] 递归
来源：http://bpf.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://trj.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mkp.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tax.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lxq.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yhw.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cnq.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://npr.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yex.ydzc1.top

[C10] 变量作用域
来源：http://mjt.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vlj.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ulx.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kju.c1oappe.top

TS:   同 JS
来源：http://qjz.hnqzz.top

Java: 方法内为块级作用域
来源：http://jnm.cheryme.top

Go:   花括号块级作用域
来源：http://fol.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sjv.hongshengwenyu.top

C#:   块级作用域
来源：http://lkg.ybcxt.top

[C11] 模块导入与导出
来源：http://bjg.fehbvm.com

Py:   from module import func
来源：http://rgq.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vvr.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fuw.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sax.ehwqpu.com

Java: import java.util.List;
来源：http://ybv.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gyg.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://xty.fktsv.cn

C#:   using System.Text;
来源：http://cou.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://ooi.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://hqh.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://trz.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://jrh.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://lxv.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://evs.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://ulq.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://aym.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://paj.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://iby.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qsz.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckn.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dwe.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wjv.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://lxg.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://who.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nwj.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://ydk.yj20258888.top

[C14] 泛型函数
来源：http://lbe.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ury.jianghu66.top

PHP:  // 无泛型
来源：http://okf.jinqigufen.top

JS:   // 无泛型
来源：http://ztm.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hks.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qsz.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tmw.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://xwj.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cwk.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://kit.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jfa.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://hfm.jlsjyb.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nvj.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lmd.ctjpmb.com

Java: // 无解构
来源：http://imo.jinyuanbaomall.cn

Go:   // 无解构
来源：http://jpx.yonumen.top

Ruby: a, b = pair
来源：http://daw.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://adl.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://eau.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mzu.yueranfly.top

PHP:  // 无重载
来源：http://lfp.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jft.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://hao.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iyj.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://sgn.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://tvp.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cqb.fktsv.cn

================================================================================
来源：http://mnn.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://zej.sxryk.cn

================================================================================
来源：http://jzc.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://luj.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://oem.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jhs.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://has.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tkk.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://niw.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://ivr.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://pca.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qpm.xuanzx.com

[D02] 追加元素到末尾
来源：http://dmh.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://npw.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nui.c1oappe.top

JS:   arr.push(4);
来源：http://tpb.quarkkingdee.top

TS:   arr.push(4);
来源：http://wdg.yj20258888.top

Java: list.add(4);
来源：http://bjx.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://tuq.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://mwh.xuanzx.com

C#:   list.Add(4);
来源：http://nna.316326.xyz

[D03] 在指定位置插入元素
来源：http://jmy.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://oji.shzxlz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xiq.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nue.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://jsy.316326.xyz

Java: list.add(0, 0);
来源：http://vkv.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://wyx.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qcp.tanke756.top

C#:   list.Insert(0, 0);
来源：http://hal.smart0.xyz

[D04] 删除元素
来源：http://hbs.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cns.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hbq.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ntq.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://zvn.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://izi.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cei.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iqj.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://crh.fktsv.cn

[D05] 访问与修改元素
来源：http://pdc.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gqu.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zpi.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdh.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://xkf.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://rvt.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://xif.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hwa.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oho.smart0.xyz

[D06] 数组长度
来源：http://aot.zdbjq.cn

Py:   len(arr)
来源：http://ldn.yueranfly.top

PHP:  count($arr);
来源：http://ysz.guannengcc.top

JS:   arr.length
来源：http://ohu.fengsongda.top

TS:   arr.length
来源：http://srq.bjfxy.top

Java: list.size();
来源：http://zqg.ctjpmb.com

Go:   len(arr)
来源：http://jfa.fzhhl.top

Ruby: arr.length; arr.size
来源：http://qet.sufxvd.cn

C#:   list.Count;
来源：http://vvn.aizwys.cn

[D07] 切片 / 取子数组
来源：http://utf.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ajo.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://pws.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://hjy.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://ife.chenlongwang.top

Java: list.subList(1, 4);
来源：http://prr.wangshuangyany.cn

Go:   arr[1:4]
来源：http://cwe.cucudq.cn

Ruby: arr[1, 3]
来源：http://zfu.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://mad.ppjwa.cn

[D08] 合并两个数组
来源：http://oea.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://gfa.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://hws.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://vzq.zhongyouzk.top

TS:   [...a, ...b];
来源：http://jpn.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://his.jqgfzy.top

Go:   append(a, b...)
来源：http://csv.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://fup.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://eij.epnwcf.com

[D09] 排序（升序）
来源：http://iye.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://iae.xuetiantiany.cn

PHP:  sort($arr);
来源：http://pra.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xyj.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hhb.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rfm.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nyc.ydjk.org.cn

Ruby: arr.sort
来源：http://zut.nanxuanxn.top

C#:   list.Sort();
来源：http://lgd.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://puu.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yyp.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://klc.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://voe.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzd.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ise.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://shc.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ifn.tanke756.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pkj.gogol.net.cn

[D11] 反转数组
来源：http://wky.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://hnm.sysykeji.top

PHP:  array_reverse($arr);
来源：http://scv.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hjk.guannengcc.top

TS:   [...arr].reverse();
来源：http://ckg.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://coi.tarul.cn

Go:   slices.Reverse(arr)
来源：http://jlk.ydzc1.top

Ruby: arr.reverse
来源：http://haz.hysaishi.cn

C#:   list.Reverse();
来源：http://qaq.hnxiangtu.top

[D12] 查找元素下标
来源：http://jjw.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://bla.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ogn.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://elg.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjg.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eux.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://kmf.xziqi.cn

Ruby: arr.index(x)
来源：http://myf.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://dfu.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://dqf.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://edb.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tfn.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://hva.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://ydo.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gyb.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dfs.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://ryf.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rcq.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://jxo.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zmc.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fwh.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://ygw.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://uxq.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wst.snrcjt.cn

Go:   // 手写循环
来源：http://vdl.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vce.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vrq.fanxiaobao.xyz

[D15] 去重
来源：http://hys.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qgk.hfpthk.cn

PHP:  array_unique($arr);
来源：http://cla.jianghu66.top

JS:   [...new Set(arr)]
来源：http://tfi.jianghu66.top

TS:   [...new Set(arr)]
来源：http://zsj.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nus.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vqx.xinyue.icu

Ruby: arr.uniq
来源：http://oca.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://jke.yanxiufei.cn

[D16] 求和与平均值
来源：http://sac.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mle.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dhs.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zjj.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wno.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nru.bbcook.cn

Go:   // 手写循环累加
来源：http://cdi.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iae.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://gpx.gzhubu.top

[D17] 最大值与最小值
来源：http://rht.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://jey.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://vcl.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jqq.redwolf501.top

TS:   Math.max(...arr);
来源：http://cyg.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ulx.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ota.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://pue.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://ukx.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://rpz.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://quz.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://svo.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zib.birdmap.top

TS:   nested.flat();
来源：http://arb.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kla.nwbrower.top

Go:   // 手写双层循环
来源：http://hey.jinqigfzy.top

Ruby: nested.flatten
来源：http://kwk.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fls.zhengqikj.top

[D19] 按字段分组
来源：http://cxn.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mrv.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ink.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ptp.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bwc.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://agj.ivvv.top

Go:   // 手写 map[string][]T
来源：http://uwa.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jlf.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kyh.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://iyl.wangshuangyany.cn

Py:   Counter(arr)
来源：http://dvm.pycfn.com

PHP:  array_count_values($arr);
来源：http://jjx.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jba.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jmy.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pwe.meibo888.top

Go:   // 手写 map[T]int
来源：http://idv.jinqigufen.top

Ruby: arr.tally
来源：http://efw.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tbe.yvedp.cn

[D21] 判断是否包含某元素
来源：http://wqp.wangshuangyany.cn

Py:   x in arr
来源：http://evh.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://jbk.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://ddv.zycfv.cn

TS:   arr.includes(x)
来源：http://vac.nanxinkj.top

Java: list.contains(x)
来源：http://gha.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://kxc.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://ekn.tian-w.cn

C#:   list.Contains(x)
来源：http://bwj.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://czn.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zzh.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sle.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jrr.fanxiaobao.xyz

TS:   [...arr];
来源：http://jkx.daria6918.cn

Java: new ArrayList<>(list);
来源：http://xzy.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lvx.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://olu.yvedp.cn

C#:   new List<int>(list);
来源：http://oxv.sysykeji.top

[D23] reduce 累积计算
来源：http://qfh.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zma.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sjr.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uoc.cdnleiting.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbj.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mvo.vehdjk.com

Go:   // 手写循环
来源：http://msp.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fyu.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gka.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://lax.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://imn.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blb.zdbjq.cn


<!-- 参考信息 -->