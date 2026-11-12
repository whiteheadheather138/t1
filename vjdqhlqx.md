代发 wailian999

C#:   list.Reverse();
来源：http://uqk.quarkkingdee.top

[D12] 查找元素下标
来源：http://eld.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://pze.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://egx.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rfr.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vew.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ilj.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://hxb.vehdjk.com

Ruby: arr.index(x)
来源：http://dmo.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://ukc.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://ezd.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qgb.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zfd.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://vqg.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://rtc.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vfa.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://grc.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ukq.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jrj.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://dsj.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bno.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zfh.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://dcs.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://xwg.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://vci.nwbrower.top

Go:   // 手写循环
来源：http://pgj.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ayn.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://wjo.jyoumei.cn

[D15] 去重
来源：http://bel.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hor.aibaodan.cn

PHP:  array_unique($arr);
来源：http://roo.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://uad.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://iyg.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dto.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://kog.zdqjudy.top

Ruby: arr.uniq
来源：http://imh.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://kss.yj20258888.top

[D16] 求和与平均值
来源：http://vnz.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wbm.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dxl.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gca.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzl.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ikm.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://yvf.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qsz.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://bej.jyoumei.cn

[D17] 最大值与最小值
来源：http://bgf.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://glq.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://ros.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zai.52xcode.cn

TS:   Math.max(...arr);
来源：http://ove.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ast.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gdn.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://ysm.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://lsd.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://awk.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://txy.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://wnl.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fpb.zdqjudy.top

TS:   nested.flat();
来源：http://nsb.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mso.aibaodan.cn

Go:   // 手写双层循环
来源：http://zgg.quarkkingdee.top

Ruby: nested.flatten
来源：http://qjn.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ddz.52xcode.cn

[D19] 按字段分组
来源：http://ygk.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bqq.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nks.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qpb.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cwx.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://klp.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://pbr.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qmq.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ypy.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://fty.meibo888.top

Py:   Counter(arr)
来源：http://ojq.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://hcb.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rtg.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rtz.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://drc.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://svv.vqdsnc.cn

Ruby: arr.tally
来源：http://rfx.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bqs.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://moc.yuanzhike.top

Py:   x in arr
来源：http://glh.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://lko.sxryk.cn

JS:   arr.includes(x)
来源：http://quo.zdbjq.cn

TS:   arr.includes(x)
来源：http://jdd.fzhhl.top

Java: list.contains(x)
来源：http://mxl.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://cgu.jinqigufen.top

Ruby: arr.include?(x)
来源：http://twx.sxryk.cn

C#:   list.Contains(x)
来源：http://pbu.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://swr.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ebl.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zfo.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qpx.hammf.cn

TS:   [...arr];
来源：http://euo.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://dgf.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://woi.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://blb.jinqigfzy.top

C#:   new List<int>(list);
来源：http://xey.dianchejie.cn

[D23] reduce 累积计算
来源：http://hcl.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://omq.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://svx.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://npu.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ctg.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qmx.guannengcc.top

Go:   // 手写循环
来源：http://vof.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://imx.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://okr.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://aiz.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kkb.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dkn.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pwm.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fev.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hkl.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jtg.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lyx.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jem.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://cra.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qwm.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hel.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ifb.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://arp.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://imy.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sdb.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xgd.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oha.hongshengwenyu.top

[D26] 数组转字符串
来源：http://mof.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://xbt.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://ztz.cheryme.top

JS:   arr.join(", ")
来源：http://aar.gzhubu.top

TS:   arr.join(", ")
来源：http://zzt.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://uwg.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://jtk.chenlongwang.top

Ruby: arr.join(", ")
来源：http://jpv.mhx1999.top

C#:   string.Join(", ", list)
来源：http://wqm.hnqzz.top

================================================================================
来源：http://opb.c1oappe.top

E. 字符串处理
来源：http://cpm.aibaodan.cn

================================================================================
来源：http://tze.jinqigufen.top

[E01] 拼接字符串
来源：http://ral.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bqz.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rvc.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gcz.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kpa.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ukg.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ivb.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zub.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ada.yj20258.top

[E02] 重复字符串
来源：http://ssh.ctjpmb.com

