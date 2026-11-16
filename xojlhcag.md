代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jth.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://idn.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fyo.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://die.0kj1m.cn

Ruby: arr.index(x)
来源：http://ytq.jianghu66.top

C#:   list.IndexOf(x);
来源：http://mqd.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://owv.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rgh.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qma.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://bzs.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://yid.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bcf.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pvg.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zat.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hge.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://qxy.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dak.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vrt.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://vwu.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://gme.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ypf.sjlbkw.cn

Go:   // 手写循环
来源：http://kzn.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://vze.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://whs.zdqjudy.top

[D15] 去重
来源：http://ljb.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://scp.sweek.top

PHP:  array_unique($arr);
来源：http://hzh.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://bow.jianghu66.top

TS:   [...new Set(arr)]
来源：http://don.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lgp.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://gpz.shangyingyoupin.top

Ruby: arr.uniq
来源：http://gge.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://owp.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://edt.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rvp.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hgc.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://heb.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://npp.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tpu.quarkkingdee.top

Go:   // 手写循环累加
来源：http://rsc.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ukh.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://cgp.fehbvm.com

[D17] 最大值与最小值
来源：http://ktw.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://dyl.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://jsa.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vqs.c1oappe.top

TS:   Math.max(...arr);
来源：http://xvb.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ugk.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://asv.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://hko.tarul.cn

C#:   list.Max();  list.Min()
来源：http://xvx.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://xvf.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://llr.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://vyp.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jnu.xylfe.cn

TS:   nested.flat();
来源：http://qin.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dwc.hywenlv.cn

Go:   // 手写双层循环
来源：http://jzn.guowangkeji.top

Ruby: nested.flatten
来源：http://ivl.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fuw.ctjpmb.com

[D19] 按字段分组
来源：http://whs.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gjh.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yjs.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://huv.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qan.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kxb.uphjek.com

Go:   // 手写 map[string][]T
来源：http://knl.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cba.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rfn.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://xyz.shuidangran.top

Py:   Counter(arr)
来源：http://dkd.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://wuk.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://puw.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jkh.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jzc.ydzc1.top

Go:   // 手写 map[T]int
来源：http://gyp.zycfv.cn

Ruby: arr.tally
来源：http://gyk.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fwi.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://ome.xinyue.icu

Py:   x in arr
来源：http://qld.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://lrr.yonumen.top

JS:   arr.includes(x)
来源：http://zqo.ydjk.org.cn

TS:   arr.includes(x)
来源：http://hwr.mhx1999.top

Java: list.contains(x)
来源：http://qix.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://dqu.xinyue.icu

Ruby: arr.include?(x)
来源：http://rdp.aibaodan.cn

C#:   list.Contains(x)
来源：http://wxf.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://pir.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tco.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ngb.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oxd.sweek.top

TS:   [...arr];
来源：http://tdz.andypj.xyz

Java: new ArrayList<>(list);
来源：http://wnr.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vil.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://aqg.sjlbkw.cn

C#:   new List<int>(list);
来源：http://shq.zhoulong.xyz

[D23] reduce 累积计算
来源：http://eez.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ucd.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rxc.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvn.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oho.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://yrc.uphjek.com

Go:   // 手写循环
来源：http://emh.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ona.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kgl.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://zdc.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mer.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lkr.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vna.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://plu.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jig.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hoz.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kbh.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pvy.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://vkz.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://exp.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://usw.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ndk.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xlg.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jxw.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://agt.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bic.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pvq.havefunace.top

[D26] 数组转字符串
来源：http://acx.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://bfz.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://fsd.fzhhl.top

JS:   arr.join(", ")
来源：http://hxd.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://dwf.zhijiandao.cn

Java: String.join(", ", list)
来源：http://jln.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://quz.nwbrower.top

Ruby: arr.join(", ")
来源：http://xqw.smart0.xyz

C#:   string.Join(", ", list)
来源：http://eov.shangyingyoupin.top

================================================================================
来源：http://fxt.yongpay.top

E. 字符串处理
来源：http://fkw.fktsv.cn

================================================================================
来源：http://mmr.andypj.xyz

[E01] 拼接字符串
来源：http://hmc.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://scr.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gsv.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yhj.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ncz.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ppk.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://una.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zlx.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://flz.tian-w.cn

[E02] 重复字符串
来源：http://xqh.yanxiufei.cn

