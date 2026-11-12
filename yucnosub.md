代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zfr.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qqv.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tcm.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ktk.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nwf.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dcu.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://chm.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qyi.fzhhl.top

[C10] 变量作用域
来源：http://vbe.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jva.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wei.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yqe.shzxlz.cn

TS:   同 JS
来源：http://lmt.smart0.xyz

Java: 方法内为块级作用域
来源：http://oyk.jinqigfzy.top

Go:   花括号块级作用域
来源：http://tyr.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nih.gaohongyu789.top

C#:   块级作用域
来源：http://few.zhongyouzk.top

[C11] 模块导入与导出
来源：http://daz.zdbjq.cn

Py:   from module import func
来源：http://nwa.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ieq.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://spe.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bed.cdnleiting.top

Java: import java.util.List;
来源：http://shc.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mnq.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://lpg.daxiang520.top

C#:   using System.Text;
来源：http://viz.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://lfe.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://phr.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://sad.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://sbe.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://uso.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ilg.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://vuy.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://eow.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yop.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://hwa.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zpn.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qrl.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bww.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kts.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://yhu.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://err.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dlx.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://typ.xinyue.icu

[C14] 泛型函数
来源：http://ttl.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pej.zycfv.cn

PHP:  // 无泛型
来源：http://tmo.nwbrower.top

JS:   // 无泛型
来源：http://xss.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bna.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://piz.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ukb.bbcook.cn

Ruby: # 无泛型
来源：http://vzf.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://exz.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://xay.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iuz.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://vjf.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wjs.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzx.nwbrower.top

Java: // 无解构
来源：http://nbe.meibo888.top

Go:   // 无解构
来源：http://pmi.daria6918.cn

Ruby: a, b = pair
来源：http://qva.cashguo.top

C#:   var (a, b) = pair;
来源：http://ktr.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://wvy.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hcp.pycfn.com

PHP:  // 无重载
来源：http://eay.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sqw.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://oql.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://mqs.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://kbm.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://kja.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzg.yj20258888.top

================================================================================
来源：http://pzi.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://vwi.hcnkem.com

================================================================================
来源：http://mqq.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://umd.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nwm.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vnu.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vps.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://voo.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pwt.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://ksv.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://wkc.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sau.vehdjk.com

[D02] 追加元素到末尾
来源：http://agy.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qjb.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ztc.xylfe.cn

JS:   arr.push(4);
来源：http://xqq.bbcook.cn

TS:   arr.push(4);
来源：http://ors.jqgufenzy.top

Java: list.add(4);
来源：http://nin.daxiang520.top

Go:   arr = append(arr, 4)
来源：http://piy.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://qmj.0kj1m.cn

C#:   list.Add(4);
来源：http://jyz.birdmap.top

[D03] 在指定位置插入元素
来源：http://nsl.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://ozb.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qjz.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sxi.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://wdn.yonumen.top

Java: list.add(0, 0);
来源：http://aoa.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://ujo.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://smj.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://kvc.jiagoushi.top

[D04] 删除元素
来源：http://grt.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://itt.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ynz.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvz.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://obu.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://srg.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ujg.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pus.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vrj.fzhhl.top

[D05] 访问与修改元素
来源：http://piu.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kio.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rev.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ndf.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://msu.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://cln.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://vzc.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rol.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tvz.xuetiantiany.cn

[D06] 数组长度
来源：http://gmh.haohaochexian.top

Py:   len(arr)
来源：http://vyz.gogol.net.cn

PHP:  count($arr);
来源：http://ooz.shanyushiyangtech.top

JS:   arr.length
来源：http://huj.haohaochexian.top

TS:   arr.length
来源：http://amt.wangdashe.top

Java: list.size();
来源：http://ibp.gzhubu.top

Go:   len(arr)
来源：http://trr.andypj.xyz

Ruby: arr.length; arr.size
来源：http://zjv.aizwys.cn

C#:   list.Count;
来源：http://ibv.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://auj.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gkk.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hic.sweek.top

JS:   arr.slice(1, 4);
来源：http://qtf.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://cnh.sufxvd.cn

Java: list.subList(1, 4);
来源：http://udw.meibo888.top

Go:   arr[1:4]
来源：http://qfw.ivvv.top

Ruby: arr[1, 3]
来源：http://ast.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://dsw.dashuyun.cn

[D08] 合并两个数组
来源：http://dtl.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://wsg.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://ynf.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dpo.fzhhl.top

TS:   [...a, ...b];
来源：http://fox.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dgh.guowangkeji.top

