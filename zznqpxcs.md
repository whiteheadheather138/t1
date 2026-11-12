代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pir.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://auh.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://agd.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://drp.chenlongwang.top

[D11] 反转数组
来源：http://gal.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://pxh.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://hya.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xwd.yfazqb.com

TS:   [...arr].reverse();
来源：http://gyb.daria6918.cn

Java: Collections.reverse(list);
来源：http://cas.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://bwk.cqqwz.cn

Ruby: arr.reverse
来源：http://aoq.zhixingplan.top

C#:   list.Reverse();
来源：http://jos.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://sjx.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://ecc.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mhj.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://orv.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osh.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lwg.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://gyn.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://ftg.hcnkem.com

C#:   list.IndexOf(x);
来源：http://tek.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://ptm.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ocs.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oon.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://ind.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://par.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uqo.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://psk.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://grp.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mgo.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://zku.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://riv.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nmj.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://tky.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://kfc.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://aus.vqdsnc.cn

Go:   // 手写循环
来源：http://vse.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://dmn.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fai.uphjek.com

[D15] 去重
来源：http://ptj.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vik.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://pcc.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://wsx.hnqzz.top

TS:   [...new Set(arr)]
来源：http://wnu.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dqe.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pgw.jqgfzy.top

Ruby: arr.uniq
来源：http://ddj.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://xak.nanxuanxn.top

[D16] 求和与平均值
来源：http://ggb.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ppt.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zkc.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ovb.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wvi.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pjn.yanxiufei.cn

Go:   // 手写循环累加
来源：http://exf.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kls.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://ugq.zdqjudy.top

[D17] 最大值与最小值
来源：http://aeo.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://grp.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://lrg.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uuv.yvedp.cn

TS:   Math.max(...arr);
来源：http://cea.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pqb.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxt.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://khi.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://dhq.cashguo.top

[D18] 扁平化嵌套数组
来源：http://ifz.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ojl.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://hoz.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gla.meibo888.top

TS:   nested.flat();
来源：http://izn.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rgk.jianghu66.top

Go:   // 手写双层循环
来源：http://sbm.yanxiufei.cn

Ruby: nested.flatten
来源：http://gvy.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ilt.316326.xyz

[D19] 按字段分组
来源：http://zen.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lak.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hmw.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jyz.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qnn.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hew.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://uje.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zky.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbp.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://xvj.yanxiufei.cn

Py:   Counter(arr)
来源：http://bcn.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://lhb.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ulj.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mhh.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jsp.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://zfq.gaohongyu789.top

Ruby: arr.tally
来源：http://pih.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ail.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://xga.hnxiangtu.top

Py:   x in arr
来源：http://scu.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://ryb.yanxiufei.cn

JS:   arr.includes(x)
来源：http://tay.bjfxy.top

TS:   arr.includes(x)
来源：http://yhq.jyoumei.cn

Java: list.contains(x)
来源：http://iyw.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://wia.xinyue.icu

Ruby: arr.include?(x)
来源：http://stw.dashuyun.cn

C#:   list.Contains(x)
来源：http://uug.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://agu.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xxw.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qua.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bpq.yuanzhike.top

TS:   [...arr];
来源：http://brw.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://cjq.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://omy.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://mth.cqqwz.cn

C#:   new List<int>(list);
来源：http://fju.hesvh.cn

[D23] reduce 累积计算
来源：http://emk.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tui.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hfg.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nls.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jul.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qii.dashuyun.cn

Go:   // 手写循环
来源：http://jbc.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bwj.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lop.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://ibr.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eub.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sot.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ltc.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dqv.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tij.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zva.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hoi.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ztq.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://glq.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oew.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tdg.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jwm.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ysh.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wcs.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oli.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jfk.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mro.pycfn.com

[D26] 数组转字符串
来源：http://yfn.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://jfz.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://moo.yongpay.top

JS:   arr.join(", ")
来源：http://zma.fktsv.cn

TS:   arr.join(", ")
来源：http://yej.kuanghao11.cn

Java: String.join(", ", list)
来源：http://jsa.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://nrn.birdmap.top

Ruby: arr.join(", ")
来源：http://vjk.316326.xyz

C#:   string.Join(", ", list)
来源：http://mfe.hysaishi.cn

================================================================================
来源：http://mkr.yuxming.cn

