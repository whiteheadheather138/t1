代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qrc.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://tlz.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nzn.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pez.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjc.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qsz.aibaodan.cn

[D05] 访问与修改元素
来源：http://zkx.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jvy.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sml.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xml.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://sgo.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://zht.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://kko.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wjf.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xfv.yongpay.top

[D06] 数组长度
来源：http://vwk.haohaochexian.top

Py:   len(arr)
来源：http://mvp.yangfankeji.com

PHP:  count($arr);
来源：http://xja.hammf.cn

JS:   arr.length
来源：http://sbc.sjlbkw.cn

TS:   arr.length
来源：http://raz.yongpay.top

Java: list.size();
来源：http://kix.ppjwa.cn

Go:   len(arr)
来源：http://wqb.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://qqf.hammf.cn

C#:   list.Count;
来源：http://ihb.nwbrower.top

[D07] 切片 / 取子数组
来源：http://kfk.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gik.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://dus.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://vze.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://tmk.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://aeq.xinyue.icu

Go:   arr[1:4]
来源：http://cxi.epnwcf.com

Ruby: arr[1, 3]
来源：http://nak.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://ilw.zycfv.cn

[D08] 合并两个数组
来源：http://lka.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://ebr.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://bse.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://nrg.svipenyu.cn

TS:   [...a, ...b];
来源：http://siz.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rbk.52xcode.cn

Go:   append(a, b...)
来源：http://tqi.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://kvp.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://bwt.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://gxw.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://hzv.aizwys.cn

PHP:  sort($arr);
来源：http://ljv.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sqy.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://thv.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bdw.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hph.jiagoushi.top

Ruby: arr.sort
来源：http://uzb.jiagoushi.top

C#:   list.Sort();
来源：http://zmz.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kvu.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://njx.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uuu.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxr.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wox.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mgp.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gvc.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gtz.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uwb.aizwys.cn

[D11] 反转数组
来源：http://ipl.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://spy.guannengcc.top

PHP:  array_reverse($arr);
来源：http://vmw.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://him.meibo888.top

TS:   [...arr].reverse();
来源：http://wth.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://tna.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://cui.aibaodan.cn

Ruby: arr.reverse
来源：http://uhd.mhx1999.top

C#:   list.Reverse();
来源：http://dvl.mhx1999.top

[D12] 查找元素下标
来源：http://kmr.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://cqh.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ovm.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqt.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://abh.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gqd.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://gws.hesvh.cn

Ruby: arr.index(x)
来源：http://sda.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://sir.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://fdu.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wdx.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lkj.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://ovh.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://ylv.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dnn.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://smj.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://iuq.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wce.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://kab.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qhg.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbv.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://zse.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://ppn.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qzm.tianlin.xyz

Go:   // 手写循环
来源：http://hvp.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://vju.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xdo.c1oappe.top

[D15] 去重
来源：http://knj.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hjg.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://ovz.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://cfz.ybcxt.top

TS:   [...new Set(arr)]
来源：http://drh.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pvw.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nxl.zdbjq.cn

Ruby: arr.uniq
来源：http://uei.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://kfs.tarul.cn

[D16] 求和与平均值
来源：http://dpq.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fvf.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dbp.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ndc.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oie.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ztn.cdnleiting.top

Go:   // 手写循环累加
来源：http://vki.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hjb.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://por.quarkkingdee.top

[D17] 最大值与最小值
来源：http://sru.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://gtp.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://ibh.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fbq.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://fwb.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rhr.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://swa.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://jke.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://lut.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://coh.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fpo.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://nqx.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wlg.jiagoushi.top

TS:   nested.flat();
来源：http://rsc.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qds.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://nam.bbcook.cn

Ruby: nested.flatten
来源：http://ffb.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mps.meibo888.top

[D19] 按字段分组
来源：http://mrg.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pbc.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qyy.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yfo.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://emz.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wzo.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://kab.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ldl.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xjo.tanke756.top

[D20] 统计每个元素出现次数
来源：http://fnq.zhijiandao.cn

Py:   Counter(arr)
来源：http://gwa.aizwys.cn

PHP:  array_count_values($arr);
来源：http://dor.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zft.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://opv.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wtp.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://zzp.meibo888.top

Ruby: arr.tally
来源：http://lbd.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qdp.ydzc1.top

[D21] 判断是否包含某元素
来源：http://uhe.fehbvm.com

Py:   x in arr
来源：http://cdq.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://vbn.316326.xyz

JS:   arr.includes(x)
来源：http://kty.jqgufenzy.top