Py:   "ab" * 3
来源：http://dvw.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://kkw.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://rlw.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://zna.cqqwz.cn

Java: "ab".repeat(3)
来源：http://jvf.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://kuj.gogol.net.cn

Ruby: "ab" * 3
来源：http://jex.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://siw.epnwcf.com

[E03] 截取子串
来源：http://sqn.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oup.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oxa.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://flm.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://ngs.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://gke.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fxq.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://gax.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://eng.cashguo.top

[E04] 查找子串位置
来源：http://vnu.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://kik.yj20258888.top

PHP:  strpos($s, "x");
来源：http://etv.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wco.yuanzhike.top

TS:   s.indexOf("x")
来源：http://tjh.nwbrower.top

Java: s.indexOf("x")
来源：http://agv.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://adq.aibaodan.cn

Ruby: s.index("x")
来源：http://fws.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://yow.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qvn.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ekd.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zuh.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://div.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://riy.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyw.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wdi.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ijv.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dmv.jinqigufen.top

[E06] 替换子串
来源：http://tyv.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kzi.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://frh.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ygm.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://iwj.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vuf.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mug.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cvh.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://eyz.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://miy.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jbi.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ozl.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uvf.shanyushiyangtech.top

TS:   s.split(",")
来源：http://ncy.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tas.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bid.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://kon.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yrt.smart0.xyz

[E08] 数组按分隔符合并
来源：http://dvt.jqgufenzy.top

Py:   ",".join(items)
来源：http://mjh.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://vhx.yuxming.cn

JS:   items.join(",")
来源：http://ksb.52xcode.cn

TS:   items.join(",")
来源：http://ygw.yangfankeji.com

Java: String.join(",", items)
来源：http://dhh.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://btf.uphjek.com

Ruby: items.join(",")
来源：http://nrv.vehdjk.com

C#:   string.Join(",", items)
来源：http://grb.hywenlv.cn

[E09] 去除所有空白字符
来源：http://ehb.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pcn.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cyc.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://cyf.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://qoz.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://enh.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://chl.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://vxz.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ifj.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://uoj.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ygg.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dfs.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://ouq.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://dlw.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://rao.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hra.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cfr.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ukl.epnwcf.com

[E11] 反转字符串
来源：http://ndi.xziqi.cn

Py:   s[::-1]
来源：http://ztv.chenzaomai.com

PHP:  strrev($s);
来源：http://coe.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://nsy.yongpay.top

TS:   [...s].reverse().join("")
来源：http://ase.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vyk.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://uda.kuanghao11.cn

Ruby: s.reverse
来源：http://xpu.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://dga.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://pps.chenlongwang.top

Py:   s.count("a")
来源：http://qwa.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://asg.bjfxy.top

JS:   s.split("a").length - 1
来源：http://bns.yj20258888.top

TS:   s.split("a").length - 1
来源：http://hvb.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ggj.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://mov.hesvh.cn

Ruby: s.count("a")
来源：http://bea.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://aiv.daxiang520.top

[E13] 逐字符遍历
来源：http://abg.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://vgt.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lxn.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yku.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://thy.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://few.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eyw.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dct.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ecc.xylfe.cn

[E14] URL 编码与 Base64
来源：http://zwc.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dzp.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tuc.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://akd.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tyh.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jpc.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://epj.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ozt.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vcu.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://nze.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fbf.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mcf.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dkl.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kjg.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wuv.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hvo.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ahz.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rlb.shzxlz.cn

[E16] 数字千分位
来源：http://tnv.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://jyp.guannengcc.top

PHP:  number_format(1234567);
来源：http://ylx.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xpd.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wlo.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zze.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xes.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jnc.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://sbd.tianlin.xyz

[E17] 首字母大写
来源：http://inq.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xuy.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://nvs.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxy.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zxq.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://svn.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wtx.hammf.cn

Ruby: s.capitalize
来源：http://kzj.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xll.jiagoushi.top

[E18] 模板占位符替换
来源：http://lrx.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kwz.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vwc.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://beb.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vca.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jxe.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xqf.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kss.yuxming.cn


<!-- 参考信息 -->