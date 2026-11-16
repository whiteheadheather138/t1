代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jgv.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mid.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ihm.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aya.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://trz.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sqp.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fap.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://omp.hfpthk.cn

[C10] 变量作用域
来源：http://ayy.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mgb.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nne.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jsv.zhongyouzk.top

TS:   同 JS
来源：http://ojp.zhixingplan.top

Java: 方法内为块级作用域
来源：http://bvr.yuanzhike.top

Go:   花括号块级作用域
来源：http://cwz.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://znb.hnqzz.top

C#:   块级作用域
来源：http://fxx.daria6918.cn

[C11] 模块导入与导出
来源：http://yyj.cdnleiting.top

Py:   from module import func
来源：http://pns.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://atl.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wek.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rjt.jlsjyb.cn

Java: import java.util.List;
来源：http://ywu.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nhb.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://ify.gaohongyu789.top

C#:   using System.Text;
来源：http://upv.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://pmg.hfpthk.cn

Py:   (lambda: print("run"))()
来源：http://ebs.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://ygu.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://wfh.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://cxq.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://obe.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://zbe.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://wob.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://skj.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://azq.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vmx.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ylx.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aed.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxs.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://jlw.mhx1999.top

Go:   func add(a, b int) int
来源：http://fxt.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ksi.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iqs.uphjek.com

[C14] 泛型函数
来源：http://bcx.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://brb.gaohongyu789.top

PHP:  // 无泛型
来源：http://hgr.aizwys.cn

JS:   // 无泛型
来源：http://lyv.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fpm.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ndr.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ibo.jinqigfzy.top

Ruby: # 无泛型
来源：http://jeg.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mpz.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://wnf.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gyn.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://wpc.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lav.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jph.yfazqb.com

Java: // 无解构
来源：http://wfm.yonumen.top

Go:   // 无解构
来源：http://xax.vqdsnc.cn

Ruby: a, b = pair
来源：http://nyg.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://shi.bjfxy.top

[C16] 函数 / 方法重载
来源：http://dgj.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hnn.pengpengdd.cyou

PHP:  // 无重载
来源：http://fsi.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://daw.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://fhq.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qtc.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://zdy.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://stv.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://daw.cqqwz.cn

================================================================================
来源：http://mxa.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://ipd.jyoumei.cn

================================================================================
来源：http://rln.meibo888.top

[D01] 创建数组 / 列表
来源：http://ixn.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://beq.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rlb.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hng.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mye.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ywr.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://nbk.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://myf.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gkt.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://crg.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nzo.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tbg.birdmap.top

JS:   arr.push(4);
来源：http://daa.mhx1999.top

TS:   arr.push(4);
来源：http://axh.birdmap.top

Java: list.add(4);
来源：http://okx.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://znf.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://wuy.hammf.cn

C#:   list.Add(4);
来源：http://cpi.c1oappe.top

[D03] 在指定位置插入元素
来源：http://dxa.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://ztx.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ehx.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzp.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://rkc.aibaodan.cn

Java: list.add(0, 0);
来源：http://wtj.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zaz.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fer.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://ajr.shzxlz.cn

[D04] 删除元素
来源：http://toa.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mbg.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tvo.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lbw.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://mht.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aja.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://juk.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sxe.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zjd.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://uqh.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xwk.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cha.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rpc.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://uhl.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://gsp.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://boy.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cec.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hpb.zhoulong.xyz

[D06] 数组长度
来源：http://rtt.316326.xyz

Py:   len(arr)
来源：http://kvx.daxiang520.top

PHP:  count($arr);
来源：http://brf.ywan-chungtsiang.top

JS:   arr.length
来源：http://eoi.chenzaomai.com

TS:   arr.length
来源：http://jwx.zycfv.cn

Java: list.size();
来源：http://bta.cdnleiting.top

Go:   len(arr)
来源：http://fun.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://vvp.yj20258.top

C#:   list.Count;
来源：http://gel.xziqi.cn

[D07] 切片 / 取子数组
来源：http://xor.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oqg.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gyw.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://bev.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://eva.cheryme.top

Java: list.subList(1, 4);
来源：http://vrm.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://nds.jyoumei.cn

Ruby: arr[1, 3]
来源：http://yky.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://xju.jianghu66.top

[D08] 合并两个数组
来源：http://cnt.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://jaf.ivvv.top

PHP:  array_merge($a, $b);
来源：http://yos.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wum.chenlongwang.top

