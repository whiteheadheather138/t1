代发 wailian999

[D03] 在指定位置插入元素
来源：http://tlt.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://kxb.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://opj.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hhz.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://dmf.bjfxy.top

Java: list.add(0, 0);
来源：http://knj.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://pad.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yhs.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://vsj.nanxuanxn.top

[D04] 删除元素
来源：http://jbw.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://odu.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qeo.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ixt.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://tvo.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mxr.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hmi.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rsy.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uoj.ydjk.org.cn

[D05] 访问与修改元素
来源：http://fgm.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sak.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://igl.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://phs.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://apl.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://vre.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://lxz.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sps.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qxb.epnwcf.com

[D06] 数组长度
来源：http://mfm.mhx1999.top

Py:   len(arr)
来源：http://nlq.ivvv.top

PHP:  count($arr);
来源：http://gvz.shangyingyoupin.top

JS:   arr.length
来源：http://vln.zhengqikj.top

TS:   arr.length
来源：http://oxn.yanxiufei.cn

Java: list.size();
来源：http://aoy.yongpay.top

Go:   len(arr)
来源：http://nvr.yfazqb.com

Ruby: arr.length; arr.size
来源：http://bqi.guowangkeji.top

C#:   list.Count;
来源：http://kug.ydzc1.top

[D07] 切片 / 取子数组
来源：http://ied.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fha.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://wbj.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://bkg.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://pft.yuanzhike.top

Java: list.subList(1, 4);
来源：http://lxa.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://fia.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://slj.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://rmz.fehbvm.com

[D08] 合并两个数组
来源：http://hpo.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://blv.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://lys.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://smq.jianghu66.top

TS:   [...a, ...b];
来源：http://ngw.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rlq.cucudq.cn

Go:   append(a, b...)
来源：http://vsr.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://pgn.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://czl.nanxinkj.top

[D09] 排序（升序）
来源：http://xfo.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://eid.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://ubi.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iry.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://hvi.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gku.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nse.haohaochexian.top

Ruby: arr.sort
来源：http://xyl.jinqigfzy.top

C#:   list.Sort();
来源：http://acs.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vlw.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qiu.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blj.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vnc.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pvi.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uwp.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cys.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dly.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qba.zhijiandao.cn

[D11] 反转数组
来源：http://ovc.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rwf.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://lxj.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tnx.bbcook.cn

TS:   [...arr].reverse();
来源：http://hnt.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://asb.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://edk.nanxinkj.top

Ruby: arr.reverse
来源：http://kkq.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://aub.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://opz.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://guw.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://roe.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ajp.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mtd.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fmu.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://cpr.nanxuanxn.top

Ruby: arr.index(x)
来源：http://jaw.fzhhl.top

C#:   list.IndexOf(x);
来源：http://mib.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://ubl.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iay.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sju.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://ons.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://vna.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://whi.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jbt.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yuv.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xvo.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://wab.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uwo.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fnp.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://igm.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://yyg.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nrz.quarkkingdee.top

Go:   // 手写循环
来源：http://pbi.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ius.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tye.yj20258.top

[D15] 去重
来源：http://wil.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cev.sxryk.cn

PHP:  array_unique($arr);
来源：http://fvh.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://wva.nwbrower.top

TS:   [...new Set(arr)]
来源：http://oax.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://anc.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://btc.ydzc1.top

Ruby: arr.uniq
来源：http://krj.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://ifz.gaohongyu789.top

[D16] 求和与平均值
来源：http://xzq.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nsw.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://frd.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ear.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gjn.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zmk.cucudq.cn

Go:   // 手写循环累加
来源：http://muq.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cip.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://rqt.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://orx.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://err.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://nhm.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gxi.hammf.cn

TS:   Math.max(...arr);
来源：http://fgq.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://nwq.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wqu.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://cvp.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://lcc.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://yrl.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kxu.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://rey.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cbm.ybcxt.top

TS:   nested.flat();
来源：http://hwq.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fgr.cheryme.top

Go:   // 手写双层循环
来源：http://nry.gogol.net.cn

Ruby: nested.flatten
来源：http://zof.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dqs.zhijiandao.cn

[D19] 按字段分组
来源：http://wtz.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wbn.0kj1m.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nmp.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bdy.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rek.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dbt.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://zgv.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vin.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://byp.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://cwu.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://xbr.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://nlm.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://epd.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://idj.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://anw.fzhhl.top