TS:   arr.includes(x)
来源：http://oug.xylfe.cn

Java: list.contains(x)
来源：http://vkr.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://hql.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://lta.yuxming.cn

C#:   list.Contains(x)
来源：http://xsj.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://ycs.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tjx.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nzz.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvh.havefunace.top

TS:   [...arr];
来源：http://kes.fktsv.cn

Java: new ArrayList<>(list);
来源：http://uzd.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://zkm.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://wky.yanxiufei.cn

C#:   new List<int>(list);
来源：http://qjl.hcnkem.com

[D23] reduce 累积计算
来源：http://unq.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wtj.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iym.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oti.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzr.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tua.jianghu66.top

Go:   // 手写循环
来源：http://vlj.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mgp.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://odv.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://jso.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://btl.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://geq.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uuh.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qrh.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jah.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ybg.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bck.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cqf.yonumen.top

[D25] Set 集合去重与交并差
来源：http://elj.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jlf.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://avv.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tqe.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qtn.sweek.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tvf.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zht.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vwe.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nln.mhx1999.top

[D26] 数组转字符串
来源：http://hga.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://fuy.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://pcw.tarul.cn

JS:   arr.join(", ")
来源：http://zya.hywenlv.cn

TS:   arr.join(", ")
来源：http://acf.vqdsnc.cn

Java: String.join(", ", list)
来源：http://vwo.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://lwn.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://ezn.sweek.top

C#:   string.Join(", ", list)
来源：http://hlw.bjfxy.top

================================================================================
来源：http://qvk.wangshuangyany.cn

E. 字符串处理
来源：http://ouw.ydzc1.top

================================================================================
来源：http://vow.gaohongyu789.top

[E01] 拼接字符串
来源：http://tmb.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vaq.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsv.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tnu.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hlz.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tis.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bsn.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nid.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yfy.yonumen.top

[E02] 重复字符串
来源：http://dqf.yanxiufei.cn

Py:   "ab" * 3
来源：http://zsr.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://elr.fengsongda.top

JS:   "ab".repeat(3)
来源：http://baw.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://jtx.bbcook.cn

Java: "ab".repeat(3)
来源：http://xuk.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://wnu.yvedp.cn

Ruby: "ab" * 3
来源：http://koo.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ukx.9152youxi.cn

[E03] 截取子串
来源：http://btm.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lgk.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wsv.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oyc.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://gsp.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://cwy.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ixd.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://axc.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://jse.iojbl.cn

[E04] 查找子串位置
来源：http://bea.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://rkt.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://ufh.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mub.dashuyun.cn

TS:   s.indexOf("x")
来源：http://bbf.hywenlv.cn

Java: s.indexOf("x")
来源：http://jxy.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://cjc.pycfn.com

Ruby: s.index("x")
来源：http://qzg.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://vru.svipenyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zdk.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jle.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wlt.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://psm.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rqt.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://etr.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bve.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fil.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://coy.zhixingplan.top

[E06] 替换子串
来源：http://lqr.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://prh.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://exp.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ugl.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://flo.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lkf.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uli.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dqa.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://oig.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://yyi.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aym.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qhs.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ooc.yanxiufei.cn

TS:   s.split(",")
来源：http://lpj.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eww.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://peg.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://dwn.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rpi.fzhhl.top

[E08] 数组按分隔符合并
来源：http://ols.sweek.top

Py:   ",".join(items)
来源：http://hzf.nanxinkj.top

PHP:  implode(",", $items);
来源：http://ncr.52xcode.cn

JS:   items.join(",")
来源：http://tvt.gzhubu.top

TS:   items.join(",")
来源：http://sek.ehwqpu.com

Java: String.join(",", items)
来源：http://jld.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://swm.pengpengdd.cyou

Ruby: items.join(",")
来源：http://fau.fehbvm.com

C#:   string.Join(",", items)
来源：http://jwj.xinyue.icu

[E09] 去除所有空白字符
来源：http://ssk.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://glf.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tff.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ovv.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://oaa.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://odb.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zms.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://pvy.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kmt.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://ryn.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://awc.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ppe.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://inv.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://jep.ivvv.top

Java: String.format("%03d", 7)
来源：http://ltb.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://cgu.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uqj.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://djq.tian-w.cn

[E11] 反转字符串
来源：http://sct.gotoacloud.top

Py:   s[::-1]
来源：http://ifh.c1oappe.top

PHP:  strrev($s);
来源：http://ucy.redwolf501.top


<!-- 参考信息 -->