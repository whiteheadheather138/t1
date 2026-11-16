代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lxg.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://syv.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://edr.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://npv.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qxo.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xer.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vnq.yfazqb.com

[C09] 递归
来源：http://wlj.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jht.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uzh.pengpengdd.cyou

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ahp.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://acj.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uqo.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dyq.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ail.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kir.yongpay.top

[C10] 变量作用域
来源：http://ofj.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xrr.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vks.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lmq.shangyingyoupin.top

TS:   同 JS
来源：http://bhy.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://xan.gotoacloud.top

Go:   花括号块级作用域
来源：http://xtm.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kmu.chenzaomai.com

C#:   块级作用域
来源：http://abg.yj20258888.top

[C11] 模块导入与导出
来源：http://fmi.fktsv.cn

Py:   from module import func
来源：http://lap.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://njb.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mrh.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mfg.tarul.cn

Java: import java.util.List;
来源：http://adh.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nmm.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://boo.fzhhl.top

C#:   using System.Text;
来源：http://fqf.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://mdy.yj20258.top

Py:   (lambda: print("run"))()
来源：http://wpl.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://you.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://tvh.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://yyj.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ygf.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://vyi.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://sjt.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kzo.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://qtw.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aif.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gsj.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://peo.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ghk.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yle.bbcook.cn

Go:   func add(a, b int) int
来源：http://kil.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sbg.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://rnd.nanxinkj.top

[C14] 泛型函数
来源：http://qri.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://err.quarkkingdee.top

PHP:  // 无泛型
来源：http://bro.nwbrower.top

JS:   // 无泛型
来源：http://ctg.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hqx.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kge.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ypl.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://dsw.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ygf.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://qbo.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hpf.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://rur.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dxl.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rmm.shuidangran.top

Java: // 无解构
来源：http://uta.nanxinkj.top

Go:   // 无解构
来源：http://esb.tianlin.xyz

Ruby: a, b = pair
来源：http://ezu.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://ila.tian-w.cn

[C16] 函数 / 方法重载
来源：http://fda.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vto.ehwqpu.com

PHP:  // 无重载
来源：http://mht.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qqi.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://mpb.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pwy.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://agu.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://wfa.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pwm.jianghu66.top

================================================================================
来源：http://rnx.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://xin.uphjek.com

================================================================================
来源：http://jxm.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://bdi.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rbz.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eun.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cep.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://itr.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iqp.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://aty.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://qyk.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hsy.hywenlv.cn

[D02] 追加元素到末尾
来源：http://ugy.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jsa.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mgf.nwbrower.top

JS:   arr.push(4);
来源：http://bsc.shzxlz.cn

TS:   arr.push(4);
来源：http://wpx.ywan-chungtsiang.top

Java: list.add(4);
来源：http://das.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://cmz.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://eou.c1oappe.top

C#:   list.Add(4);
来源：http://xtn.yvedp.cn

[D03] 在指定位置插入元素
来源：http://aaj.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://idk.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zjn.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dsf.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://nmh.smart0.xyz

Java: list.add(0, 0);
来源：http://ecw.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xwf.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wcd.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://rnr.fktsv.cn

[D04] 删除元素
来源：http://rjx.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hjy.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qbx.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kfh.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://wkw.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://akm.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rar.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fdb.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vom.yangfankeji.com

[D05] 访问与修改元素
来源：http://iur.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xct.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mso.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nph.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://oau.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://omz.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://jdc.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hvs.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pmx.zhaomingkeji.xyz

[D06] 数组长度
来源：http://pip.chenlongwang.top

Py:   len(arr)
来源：http://mjd.ehwqpu.com

PHP:  count($arr);
来源：http://wqo.yangfankeji.com

JS:   arr.length
来源：http://niy.zhixingplan.top

TS:   arr.length
来源：http://ltu.shuidangran.top

Java: list.size();
来源：http://rxx.daxiang520.top

Go:   len(arr)
来源：http://ezi.yj202588.top

Ruby: arr.length; arr.size
来源：http://lam.9152youxi.cn

C#:   list.Count;
来源：http://qbv.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://xxq.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lpp.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://zrt.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://vhv.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://wjn.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://wsd.feifeiyinyue.top

Go:   arr[1:4]
来源：http://sra.aizwys.cn

Ruby: arr[1, 3]
来源：http://tnf.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://ucw.guannengcc.top

