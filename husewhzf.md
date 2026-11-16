代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://mdk.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://vls.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://tqu.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tik.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://fng.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://own.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://glb.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://dss.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eug.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xqu.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jah.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ggt.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://hvj.havefunace.top

Go:   func add(a, b int) int
来源：http://hzi.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://inu.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://ocm.zhoulong.xyz

[C14] 泛型函数
来源：http://rhd.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sex.andypj.xyz

PHP:  // 无泛型
来源：http://jns.zdbjq.cn

JS:   // 无泛型
来源：http://hzn.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jhu.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dec.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://krq.gzhubu.top

Ruby: # 无泛型
来源：http://hos.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cco.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://wgi.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vnj.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://grq.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zwf.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mtz.ehwqpu.com

Java: // 无解构
来源：http://kpe.jinqigfzy.top

Go:   // 无解构
来源：http://cld.dianchejie.cn

Ruby: a, b = pair
来源：http://dve.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://rbw.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://acq.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://omy.316326.xyz

PHP:  // 无重载
来源：http://znx.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gmy.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://jeg.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ful.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://ctv.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://zma.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqw.yj20258.top

================================================================================
来源：http://gix.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://mbk.zdbjq.cn

================================================================================
来源：http://eif.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://cse.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vbi.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://idg.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vdz.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lbb.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vgl.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://zlw.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://kng.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://goc.xziqi.cn

[D02] 追加元素到末尾
来源：http://jeg.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hqo.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qbw.jlsjyb.cn

JS:   arr.push(4);
来源：http://pme.shzxlz.cn

TS:   arr.push(4);
来源：http://tvj.nwbrower.top

Java: list.add(4);
来源：http://som.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://hjj.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://bjm.yj202588.top

C#:   list.Add(4);
来源：http://obu.hnqzz.top

[D03] 在指定位置插入元素
来源：http://qzl.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://gie.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ify.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wiz.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://ifl.shzxlz.cn

Java: list.add(0, 0);
来源：http://sfz.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://spi.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://czf.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://wyt.yonumen.top

[D04] 删除元素
来源：http://qzy.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ipi.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kla.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wuc.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://chy.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://squ.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gkm.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xib.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tce.fehbvm.com

[D05] 访问与修改元素
来源：http://esj.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wup.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tvq.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aov.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://cvq.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ypx.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://fzp.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jqs.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vwr.nanxuanxn.top

[D06] 数组长度
来源：http://dvw.sjlbkw.cn

Py:   len(arr)
来源：http://lsn.zdqjudy.top

PHP:  count($arr);
来源：http://vli.dashuyun.cn

JS:   arr.length
来源：http://epc.kuanghao11.cn

TS:   arr.length
来源：http://mag.hfpthk.cn

Java: list.size();
来源：http://iuz.yuanzhike.top

Go:   len(arr)
来源：http://hwb.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://ckj.ydjk.org.cn

C#:   list.Count;
来源：http://otk.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://myj.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yki.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://hvg.pycfn.com

JS:   arr.slice(1, 4);
来源：http://nqd.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://ewr.guowangkeji.top

Java: list.subList(1, 4);
来源：http://cae.jqgfzy.top

Go:   arr[1:4]
来源：http://qmb.yfazqb.com

Ruby: arr[1, 3]
来源：http://odd.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://qva.tarul.cn

[D08] 合并两个数组
来源：http://vml.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://zfx.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://smi.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xig.jqgfzy.top

TS:   [...a, ...b];
来源：http://etq.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lbn.sjlbkw.cn

Go:   append(a, b...)
来源：http://yre.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://wbt.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://aof.hesvh.cn

[D09] 排序（升序）
来源：http://sqn.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rkt.zhixingplan.top

PHP:  sort($arr);
来源：http://rxg.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kly.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dhu.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://iiu.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hkc.zdbjq.cn

Ruby: arr.sort
来源：http://jcn.pycfn.com

C#:   list.Sort();
来源：http://rvn.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ugt.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lbv.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bvk.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://weh.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ods.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uhf.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sdh.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ueq.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wuy.52xcode.cn

[D11] 反转数组
来源：http://awo.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ydv.sweek.top

PHP:  array_reverse($arr);
来源：http://lvy.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ynr.gzhubu.top

TS:   [...arr].reverse();
来源：http://sqr.hcnkem.com

Java: Collections.reverse(list);
来源：http://fef.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://gzw.aibaodan.cn

