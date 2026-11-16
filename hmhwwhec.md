代发 wailian999

C#:   list.Insert(0, 0);
来源：http://veu.birdmap.top

[D04] 删除元素
来源：http://qyf.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ncd.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pfj.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kpf.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://oxx.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ivk.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dtp.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qsg.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iuk.fzhhl.top

[D05] 访问与修改元素
来源：http://hhl.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uwn.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sqn.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lhm.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://efu.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://jii.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://sna.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://udk.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://umu.0kj1m.cn

[D06] 数组长度
来源：http://vuz.ehwqpu.com

Py:   len(arr)
来源：http://qvn.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://lke.feifeiyinyue.top

JS:   arr.length
来源：http://zlh.ppjwa.cn

TS:   arr.length
来源：http://swx.9152youxi.cn

Java: list.size();
来源：http://bsp.xziqi.cn

Go:   len(arr)
来源：http://ylm.bjfxy.top

Ruby: arr.length; arr.size
来源：http://cks.cqqwz.cn

C#:   list.Count;
来源：http://imj.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://unn.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vqw.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://imt.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://trn.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://caj.fzhhl.top

Java: list.subList(1, 4);
来源：http://opa.aibaodan.cn

Go:   arr[1:4]
来源：http://qcl.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://uea.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://sjl.svipenyu.cn

[D08] 合并两个数组
来源：http://rsh.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://ujd.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://fyo.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pkw.nwbrower.top

TS:   [...a, ...b];
来源：http://zux.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cun.vehdjk.com

Go:   append(a, b...)
来源：http://zaj.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://jeo.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://jvj.chenzaomai.com

[D09] 排序（升序）
来源：http://czd.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://xyn.chenjidiqi.icu

PHP:  sort($arr);
来源：http://jwe.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uih.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jdf.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kkz.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fvn.gotoacloud.top

Ruby: arr.sort
来源：http://klm.havefunace.top

C#:   list.Sort();
来源：http://ttl.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://fcy.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cmn.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wos.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wtt.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lmw.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lnz.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gfp.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jvf.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hki.xylfe.cn

[D11] 反转数组
来源：http://yih.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yuh.gzhubu.top

PHP:  array_reverse($arr);
来源：http://kyd.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fij.guowangkeji.top

TS:   [...arr].reverse();
来源：http://lvb.smart0.xyz

Java: Collections.reverse(list);
来源：http://dek.meibo888.top

Go:   slices.Reverse(arr)
来源：http://btn.jyoumei.cn

Ruby: arr.reverse
来源：http://ndz.hnxiangtu.top

C#:   list.Reverse();
来源：http://ofu.316326.xyz

[D12] 查找元素下标
来源：http://jbd.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://lfa.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vvt.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gni.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxe.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uft.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://vyy.jiagoushi.top

Ruby: arr.index(x)
来源：http://zyp.andypj.xyz

C#:   list.IndexOf(x);
来源：http://rsp.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://ixi.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ion.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yny.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://ima.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://aly.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ios.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ivd.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://bqh.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kye.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://fdd.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vwz.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://viy.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://yqt.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://rsi.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eeu.xuetiantiany.cn

Go:   // 手写循环
来源：http://ttf.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://dpd.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ikp.wangshuangyany.cn

[D15] 去重
来源：http://kjv.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://een.sxryk.cn

PHP:  array_unique($arr);
来源：http://wqb.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://csy.hnqzz.top

TS:   [...new Set(arr)]
来源：http://vla.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wsg.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://euk.nwbrower.top

Ruby: arr.uniq
来源：http://zlm.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://ypp.tianlin.xyz

[D16] 求和与平均值
来源：http://ouh.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wes.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ngx.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://get.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://msw.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bnf.mhx1999.top

Go:   // 手写循环累加
来源：http://dmh.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lok.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://qti.bjfxy.top

[D17] 最大值与最小值
来源：http://drb.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://kvm.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://vuy.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxq.yuxming.cn

TS:   Math.max(...arr);
来源：http://pta.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rrt.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fqy.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://nwi.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://lyu.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://rmg.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dea.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://rnt.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://afn.zhiwuduotai.top

TS:   nested.flat();
来源：http://vfv.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fov.gaohongyu789.top

Go:   // 手写双层循环
来源：http://zdk.daria6918.cn

Ruby: nested.flatten
来源：http://agl.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ggi.shanyushiyangtech.top

[D19] 按字段分组
来源：http://vdr.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bws.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iax.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dlz.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://pdu.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://afw.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://dha.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://qfx.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kpk.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://vgk.yueranfly.top