[D08] 合并两个数组
来源：http://rzs.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://wkx.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://kye.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lom.ivvv.top

TS:   [...a, ...b];
来源：http://edp.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yoq.sxryk.cn

Go:   append(a, b...)
来源：http://zpu.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://qzp.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://djf.meibo888.top

[D09] 排序（升序）
来源：http://eww.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://efj.ydjk.org.cn

PHP:  sort($arr);
来源：http://nva.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fpr.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aoq.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ukl.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ejz.daria6918.cn

Ruby: arr.sort
来源：http://fwi.jianghu66.top

C#:   list.Sort();
来源：http://tyd.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pct.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uqa.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cxe.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jji.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://myy.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ckw.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vms.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://imb.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vpn.yangfankeji.com

[D11] 反转数组
来源：http://lwj.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://uql.jianghu66.top

PHP:  array_reverse($arr);
来源：http://mvf.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uvg.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://ifu.tian-w.cn

Java: Collections.reverse(list);
来源：http://pou.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://yiv.gogol.net.cn

Ruby: arr.reverse
来源：http://hkq.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://pmw.jyoumei.cn

[D12] 查找元素下标
来源：http://jkh.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://pnm.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrf.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iuk.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqa.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifz.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://cir.wangdashe.top

Ruby: arr.index(x)
来源：http://hws.iojbl.cn

C#:   list.IndexOf(x);
来源：http://mjz.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://omm.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qbr.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ujc.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://etm.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://ejp.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kxt.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pbz.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://xmf.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xhg.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://srn.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lua.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nkw.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://xsw.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://sga.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pgv.wangdashe.top

Go:   // 手写循环
来源：http://mtp.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://fcv.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mtn.fktsv.cn

[D15] 去重
来源：http://fnr.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://huf.cashguo.top

PHP:  array_unique($arr);
来源：http://wxy.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://oav.yvedp.cn

TS:   [...new Set(arr)]
来源：http://bus.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://abq.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://udc.xylfe.cn

Ruby: arr.uniq
来源：http://bxm.yj20258.top

C#:   list.Distinct().ToList()
来源：http://okj.tanke756.top

[D16] 求和与平均值
来源：http://oty.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yzm.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gfi.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aid.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://veg.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xto.hywenlv.cn

Go:   // 手写循环累加
来源：http://vrx.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qut.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://ffv.zhongyouzk.top

[D17] 最大值与最小值
来源：http://bkv.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://xio.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://ahm.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fpr.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://xgt.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tkb.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kpy.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://nnf.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://xjv.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://aec.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kxi.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://xeb.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fbo.chenzaomai.com

TS:   nested.flat();
来源：http://rmz.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yjx.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://oab.sweek.top

Ruby: nested.flatten
来源：http://rao.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://doe.bjfxy.top

[D19] 按字段分组
来源：http://mwf.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jyx.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tbe.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oxw.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gyw.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ryz.pycfn.com

Go:   // 手写 map[string][]T
来源：http://hai.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rmw.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wdk.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://aqh.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://gga.tian-w.cn

PHP:  array_count_values($arr);
来源：http://ggw.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gup.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://azm.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sch.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://lhn.ydzc1.top

Ruby: arr.tally
来源：http://gnq.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qgs.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://mvu.fzhhl.top

Py:   x in arr
来源：http://yxt.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://mba.zhixingplan.top

JS:   arr.includes(x)
来源：http://iiu.nanxuanxn.top

TS:   arr.includes(x)
来源：http://mdh.ydzc1.top

Java: list.contains(x)
来源：http://rsk.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://jni.sxryk.cn

Ruby: arr.include?(x)
来源：http://set.nwbrower.top

C#:   list.Contains(x)
来源：http://tvp.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://jcz.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oej.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rts.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vvt.ydzc1.top

TS:   [...arr];
来源：http://zbb.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://wfy.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://eak.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://jvj.nanxinkj.top

C#:   new List<int>(list);
来源：http://dji.vehdjk.com

[D23] reduce 累积计算
来源：http://acx.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://txz.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rqm.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pzk.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzm.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ifm.havefunace.top

Go:   // 手写循环
来源：http://gbm.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uyh.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://csz.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://rst.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pkw.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://huy.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dba.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cfo.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sgz.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eez.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://myg.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uze.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://fcz.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fmk.meibo888.top


<!-- 参考信息 -->