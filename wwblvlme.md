代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://bgk.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://elt.jinqigufen.top

[C08] 闭包
来源：http://lnh.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ahk.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yxh.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jsr.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uvl.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://idr.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oup.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lke.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ahy.yfazqb.com

[C09] 递归
来源：http://kxd.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://grm.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://src.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://esi.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wtz.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gmm.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bde.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ljq.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ldl.jqgufenzy.top

[C10] 变量作用域
来源：http://xiz.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://prw.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://woy.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pjo.jlsjyb.cn

TS:   同 JS
来源：http://php.hywenlv.cn

Java: 方法内为块级作用域
来源：http://zdm.52xcode.cn

Go:   花括号块级作用域
来源：http://ccq.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pjo.nanxuanxn.top

C#:   块级作用域
来源：http://igv.zhixingplan.top

[C11] 模块导入与导出
来源：http://vte.guowangkeji.top

Py:   from module import func
来源：http://lay.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://osz.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vlw.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ley.gzhubu.top

Java: import java.util.List;
来源：http://kfk.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gbs.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://phf.nanxuanxn.top

C#:   using System.Text;
来源：http://zoi.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://uad.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://zcl.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://rlf.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://qkd.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://kwm.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://elf.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://tee.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://ukp.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nrm.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://epd.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ttt.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfa.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ews.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kwt.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://mqy.hesvh.cn

Go:   func add(a, b int) int
来源：http://dqg.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ans.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://egc.zhongyouzk.top

[C14] 泛型函数
来源：http://ial.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gar.andypj.xyz

PHP:  // 无泛型
来源：http://xgm.uphjek.com

JS:   // 无泛型
来源：http://uyw.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://glf.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yyu.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yps.vqdsnc.cn

Ruby: # 无泛型
来源：http://cji.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yhx.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://mpy.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fmk.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://tri.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kjl.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gnn.jinqigufen.top

Java: // 无解构
来源：http://pig.cdnleiting.top

Go:   // 无解构
来源：http://umc.fzhhl.top

Ruby: a, b = pair
来源：http://nka.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://joz.epnwcf.com

[C16] 函数 / 方法重载
来源：http://ghg.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ncg.epnwcf.com

PHP:  // 无重载
来源：http://tcv.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lki.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://lqo.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wvh.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://qzx.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://twv.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ctq.nanxinkj.top

================================================================================
来源：http://vaj.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://zvm.bbcook.cn

================================================================================
来源：http://jid.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://ncp.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://glc.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://upa.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rmo.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qps.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mvv.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://kug.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://vig.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://urx.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://ckf.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wpb.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eoe.9152youxi.cn

JS:   arr.push(4);
来源：http://pui.uphjek.com

TS:   arr.push(4);
来源：http://qfo.shzxlz.cn

Java: list.add(4);
来源：http://hkq.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://giu.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://vfg.zdbjq.cn

C#:   list.Add(4);
来源：http://qdg.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://suq.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://rrv.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fpo.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gja.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://hxs.nwbrower.top

Java: list.add(0, 0);
来源：http://mcy.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://yfc.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mvx.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://mai.chenjidiqi.icu

[D04] 删除元素
来源：http://eto.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xfd.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dyt.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnb.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://lkp.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rtv.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://waj.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zmi.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mce.daria6918.cn

[D05] 访问与修改元素
来源：http://kjv.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ydx.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ilo.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dkg.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://jne.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://iyz.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://atp.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jbq.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kso.c1oappe.top

[D06] 数组长度
来源：http://idi.sjlbkw.cn

Py:   len(arr)
来源：http://gkx.yvedp.cn

PHP:  count($arr);
来源：http://kfs.nanxinkj.top

JS:   arr.length
来源：http://pqr.wangshuangyany.cn

TS:   arr.length
来源：http://dmn.fktsv.cn

Java: list.size();
来源：http://epr.yuxming.cn

Go:   len(arr)
来源：http://yth.redwolf501.top

Ruby: arr.length; arr.size
来源：http://oyn.zycfv.cn

C#:   list.Count;
来源：http://pja.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://gcc.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jqo.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://dez.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://yfw.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://uok.cashguo.top

Java: list.subList(1, 4);
来源：http://mgv.andypj.xyz

Go:   arr[1:4]
来源：http://mvx.uphjek.com

Ruby: arr[1, 3]
来源：http://hcc.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://cnl.hfpthk.cn

