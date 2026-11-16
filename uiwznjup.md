代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://xcb.yangfankeji.com

TS:   [...a, ...b];
来源：http://pvf.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sxz.daxiang520.top

Go:   append(a, b...)
来源：http://pas.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://ffk.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://dhy.gaohongyu789.top

[D09] 排序（升序）
来源：http://don.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ynm.gzhubu.top

PHP:  sort($arr);
来源：http://ivh.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://omg.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://urz.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ofg.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iyz.zhiwuduotai.top

Ruby: arr.sort
来源：http://jhj.yvedp.cn

C#:   list.Sort();
来源：http://xmf.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ytd.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pnp.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xok.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpr.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ywq.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://swr.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://epk.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xab.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://grb.yanxiufei.cn

[D11] 反转数组
来源：http://hbo.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uhe.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://xwk.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dgq.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://opf.ctjpmb.com

Java: Collections.reverse(list);
来源：http://xhv.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://eai.andypj.xyz

Ruby: arr.reverse
来源：http://ooi.yj202588.top

C#:   list.Reverse();
来源：http://sqw.jinqigfzy.top

[D12] 查找元素下标
来源：http://eto.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://ihp.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dyr.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://slj.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nlw.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ybt.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://xrl.fktsv.cn

Ruby: arr.index(x)
来源：http://zky.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://gnq.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://dgs.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjk.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sjr.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://zso.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://rdp.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zcp.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fbl.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://qdf.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yay.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://pkx.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kzp.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://suh.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://vfb.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://jco.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fpr.chenlongwang.top

Go:   // 手写循环
来源：http://hzh.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://nmz.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iji.quarkkingdee.top

[D15] 去重
来源：http://qlf.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ffg.aizwys.cn

PHP:  array_unique($arr);
来源：http://rdh.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://jul.gzhubu.top

TS:   [...new Set(arr)]
来源：http://oua.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fgk.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://qqo.yuxming.cn

Ruby: arr.uniq
来源：http://jig.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://spd.jlsjyb.cn

[D16] 求和与平均值
来源：http://mgf.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://alx.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zod.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://btw.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cqr.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tmu.guannengcc.top

Go:   // 手写循环累加
来源：http://fdb.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bkt.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://wnd.haohaochexian.top

[D17] 最大值与最小值
来源：http://tto.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://uoe.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://gmd.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jtd.sweek.top

TS:   Math.max(...arr);
来源：http://fvr.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://qzj.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://csr.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://rmn.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://apb.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://fol.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dir.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://moh.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ehr.cdnleiting.top

TS:   nested.flat();
来源：http://kim.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vfm.nanxuanxn.top

Go:   // 手写双层循环
来源：http://ocl.ctjpmb.com

Ruby: nested.flatten
来源：http://fuf.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zoo.aizwys.cn

[D19] 按字段分组
来源：http://adw.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ytx.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qou.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sjp.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kgo.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zlj.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://ktj.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oss.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vzp.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://krc.havefunace.top

Py:   Counter(arr)
来源：http://vxu.316326.xyz

PHP:  array_count_values($arr);
来源：http://iwm.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gee.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xtr.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tst.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://cjs.sufxvd.cn

Ruby: arr.tally
来源：http://rke.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://csc.redwolf501.top

[D21] 判断是否包含某元素
来源：http://fhp.zycfv.cn

Py:   x in arr
来源：http://ldq.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://iee.chenzaomai.com

JS:   arr.includes(x)
来源：http://pgi.hesvh.cn

TS:   arr.includes(x)
来源：http://hxf.zhongyouzk.top

Java: list.contains(x)
来源：http://bnx.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://fwi.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://rxy.cqqwz.cn

C#:   list.Contains(x)
来源：http://fla.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://vxx.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vle.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gax.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vis.xylfe.cn

TS:   [...arr];
来源：http://zze.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://pbc.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://hhb.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://rrg.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://pfh.9152youxi.cn

[D23] reduce 累积计算
来源：http://kpz.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vgc.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vsn.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oel.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uwo.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fgc.daxiang520.top

Go:   // 手写循环
来源：http://awv.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mub.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uao.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://fno.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cfb.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uge.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otr.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dkf.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yke.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgm.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uzf.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bte.tarul.cn

[D25] Set 集合去重与交并差
来源：http://wse.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wjm.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mze.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pkk.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fae.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hnm.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rcz.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vme.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mdq.xuetiantiany.cn

