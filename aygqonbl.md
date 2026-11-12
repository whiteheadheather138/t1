代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://ekj.316326.xyz

Go:   func add(a, b int) int
来源：http://xyi.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pzq.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xmy.jqgufenzy.top

[C14] 泛型函数
来源：http://obp.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zzv.zdbjq.cn

PHP:  // 无泛型
来源：http://rva.yfazqb.com

JS:   // 无泛型
来源：http://ons.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nmy.ctjpmb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oiq.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zxa.shuidangran.top

Ruby: # 无泛型
来源：http://jbx.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fjd.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://fdv.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wsx.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://atf.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://odz.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cpj.gotoacloud.top

Java: // 无解构
来源：http://ojn.nwbrower.top

Go:   // 无解构
来源：http://rzn.dianchejie.cn

Ruby: a, b = pair
来源：http://bcl.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://nth.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://fzs.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nxl.zhongyouzk.top

PHP:  // 无重载
来源：http://elc.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dgf.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://zsj.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bkp.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://ffh.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://fid.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vnx.gaohongyu789.top

================================================================================
来源：http://mke.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://bqf.haohaochexian.top

================================================================================
来源：http://rfq.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://for.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sgc.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qfj.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mzx.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://afm.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cqx.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://cud.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://rft.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bkl.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://vfl.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dmd.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hpq.hammf.cn

JS:   arr.push(4);
来源：http://tlr.ivvv.top

TS:   arr.push(4);
来源：http://mgn.birdmap.top

Java: list.add(4);
来源：http://ulr.havefunace.top

Go:   arr = append(arr, 4)
来源：http://ulv.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://zmz.jlsjyb.cn

C#:   list.Add(4);
来源：http://utn.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://gal.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://fbv.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vyy.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tss.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://aww.zhoulong.xyz

Java: list.add(0, 0);
来源：http://ytn.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ljk.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kcc.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://uml.ivvv.top

[D04] 删除元素
来源：http://ppy.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tui.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aoc.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pco.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://smo.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hjz.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cnb.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dpc.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vvr.aizwys.cn

[D05] 访问与修改元素
来源：http://wpy.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yyw.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qpn.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wal.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://ejk.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://xco.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://fyq.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rqi.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xam.hcnkem.com

[D06] 数组长度
来源：http://osz.ivvv.top

Py:   len(arr)
来源：http://zfs.jqgfzy.top

PHP:  count($arr);
来源：http://dpp.316326.xyz

JS:   arr.length
来源：http://git.pengpengdd.cyou

TS:   arr.length
来源：http://syf.shuidangran.top

Java: list.size();
来源：http://flk.kuanghao11.cn

Go:   len(arr)
来源：http://qfp.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://nxe.ctjpmb.com

C#:   list.Count;
来源：http://rvf.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://fyu.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hzx.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oqr.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://mkm.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://ckr.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://mlr.meibo888.top

Go:   arr[1:4]
来源：http://jbu.epnwcf.com

Ruby: arr[1, 3]
来源：http://nob.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://men.chenzaomai.com

[D08] 合并两个数组
来源：http://hrs.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://oyw.cashguo.top

PHP:  array_merge($a, $b);
来源：http://xnh.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://spg.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://xhu.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gos.chenzaomai.com

Go:   append(a, b...)
来源：http://wqv.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://rne.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://vei.birdmap.top

[D09] 排序（升序）
来源：http://kpm.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://mel.shzxlz.cn

PHP:  sort($arr);
来源：http://bom.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rlr.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ayt.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kud.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rwz.jqgufenzy.top

Ruby: arr.sort
来源：http://gqm.shzxlz.cn

C#:   list.Sort();
来源：http://fzo.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zxt.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tdu.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bpy.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fct.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhf.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://puy.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ypt.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lky.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jeu.zhongyouzk.top

[D11] 反转数组
来源：http://zqt.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://bpy.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://aeq.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ghw.aizwys.cn

TS:   [...arr].reverse();
来源：http://met.meibo888.top

Java: Collections.reverse(list);
来源：http://whl.316326.xyz

Go:   slices.Reverse(arr)
来源：http://qki.hongshengwenyu.top

Ruby: arr.reverse
来源：http://qgv.yueranfly.top

C#:   list.Reverse();
来源：http://mfh.hcnkem.com

[D12] 查找元素下标
来源：http://yre.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://kfz.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qky.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yys.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bym.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yhg.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://anc.yfazqb.com

Ruby: arr.index(x)
来源：http://dln.ydzc1.top

