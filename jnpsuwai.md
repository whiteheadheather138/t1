代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://abz.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayf.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pvc.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://rfd.sysykeji.top

Ruby: arr.index(x)
来源：http://vyw.hcnkem.com

C#:   list.IndexOf(x);
来源：http://pqc.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://vwh.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lyw.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ivj.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://wth.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://dfc.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pby.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ogy.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://ghd.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hxw.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://mci.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tya.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bjs.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://edd.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://vpr.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sdu.zycfv.cn

Go:   // 手写循环
来源：http://usf.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lvw.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mpe.zhongyouzk.top

[D15] 去重
来源：http://wut.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lcz.nanxinkj.top

PHP:  array_unique($arr);
来源：http://ufb.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://unf.xinyue.icu

TS:   [...new Set(arr)]
来源：http://urx.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kfs.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://pjd.chenjidiqi.icu

Ruby: arr.uniq
来源：http://lmh.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://abi.hfpthk.cn

[D16] 求和与平均值
来源：http://bih.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://udw.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wsu.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ruv.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xpc.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kyc.sysykeji.top

Go:   // 手写循环累加
来源：http://ugv.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kys.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://gvn.nwbrower.top

[D17] 最大值与最小值
来源：http://agt.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://mcl.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://zyb.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dqd.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://xnk.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ioz.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vny.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://tde.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://lrr.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://psp.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qop.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://wbf.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://led.zhengqikj.top

TS:   nested.flat();
来源：http://exf.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gzm.0kj1m.cn

Go:   // 手写双层循环
来源：http://ubl.ehwqpu.com

Ruby: nested.flatten
来源：http://zze.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jrz.dianchejie.cn

[D19] 按字段分组
来源：http://ahg.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gtw.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://olc.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bhx.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ann.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aok.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://mne.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iam.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ixr.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://zgo.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://tjs.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://csa.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mad.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vue.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ihr.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://yxi.fehbvm.com

Ruby: arr.tally
来源：http://jnd.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tsc.yj20258.top

[D21] 判断是否包含某元素
来源：http://rna.gotoacloud.top

Py:   x in arr
来源：http://xrc.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://qqi.jyoumei.cn

JS:   arr.includes(x)
来源：http://qnr.zycfv.cn

TS:   arr.includes(x)
来源：http://stj.dashuyun.cn

Java: list.contains(x)
来源：http://cpd.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://ink.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://ayp.pycfn.com

C#:   list.Contains(x)
来源：http://hkd.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://rck.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://usv.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gos.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://alw.tanke756.top

TS:   [...arr];
来源：http://dtw.yuxming.cn

Java: new ArrayList<>(list);
来源：http://rmi.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://beu.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://aod.zhongyouzk.top

C#:   new List<int>(list);
来源：http://cwu.sysykeji.top

[D23] reduce 累积计算
来源：http://xsj.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyr.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lji.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://epa.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://arj.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qwt.bbcook.cn

Go:   // 手写循环
来源：http://hid.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wqh.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ruc.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://vke.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uot.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oly.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ftz.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hvy.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zse.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jro.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://erd.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mts.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://eln.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ala.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dia.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eyk.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aiw.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wgb.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ytm.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ump.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pkj.ybcxt.top

[D26] 数组转字符串
来源：http://tpx.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://aro.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://zgc.jlsjyb.cn

JS:   arr.join(", ")
来源：http://oyj.jinqigfzy.top

TS:   arr.join(", ")
来源：http://prb.yonumen.top

Java: String.join(", ", list)
来源：http://lpr.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://ksx.gotoacloud.top

Ruby: arr.join(", ")
来源：http://oya.bbcook.cn

C#:   string.Join(", ", list)
来源：http://ata.wangshuangyany.cn

================================================================================
来源：http://eon.bjfxy.top

E. 字符串处理
来源：http://dsm.fktsv.cn

================================================================================
来源：http://gdx.fehbvm.com

[E01] 拼接字符串
来源：http://xco.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uql.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eng.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppd.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ufp.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oab.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jyx.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jtr.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ech.wangdashe.top

[E02] 重复字符串
来源：http://ikd.yj20258888.top

Py:   "ab" * 3
来源：http://rey.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://rnq.shuidangran.top

JS:   "ab".repeat(3)
来源：http://afp.fktsv.cn

TS:   "ab".repeat(3)
来源：http://vcg.yj202588.top

