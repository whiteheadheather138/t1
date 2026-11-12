代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lnn.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yff.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://awk.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jti.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rtb.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qxu.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ber.fanxiaobao.xyz

[C09] 递归
来源：http://evs.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bpv.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gtl.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edz.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wez.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xej.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ekr.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://djg.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bjp.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://evf.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nli.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kjb.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nxc.aizwys.cn

TS:   同 JS
来源：http://rha.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://hig.dashuyun.cn

Go:   花括号块级作用域
来源：http://xhp.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qac.cdnleiting.top

C#:   块级作用域
来源：http://iku.haohaochexian.top

[C11] 模块导入与导出
来源：http://gqm.yuxming.cn

Py:   from module import func
来源：http://fec.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lza.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wif.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dsd.shzxlz.cn

Java: import java.util.List;
来源：http://apo.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cjv.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://jmi.redwolf501.top

C#:   using System.Text;
来源：http://pwr.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://okv.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://tux.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://dnz.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://eob.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://nnp.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uhk.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://yom.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://qgj.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nki.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://klk.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qau.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://smb.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bgm.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tvn.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bfn.hnqzz.top

Go:   func add(a, b int) int
来源：http://tdg.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nht.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yow.hesvh.cn

[C14] 泛型函数
来源：http://vbs.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oel.nanxuanxn.top

PHP:  // 无泛型
来源：http://jhk.pycfn.com

JS:   // 无泛型
来源：http://vff.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xzn.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kwg.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jxd.shzxlz.cn

Ruby: # 无泛型
来源：http://ixl.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://owi.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://erx.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bgs.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://qpt.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xtc.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://toi.zhongyouzk.top

Java: // 无解构
来源：http://cqx.jinqigfzy.top

Go:   // 无解构
来源：http://zbm.ydjk.org.cn

Ruby: a, b = pair
来源：http://afy.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://lwm.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://dpw.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ypo.ivvv.top

PHP:  // 无重载
来源：http://gas.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qtn.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://fkd.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kng.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://kvr.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://djv.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uit.dashuyun.cn

================================================================================
来源：http://llb.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://jbh.zdbjq.cn

================================================================================
来源：http://amw.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://ixw.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ncy.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ciz.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vrh.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rvq.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bxa.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://lft.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://uxr.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mhn.yj20258888.top

[D02] 追加元素到末尾
来源：http://lao.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pir.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sgc.wangdashe.top

JS:   arr.push(4);
来源：http://byl.jinqigfzy.top

TS:   arr.push(4);
来源：http://yft.316326.xyz

Java: list.add(4);
来源：http://fen.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://wyu.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://bop.bjfxy.top

C#:   list.Add(4);
来源：http://dfv.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://yji.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://qhx.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bdp.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zek.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://zjn.aibaodan.cn

Java: list.add(0, 0);
来源：http://fsh.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sni.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cdj.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://rrx.nanxuanxn.top

[D04] 删除元素
来源：http://ied.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eux.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jcs.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqv.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://cvf.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://smx.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xum.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uen.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zid.uphjek.com

[D05] 访问与修改元素
来源：http://dcb.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nsk.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lzm.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://axh.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://abd.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://xfr.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://bgy.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gqq.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://utm.vqdsnc.cn

[D06] 数组长度
来源：http://xgn.ivvv.top

Py:   len(arr)
来源：http://jjt.wangshuangyany.cn

PHP:  count($arr);
来源：http://gag.yj20258888.top

JS:   arr.length
来源：http://pbm.zhoulong.xyz

TS:   arr.length
来源：http://tlr.zhixingplan.top

Java: list.size();
来源：http://lsw.yuanzhike.top

Go:   len(arr)
来源：http://fot.uphjek.com

Ruby: arr.length; arr.size
来源：http://ejn.daria6918.cn

C#:   list.Count;
来源：http://jpp.xylfe.cn

[D07] 切片 / 取子数组
来源：http://pph.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://acb.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vmp.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://iar.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://xae.ydzc1.top

Java: list.subList(1, 4);
来源：http://ccq.zhengqikj.top

Go:   arr[1:4]
来源：http://nhy.yvedp.cn

Ruby: arr[1, 3]
来源：http://dej.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://sss.gotoacloud.top

[D08] 合并两个数组
来源：http://nbi.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://gzu.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://bla.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://igb.hfpthk.cn

