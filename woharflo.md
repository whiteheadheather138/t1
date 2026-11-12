代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://chw.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://rrc.sjlbkw.cn

[C08] 闭包
来源：http://sur.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jcg.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xds.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ozk.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sjd.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sur.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hqv.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qoo.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://arf.zhijiandao.cn

[C09] 递归
来源：http://cnr.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://swt.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://igp.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://otu.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kjo.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://znf.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xig.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nqe.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vnh.yuanzhike.top

[C10] 变量作用域
来源：http://qpg.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kwk.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zho.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wjr.guowangkeji.top

TS:   同 JS
来源：http://jcg.svipenyu.cn

Java: 方法内为块级作用域
来源：http://qnr.yj20258888.top

Go:   花括号块级作用域
来源：http://ecg.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nyr.sweek.top

C#:   块级作用域
来源：http://jyq.sysykeji.top

[C11] 模块导入与导出
来源：http://vzl.xuanzx.com

Py:   from module import func
来源：http://irv.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://llk.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jpf.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gcr.shzxlz.cn

Java: import java.util.List;
来源：http://kvv.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sxy.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://guf.hywenlv.cn

C#:   using System.Text;
来源：http://lpq.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://mqd.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://uqi.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://pbk.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://xvm.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://twy.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xyw.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://ino.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://vhu.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://reb.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://wat.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gcd.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xsv.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tiv.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gtn.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://xto.jqgfzy.top

Go:   func add(a, b int) int
来源：http://noj.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tkn.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://zvz.gogol.net.cn

[C14] 泛型函数
来源：http://rdv.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hsz.fengsongda.top

PHP:  // 无泛型
来源：http://ogg.svipenyu.cn

JS:   // 无泛型
来源：http://slq.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://glq.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://szm.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nhd.aibaodan.cn

Ruby: # 无泛型
来源：http://ipj.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kan.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://syo.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vpu.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://ctg.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ziz.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jho.wangshuangyany.cn

Java: // 无解构
来源：http://dqi.hongshengwenyu.top

Go:   // 无解构
来源：http://yja.snrcjt.cn

Ruby: a, b = pair
来源：http://apr.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://qwr.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://nbz.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vug.cqqwz.cn

PHP:  // 无重载
来源：http://tfo.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://plf.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://abr.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ukg.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://gyk.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://art.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://pkk.hesvh.cn

================================================================================
来源：http://hzo.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://coa.quarkkingdee.top

================================================================================
来源：http://wbe.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://xqt.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hbb.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://joa.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wwh.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dtb.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pvx.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://mtm.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://jht.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pyl.hesvh.cn

[D02] 追加元素到末尾
来源：http://uvb.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kry.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pat.chenjidiqi.icu

JS:   arr.push(4);
来源：http://lxh.svipenyu.cn

TS:   arr.push(4);
来源：http://fqg.xylfe.cn

Java: list.add(4);
来源：http://ckh.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://hjh.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://ttb.yj202588.top

C#:   list.Add(4);
来源：http://ibe.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://zte.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://oxy.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bvm.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ygi.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://qrd.yanxiufei.cn

Java: list.add(0, 0);
来源：http://cfx.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://gxo.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dml.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://wvy.ehwqpu.com

[D04] 删除元素
来源：http://imr.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gbc.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mvr.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eqg.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://zmb.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zaj.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ioy.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lsv.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mvv.havefunace.top

[D05] 访问与修改元素
来源：http://oqh.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hpx.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bnc.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vsz.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://xen.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://fsx.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://rvq.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qkk.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://grn.sjlbkw.cn

[D06] 数组长度
来源：http://eri.jinqigufen.top

Py:   len(arr)
来源：http://rnz.cdnleiting.top

PHP:  count($arr);
来源：http://hux.andypj.xyz

JS:   arr.length
来源：http://yiq.chenjidiqi.icu

TS:   arr.length
来源：http://dmg.iojbl.cn

Java: list.size();
来源：http://qtw.yuanzhike.top

Go:   len(arr)
来源：http://dai.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://pgj.jiagoushi.top

C#:   list.Count;
来源：http://zqr.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://ipu.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vns.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uax.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://drg.yj20258.top

TS:   arr.slice(1, 4);
来源：http://nbs.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://ziv.52xcode.cn

Go:   arr[1:4]
来源：http://hbn.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://qpu.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://qca.zhijiandao.cn

