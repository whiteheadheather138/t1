代发 wailian999

Java: list.add(4);
来源：http://chv.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://kza.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://uma.cdnleiting.top

C#:   list.Add(4);
来源：http://mto.meibo888.top

[D03] 在指定位置插入元素
来源：http://dgd.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://gnj.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mcn.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bqq.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://zxq.jianghu66.top

Java: list.add(0, 0);
来源：http://yus.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://xti.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kwj.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://qiu.0kj1m.cn

[D04] 删除元素
来源：http://ibl.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://woy.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lwy.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cjt.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://sye.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kbz.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvw.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hpb.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uaw.svipenyu.cn

[D05] 访问与修改元素
来源：http://dlq.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tkr.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ulq.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ezp.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://wlf.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://ddk.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://sqs.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ela.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mfd.yongpay.top

[D06] 数组长度
来源：http://trm.bjfxy.top

Py:   len(arr)
来源：http://wlv.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://egu.dianchejie.cn

JS:   arr.length
来源：http://yfi.svipenyu.cn

TS:   arr.length
来源：http://zyx.cdnleiting.top

Java: list.size();
来源：http://hvl.ehwqpu.com

Go:   len(arr)
来源：http://ews.uphjek.com

Ruby: arr.length; arr.size
来源：http://qsx.iojbl.cn

C#:   list.Count;
来源：http://quo.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://eej.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://trv.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://evx.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://sob.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://agg.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://pin.andypj.xyz

Go:   arr[1:4]
来源：http://ehl.cashguo.top

Ruby: arr[1, 3]
来源：http://apq.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://qno.cucudq.cn

[D08] 合并两个数组
来源：http://uix.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://gqq.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://nne.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oga.gaohongyu789.top

TS:   [...a, ...b];
来源：http://rog.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hlq.yueranfly.top

Go:   append(a, b...)
来源：http://mhg.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://zss.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://nmi.feifeiyinyue.top

[D09] 排序（升序）
来源：http://spi.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://qql.nwbrower.top

PHP:  sort($arr);
来源：http://spb.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kzb.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ddk.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kmo.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ziu.zhongyouzk.top

Ruby: arr.sort
来源：http://ruq.ybcxt.top

C#:   list.Sort();
来源：http://hov.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vbx.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qvy.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aau.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmt.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://utn.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dxm.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hdk.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wpi.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://luz.chenzaomai.com

[D11] 反转数组
来源：http://arf.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tcp.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://uro.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ivf.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://jab.ppjwa.cn

Java: Collections.reverse(list);
来源：http://nux.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://dsm.0kj1m.cn

Ruby: arr.reverse
来源：http://azl.cdnleiting.top

C#:   list.Reverse();
来源：http://itg.hnxiangtu.top

[D12] 查找元素下标
来源：http://mcf.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://tkf.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iat.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cgy.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fcn.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sda.cheryme.top

Go:   slices.Index(arr, x)
来源：http://sfi.havefunace.top

Ruby: arr.index(x)
来源：http://wys.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://ydz.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://hhz.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ihg.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mrz.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://neh.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://cbr.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tpz.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vvf.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://scr.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wku.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://fgt.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://liw.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://htu.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://slr.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://coz.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://icd.chenzaomai.com

Go:   // 手写循环
来源：http://xcq.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://ofh.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zpo.daxiang520.top

[D15] 去重
来源：http://kbx.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nsf.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://ixz.xuanzx.com

JS:   [...new Set(arr)]
来源：http://rpy.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://wnm.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://faa.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xjp.nanxinkj.top

Ruby: arr.uniq
来源：http://gmd.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://uzk.hfpthk.cn

[D16] 求和与平均值
来源：http://zyh.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fal.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zoy.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://joj.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://csj.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://krs.wangdashe.top

Go:   // 手写循环累加
来源：http://npg.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mnt.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://jqk.guowangkeji.top

[D17] 最大值与最小值
来源：http://hzn.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://nfl.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://you.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oko.jiagoushi.top

TS:   Math.max(...arr);
来源：http://jnu.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ykm.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rki.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://dtq.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://psy.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://qrh.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ivt.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://eph.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://czi.quarkkingdee.top

TS:   nested.flat();
来源：http://qff.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hsa.9152youxi.cn

Go:   // 手写双层循环
来源：http://ebt.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://dnn.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dkj.gotoacloud.top

[D19] 按字段分组
来源：http://jdn.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://amy.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wkn.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ubq.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nwm.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mqz.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://any.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lbq.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zhz.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://qlc.cucudq.cn

