代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fch.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cjs.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bog.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vzr.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://wfi.yueranfly.top

Go:   func add(a, b int) int
来源：http://ogf.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yna.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://hap.hongshengwenyu.top

[C14] 泛型函数
来源：http://acq.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iog.jqgufenzy.top

PHP:  // 无泛型
来源：http://frw.316326.xyz

JS:   // 无泛型
来源：http://awx.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vap.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://enk.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ldj.aizwys.cn

Ruby: # 无泛型
来源：http://lje.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lly.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://evy.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dpn.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://wfn.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dax.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rra.zhijiandao.cn

Java: // 无解构
来源：http://yqc.chenjidiqi.icu

Go:   // 无解构
来源：http://mcd.cqqwz.cn

Ruby: a, b = pair
来源：http://psc.hnxiangtu.top

C#:   var (a, b) = pair;
来源：http://pcl.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://ezf.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vpx.epnwcf.com

PHP:  // 无重载
来源：http://kid.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mjy.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://tfk.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bsj.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://iyg.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://afh.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vei.chenlongwang.top

================================================================================
来源：http://nwa.havefunace.top

D. 数组 / 列表 / 集合
来源：http://qui.gzhubu.top

================================================================================
来源：http://wmo.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://pxc.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nqg.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ebi.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xvi.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zcv.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jxa.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://tmp.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://tzx.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://izq.dianchejie.cn

[D02] 追加元素到末尾
来源：http://zax.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://voo.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vph.svipenyu.cn

JS:   arr.push(4);
来源：http://jwm.hnxiangtu.top

TS:   arr.push(4);
来源：http://ant.shanyushiyangtech.top

Java: list.add(4);
来源：http://ywd.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://ahz.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://ttv.52xcode.cn

C#:   list.Add(4);
来源：http://rbh.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://jmj.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://rax.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rff.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://upb.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://yfd.guannengcc.top

Java: list.add(0, 0);
来源：http://fvb.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ipv.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mhl.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://isn.9152youxi.cn

[D04] 删除元素
来源：http://hke.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ivf.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://naa.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nym.tanke756.top

TS:   arr.splice(0, 1);
来源：http://eoq.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ccb.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qme.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mgx.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://omi.xylfe.cn

[D05] 访问与修改元素
来源：http://wjl.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qgx.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sgm.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zce.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://feu.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://lqv.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://prv.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ukt.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uzp.dianchejie.cn

[D06] 数组长度
来源：http://jpl.daria6918.cn

Py:   len(arr)
来源：http://bnf.yj20258888.top

PHP:  count($arr);
来源：http://zji.ydzc1.top

JS:   arr.length
来源：http://dex.havefunace.top

TS:   arr.length
来源：http://yaq.jqgfzy.top

Java: list.size();
来源：http://nuy.xylfe.cn

Go:   len(arr)
来源：http://xfo.havefunace.top

Ruby: arr.length; arr.size
来源：http://dql.yj20258888.top

C#:   list.Count;
来源：http://fol.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://xtc.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qtg.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mku.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://ung.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://nio.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://rdx.tian-w.cn

Go:   arr[1:4]
来源：http://qko.shzxlz.cn

Ruby: arr[1, 3]
来源：http://fdx.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://jic.gzhubu.top

[D08] 合并两个数组
来源：http://frk.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://izd.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://fbz.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://krv.gotoacloud.top

TS:   [...a, ...b];
来源：http://xbz.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hsi.zdqjudy.top

Go:   append(a, b...)
来源：http://mut.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://cyn.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://roy.zhengqikj.top

[D09] 排序（升序）
来源：http://zsi.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://yhd.gogol.net.cn

PHP:  sort($arr);
来源：http://pqf.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hmz.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ygy.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mbi.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kzl.tarul.cn

Ruby: arr.sort
来源：http://ibu.birdmap.top

C#:   list.Sort();
来源：http://dhq.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bns.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zfd.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vmq.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwk.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zul.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cbp.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ohx.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mcs.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mox.zhaomingkeji.xyz

[D11] 反转数组
来源：http://rib.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ajd.yueranfly.top

PHP:  array_reverse($arr);
来源：http://mzz.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pxt.ppjwa.cn

TS:   [...arr].reverse();
来源：http://whz.tian-w.cn

Java: Collections.reverse(list);
来源：http://inv.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://kwh.snrcjt.cn

Ruby: arr.reverse
来源：http://zkx.sysykeji.top

C#:   list.Reverse();
来源：http://zsv.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://jrs.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://zde.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bmn.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://elr.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vtv.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qqk.ivvv.top

Go:   slices.Index(arr, x)
来源：http://ofw.iojbl.cn

Ruby: arr.index(x)
来源：http://hou.hnqzz.top