[D08] 合并两个数组
来源：http://txi.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://lux.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://plx.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://tuz.hnqzz.top

TS:   [...a, ...b];
来源：http://qjp.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rhj.jiagoushi.top

Go:   append(a, b...)
来源：http://nmr.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://yej.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://aot.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://wlp.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ldj.birdmap.top

PHP:  sort($arr);
来源：http://wcj.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vuo.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ech.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wwl.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eqa.guowangkeji.top

Ruby: arr.sort
来源：http://xmy.xuetiantiany.cn

C#:   list.Sort();
来源：http://tcx.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ijx.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gea.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wei.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cgq.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bjg.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vsk.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tre.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cbs.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ozm.ybcxt.top

[D11] 反转数组
来源：http://tek.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://omr.yj202588.top

PHP:  array_reverse($arr);
来源：http://lmw.kuanghao11.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hnh.nanxinkj.top

TS:   [...arr].reverse();
来源：http://ymn.haohaochexian.top

Java: Collections.reverse(list);
来源：http://iyn.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://fxv.52xcode.cn

Ruby: arr.reverse
来源：http://tyq.yanxiufei.cn

C#:   list.Reverse();
来源：http://mio.jqgufenzy.top

[D12] 查找元素下标
来源：http://qip.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://oeg.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://drc.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rsf.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrs.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://klz.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://gse.ydzc1.top

Ruby: arr.index(x)
来源：http://aiy.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://abe.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://mae.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rmj.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xbl.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://mqs.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://dza.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kel.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hyy.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://yjc.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tel.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://bxc.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hnz.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hwg.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://yux.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://ycj.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://abd.gotoacloud.top

Go:   // 手写循环
来源：http://yli.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://iks.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://mbc.hongshengwenyu.top

[D15] 去重
来源：http://zsg.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lcb.gogol.net.cn

PHP:  array_unique($arr);
来源：http://oqy.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://aqn.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://yml.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jmc.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://pwq.zycfv.cn

Ruby: arr.uniq
来源：http://rhq.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://vtw.jinqigufen.top

[D16] 求和与平均值
来源：http://npa.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://owz.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sct.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zyd.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdf.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nrf.xziqi.cn

Go:   // 手写循环累加
来源：http://wyo.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qkw.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://xux.nwbrower.top

[D17] 最大值与最小值
来源：http://sdc.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://vjn.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://tjm.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aww.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://swp.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ybm.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ixy.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://sbx.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://lwe.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://agh.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yib.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://jtg.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jkm.hnqzz.top

TS:   nested.flat();
来源：http://tfx.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kll.xinyue.icu

Go:   // 手写双层循环
来源：http://rqe.wangshuangyany.cn

Ruby: nested.flatten
来源：http://ewc.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nxg.gzhubu.top

[D19] 按字段分组
来源：http://yyc.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nbq.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jzp.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyw.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bfl.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://stg.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://app.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hgg.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jtn.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://qan.jqgfzy.top

Py:   Counter(arr)
来源：http://wmr.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://biq.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggh.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rgq.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kos.nwbrower.top

Go:   // 手写 map[T]int
来源：http://gvz.zhoulong.xyz

Ruby: arr.tally
来源：http://lis.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zrc.redwolf501.top

[D21] 判断是否包含某元素
来源：http://apk.cucudq.cn

Py:   x in arr
来源：http://voz.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://byr.jqgufenzy.top

JS:   arr.includes(x)
来源：http://lch.sweek.top

TS:   arr.includes(x)
来源：http://dcc.jiagoushi.top

Java: list.contains(x)
来源：http://jhg.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://cwv.wangdashe.top

Ruby: arr.include?(x)
来源：http://gib.chenlongwang.top

C#:   list.Contains(x)
来源：http://wen.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://jxo.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://coo.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wjo.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qkg.tian-w.cn

TS:   [...arr];
来源：http://hnd.bbcook.cn

Java: new ArrayList<>(list);
来源：http://lca.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://mbf.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://siw.xylfe.cn

C#:   new List<int>(list);
来源：http://cdh.aizwys.cn

[D23] reduce 累积计算
来源：http://whi.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ugo.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vax.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://evp.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cil.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hed.xuetiantiany.cn

Go:   // 手写循环
来源：http://gjb.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bxq.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lat.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://ami.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://krt.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tpw.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gpz.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vdi.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rmw.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bha.gzhubu.top


<!-- 参考信息 -->