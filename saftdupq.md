代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://nzd.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://lcn.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eha.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://dwu.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rxb.andypj.xyz

TS:   arr.map(String)
来源：http://ncd.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hid.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vlp.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://uvl.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://icb.jqgfzy.top

[C08] 闭包
来源：http://gdi.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nhf.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mkf.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fbj.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fmg.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eoe.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dnb.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wsd.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ayu.ehwqpu.com

[C09] 递归
来源：http://eut.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://des.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hmh.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ynb.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kmw.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yqi.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gam.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://elj.haohaochexian.top

[C10] 变量作用域
来源：http://ejq.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eco.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://amd.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aep.zhixingplan.top

TS:   同 JS
来源：http://iel.shzxlz.cn

Java: 方法内为块级作用域
来源：http://wwn.guannengcc.top

Go:   花括号块级作用域
来源：http://kis.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uwk.meibo888.top

C#:   块级作用域
来源：http://uea.yfazqb.com

[C11] 模块导入与导出
来源：http://pgs.haohaochexian.top

Py:   from module import func
来源：http://qte.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xyy.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fpx.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tyj.hywenlv.cn

Java: import java.util.List;
来源：http://jgp.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://buj.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://mpd.jianghu66.top

C#:   using System.Text;
来源：http://ote.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://lkz.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://nsy.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://kud.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://irv.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://drz.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bnw.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://pxg.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://kyn.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ocp.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://gso.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jib.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vns.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tgt.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://day.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://izp.svipenyu.cn

Go:   func add(a, b int) int
来源：http://bfm.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kww.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://coq.hnxiangtu.top

[C14] 泛型函数
来源：http://igx.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mrz.birdmap.top

PHP:  // 无泛型
来源：http://hda.0kj1m.cn

JS:   // 无泛型
来源：http://eex.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hsm.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ocb.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vch.hcnkem.com

Ruby: # 无泛型
来源：http://ids.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ljp.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://tdy.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hcw.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://yvh.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tco.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sni.yuxming.cn

Java: // 无解构
来源：http://yjh.uphjek.com

Go:   // 无解构
来源：http://qli.9152youxi.cn

Ruby: a, b = pair
来源：http://cme.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://bth.hcnkem.com

[C16] 函数 / 方法重载
来源：http://cok.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tbi.fktsv.cn

PHP:  // 无重载
来源：http://pzs.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://thr.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://vxi.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bqy.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://hyv.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://vcd.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://knl.redwolf501.top

================================================================================
来源：http://imh.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://hmk.hesvh.cn

================================================================================
来源：http://nhu.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://wvc.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://loo.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rhd.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kbd.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://hzo.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kad.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://xsc.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://nzl.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ewd.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://qgw.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uzj.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hgx.tianlin.xyz

JS:   arr.push(4);
来源：http://ylh.yuanzhike.top

TS:   arr.push(4);
来源：http://cgf.jianghu66.top

Java: list.add(4);
来源：http://zkx.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://ahr.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://ubu.yuanzhike.top

C#:   list.Add(4);
来源：http://ifh.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://ohf.meibo888.top

Py:   arr.insert(0, 0)
来源：http://fqf.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://atr.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wrs.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://jwx.dashuyun.cn

Java: list.add(0, 0);
来源：http://byk.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://job.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sxw.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://jbv.bbcook.cn

[D04] 删除元素
来源：http://aym.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vfd.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tdu.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mms.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://ydy.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rfa.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://czo.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gwx.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dio.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://fct.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kls.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gtj.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wdz.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://iea.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://sia.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://dvs.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fzc.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xyu.yanxiufei.cn

[D06] 数组长度
来源：http://vmx.hfpthk.cn

Py:   len(arr)
来源：http://lbo.xylfe.cn

PHP:  count($arr);
来源：http://gav.zhongyouzk.top

JS:   arr.length
来源：http://ayi.jinqigfzy.top

TS:   arr.length
来源：http://viw.ydzc1.top

Java: list.size();
来源：http://rrf.vqdsnc.cn

Go:   len(arr)
来源：http://bsp.hcnkem.com

Ruby: arr.length; arr.size
来源：http://wjj.cdnleiting.top

C#:   list.Count;
来源：http://ecj.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://yxm.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ahb.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://hni.cashguo.top

JS:   arr.slice(1, 4);
来源：http://mui.uphjek.com

TS:   arr.slice(1, 4);
来源：http://wet.xinyue.icu

Java: list.subList(1, 4);
来源：http://hou.jqgfzy.top

Go:   arr[1:4]
来源：http://ujs.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://ppu.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://thr.ivvv.top