Go:   append(a, b...)
来源：http://pwy.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://rrp.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://lfb.cqqwz.cn

[D09] 排序（升序）
来源：http://vbs.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://rch.fzhhl.top

PHP:  sort($arr);
来源：http://rwf.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nsv.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ljt.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://fks.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zml.hfpthk.cn

Ruby: arr.sort
来源：http://nny.bjfxy.top

C#:   list.Sort();
来源：http://ycu.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mrq.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fjw.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lky.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uua.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hhl.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xze.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dyj.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uds.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lnt.sweek.top

[D11] 反转数组
来源：http://shn.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://ota.shuidangran.top

PHP:  array_reverse($arr);
来源：http://gdq.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gar.xylfe.cn

TS:   [...arr].reverse();
来源：http://ajg.xuanzx.com

Java: Collections.reverse(list);
来源：http://haj.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://abh.ppjwa.cn

Ruby: arr.reverse
来源：http://czc.fktsv.cn

C#:   list.Reverse();
来源：http://oru.yanxiufei.cn

[D12] 查找元素下标
来源：http://zbf.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://pei.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://usq.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wad.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ssl.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zqb.uphjek.com

Go:   slices.Index(arr, x)
来源：http://kfy.redwolf501.top

Ruby: arr.index(x)
来源：http://ngq.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://vrn.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://gzs.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://opg.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sxi.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://row.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://dvy.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://moi.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jmb.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://nbl.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zay.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://bgw.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fgb.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://osl.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://xty.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://qis.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gss.tian-w.cn

Go:   // 手写循环
来源：http://qqn.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://eoj.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://stx.ppjwa.cn

[D15] 去重
来源：http://epg.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dcr.xziqi.cn

PHP:  array_unique($arr);
来源：http://qqg.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://kba.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://rgi.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oua.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://str.cucudq.cn

Ruby: arr.uniq
来源：http://equ.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://qjm.hfpthk.cn

[D16] 求和与平均值
来源：http://sdt.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://flc.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://laq.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ksf.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ldm.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mol.mhx1999.top

Go:   // 手写循环累加
来源：http://uin.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hmq.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://lvt.svipenyu.cn

[D17] 最大值与最小值
来源：http://sad.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://yhm.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://szx.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzd.sweek.top

TS:   Math.max(...arr);
来源：http://eml.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eqr.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hfv.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://nuh.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://afq.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://lnn.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kac.yj20258.top

PHP:  array_merge(...$nested);
来源：http://wux.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ljz.zycfv.cn

TS:   nested.flat();
来源：http://ieq.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jys.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://fzg.hywenlv.cn

Ruby: nested.flatten
来源：http://ekr.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ucp.havefunace.top

[D19] 按字段分组
来源：http://wos.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nsx.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mkw.jlsjyb.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uju.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://tkf.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://caj.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://mof.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://yli.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mdu.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://mge.xziqi.cn

Py:   Counter(arr)
来源：http://fhs.yuxming.cn

PHP:  array_count_values($arr);
来源：http://huy.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uzu.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yfv.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yiu.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://zze.sufxvd.cn

Ruby: arr.tally
来源：http://zza.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bxe.zycfv.cn

[D21] 判断是否包含某元素
来源：http://rfg.yj20258888.top

Py:   x in arr
来源：http://rdj.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://fot.hnxiangtu.top

JS:   arr.includes(x)
来源：http://fuh.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://uuh.jlsjyb.cn

Java: list.contains(x)
来源：http://wyp.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://idy.jianghu66.top

Ruby: arr.include?(x)
来源：http://sjy.ydzc1.top

C#:   list.Contains(x)
来源：http://uor.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://van.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://igl.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lcp.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fla.zhongyouzk.top

TS:   [...arr];
来源：http://lrm.tian-w.cn

Java: new ArrayList<>(list);
来源：http://yqh.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://ryu.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://ylg.yuxming.cn

C#:   new List<int>(list);
来源：http://emx.xinyue.icu

[D23] reduce 累积计算
来源：http://nvk.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yrm.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pkb.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://crr.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tzz.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pul.c1oappe.top

Go:   // 手写循环
来源：http://ahb.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://apk.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tpq.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://rjw.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sbt.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xae.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hpv.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mdn.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lzm.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://izl.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nwd.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oqu.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://gpy.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ukb.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tla.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lij.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qus.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fdk.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://otq.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uzh.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eeu.ppjwa.cn

[D26] 数组转字符串
来源：http://irc.wangshuangyany.cn


<!-- 参考信息 -->