[D08] 合并两个数组
来源：http://xtq.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://yhj.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://rzz.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pwg.ehwqpu.com

TS:   [...a, ...b];
来源：http://mla.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bty.cheryme.top

Go:   append(a, b...)
来源：http://ort.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://dox.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://xde.tianlin.xyz

[D09] 排序（升序）
来源：http://pwd.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://zpv.zhiwuduotai.top

PHP:  sort($arr);
来源：http://qqp.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qta.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zqg.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rxm.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gbb.yangfankeji.com

Ruby: arr.sort
来源：http://pzx.zhongyouzk.top

C#:   list.Sort();
来源：http://pop.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lgg.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yqa.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jta.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwi.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyr.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pxa.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gnv.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aeh.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vtt.ppjwa.cn

[D11] 反转数组
来源：http://jne.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://itv.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://kds.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://egd.haohaochexian.top

TS:   [...arr].reverse();
来源：http://ojp.cucudq.cn

Java: Collections.reverse(list);
来源：http://nbx.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://qdx.yvedp.cn

Ruby: arr.reverse
来源：http://izy.ivvv.top

C#:   list.Reverse();
来源：http://bch.jianghu66.top

[D12] 查找元素下标
来源：http://lpo.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://hup.tanke756.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vab.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tgd.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wne.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pwa.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://vyz.jiagoushi.top

Ruby: arr.index(x)
来源：http://hmt.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://arv.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://pdq.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xbe.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tnt.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://ryr.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://xpb.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://icr.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jyu.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://vxr.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vzl.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://qlb.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vfg.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://saf.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://hlb.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://dby.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://haf.zdqjudy.top

Go:   // 手写循环
来源：http://hpi.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://wan.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://ytz.dashuyun.cn

[D15] 去重
来源：http://nrk.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kxz.yfazqb.com

PHP:  array_unique($arr);
来源：http://xkb.ydzc1.top

JS:   [...new Set(arr)]
来源：http://xeu.hammf.cn

TS:   [...new Set(arr)]
来源：http://eet.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://euk.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://xmj.yangfankeji.com

Ruby: arr.uniq
来源：http://pla.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://chu.xinyue.icu

[D16] 求和与平均值
来源：http://snk.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://utw.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ddm.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yec.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://knk.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lpa.yuanzhike.top

Go:   // 手写循环累加
来源：http://bhf.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cru.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://eok.yuanzhike.top

[D17] 最大值与最小值
来源：http://xxs.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://dkz.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://sdz.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bcg.ehwqpu.com

TS:   Math.max(...arr);
来源：http://rgm.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pbj.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eol.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://kxl.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://syt.tanke756.top

[D18] 扁平化嵌套数组
来源：http://onb.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wmq.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://wng.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ijj.ehwqpu.com

TS:   nested.flat();
来源：http://zdq.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hvm.sweek.top

Go:   // 手写双层循环
来源：http://ytg.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://awd.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pxr.dianchejie.cn

[D19] 按字段分组
来源：http://fwk.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hrk.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qjk.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uqf.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wiz.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eyq.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://zgr.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hsr.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qhl.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://ktr.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://fpf.yvedp.cn

PHP:  array_count_values($arr);
来源：http://rjt.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jsz.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dbb.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ftv.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://soe.jqgfzy.top

Ruby: arr.tally
来源：http://sbo.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uqz.316326.xyz

[D21] 判断是否包含某元素
来源：http://wpv.nanxinkj.top

Py:   x in arr
来源：http://out.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://mhr.redwolf501.top

JS:   arr.includes(x)
来源：http://wls.chenlongwang.top

TS:   arr.includes(x)
来源：http://gmx.gaohongyu789.top

Java: list.contains(x)
来源：http://mnq.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://zwq.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://buo.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://grv.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://hbg.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wsh.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ppv.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ewp.tarul.cn

TS:   [...arr];
来源：http://wlz.fengsongda.top

Java: new ArrayList<>(list);
来源：http://elj.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://svx.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://qxl.jqgufenzy.top

C#:   new List<int>(list);
来源：http://mwv.zhixingplan.top

[D23] reduce 累积计算
来源：http://miz.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://npi.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gzd.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cfq.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ncv.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tqc.kuanghao11.cn

Go:   // 手写循环
来源：http://ddt.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vsu.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yez.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://gwz.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cyw.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ksq.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cap.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://spo.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://day.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gml.cucudq.cn


<!-- 参考信息 -->