Go:   // 手写 map[T]int
来源：http://kgj.andypj.xyz

Ruby: arr.tally
来源：http://gps.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wjh.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://oqq.sufxvd.cn

Py:   x in arr
来源：http://zjy.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://efi.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://bms.chenlongwang.top

TS:   arr.includes(x)
来源：http://pmq.daria6918.cn

Java: list.contains(x)
来源：http://wda.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://zyk.cucudq.cn

Ruby: arr.include?(x)
来源：http://hph.tanke756.top

C#:   list.Contains(x)
来源：http://lfr.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://dbv.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nxu.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vax.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://duo.guowangkeji.top

TS:   [...arr];
来源：http://zwp.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://gsb.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://ufb.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://tnj.jqgufenzy.top

C#:   new List<int>(list);
来源：http://jcd.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://zvj.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dnc.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uir.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fgz.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qpz.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rbh.hywenlv.cn

Go:   // 手写循环
来源：http://wph.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://whu.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hno.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://sqq.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zzm.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bwd.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://thr.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nvy.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zdw.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gwz.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zbt.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://etj.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://yxo.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mzf.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aho.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ihs.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dgl.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qso.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qid.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://war.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zii.hfpthk.cn

[D26] 数组转字符串
来源：http://amv.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://vwe.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://xul.yfazqb.com

JS:   arr.join(", ")
来源：http://ntw.cashguo.top

TS:   arr.join(", ")
来源：http://xcd.jlsjyb.cn

Java: String.join(", ", list)
来源：http://kzl.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://uow.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://upe.andypj.xyz

C#:   string.Join(", ", list)
来源：http://vnr.sxryk.cn

================================================================================
来源：http://psn.fehbvm.com

E. 字符串处理
来源：http://abk.fehbvm.com

================================================================================
来源：http://gkd.chenjidiqi.icu

[E01] 拼接字符串
来源：http://pnt.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bls.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tei.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wsa.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pia.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cea.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dqg.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ude.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://crm.mhx1999.top

[E02] 重复字符串
来源：http://jxt.jyoumei.cn

Py:   "ab" * 3
来源：http://sws.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://zru.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://bgn.yj20258.top

TS:   "ab".repeat(3)
来源：http://vvr.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://sln.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://frv.316326.xyz

Ruby: "ab" * 3
来源：http://yyx.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://flx.52xcode.cn

[E03] 截取子串
来源：http://rln.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yhs.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cdh.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ygq.shuidangran.top

TS:   s.slice(1, 4)
来源：http://hav.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://tpi.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zgq.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ror.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://ody.daxiang520.top

[E04] 查找子串位置
来源：http://rkh.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://fvj.epnwcf.com

PHP:  strpos($s, "x");
来源：http://pso.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://igp.jiagoushi.top

TS:   s.indexOf("x")
来源：http://jgo.bjfxy.top

Java: s.indexOf("x")
来源：http://dfc.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://acf.xinyue.icu

Ruby: s.index("x")
来源：http://xul.yongpay.top

C#:   s.IndexOf("x")
来源：http://asy.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iuu.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ssh.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://imz.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgd.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ifq.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btb.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lrf.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kpd.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://icm.quarkkingdee.top

[E06] 替换子串
来源：http://igz.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://miy.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://qxh.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujs.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://ita.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://akv.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hlo.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mwc.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://osb.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://ebn.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://exr.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jqy.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bcx.fehbvm.com

TS:   s.split(",")
来源：http://xpj.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nvy.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zdu.cheryme.top

Ruby: s.split(",");  s.split
来源：http://yst.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kii.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://alr.ydzc1.top

Py:   ",".join(items)
来源：http://gvl.chenlongwang.top

PHP:  implode(",", $items);
来源：http://nrk.uphjek.com

JS:   items.join(",")
来源：http://rlv.quarkkingdee.top

TS:   items.join(",")
来源：http://ekt.zhongyouzk.top

Java: String.join(",", items)
来源：http://hri.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://fga.zycfv.cn

Ruby: items.join(",")
来源：http://qft.cqqwz.cn

C#:   string.Join(",", items)
来源：http://nso.ehwqpu.com

[E09] 去除所有空白字符
来源：http://pwx.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zcz.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wja.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://wnt.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://nfy.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://yjp.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://boz.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fhp.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yjh.ctjpmb.com


<!-- 参考信息 -->