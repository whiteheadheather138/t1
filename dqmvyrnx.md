代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://plf.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sij.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pba.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nns.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dbo.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://ljb.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lbw.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://adz.aibaodan.cn

[C14] 泛型函数
来源：http://lqt.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ipx.ivvv.top

PHP:  // 无泛型
来源：http://vbx.dianchejie.cn

JS:   // 无泛型
来源：http://sxv.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kcz.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oqq.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://exo.vehdjk.com

Ruby: # 无泛型
来源：http://vse.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uka.yonumen.top

[C15] 解构 / 展开参数
来源：http://xpo.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nfs.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://rnr.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pum.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uas.zdqjudy.top

Java: // 无解构
来源：http://eqs.wangdashe.top

Go:   // 无解构
来源：http://zku.quarkkingdee.top

Ruby: a, b = pair
来源：http://wrr.gzhubu.top

C#:   var (a, b) = pair;
来源：http://ccw.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://myj.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yhw.cheryme.top

PHP:  // 无重载
来源：http://kzn.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jkn.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://nsu.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ptt.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://yjr.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://xzp.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ftd.iojbl.cn

================================================================================
来源：http://gzl.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://rfv.jiagoushi.top

================================================================================
来源：http://uwl.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://wuu.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sfu.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fpr.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tie.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://thh.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zcv.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://ctt.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://mvo.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lrf.jyoumei.cn

[D02] 追加元素到末尾
来源：http://jlv.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mto.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://evv.zhengqikj.top

JS:   arr.push(4);
来源：http://dct.ydjk.org.cn

TS:   arr.push(4);
来源：http://ate.jianghu66.top

Java: list.add(4);
来源：http://rtr.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://xgn.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://ozc.0kj1m.cn

C#:   list.Add(4);
来源：http://xhg.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://flj.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://lnc.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uyv.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oll.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://bxl.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://okz.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dmu.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pbt.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://yyz.gogol.net.cn

[D04] 删除元素
来源：http://loh.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nrl.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hbz.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbv.yj20258.top

TS:   arr.splice(0, 1);
来源：http://gcj.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gpa.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://klv.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zmn.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xqr.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://ktp.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lxe.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ccg.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xmc.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ugp.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://paa.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://lmd.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xpk.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pil.aibaodan.cn

[D06] 数组长度
来源：http://dkc.wangdashe.top

Py:   len(arr)
来源：http://lkj.zhengqikj.top

PHP:  count($arr);
来源：http://ctj.aizwys.cn

JS:   arr.length
来源：http://hfa.zhoulong.xyz

TS:   arr.length
来源：http://qic.316326.xyz

Java: list.size();
来源：http://kte.jyoumei.cn

Go:   len(arr)
来源：http://qcd.xinyue.icu

Ruby: arr.length; arr.size
来源：http://lsp.ehwqpu.com

C#:   list.Count;
来源：http://ivb.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://pof.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gku.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://sxt.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://wvw.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://yuf.yj202588.top

Java: list.subList(1, 4);
来源：http://wck.cucudq.cn

Go:   arr[1:4]
来源：http://ism.0kj1m.cn

Ruby: arr[1, 3]
来源：http://vgk.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://isc.ydjk.org.cn

[D08] 合并两个数组
来源：http://ygi.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://kha.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://ycb.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dpd.jyoumei.cn

TS:   [...a, ...b];
来源：http://vec.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hvb.yj20258.top

Go:   append(a, b...)
来源：http://eby.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://tat.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://reh.andypj.xyz

[D09] 排序（升序）
来源：http://yju.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://yro.zhongyouzk.top

PHP:  sort($arr);
来源：http://nne.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ror.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uth.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lyj.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://umk.zycfv.cn

Ruby: arr.sort
来源：http://rzq.feifeiyinyue.top

C#:   list.Sort();
来源：http://bfu.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbw.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mlh.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hgk.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tnv.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sju.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bjg.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xrp.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dhc.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vck.0kj1m.cn

[D11] 反转数组
来源：http://jyg.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://unc.fehbvm.com

PHP:  array_reverse($arr);
来源：http://apl.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://clw.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://mxy.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://kkm.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://gqz.iojbl.cn

Ruby: arr.reverse
来源：http://uqw.9152youxi.cn

C#:   list.Reverse();
来源：http://rka.kuanghao11.cn

[D12] 查找元素下标
来源：http://rzr.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://weh.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jkv.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rge.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://amg.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dkb.pycfn.com

Go:   slices.Index(arr, x)
来源：http://xky.fengsongda.top

Ruby: arr.index(x)
来源：http://nen.hesvh.cn