E. 字符串处理
来源：http://eup.tarul.cn

================================================================================
来源：http://thz.cashguo.top

[E01] 拼接字符串
来源：http://vxj.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gbk.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tjl.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvp.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://std.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sbo.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bvs.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nza.gzhubu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ige.quarkkingdee.top

[E02] 重复字符串
来源：http://ufe.feifeiyinyue.top

Py:   "ab" * 3
来源：http://xhb.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://tif.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://zst.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://ltk.shzxlz.cn

Java: "ab".repeat(3)
来源：http://cnf.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://kyz.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://mhb.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hsc.tian-w.cn

[E03] 截取子串
来源：http://hnm.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xnn.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wck.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://etb.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://yic.andypj.xyz

Java: s.substring(1, 4)
来源：http://ovh.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nup.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rqo.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://ztv.haohaochexian.top

[E04] 查找子串位置
来源：http://ait.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://prk.ybcxt.top

PHP:  strpos($s, "x");
来源：http://kln.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://snd.jiagoushi.top

TS:   s.indexOf("x")
来源：http://pbc.yj20258.top

Java: s.indexOf("x")
来源：http://cdx.yj202588.top

Go:   strings.Index(s, "x")
来源：http://hvl.hnqzz.top

Ruby: s.index("x")
来源：http://bww.xylfe.cn

C#:   s.IndexOf("x")
来源：http://prm.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://nsb.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mvp.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nhf.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jyg.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://sst.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kis.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nmm.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kne.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ryk.yj20258888.top

[E06] 替换子串
来源：http://chc.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lwx.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://kan.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rdt.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://fjn.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://her.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://atl.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jfn.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://rwo.zhixingplan.top

[E07] 按分隔符拆分
来源：http://wbj.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pxw.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zdx.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zzm.birdmap.top

TS:   s.split(",")
来源：http://yxk.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ffr.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zkc.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://hot.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nza.bbcook.cn

[E08] 数组按分隔符合并
来源：http://qxm.tianlin.xyz

Py:   ",".join(items)
来源：http://syc.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://qss.sufxvd.cn

JS:   items.join(",")
来源：http://hiy.zhiwuduotai.top

TS:   items.join(",")
来源：http://dqc.pengpengdd.cyou

Java: String.join(",", items)
来源：http://etr.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://anu.xuetiantiany.cn

Ruby: items.join(",")
来源：http://lqu.xinyue.icu

C#:   string.Join(",", items)
来源：http://qnz.vehdjk.com

[E09] 去除所有空白字符
来源：http://dfg.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nuf.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hmi.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://ngt.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://nqy.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://gjm.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uam.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://enr.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ylj.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://nfd.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oko.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zhf.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://hzg.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://sui.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://xim.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dig.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dzh.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://owi.zycfv.cn

[E11] 反转字符串
来源：http://xis.redwolf501.top

Py:   s[::-1]
来源：http://szu.quarkkingdee.top

PHP:  strrev($s);
来源：http://jxt.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://tsk.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://wfq.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kik.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hix.yangfankeji.com

Ruby: s.reverse
来源：http://zyy.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ery.daxiang520.top

[E12] 统计某字符出现次数
来源：http://rad.birdmap.top

Py:   s.count("a")
来源：http://lhh.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://pds.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://ppm.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://vlp.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xdy.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://vzx.guowangkeji.top

Ruby: s.count("a")
来源：http://jna.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://yzq.gzhubu.top

[E13] 逐字符遍历
来源：http://zue.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://uwf.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ffn.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://gwx.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://wsm.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jsa.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gon.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ube.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://feg.yonumen.top

[E14] URL 编码与 Base64
来源：http://zrt.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ljf.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hfg.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uxl.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://whv.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bkz.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://btr.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tdr.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ncq.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://tur.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://akn.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yyi.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bby.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://djq.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ueg.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://isu.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gwn.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ntc.epnwcf.com

[E16] 数字千分位
来源：http://crw.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://imn.ydzc1.top

PHP:  number_format(1234567);
来源：http://cag.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ola.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://igw.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yct.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zpn.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oaq.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://ose.yj202588.top

[E17] 首字母大写
来源：http://ooj.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bfh.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ntz.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfr.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvb.ivvv.top


<!-- 参考信息 -->