TS:   [...a, ...b];
来源：http://gag.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pjw.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://aoh.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://bia.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://gzs.bbcook.cn

[D09] 排序（升序）
来源：http://dop.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://shd.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://xof.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fxn.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mne.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yvq.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ytz.zdqjudy.top

Ruby: arr.sort
来源：http://zap.nwbrower.top

C#:   list.Sort();
来源：http://oua.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zub.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uty.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xuj.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://txa.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rka.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zag.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qeh.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://brh.tanke756.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lxs.yj20258.top

[D11] 反转数组
来源：http://plw.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ovx.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://bqm.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tle.tanke756.top

TS:   [...arr].reverse();
来源：http://rxj.nanxinkj.top

Java: Collections.reverse(list);
来源：http://yib.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://ftm.tian-w.cn

Ruby: arr.reverse
来源：http://von.yfazqb.com

C#:   list.Reverse();
来源：http://lmu.cheryme.top

[D12] 查找元素下标
来源：http://oye.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://lkl.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zol.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ghq.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hdp.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vjz.birdmap.top

Go:   slices.Index(arr, x)
来源：http://trg.zdqjudy.top

Ruby: arr.index(x)
来源：http://kax.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://awh.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://hqa.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ojj.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fbl.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://efc.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://lvc.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lxe.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mve.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xsx.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aqb.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://wlj.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yhk.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://caz.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://ppm.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://ems.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fuf.daria6918.cn

Go:   // 手写循环
来源：http://oyn.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vxf.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lzz.shanyushiyangtech.top

[D15] 去重
来源：http://srx.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nvp.yueranfly.top

PHP:  array_unique($arr);
来源：http://oha.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://hba.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://gdj.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gdz.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://jvv.hnqzz.top

Ruby: arr.uniq
来源：http://nrx.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://fik.zhoulong.xyz

[D16] 求和与平均值
来源：http://eed.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ety.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bwm.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xdp.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpt.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uvv.yj20258888.top

Go:   // 手写循环累加
来源：http://coq.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wax.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://lmb.smart0.xyz

[D17] 最大值与最小值
来源：http://zyg.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://agk.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://lqd.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lhz.snrcjt.cn

TS:   Math.max(...arr);
来源：http://skh.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ahz.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zfk.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://fpu.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://dhw.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://sgf.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qqf.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://ryw.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fuf.cdnleiting.top

TS:   nested.flat();
来源：http://alp.jinqigfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mvi.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://iai.hfpthk.cn

Ruby: nested.flatten
来源：http://rgx.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kgq.gogol.net.cn

[D19] 按字段分组
来源：http://yzn.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wif.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rfa.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xdw.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bat.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ygq.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://bjm.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://shn.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ozd.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://fcu.hammf.cn

Py:   Counter(arr)
来源：http://aga.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://qbu.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyw.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrv.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jvm.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://pzk.nwbrower.top

Ruby: arr.tally
来源：http://qep.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yjo.bjfxy.top

[D21] 判断是否包含某元素
来源：http://uej.wangshuangyany.cn

Py:   x in arr
来源：http://jkg.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://fzg.nanxuanxn.top

JS:   arr.includes(x)
来源：http://wet.yj20258888.top

TS:   arr.includes(x)
来源：http://vwl.yfazqb.com

Java: list.contains(x)
来源：http://czt.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://uvi.xylfe.cn

Ruby: arr.include?(x)
来源：http://fma.fengsongda.top

C#:   list.Contains(x)
来源：http://rmt.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://wgo.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hax.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fbw.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvq.jinghuilouyu.cn

TS:   [...arr];
来源：http://mhk.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://rcd.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://smb.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://hkf.zhixingplan.top

C#:   new List<int>(list);
来源：http://ddu.mhx1999.top

[D23] reduce 累积计算
来源：http://eyu.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fdp.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oif.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://emm.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzx.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lie.cdnleiting.top

Go:   // 手写循环
来源：http://xjh.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obg.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lsq.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://yhc.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mby.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nqg.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dtr.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qmd.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xtc.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kaa.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rmx.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ywh.tanke756.top

[D25] Set 集合去重与交并差
来源：http://kgg.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mij.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pfj.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chm.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ndz.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bdu.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aso.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iaz.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mde.jyoumei.cn

[D26] 数组转字符串
来源：http://vss.xingfuxueyuan.xyz


<!-- 参考信息 -->