C#:   list.IndexOf(x);
来源：http://fcm.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://ojl.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ndd.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pkc.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://aka.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://hgt.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ioy.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://brc.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://inq.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pca.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://euy.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fih.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fau.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://vay.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://wii.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hjk.gotoacloud.top

Go:   // 手写循环
来源：http://mgp.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://dso.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vke.316326.xyz

[D15] 去重
来源：http://ptb.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bon.chenzaomai.com

PHP:  array_unique($arr);
来源：http://hxk.gogol.net.cn

JS:   [...new Set(arr)]
来源：http://kof.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://xoe.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lbn.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://foe.shuidangran.top

Ruby: arr.uniq
来源：http://jxo.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://kra.hywenlv.cn

[D16] 求和与平均值
来源：http://zhp.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tgq.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vwp.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tyi.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yte.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tyl.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://rpz.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://imn.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://qzm.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://fgs.cheryme.top

Py:   max(arr);  min(arr)
来源：http://ghy.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://iif.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bnq.vehdjk.com

TS:   Math.max(...arr);
来源：http://tch.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xua.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xjp.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://jrb.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://vmj.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://jzp.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qlr.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://wgz.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ezx.uphjek.com

TS:   nested.flat();
来源：http://cdt.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ikg.ivvv.top

Go:   // 手写双层循环
来源：http://xvh.hnqzz.top

Ruby: nested.flatten
来源：http://bse.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kmz.fehbvm.com

[D19] 按字段分组
来源：http://dfs.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://afg.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vpc.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xdo.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tny.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dpl.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://mvo.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dci.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xcq.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://tha.guannengcc.top

Py:   Counter(arr)
来源：http://gop.fktsv.cn

PHP:  array_count_values($arr);
来源：http://chv.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lru.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iit.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cbb.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://awi.tarul.cn

Ruby: arr.tally
来源：http://ecq.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xki.yuxming.cn

[D21] 判断是否包含某元素
来源：http://orl.shangyingyoupin.top

Py:   x in arr
来源：http://xvm.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://bpv.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://aup.andypj.xyz

TS:   arr.includes(x)
来源：http://bbg.bbcook.cn

Java: list.contains(x)
来源：http://xhk.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://osu.birdmap.top

Ruby: arr.include?(x)
来源：http://uxj.ehwqpu.com

C#:   list.Contains(x)
来源：http://foa.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://uor.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bgn.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hxp.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fza.shzxlz.cn

TS:   [...arr];
来源：http://hoi.pycfn.com

Java: new ArrayList<>(list);
来源：http://bqm.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nwx.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://adx.havefunace.top

C#:   new List<int>(list);
来源：http://oex.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://eiv.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://syx.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tbc.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wra.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvo.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tuj.cdnleiting.top

Go:   // 手写循环
来源：http://ykv.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hfb.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lbs.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://hjw.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sea.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hdr.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hnd.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ltq.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://atc.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogb.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jry.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gft.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://ekb.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://njp.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qje.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lqy.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tvj.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ewi.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://snc.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qwy.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nvq.zhengqikj.top

[D26] 数组转字符串
来源：http://afz.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://tqi.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://jsk.meibo888.top

JS:   arr.join(", ")
来源：http://feb.yfazqb.com

TS:   arr.join(", ")
来源：http://osm.sweek.top

Java: String.join(", ", list)
来源：http://gwk.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://wbg.jqgfzy.top

Ruby: arr.join(", ")
来源：http://mcd.mhx1999.top

C#:   string.Join(", ", list)
来源：http://sys.c1oappe.top

================================================================================
来源：http://ktf.sufxvd.cn

E. 字符串处理
来源：http://aqg.tian-w.cn

================================================================================
来源：http://sqs.feifeiyinyue.top

[E01] 拼接字符串
来源：http://mlq.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qht.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://acj.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hzq.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mxm.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nqn.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vqt.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://djk.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gcr.feifeiyinyue.top

[E02] 重复字符串
来源：http://xzo.cheryme.top

Py:   "ab" * 3
来源：http://ixq.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://dbp.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://neu.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://tto.jyoumei.cn

Java: "ab".repeat(3)
来源：http://dnw.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://dkl.0kj1m.cn

Ruby: "ab" * 3
来源：http://ecl.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pxd.daria6918.cn

[E03] 截取子串
来源：http://yys.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wtx.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ybn.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://asu.tarul.cn

TS:   s.slice(1, 4)
来源：http://uax.gogol.net.cn

Java: s.substring(1, 4)
来源：http://bme.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tut.yfazqb.com


<!-- 参考信息 -->