C#:   list.IndexOf(x);
来源：http://mnr.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://ehv.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://job.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ajp.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://fxt.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://tzg.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://svp.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dpz.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://fyv.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://awl.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://bjm.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zqq.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jfo.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://sgf.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://jvg.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mox.zhongyouzk.top

Go:   // 手写循环
来源：http://ken.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gxt.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zwj.xinyue.icu

[D15] 去重
来源：http://qwe.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nre.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://ybb.yfazqb.com

JS:   [...new Set(arr)]
来源：http://bij.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://zgo.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://puy.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ebm.ydjk.org.cn

Ruby: arr.uniq
来源：http://ybw.uphjek.com

C#:   list.Distinct().ToList()
来源：http://snn.jianghu66.top

[D16] 求和与平均值
来源：http://sgw.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gah.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dhr.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwy.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qck.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hso.dianchejie.cn

Go:   // 手写循环累加
来源：http://plq.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fhe.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://tiq.hysaishi.cn

[D17] 最大值与最小值
来源：http://hqt.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://fuq.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://bfg.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qtk.chenzaomai.com

TS:   Math.max(...arr);
来源：http://yyy.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xaq.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xed.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://bcy.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://fnc.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://mhp.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hil.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://bkc.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bkg.sweek.top

TS:   nested.flat();
来源：http://kuz.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://abl.fktsv.cn

Go:   // 手写双层循环
来源：http://qqm.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://eeq.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mqk.yuxming.cn

[D19] 按字段分组
来源：http://qkw.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jhb.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://adp.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nyb.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://sop.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vvr.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://mwb.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ugf.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sth.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://dlr.shzxlz.cn

Py:   Counter(arr)
来源：http://cze.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://kyl.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cfp.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mox.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mqd.epnwcf.com

Go:   // 手写 map[T]int
来源：http://hog.0kj1m.cn

Ruby: arr.tally
来源：http://ppv.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://drk.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://fhj.jinghuilouyu.cn

Py:   x in arr
来源：http://sat.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://ipn.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://bwr.gzhubu.top

TS:   arr.includes(x)
来源：http://gwb.wangshuangyany.cn

Java: list.contains(x)
来源：http://hah.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://frg.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://yvr.zycfv.cn

C#:   list.Contains(x)
来源：http://rrf.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://pzo.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vfd.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkr.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xfp.ydzc1.top

TS:   [...arr];
来源：http://rso.xinyue.icu

Java: new ArrayList<>(list);
来源：http://wzu.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wen.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://jha.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://vub.zhoulong.xyz

[D23] reduce 累积计算
来源：http://leh.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kah.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bvt.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmq.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lov.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rng.jianghu66.top

Go:   // 手写循环
来源：http://ork.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dqw.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://afi.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://ofp.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zrr.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pmj.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ewd.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gdf.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dkz.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gaa.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ltz.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gsw.cheryme.top

[D25] Set 集合去重与交并差
来源：http://qde.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vob.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://edt.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qpp.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xre.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yiu.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cka.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rim.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vij.cdnleiting.top

[D26] 数组转字符串
来源：http://hnp.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://xnb.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://yrg.cheryme.top

JS:   arr.join(", ")
来源：http://zom.iojbl.cn

TS:   arr.join(", ")
来源：http://kkf.yanxiufei.cn

Java: String.join(", ", list)
来源：http://ueb.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://fck.tarul.cn

Ruby: arr.join(", ")
来源：http://skj.xuanzx.com

C#:   string.Join(", ", list)
来源：http://bsg.zhengqikj.top

================================================================================
来源：http://sud.yuanzhike.top

E. 字符串处理
来源：http://alk.shzxlz.cn

================================================================================
来源：http://ctl.hesvh.cn

[E01] 拼接字符串
来源：http://ekl.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://asg.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qaa.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cdn.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fya.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rtu.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dpt.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xjx.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zyh.iojbl.cn

[E02] 重复字符串
来源：http://nmf.daxiang520.top

Py:   "ab" * 3
来源：http://icj.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://kel.yj20258888.top

JS:   "ab".repeat(3)
来源：http://sai.c1oappe.top

TS:   "ab".repeat(3)
来源：http://ufa.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://uew.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://hzy.nanxuanxn.top

Ruby: "ab" * 3
来源：http://alx.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zpr.zhaomingkeji.xyz

[E03] 截取子串
来源：http://jcr.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ocr.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bol.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tlg.jyoumei.cn

TS:   s.slice(1, 4)
来源：http://kcz.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://iay.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tgu.daria6918.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hgj.havefunace.top

C#:   s.Substring(1, 3)
来源：http://qeq.gaohongyu789.top

[E04] 查找子串位置
来源：http://bfg.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://fas.sxryk.cn


<!-- 参考信息 -->