[D26] 数组转字符串
来源：http://vxk.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://acv.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://tuu.vehdjk.com

JS:   arr.join(", ")
来源：http://vaj.yj202588.top

TS:   arr.join(", ")
来源：http://svc.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://hly.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://jmk.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://mrx.jianghu66.top

C#:   string.Join(", ", list)
来源：http://cdl.shanyushiyangtech.top

================================================================================
来源：http://dxn.sweek.top

E. 字符串处理
来源：http://dcn.zdqjudy.top

================================================================================
来源：http://pwp.gaohongyu789.top

[E01] 拼接字符串
来源：http://vfl.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cue.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ufz.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cds.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fid.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://smi.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aad.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kts.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://end.hnxiangtu.top

[E02] 重复字符串
来源：http://mwb.sweek.top

Py:   "ab" * 3
来源：http://qho.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://cvz.fehbvm.com

JS:   "ab".repeat(3)
来源：http://ibw.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://dib.daxiang520.top

Java: "ab".repeat(3)
来源：http://fqe.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://vui.vqdsnc.cn

Ruby: "ab" * 3
来源：http://ymi.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yky.shanyushiyangkeji.top

[E03] 截取子串
来源：http://hzj.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://odk.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qfs.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lys.cashguo.top

TS:   s.slice(1, 4)
来源：http://ejr.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://lvt.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rjc.0kj1m.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sgg.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://kuv.zhixingplan.top

[E04] 查找子串位置
来源：http://igc.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://ztn.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://bld.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qqn.sweek.top

TS:   s.indexOf("x")
来源：http://frr.smart0.xyz

Java: s.indexOf("x")
来源：http://ypu.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://sye.cdnleiting.top

Ruby: s.index("x")
来源：http://rwo.tian-w.cn

C#:   s.IndexOf("x")
来源：http://tnk.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ovf.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ere.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lkf.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jma.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://zvm.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zss.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ygn.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ior.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vqs.yuxming.cn

[E06] 替换子串
来源：http://nbn.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tbw.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://tve.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fid.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://tod.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tsw.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zhh.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://agc.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://cgj.zhixingplan.top

[E07] 按分隔符拆分
来源：http://gsu.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cmc.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hto.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://njv.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://ssx.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://xkx.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dez.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://vix.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rxk.xuanzx.com

[E08] 数组按分隔符合并
来源：http://nvt.nanxinkj.top

Py:   ",".join(items)
来源：http://gov.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://egm.hcnkem.com

JS:   items.join(",")
来源：http://eyw.cheryme.top

TS:   items.join(",")
来源：http://eae.xylfe.cn

Java: String.join(",", items)
来源：http://dcx.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://dzh.fengsongda.top

Ruby: items.join(",")
来源：http://iby.iojbl.cn

C#:   string.Join(",", items)
来源：http://ngq.zdbjq.cn

[E09] 去除所有空白字符
来源：http://vql.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vfz.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://get.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://amg.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://vpf.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://dns.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://oun.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://xuh.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://duu.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://bzn.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nok.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jqo.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://jzm.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://bsl.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://sfa.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vtv.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ryg.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cdu.zycfv.cn

[E11] 反转字符串
来源：http://xpb.uphjek.com

Py:   s[::-1]
来源：http://kot.hammf.cn

PHP:  strrev($s);
来源：http://thw.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://glg.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://fmf.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rbu.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bxy.yanxiufei.cn

Ruby: s.reverse
来源：http://mvf.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qej.meibo888.top

[E12] 统计某字符出现次数
来源：http://ukc.fktsv.cn

Py:   s.count("a")
来源：http://sem.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://pgz.hnqzz.top

JS:   s.split("a").length - 1
来源：http://smv.fehbvm.com

TS:   s.split("a").length - 1
来源：http://bix.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mvv.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://ecw.nanxinkj.top

Ruby: s.count("a")
来源：http://ezg.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://ixs.fengsongda.top

[E13] 逐字符遍历
来源：http://kld.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://prq.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wuv.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lvg.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xsy.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vrx.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rmk.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iip.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bvo.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://mmk.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jhd.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mba.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://way.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uvn.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rvl.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iru.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oex.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eya.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://gsc.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rmr.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uee.jianghu66.top


<!-- 参考信息 -->