Py:   "ab" * 3
来源：http://sil.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://gsa.xziqi.cn

JS:   "ab".repeat(3)
来源：http://ohy.tanke756.top

TS:   "ab".repeat(3)
来源：http://dwc.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://cxw.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://tcf.pycfn.com

Ruby: "ab" * 3
来源：http://mnx.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tni.c1oappe.top

[E03] 截取子串
来源：http://lyr.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://trg.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ezt.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vfs.guannengcc.top

TS:   s.slice(1, 4)
来源：http://ozu.yuanzhike.top

Java: s.substring(1, 4)
来源：http://wkn.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jgx.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://dip.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://zjt.jyoumei.cn

[E04] 查找子串位置
来源：http://wmd.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://pay.epnwcf.com

PHP:  strpos($s, "x");
来源：http://gaj.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mwp.shuidangran.top

TS:   s.indexOf("x")
来源：http://wuw.aizwys.cn

Java: s.indexOf("x")
来源：http://yau.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://pwm.hfpthk.cn

Ruby: s.index("x")
来源：http://dvg.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://gjg.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://isa.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vxk.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://znm.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nmi.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bdk.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ryv.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tpr.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iup.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jbz.nwbrower.top

[E06] 替换子串
来源：http://gjy.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nru.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://lss.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pxb.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://syd.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kqp.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tmt.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ide.birdmap.top

C#:   s.Replace("a", "b")
来源：http://imu.daria6918.cn

[E07] 按分隔符拆分
来源：http://djm.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blc.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pdw.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://enx.xylfe.cn

TS:   s.split(",")
来源：http://klp.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://jnt.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://skv.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://imo.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rjz.mhx1999.top

[E08] 数组按分隔符合并
来源：http://kui.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://vdr.hcnkem.com

PHP:  implode(",", $items);
来源：http://mxe.tian-w.cn

JS:   items.join(",")
来源：http://ixv.jiagoushi.top

TS:   items.join(",")
来源：http://ewp.cheryme.top

Java: String.join(",", items)
来源：http://fva.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://zrz.hnxiangtu.top

Ruby: items.join(",")
来源：http://sst.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://bwx.yvedp.cn

[E09] 去除所有空白字符
来源：http://des.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wdh.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://srf.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://kxa.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://vyl.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://aqt.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rlm.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://kxg.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mgn.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://yiy.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cyq.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oci.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://qlx.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://rhv.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://ekz.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wwg.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lmt.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qzz.hcnkem.com

[E11] 反转字符串
来源：http://unw.tian-w.cn

Py:   s[::-1]
来源：http://dre.tarul.cn

PHP:  strrev($s);
来源：http://nlg.meibo888.top

JS:   [...s].reverse().join("")
来源：http://llj.meibo888.top

TS:   [...s].reverse().join("")
来源：http://xpo.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://zof.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://paq.wangshuangyany.cn

Ruby: s.reverse
来源：http://hdv.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aep.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://hrq.dianchejie.cn

Py:   s.count("a")
来源：http://ank.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://rgc.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://jxn.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://nxt.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uws.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://bfa.yvedp.cn

Ruby: s.count("a")
来源：http://mit.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://dch.ppjwa.cn

[E13] 逐字符遍历
来源：http://ejg.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://txo.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baq.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gci.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fqi.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qdc.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rzk.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://psk.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ljw.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://ncs.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eqw.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://goe.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bwa.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eia.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pqu.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rjz.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yzi.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qgw.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://uza.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tzc.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fxe.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lbq.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jws.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rub.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vps.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://unu.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jrs.andypj.xyz

[E16] 数字千分位
来源：http://qko.yuxming.cn

Py:   f"{1234567:,}"
来源：http://wvn.svipenyu.cn

PHP:  number_format(1234567);
来源：http://wef.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jfa.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gmf.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wsz.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nwo.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vmc.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://ooo.nwbrower.top

[E17] 首字母大写
来源：http://iok.xinyue.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mzt.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hvb.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovg.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oat.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hir.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nzw.gaohongyu789.top

Ruby: s.capitalize
来源：http://quc.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wbi.ydjk.org.cn

[E18] 模板占位符替换
来源：http://jeg.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tgv.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yiz.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hvh.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dez.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gud.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mwb.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ojq.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://shy.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://zld.haohaochexian.top

Py:   s.splitlines()
来源：http://nbh.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dik.jinyuanbaomall.cn


<!-- 参考信息 -->