Java: "ab".repeat(3)
来源：http://eoj.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://aqo.jinqigfzy.top

Ruby: "ab" * 3
来源：http://rib.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://laf.sxryk.cn

[E03] 截取子串
来源：http://vpf.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jnm.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xug.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wkh.shuidangran.top

TS:   s.slice(1, 4)
来源：http://nnr.meibo888.top

Java: s.substring(1, 4)
来源：http://dcj.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fxc.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://kqi.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://qij.meibo888.top

[E04] 查找子串位置
来源：http://gep.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://qzh.hesvh.cn

PHP:  strpos($s, "x");
来源：http://rbl.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jss.yj202588.top

TS:   s.indexOf("x")
来源：http://jdy.cqqwz.cn

Java: s.indexOf("x")
来源：http://lpy.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://ocg.ydjk.org.cn

Ruby: s.index("x")
来源：http://xcf.yvedp.cn

C#:   s.IndexOf("x")
来源：http://yrz.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qqx.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ypm.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rmt.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzy.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mtn.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://alg.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dua.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kuz.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sdw.dashuyun.cn

[E06] 替换子串
来源：http://vfq.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://thh.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://lyj.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wry.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://ivd.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iff.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bgd.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ulp.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://jrg.daria6918.cn

[E07] 按分隔符拆分
来源：http://umo.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qky.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zjn.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xmz.cucudq.cn

TS:   s.split(",")
来源：http://hxx.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://wji.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://reb.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://utc.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jrn.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://njf.chenzaomai.com

Py:   ",".join(items)
来源：http://aks.tianlin.xyz

PHP:  implode(",", $items);
来源：http://tby.smart0.xyz

JS:   items.join(",")
来源：http://juh.zdbjq.cn

TS:   items.join(",")
来源：http://rsj.shzxlz.cn

Java: String.join(",", items)
来源：http://upi.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://bih.smart0.xyz

Ruby: items.join(",")
来源：http://kbe.jinqigufen.top

C#:   string.Join(",", items)
来源：http://fdd.dianchejie.cn

[E09] 去除所有空白字符
来源：http://lhb.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tsl.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wxq.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://lag.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://ilf.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://njw.zhiwuduotai.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wiv.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xuy.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yqs.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://lvi.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://atj.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://atf.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://kff.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://qas.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://zfd.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://csy.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ngo.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ofl.sweek.top

[E11] 反转字符串
来源：http://uwh.cdnleiting.top

Py:   s[::-1]
来源：http://uqz.nwbrower.top

PHP:  strrev($s);
来源：http://yih.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://whn.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://non.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bqd.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rds.guannengcc.top

Ruby: s.reverse
来源：http://zow.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://dtx.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://gky.ehwqpu.com

Py:   s.count("a")
来源：http://ywa.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://wzh.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://jvm.meibo888.top

TS:   s.split("a").length - 1
来源：http://tqf.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blo.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://awu.nanxuanxn.top

Ruby: s.count("a")
来源：http://pid.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://ksi.zhijiandao.cn

[E13] 逐字符遍历
来源：http://ukt.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://iws.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hzn.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://irz.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://chx.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://agt.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oni.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://luy.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wmk.yj202588.top

[E14] URL 编码与 Base64
来源：http://vdq.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rtu.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cgg.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://euz.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tsl.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ztr.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nkw.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qnf.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wep.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://fvt.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ogv.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kpx.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fka.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://nxw.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lxl.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ihf.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yqg.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ovg.redwolf501.top

[E16] 数字千分位
来源：http://jdq.cheryme.top

Py:   f"{1234567:,}"
来源：http://sgs.hysaishi.cn

PHP:  number_format(1234567);
来源：http://wdm.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ump.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kjt.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fcc.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zhr.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qck.havefunace.top

C#:   1234567.ToString("N0")
来源：http://vmq.birdmap.top

[E17] 首字母大写
来源：http://apu.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qkj.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://upb.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://elf.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hyk.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ywp.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gfo.zdqjudy.top

Ruby: s.capitalize
来源：http://byd.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dsh.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://bug.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ocj.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nib.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://drx.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gbz.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zqb.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nfh.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rbm.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vzh.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://ibw.dashuyun.cn

Py:   s.splitlines()
来源：http://rww.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kic.hesvh.cn


<!-- 参考信息 -->