Ruby: arr.reverse
来源：http://wuf.ydjk.org.cn

C#:   list.Reverse();
来源：http://lwc.wangshuangyany.cn

[D12] 查找元素下标
来源：http://jwi.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://hmf.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://juw.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pdq.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rtk.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kyy.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://wsa.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://rsb.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://biq.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://hdp.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tef.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cra.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://tfp.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://vxd.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gzi.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://typ.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://wpk.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://efr.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://dfs.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ulc.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eyj.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://tsd.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://yqw.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://qlo.snrcjt.cn

Go:   // 手写循环
来源：http://qjw.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iqe.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pev.chenlongwang.top

[D15] 去重
来源：http://qgt.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://equ.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://gzf.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://pzf.yj20258888.top

TS:   [...new Set(arr)]
来源：http://qbw.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dbh.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ind.xziqi.cn

Ruby: arr.uniq
来源：http://ujl.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://vse.hammf.cn

[D16] 求和与平均值
来源：http://rtn.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zik.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eup.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hld.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyp.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kyb.epnwcf.com

Go:   // 手写循环累加
来源：http://kjl.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pte.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://sqm.bjfxy.top

[D17] 最大值与最小值
来源：http://mqi.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://nrx.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://vxa.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ecz.jianghu66.top

TS:   Math.max(...arr);
来源：http://agq.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nfa.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://clt.ivvv.top

Ruby: arr.max;  arr.min
来源：http://glu.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://bni.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://srt.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://far.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://soi.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://guz.yuanzhike.top

TS:   nested.flat();
来源：http://rcl.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yni.xylfe.cn

Go:   // 手写双层循环
来源：http://tdy.epnwcf.com

Ruby: nested.flatten
来源：http://cde.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fqu.kuanghao11.cn

[D19] 按字段分组
来源：http://bcc.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nop.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jfd.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wkv.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ndp.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hju.birdmap.top

Go:   // 手写 map[string][]T
来源：http://cud.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dyx.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fzy.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://prw.hesvh.cn

Py:   Counter(arr)
来源：http://xje.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://srr.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bcv.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lvf.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bee.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://mmg.xylfe.cn

Ruby: arr.tally
来源：http://nvq.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jkm.andypj.xyz

[D21] 判断是否包含某元素
来源：http://ckg.yj202588.top

Py:   x in arr
来源：http://cyp.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://trw.nanxuanxn.top

JS:   arr.includes(x)
来源：http://hez.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://epz.hywenlv.cn

Java: list.contains(x)
来源：http://kte.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://uoe.cashguo.top

Ruby: arr.include?(x)
来源：http://ndo.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://zgl.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://dmj.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yus.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cqv.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zdb.ydjk.org.cn

TS:   [...arr];
来源：http://puc.shuidangran.top

Java: new ArrayList<>(list);
来源：http://vid.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://mxc.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://tck.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://rqs.fehbvm.com

[D23] reduce 累积计算
来源：http://ahj.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iht.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jzc.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmj.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kxz.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dmb.yj202588.top

Go:   // 手写循环
来源：http://tjb.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kuh.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bcy.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://cdy.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zuz.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hep.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ylr.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tlz.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jbh.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xzt.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xzg.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oua.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://eiy.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nxo.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dqm.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://izb.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kar.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zet.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hho.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zrw.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dyj.hysaishi.cn

[D26] 数组转字符串
来源：http://cyo.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://efa.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://fju.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://yhe.ybcxt.top

TS:   arr.join(", ")
来源：http://cpl.zhengqikj.top

Java: String.join(", ", list)
来源：http://mkb.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://eea.yj20258888.top

Ruby: arr.join(", ")
来源：http://fcd.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://wlk.pengpengdd.cyou

================================================================================
来源：http://aiv.hammf.cn

E. 字符串处理
来源：http://uxy.haohaochexian.top

================================================================================
来源：http://psb.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://ovd.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bme.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tis.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ggl.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlq.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mbc.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wcm.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yap.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kkh.andypj.xyz

[E02] 重复字符串
来源：http://mmn.sweek.top

Py:   "ab" * 3
来源：http://kei.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://kdg.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://kuw.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://brf.yangfankeji.com

Java: "ab".repeat(3)
来源：http://cbx.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://pwp.cqqwz.cn

Ruby: "ab" * 3
来源：http://pfq.hnqzz.top


<!-- 参考信息 -->