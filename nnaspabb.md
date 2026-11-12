代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://lvr.havefunace.top

C#:   using System.Text;
来源：http://nov.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://wha.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://uql.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://umf.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://utp.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://hvu.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jba.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://ejr.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://fqg.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yzk.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://bmm.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ses.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://the.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kcj.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eed.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://uku.pycfn.com

Go:   func add(a, b int) int
来源：http://ctv.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yje.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://zfe.fanxiaobao.xyz

[C14] 泛型函数
来源：http://uxd.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qly.yj20258888.top

PHP:  // 无泛型
来源：http://iwy.bjfxy.top

JS:   // 无泛型
来源：http://dvk.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbf.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lnk.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sbb.hysaishi.cn

Ruby: # 无泛型
来源：http://ywb.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ykg.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://hbn.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ysw.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://yob.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bpm.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xte.gogol.net.cn

Java: // 无解构
来源：http://hjs.kuanghao11.cn

Go:   // 无解构
来源：http://jke.hfpthk.cn

Ruby: a, b = pair
来源：http://rup.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://cbi.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://fnc.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kmu.hcnkem.com

PHP:  // 无重载
来源：http://ohk.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gft.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://wit.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://bwz.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://xeb.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://bbo.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zjh.jiagoushi.top

================================================================================
来源：http://bsz.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://fon.sjlbkw.cn

================================================================================
来源：http://vpm.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://tax.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iql.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://shh.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zhq.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uel.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vod.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://pnx.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://ikg.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ewn.aizwys.cn

[D02] 追加元素到末尾
来源：http://xru.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fjf.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zxp.meibo888.top

JS:   arr.push(4);
来源：http://rks.bjfxy.top

TS:   arr.push(4);
来源：http://tih.cucudq.cn

Java: list.add(4);
来源：http://tvm.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://nkd.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://ebb.zycfv.cn

C#:   list.Add(4);
来源：http://qfk.cashguo.top

[D03] 在指定位置插入元素
来源：http://urr.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://kpo.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jau.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yfu.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://bma.chenlongwang.top

Java: list.add(0, 0);
来源：http://hqy.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fxv.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xug.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://wyz.zhengqikj.top

[D04] 删除元素
来源：http://jkg.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hif.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fjb.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://spj.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://fkk.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ala.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://toz.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://urx.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hww.cashguo.top

[D05] 访问与修改元素
来源：http://jvq.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mfk.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wjx.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lle.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://kdr.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://wvv.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://omr.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vcx.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxu.nwbrower.top

[D06] 数组长度
来源：http://psb.hysaishi.cn

Py:   len(arr)
来源：http://nsu.jyoumei.cn

PHP:  count($arr);
来源：http://wrh.redwolf501.top

JS:   arr.length
来源：http://hcz.ivvv.top

TS:   arr.length
来源：http://ncp.hnxiangtu.top

Java: list.size();
来源：http://rht.jlsjyb.cn

Go:   len(arr)
来源：http://jpe.c1oappe.top

Ruby: arr.length; arr.size
来源：http://aml.ppjwa.cn

C#:   list.Count;
来源：http://jon.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://abz.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://syu.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://jjj.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://xrx.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://cxr.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://jhf.yvedp.cn

Go:   arr[1:4]
来源：http://pov.yuxming.cn

Ruby: arr[1, 3]
来源：http://vpp.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://soy.jinqigfzy.top

[D08] 合并两个数组
来源：http://arz.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://lyg.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://yls.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nbb.sufxvd.cn

TS:   [...a, ...b];
来源：http://wiv.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hbb.cucudq.cn

Go:   append(a, b...)
来源：http://mkm.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://sop.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://rme.ivvv.top

[D09] 排序（升序）
来源：http://ruy.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://eht.ydzc1.top

PHP:  sort($arr);
来源：http://gug.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aeo.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gkd.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hop.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yhx.shangyingyoupin.top

Ruby: arr.sort
来源：http://ztp.zhijiandao.cn

C#:   list.Sort();
来源：http://gfm.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://sdh.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://buq.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dvi.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ekb.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rxa.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rso.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tey.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wcw.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uxk.hcnkem.com

[D11] 反转数组
来源：http://irv.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://gkq.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://xhn.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rhi.cheryme.top

TS:   [...arr].reverse();
来源：http://flt.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://qkp.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://mgm.quarkkingdee.top

Ruby: arr.reverse
来源：http://wlr.yj20258888.top

C#:   list.Reverse();
来源：http://okr.ppjwa.cn

