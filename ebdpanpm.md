代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nif.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nlg.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vhq.dianchejie.cn

Ruby: # 无泛型
来源：http://pow.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iyz.yfazqb.com

[C15] 解构 / 展开参数
来源：http://yps.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uvl.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://ags.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yno.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://enz.xingfuxueyuan.xyz

Java: // 无解构
来源：http://ofj.yangfankeji.com

Go:   // 无解构
来源：http://kea.zdqjudy.top

Ruby: a, b = pair
来源：http://rnn.52xcode.cn

C#:   var (a, b) = pair;
来源：http://ygx.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://gor.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jms.zycfv.cn

PHP:  // 无重载
来源：http://apx.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oqp.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://ogc.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rhc.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://zpm.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://tgw.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fog.yangfankeji.com

================================================================================
来源：http://pdm.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://uch.pycfn.com

================================================================================
来源：http://hzl.jianghu66.top

[D01] 创建数组 / 列表
来源：http://qbu.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lcj.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fiq.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kli.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://gud.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oee.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://xxv.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://fpr.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jkf.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://xsf.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ogt.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mjz.guowangkeji.top

JS:   arr.push(4);
来源：http://byh.smart0.xyz

TS:   arr.push(4);
来源：http://zgg.snrcjt.cn

Java: list.add(4);
来源：http://nnm.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://pit.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://fbi.fzhhl.top

C#:   list.Add(4);
来源：http://igi.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://rif.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://wzz.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ewm.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://avs.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://hbs.nanxuanxn.top

Java: list.add(0, 0);
来源：http://kfo.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kmr.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jxt.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://zil.yj20258888.top

[D04] 删除元素
来源：http://xle.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ssp.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vaf.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vzy.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://ows.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nwe.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://azm.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xtb.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aee.jqgfzy.top

[D05] 访问与修改元素
来源：http://mbz.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qsj.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uht.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qtz.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://rci.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://bin.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://kql.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ogw.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mst.chenzaomai.com

[D06] 数组长度
来源：http://kec.uphjek.com

Py:   len(arr)
来源：http://bew.yj20258888.top

PHP:  count($arr);
来源：http://avq.cashguo.top

JS:   arr.length
来源：http://wgy.yonumen.top

TS:   arr.length
来源：http://mti.guannengcc.top

Java: list.size();
来源：http://qwb.sufxvd.cn

Go:   len(arr)
来源：http://ken.guannengcc.top

Ruby: arr.length; arr.size
来源：http://gbh.vehdjk.com

C#:   list.Count;
来源：http://uab.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://eit.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ked.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bhw.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://jty.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://foz.snrcjt.cn

Java: list.subList(1, 4);
来源：http://vok.xinyue.icu

Go:   arr[1:4]
来源：http://pmh.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://icm.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://dfd.tanke756.top

[D08] 合并两个数组
来源：http://icp.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://mdb.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://ytb.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iim.andypj.xyz

TS:   [...a, ...b];
来源：http://pad.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://swr.redwolf501.top

Go:   append(a, b...)
来源：http://wgm.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://lxo.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://fye.fehbvm.com

[D09] 排序（升序）
来源：http://rnr.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://azm.jiagoushi.top

PHP:  sort($arr);
来源：http://upd.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://abi.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hrp.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zty.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fln.fzhhl.top

Ruby: arr.sort
来源：http://nss.nanxuanxn.top

C#:   list.Sort();
来源：http://lwb.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yvd.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gss.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://idl.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oie.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hel.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fgk.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://txq.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vuc.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hky.316326.xyz

[D11] 反转数组
来源：http://pso.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://zhe.316326.xyz

PHP:  array_reverse($arr);
来源：http://qeg.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vox.jianghu66.top

TS:   [...arr].reverse();
来源：http://rih.cqqwz.cn

Java: Collections.reverse(list);
来源：http://mvp.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://sgt.cheryme.top

Ruby: arr.reverse
来源：http://emo.andypj.xyz

C#:   list.Reverse();
来源：http://hgk.hysaishi.cn

[D12] 查找元素下标
来源：http://sdv.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://gjb.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kqj.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://whe.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nwd.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vea.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://puv.pycfn.com

Ruby: arr.index(x)
来源：http://ing.yj20258888.top

C#:   list.IndexOf(x);
来源：http://nvi.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://hwe.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tsa.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tvy.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://apa.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://jey.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://smn.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gjv.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://duk.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yor.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://oar.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ocd.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fez.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://jim.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://qaz.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vsc.guowangkeji.top

Go:   // 手写循环
来源：http://pdl.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://dxe.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://grk.shanyushiyangkeji.top

[D15] 去重
来源：http://rlj.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://scg.fzhhl.top