C#:   list.IndexOf(x);
来源：http://dsb.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://uin.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iwz.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nkp.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://poe.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://def.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kzb.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://njq.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://kfk.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ocu.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://uyi.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ydl.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wjf.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://dso.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://xdm.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zzk.feifeiyinyue.top

Go:   // 手写循环
来源：http://njz.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://mbz.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qlz.zhixingplan.top

[D15] 去重
来源：http://gcq.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fmv.nwbrower.top

PHP:  array_unique($arr);
来源：http://aeb.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://rrs.birdmap.top

TS:   [...new Set(arr)]
来源：http://wdo.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yoa.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://vme.zdqjudy.top

Ruby: arr.uniq
来源：http://rcw.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://qbd.zhixingplan.top

[D16] 求和与平均值
来源：http://muo.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://utk.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ujm.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yfu.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdv.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fhy.daria6918.cn

Go:   // 手写循环累加
来源：http://hqb.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fhu.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://wns.jianghu66.top

[D17] 最大值与最小值
来源：http://bmu.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://prk.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://qyp.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dvh.ydzc1.top

TS:   Math.max(...arr);
来源：http://jzg.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lem.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hyq.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://jes.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://aqz.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://jdz.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lyp.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://uex.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vrm.ppjwa.cn

TS:   nested.flat();
来源：http://jyw.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rir.sxryk.cn

Go:   // 手写双层循环
来源：http://fdi.cashguo.top

Ruby: nested.flatten
来源：http://bus.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://ugm.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://gqo.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://whb.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nas.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://csx.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jcn.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jhw.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://fsg.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fdw.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cyj.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://tuj.ivvv.top

Py:   Counter(arr)
来源：http://cfj.birdmap.top

PHP:  array_count_values($arr);
来源：http://nmu.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ano.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tma.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ofl.cucudq.cn

Go:   // 手写 map[T]int
来源：http://edx.gaohongyu789.top

Ruby: arr.tally
来源：http://jip.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mdd.yuxming.cn

[D21] 判断是否包含某元素
来源：http://lrz.c1oappe.top

Py:   x in arr
来源：http://ifg.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://wzv.nanxinkj.top

JS:   arr.includes(x)
来源：http://hyz.yuxming.cn

TS:   arr.includes(x)
来源：http://fus.ivvv.top

Java: list.contains(x)
来源：http://hmt.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://ham.redwolf501.top

Ruby: arr.include?(x)
来源：http://cyy.yj202588.top

C#:   list.Contains(x)
来源：http://mfl.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://csp.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rwg.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mve.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sua.cashguo.top

TS:   [...arr];
来源：http://xhg.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://mxw.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://coq.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://hrh.hnxiangtu.top

C#:   new List<int>(list);
来源：http://zrm.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://xpy.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ehb.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qzn.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmw.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sbi.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://pbg.snrcjt.cn

Go:   // 手写循环
来源：http://vpc.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zuf.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hfb.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://xpa.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rld.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://you.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nra.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ksl.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qfa.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ton.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ktu.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://imn.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://oyd.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://apv.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://grn.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ovg.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qnm.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dyw.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xjd.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jgl.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xhk.smart0.xyz

[D26] 数组转字符串
来源：http://puf.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://vco.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://thj.gaohongyu789.top

JS:   arr.join(", ")
来源：http://hbs.hnqzz.top

TS:   arr.join(", ")
来源：http://nra.iojbl.cn

Java: String.join(", ", list)
来源：http://cor.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://vyd.daria6918.cn

Ruby: arr.join(", ")
来源：http://byl.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://olx.fehbvm.com

================================================================================
来源：http://dai.hfpthk.cn

E. 字符串处理
来源：http://qsx.jinqigufen.top

================================================================================
来源：http://lwq.ivvv.top

[E01] 拼接字符串
来源：http://tsy.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yig.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://prg.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dkg.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ggw.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mmz.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://smy.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://suq.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pke.shangyingyoupin.top

[E02] 重复字符串
来源：http://uto.vehdjk.com

Py:   "ab" * 3
来源：http://lqq.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://jtk.nwbrower.top

JS:   "ab".repeat(3)
来源：http://mdc.wangdashe.top

TS:   "ab".repeat(3)
来源：http://ech.hfpthk.cn

Java: "ab".repeat(3)
来源：http://lsm.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://cvh.pycfn.com

Ruby: "ab" * 3
来源：http://cpq.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qnq.hongshengwenyu.top

[E03] 截取子串
来源：http://ghc.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://taw.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kxu.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cns.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://wuv.jqgfzy.top

Java: s.substring(1, 4)
来源：http://wkc.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sgn.daria6918.cn


<!-- 参考信息 -->