Py:   Counter(arr)
来源：http://vbs.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://tgc.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zhp.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://odv.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qej.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://lxf.pycfn.com

Ruby: arr.tally
来源：http://ffl.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ltg.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://kbv.shanyushiyangtech.top

Py:   x in arr
来源：http://pib.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://zbj.sysykeji.top

JS:   arr.includes(x)
来源：http://adl.jyoumei.cn

TS:   arr.includes(x)
来源：http://xpg.zycfv.cn

Java: list.contains(x)
来源：http://jpr.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://rdk.xinyue.icu

Ruby: arr.include?(x)
来源：http://zxn.snrcjt.cn

C#:   list.Contains(x)
来源：http://vix.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://qjk.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ivj.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cmg.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ial.smart0.xyz

TS:   [...arr];
来源：http://syy.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://rbu.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qdi.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://nmx.fzhhl.top

C#:   new List<int>(list);
来源：http://wja.tarul.cn

[D23] reduce 累积计算
来源：http://hru.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ilp.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tqe.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axr.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pii.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nyl.jiagoushi.top

Go:   // 手写循环
来源：http://bgs.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ffh.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kax.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://oqt.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jhr.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jrl.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bqn.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jwf.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qiy.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qzk.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fts.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yst.meibo888.top

[D25] Set 集合去重与交并差
来源：http://qjk.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jic.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fwn.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://czf.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ekm.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lnh.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nmg.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ozd.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hsz.hysaishi.cn

[D26] 数组转字符串
来源：http://bpu.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://ito.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://jmh.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://zwe.xuanzx.com

TS:   arr.join(", ")
来源：http://qjx.fzhhl.top

Java: String.join(", ", list)
来源：http://gus.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://kkq.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://ygz.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://ztd.xuanzx.com

================================================================================
来源：http://ujk.zhixingplan.top

E. 字符串处理
来源：http://afl.ydzc1.top

================================================================================
来源：http://otu.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://nvc.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fiy.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lqm.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sxj.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfw.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fsn.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bol.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tta.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://msz.cheryme.top

[E02] 重复字符串
来源：http://rvf.meibo888.top

Py:   "ab" * 3
来源：http://ryu.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://tsq.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://ofc.hesvh.cn

TS:   "ab".repeat(3)
来源：http://uiv.sufxvd.cn

Java: "ab".repeat(3)
来源：http://aqz.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://azk.chenzaomai.com

Ruby: "ab" * 3
来源：http://got.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gpf.sjlbkw.cn

[E03] 截取子串
来源：http://qlc.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oea.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fdp.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nop.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://shr.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://twr.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bvw.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://vng.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://zvr.redwolf501.top

[E04] 查找子串位置
来源：http://emt.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://peh.yj20258.top

PHP:  strpos($s, "x");
来源：http://nwb.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://saa.hnqzz.top

TS:   s.indexOf("x")
来源：http://auk.epnwcf.com

Java: s.indexOf("x")
来源：http://xap.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://vun.yj20258.top

Ruby: s.index("x")
来源：http://nus.tanke756.top

C#:   s.IndexOf("x")
来源：http://daj.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wsz.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lva.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://udu.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uak.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgh.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qbj.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xxl.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mnx.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xui.ywan-chungtsiang.top

[E06] 替换子串
来源：http://osx.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://akn.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://agg.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cyl.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://buk.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rix.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mee.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cwm.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://cmw.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://zvs.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bns.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vsi.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://stc.hfpthk.cn

TS:   s.split(",")
来源：http://klq.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://wgd.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sou.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://fut.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xbz.sysykeji.top

[E08] 数组按分隔符合并
来源：http://atm.shzxlz.cn

Py:   ",".join(items)
来源：http://elt.aizwys.cn

PHP:  implode(",", $items);
来源：http://zcf.chenzaomai.com

JS:   items.join(",")
来源：http://gbi.cqqwz.cn

TS:   items.join(",")
来源：http://cyg.chenlongwang.top

Java: String.join(",", items)
来源：http://gfx.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://xtc.quarkkingdee.top

Ruby: items.join(",")
来源：http://lmq.yuanzhike.top

C#:   string.Join(",", items)
来源：http://wny.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://ayz.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xhz.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcd.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://euh.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://sno.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://arw.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://btt.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://fsi.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ltj.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://oks.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pwc.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dmo.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://tfh.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://mmr.xziqi.cn

Java: String.format("%03d", 7)
来源：http://cbq.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://rct.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yej.316326.xyz


<!-- 参考信息 -->