PHP:  array_unique($arr);
来源：http://bnq.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://kcu.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://nwn.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lxe.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://iet.ydjk.org.cn

Ruby: arr.uniq
来源：http://vmp.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://foe.cqqwz.cn

[D16] 求和与平均值
来源：http://hda.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ssl.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ymd.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://itm.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzt.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wpr.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://rgn.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tdi.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://gik.svipenyu.cn

[D17] 最大值与最小值
来源：http://bnq.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://ptw.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://fgb.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ugg.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://dyg.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://veo.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jhf.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://qkn.hammf.cn

C#:   list.Max();  list.Min()
来源：http://bqs.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://tkn.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://meq.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://tcq.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jmx.yuxming.cn

TS:   nested.flat();
来源：http://ekp.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ujc.bbcook.cn

Go:   // 手写双层循环
来源：http://xqu.nanxuanxn.top

Ruby: nested.flatten
来源：http://hos.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ays.pycfn.com

[D19] 按字段分组
来源：http://ypk.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pzo.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ogo.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://llp.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://alz.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://txy.redwolf501.top

Go:   // 手写 map[string][]T
来源：http://edl.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dmx.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://exl.sweek.top

[D20] 统计每个元素出现次数
来源：http://crf.hcnkem.com

Py:   Counter(arr)
来源：http://ind.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://hqc.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nbd.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wrt.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://djf.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://tsg.nwbrower.top

Ruby: arr.tally
来源：http://hdm.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jik.xylfe.cn

[D21] 判断是否包含某元素
来源：http://sfm.52xcode.cn

Py:   x in arr
来源：http://vrx.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://guc.havefunace.top

JS:   arr.includes(x)
来源：http://slq.hysaishi.cn

TS:   arr.includes(x)
来源：http://ebb.zhongyouzk.top

Java: list.contains(x)
来源：http://zgt.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://uub.ctjpmb.com

Ruby: arr.include?(x)
来源：http://ynh.andypj.xyz

C#:   list.Contains(x)
来源：http://afe.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://ffc.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://khr.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bem.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jco.ehwqpu.com

TS:   [...arr];
来源：http://tsv.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://sat.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://yef.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://sbv.daria6918.cn

C#:   new List<int>(list);
来源：http://wju.yonumen.top

[D23] reduce 累积计算
来源：http://isi.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gid.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gfu.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sww.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fra.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aem.birdmap.top

Go:   // 手写循环
来源：http://snq.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gpp.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://osc.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://knc.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tbv.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yxx.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fzj.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bjx.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://imk.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://awm.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bsb.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zqj.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://tup.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gds.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oia.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vwp.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dkb.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wnb.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://asv.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://inl.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oax.chenjidiqi.icu

[D26] 数组转字符串
来源：http://voy.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://abd.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://dkp.yj20258888.top

JS:   arr.join(", ")
来源：http://sbu.yanxiufei.cn

TS:   arr.join(", ")
来源：http://rfi.yuanzhike.top

Java: String.join(", ", list)
来源：http://oxn.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://ksn.xinyue.icu

Ruby: arr.join(", ")
来源：http://uce.aizwys.cn

C#:   string.Join(", ", list)
来源：http://jza.fanxiaobao.xyz

================================================================================
来源：http://kzo.jinqigfzy.top

E. 字符串处理
来源：http://wxm.jqgfzy.top

================================================================================
来源：http://gtc.cashguo.top

[E01] 拼接字符串
来源：http://dhb.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wml.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baf.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kbr.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://boq.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mml.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kkw.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gwu.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://anc.meibo888.top

[E02] 重复字符串
来源：http://eah.andypj.xyz

Py:   "ab" * 3
来源：http://dvo.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://lqt.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://olu.yj202588.top

TS:   "ab".repeat(3)
来源：http://hsf.cucudq.cn

Java: "ab".repeat(3)
来源：http://yxy.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://imf.shuidangran.top

Ruby: "ab" * 3
来源：http://rwt.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rjc.guannengcc.top

[E03] 截取子串
来源：http://kvh.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfq.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dpz.cashguo.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fgf.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://bhz.andypj.xyz

Java: s.substring(1, 4)
来源：http://zli.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yik.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://akj.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://qta.sxryk.cn

[E04] 查找子串位置
来源：http://uyg.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://qrv.tarul.cn

PHP:  strpos($s, "x");
来源：http://akv.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://odw.tarul.cn

TS:   s.indexOf("x")
来源：http://fzl.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://xrw.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://ygm.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://ecl.c1oappe.top

C#:   s.IndexOf("x")
来源：http://xqi.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pjw.nwbrower.top


<!-- 参考信息 -->