TS:   [...a, ...b];
来源：http://cir.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xab.gotoacloud.top

Go:   append(a, b...)
来源：http://agu.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://wmq.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://upf.sxryk.cn

[D09] 排序（升序）
来源：http://clk.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://mlp.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://kce.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ryz.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ooj.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ngy.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://evb.zhongyouzk.top

Ruby: arr.sort
来源：http://ldr.chenzaomai.com

C#:   list.Sort();
来源：http://qjb.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://awq.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yuj.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wbo.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vhv.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqs.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sri.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lcr.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gtn.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kmp.vqdsnc.cn

[D11] 反转数组
来源：http://qmr.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://kwx.yj20258.top

PHP:  array_reverse($arr);
来源：http://ygt.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sjj.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://bdc.tarul.cn

Java: Collections.reverse(list);
来源：http://odu.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://rwf.yj202588.top

Ruby: arr.reverse
来源：http://cts.zdbjq.cn

C#:   list.Reverse();
来源：http://nbu.yuxming.cn

[D12] 查找元素下标
来源：http://fly.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://jda.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lwx.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tix.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgz.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hdg.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://zsy.yueranfly.top

Ruby: arr.index(x)
来源：http://xhw.fzhhl.top

C#:   list.IndexOf(x);
来源：http://czp.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://pyb.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://btl.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mjl.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://sht.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://sbs.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://smz.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ejo.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://kxc.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://ame.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://zqq.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bfc.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jlg.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://lhb.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://xxz.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ill.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://iqt.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ali.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://rsc.yonumen.top

[D15] 去重
来源：http://hag.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ukv.ehwqpu.com

PHP:  array_unique($arr);
来源：http://hyt.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://ptb.vehdjk.com

TS:   [...new Set(arr)]
来源：http://axw.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qpx.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://khm.c1oappe.top

Ruby: arr.uniq
来源：http://hdx.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://vsv.jqgufenzy.top

[D16] 求和与平均值
来源：http://kxh.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tua.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yvn.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ben.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iui.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ipe.sweek.top

Go:   // 手写循环累加
来源：http://its.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ezz.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://uor.xziqi.cn

[D17] 最大值与最小值
来源：http://cmz.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://fnv.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://fzn.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eud.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://dyk.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ghc.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kne.316326.xyz

Ruby: arr.max;  arr.min
来源：http://jqf.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://qww.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://mtu.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wrq.birdmap.top

PHP:  array_merge(...$nested);
来源：http://dbk.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ryt.9152youxi.cn

TS:   nested.flat();
来源：http://lkt.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ash.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://mbj.cucudq.cn

Ruby: nested.flatten
来源：http://bdr.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://efq.zdbjq.cn

[D19] 按字段分组
来源：http://uba.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cer.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ufm.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://psw.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vlq.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ngq.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://whj.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fau.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bac.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://acu.tian-w.cn

Py:   Counter(arr)
来源：http://yae.yj20258.top

PHP:  array_count_values($arr);
来源：http://oda.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvl.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ezs.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gzi.316326.xyz

Go:   // 手写 map[T]int
来源：http://wqd.meibo888.top

Ruby: arr.tally
来源：http://nqu.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://znt.tanke756.top

[D21] 判断是否包含某元素
来源：http://ush.ydzc1.top

Py:   x in arr
来源：http://wvx.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://mps.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://dhh.yangfankeji.com

TS:   arr.includes(x)
来源：http://xuf.9152youxi.cn

Java: list.contains(x)
来源：http://wsb.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://sqn.yonumen.top

Ruby: arr.include?(x)
来源：http://qhs.yangfankeji.com

C#:   list.Contains(x)
来源：http://esk.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://yxh.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbh.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fbm.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yzc.jinyuanbaomall.cn

TS:   [...arr];
来源：http://tmc.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://tij.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://crc.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://sor.9152youxi.cn

C#:   new List<int>(list);
来源：http://jds.hnqzz.top

[D23] reduce 累积计算
来源：http://amq.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bdr.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jqm.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hef.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kiv.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uxw.meibo888.top

Go:   // 手写循环
来源：http://bte.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wxd.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://anw.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://xxf.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://igl.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vhc.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://esk.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qrw.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zrq.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zpn.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hxj.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fsr.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://qty.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tnv.0kj1m.cn


<!-- 参考信息 -->