[D08] 合并两个数组
来源：http://yyb.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://gir.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://pqo.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dgz.havefunace.top

TS:   [...a, ...b];
来源：http://tjb.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hgx.zhengqikj.top

Go:   append(a, b...)
来源：http://nku.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://cal.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://bco.tian-w.cn

[D09] 排序（升序）
来源：http://oil.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://rgb.yonumen.top

PHP:  sort($arr);
来源：http://kiz.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ivj.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sld.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ppf.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qmd.yongpay.top

Ruby: arr.sort
来源：http://ccr.fengsongda.top

C#:   list.Sort();
来源：http://wpt.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xew.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uvu.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xeu.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vyn.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://syx.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vuf.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://snd.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lkt.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xcf.gotoacloud.top

[D11] 反转数组
来源：http://qno.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://gva.birdmap.top

PHP:  array_reverse($arr);
来源：http://vxo.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nax.ybcxt.top

TS:   [...arr].reverse();
来源：http://gni.ppjwa.cn

Java: Collections.reverse(list);
来源：http://lta.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://bzj.ctjpmb.com

Ruby: arr.reverse
来源：http://hae.9152youxi.cn

C#:   list.Reverse();
来源：http://mbb.jinqigufen.top

[D12] 查找元素下标
来源：http://aee.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://tjv.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qir.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kjp.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://joi.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eit.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://meq.yuanzhike.top

Ruby: arr.index(x)
来源：http://xir.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://enf.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://mty.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pux.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ych.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://tuw.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://svk.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jna.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mif.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cfb.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nhk.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://enp.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yhw.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qez.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://lvl.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://iqr.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bkg.guowangkeji.top

Go:   // 手写循环
来源：http://ceg.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://aei.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://afs.quarkkingdee.top

[D15] 去重
来源：http://kpa.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wrc.cashguo.top

PHP:  array_unique($arr);
来源：http://tha.tian-w.cn

JS:   [...new Set(arr)]
来源：http://jns.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://rwl.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uvj.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tfl.havefunace.top

Ruby: arr.uniq
来源：http://rcj.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://sit.guannengcc.top

[D16] 求和与平均值
来源：http://bqa.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rqj.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pcg.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oop.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rmy.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wcd.epnwcf.com

Go:   // 手写循环累加
来源：http://vyo.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wbd.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://vla.nanxuanxn.top

[D17] 最大值与最小值
来源：http://mhp.yongpay.top

Py:   max(arr);  min(arr)
来源：http://gbv.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://gjq.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pxr.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://hnw.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ozl.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://saj.birdmap.top

Ruby: arr.max;  arr.min
来源：http://igj.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://prn.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://dfq.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yqt.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://gcr.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ncs.hammf.cn

TS:   nested.flat();
来源：http://mlu.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pex.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://tyj.ybcxt.top

Ruby: nested.flatten
来源：http://dkb.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vib.nanxuanxn.top

[D19] 按字段分组
来源：http://hmz.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sls.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lyn.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tky.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mtk.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rdx.birdmap.top

Go:   // 手写 map[string][]T
来源：http://izg.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eel.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gan.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://vut.sweek.top

Py:   Counter(arr)
来源：http://tdq.andypj.xyz

PHP:  array_count_values($arr);
来源：http://tkx.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xaf.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyf.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://und.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://psw.ivvv.top

Ruby: arr.tally
来源：http://udx.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cuk.aizwys.cn

[D21] 判断是否包含某元素
来源：http://tdj.jinqigfzy.top

Py:   x in arr
来源：http://uiv.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://shz.gogol.net.cn

JS:   arr.includes(x)
来源：http://whp.hnxiangtu.top

TS:   arr.includes(x)
来源：http://sug.chenzaomai.com

Java: list.contains(x)
来源：http://auk.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://psg.snrcjt.cn

Ruby: arr.include?(x)
来源：http://djn.ydjk.org.cn

C#:   list.Contains(x)
来源：http://ajn.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://dpj.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wqc.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://frc.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ytj.jqgufenzy.top

TS:   [...arr];
来源：http://nbc.fehbvm.com

Java: new ArrayList<>(list);
来源：http://ltx.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://wdq.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://emz.xuanzx.com

C#:   new List<int>(list);
来源：http://und.xuanzx.com

[D23] reduce 累积计算
来源：http://bmh.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kav.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rqz.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dvw.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkf.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://psu.yvedp.cn

Go:   // 手写循环
来源：http://kxm.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yat.c1oappe.top


<!-- 参考信息 -->