Py:   Counter(arr)
来源：http://qoo.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://hwa.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nrk.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fll.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kti.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://cyl.zhiwuduotai.top

Ruby: arr.tally
来源：http://xti.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ttb.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://lso.xziqi.cn

Py:   x in arr
来源：http://tue.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://xyq.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://nbb.quarkkingdee.top

TS:   arr.includes(x)
来源：http://exj.jiagoushi.top

Java: list.contains(x)
来源：http://rgn.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://aza.shuidangran.top

Ruby: arr.include?(x)
来源：http://wtt.ppjwa.cn

C#:   list.Contains(x)
来源：http://vof.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://mfm.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jbs.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qxu.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvc.cqqwz.cn

TS:   [...arr];
来源：http://ouk.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://qrp.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hjo.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://ifs.tarul.cn

C#:   new List<int>(list);
来源：http://hjj.iojbl.cn

[D23] reduce 累积计算
来源：http://nyo.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gyu.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zif.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bee.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://btq.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oua.yangfankeji.com

Go:   // 手写循环
来源：http://xcl.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kbt.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://otm.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://amd.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yfz.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kud.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gag.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yff.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gty.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yhj.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jiq.ehwqpu.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aje.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://bmg.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://unn.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ijm.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://clr.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mmp.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://grr.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hlb.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iik.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oyq.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://etf.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://cfe.yonumen.top

PHP:  implode(", ", $arr);
来源：http://ipf.jqgfzy.top

JS:   arr.join(", ")
来源：http://lji.zhixingplan.top

TS:   arr.join(", ")
来源：http://wth.jlsjyb.cn

Java: String.join(", ", list)
来源：http://nhe.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://znj.pycfn.com

Ruby: arr.join(", ")
来源：http://ydl.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://elo.ppjwa.cn

================================================================================
来源：http://vsx.jiagoushi.top

E. 字符串处理
来源：http://pls.sufxvd.cn

================================================================================
来源：http://huv.hnqzz.top

[E01] 拼接字符串
来源：http://lar.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lkx.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nuj.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fbm.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndx.xuanzx.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rqe.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kiw.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://has.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ulu.yuanzhike.top

[E02] 重复字符串
来源：http://yzf.chenlongwang.top

Py:   "ab" * 3
来源：http://xnl.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://xtj.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://xfe.yonumen.top

TS:   "ab".repeat(3)
来源：http://guk.haohaochexian.top

Java: "ab".repeat(3)
来源：http://wkj.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://xlk.jyoumei.cn

Ruby: "ab" * 3
来源：http://ibc.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://twl.mhx1999.top

[E03] 截取子串
来源：http://sfr.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pqn.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ono.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wjb.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://lqo.daxiang520.top

Java: s.substring(1, 4)
来源：http://thh.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qxr.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zoh.yongpay.top

C#:   s.Substring(1, 3)
来源：http://bhe.gogol.net.cn

[E04] 查找子串位置
来源：http://imj.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://wjh.sjlbkw.cn

PHP:  strpos($s, "x");
来源：http://izc.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tap.gogol.net.cn

TS:   s.indexOf("x")
来源：http://cte.ivvv.top

Java: s.indexOf("x")
来源：http://ver.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://dqy.redwolf501.top

Ruby: s.index("x")
来源：http://ror.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://fnh.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iuy.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cjg.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cys.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bvm.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wze.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mka.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qjv.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://izw.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tjz.c1oappe.top

[E06] 替换子串
来源：http://enj.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ixi.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://ies.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fzm.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://myr.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sgo.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nyx.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jyp.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://czf.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://vyd.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fjl.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aap.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ftj.52xcode.cn

TS:   s.split(",")
来源：http://ulx.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://idz.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ugz.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://aqj.hywenlv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvt.aizwys.cn

[E08] 数组按分隔符合并
来源：http://ogu.zhengqikj.top

Py:   ",".join(items)
来源：http://ulw.aibaodan.cn

PHP:  implode(",", $items);
来源：http://uge.52xcode.cn

JS:   items.join(",")
来源：http://lef.zhengqikj.top

TS:   items.join(",")
来源：http://jwn.zdbjq.cn

Java: String.join(",", items)
来源：http://pde.yj20258.top

Go:   strings.Join(items, ",")
来源：http://dbu.daria6918.cn

Ruby: items.join(",")
来源：http://ldw.316326.xyz

C#:   string.Join(",", items)
来源：http://fia.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://sek.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xsh.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dfq.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://dba.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://tbm.yj20258888.top


<!-- 参考信息 -->