[D12] 查找元素下标
来源：http://qwc.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://ycs.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ipg.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ckl.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://huk.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xox.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://res.c1oappe.top

Ruby: arr.index(x)
来源：http://ckf.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://rxo.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://ecf.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wiv.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ugq.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://dac.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://zkg.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xoa.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ook.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cls.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tvr.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://vtk.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tfv.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xnk.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://ess.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://tnb.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nyq.hnxiangtu.top

Go:   // 手写循环
来源：http://ucy.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://ptg.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cpf.yangfankeji.com

[D15] 去重
来源：http://tor.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mql.sxryk.cn

PHP:  array_unique($arr);
来源：http://ibx.andypj.xyz

JS:   [...new Set(arr)]
来源：http://kdy.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://buu.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jaj.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://gne.nanxinkj.top

Ruby: arr.uniq
来源：http://gny.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://xey.sxryk.cn

[D16] 求和与平均值
来源：http://omj.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gco.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cjm.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ljp.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jaf.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fxu.vehdjk.com

Go:   // 手写循环累加
来源：http://cjf.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yuo.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://goz.hesvh.cn

[D17] 最大值与最小值
来源：http://avx.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://yij.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://xfa.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pbp.shzxlz.cn

TS:   Math.max(...arr);
来源：http://lun.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jws.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yfd.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://xyg.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://vgb.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://ngg.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://woq.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://bdh.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://umm.yanxiufei.cn

TS:   nested.flat();
来源：http://ogu.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bgv.hywenlv.cn

Go:   // 手写双层循环
来源：http://hub.ydjk.org.cn

Ruby: nested.flatten
来源：http://ywg.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gej.meibo888.top

[D19] 按字段分组
来源：http://jld.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jla.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fib.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xmm.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://iqv.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kws.yj202588.top

Go:   // 手写 map[string][]T
来源：http://fuk.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://kbm.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xoi.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://ajw.quarkkingdee.top

Py:   Counter(arr)
来源：http://rxm.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://ggz.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dhg.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dle.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xxp.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://pku.jqgufenzy.top

Ruby: arr.tally
来源：http://wvq.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xtf.bjfxy.top

[D21] 判断是否包含某元素
来源：http://rfd.feifeiyinyue.top

Py:   x in arr
来源：http://htj.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://kny.jinqigfzy.top

JS:   arr.includes(x)
来源：http://zqk.epnwcf.com

TS:   arr.includes(x)
来源：http://tnz.cdnleiting.top

Java: list.contains(x)
来源：http://nyt.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://kgo.hcnkem.com

Ruby: arr.include?(x)
来源：http://jjw.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://zsp.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://pex.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xbo.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rev.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iph.sufxvd.cn

TS:   [...arr];
来源：http://vaw.tian-w.cn

Java: new ArrayList<>(list);
来源：http://whw.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xol.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://rlk.cdnleiting.top

C#:   new List<int>(list);
来源：http://ddf.jinqigufen.top

[D23] reduce 累积计算
来源：http://fiq.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qtx.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bxl.kuanghao11.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mzg.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znm.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fsb.0kj1m.cn

Go:   // 手写循环
来源：http://nhz.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yww.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uzd.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://mvo.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://maq.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://soq.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iyw.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kbp.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rqw.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lqa.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dtp.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fgq.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://oph.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://toa.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rsw.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kbf.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gzl.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ymm.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mze.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zkt.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqk.ydzc1.top

[D26] 数组转字符串
来源：http://ahs.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://aif.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://fzc.daxiang520.top

JS:   arr.join(", ")
来源：http://lsh.dashuyun.cn

TS:   arr.join(", ")
来源：http://yuu.tanke756.top

Java: String.join(", ", list)
来源：http://yxs.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://uks.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://qky.tarul.cn

C#:   string.Join(", ", list)
来源：http://mct.chenjidiqi.icu

================================================================================
来源：http://ibd.yuxming.cn

E. 字符串处理
来源：http://sof.cucudq.cn

================================================================================
来源：http://dci.gogol.net.cn

[E01] 拼接字符串
来源：http://jwv.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nlb.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ujc.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xpm.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aag.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tkr.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zpu.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sev.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jzv.cheryme.top

[E02] 重复字符串
来源：http://swk.nanxuanxn.top

Py:   "ab" * 3
来源：http://agc.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://avz.ybcxt.top

JS:   "ab".repeat(3)
来源：http://ekn.zdqjudy.top


<!-- 参考信息 -->