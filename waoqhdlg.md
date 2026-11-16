代发 wailian999

C#:   list.Reverse();
来源：http://vux.jqgufenzy.top

[D12] 查找元素下标
来源：http://oet.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://fps.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://icp.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kbi.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ksw.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://twx.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://agk.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://iap.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://dcl.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://utc.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rnn.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://exr.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://yqn.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://dxj.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://flr.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hgo.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://ahv.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://byo.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://zup.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bwi.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqr.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://vxn.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://kaw.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://jux.nwbrower.top

Go:   // 手写循环
来源：http://ccf.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://hhy.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jqh.hongshengwenyu.top

[D15] 去重
来源：http://cuz.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://buw.yvedp.cn

PHP:  array_unique($arr);
来源：http://dyc.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://pwz.52xcode.cn

TS:   [...new Set(arr)]
来源：http://ect.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xmu.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kbd.jinqigfzy.top

Ruby: arr.uniq
来源：http://mmq.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://nuh.yongpay.top

[D16] 求和与平均值
来源：http://kkr.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bqw.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dbp.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ret.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yhz.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eyl.hfpthk.cn

Go:   // 手写循环累加
来源：http://soe.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vez.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://wtv.zhengqikj.top

[D17] 最大值与最小值
来源：http://xbl.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://qls.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://xob.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://utz.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://qkp.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://elg.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yrf.sweek.top

Ruby: arr.max;  arr.min
来源：http://krc.sweek.top

C#:   list.Max();  list.Min()
来源：http://ffs.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://rqu.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ywg.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://oih.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cda.tarul.cn

TS:   nested.flat();
来源：http://dyq.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zjb.ydjk.org.cn

Go:   // 手写双层循环
来源：http://odr.zhiwuduotai.top

Ruby: nested.flatten
来源：http://zpi.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rio.havefunace.top

[D19] 按字段分组
来源：http://msk.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mjo.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mnv.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xdr.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://hfv.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://syy.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://agu.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rhe.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ldk.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://pdy.yvedp.cn

Py:   Counter(arr)
来源：http://dtq.yvedp.cn

PHP:  array_count_values($arr);
来源：http://oox.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cff.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gre.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qnv.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://euw.cucudq.cn

Ruby: arr.tally
来源：http://mzb.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dfp.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://pec.uphjek.com

Py:   x in arr
来源：http://ntk.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://cqt.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://yxh.sysykeji.top

TS:   arr.includes(x)
来源：http://zkq.chenjidiqi.icu

Java: list.contains(x)
来源：http://wch.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://gjr.yonumen.top

Ruby: arr.include?(x)
来源：http://voc.hammf.cn

C#:   list.Contains(x)
来源：http://xfb.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://dse.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wiz.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kvh.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yas.dianchejie.cn

TS:   [...arr];
来源：http://glk.jlsjyb.cn

Java: new ArrayList<>(list);
来源：http://qst.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://hqw.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://xnu.quarkkingdee.top

C#:   new List<int>(list);
来源：http://wbv.sjlbkw.cn

[D23] reduce 累积计算
来源：http://qum.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rev.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nwv.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gnh.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lox.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tkt.feifeiyinyue.top

Go:   // 手写循环
来源：http://uhj.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pcl.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cnb.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://yoy.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kcu.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ffk.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fgf.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ckz.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jdp.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://emb.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uee.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vqg.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://kab.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zfw.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pqd.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wvm.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sev.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ovj.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mcz.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fua.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wqq.fzhhl.top

[D26] 数组转字符串
来源：http://djc.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://sve.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://pov.zdbjq.cn

JS:   arr.join(", ")
来源：http://qze.mhx1999.top

TS:   arr.join(", ")
来源：http://xhn.snrcjt.cn

Java: String.join(", ", list)
来源：http://qwk.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://vra.tianlin.xyz

Ruby: arr.join(", ")
来源：http://mmp.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://nil.hammf.cn

================================================================================
来源：http://gfa.yonumen.top

E. 字符串处理
来源：http://sep.tianlin.xyz

================================================================================
来源：http://gqv.zhongyouzk.top

[E01] 拼接字符串
来源：http://cvn.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zgs.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jbu.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://efw.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahg.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wvx.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://scg.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zzk.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hwf.jianghu66.top

[E02] 重复字符串
来源：http://rvr.gaohongyu789.top

Py:   "ab" * 3
来源：http://wie.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://wmf.yonumen.top

JS:   "ab".repeat(3)
来源：http://qux.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://hee.c1oappe.top

Java: "ab".repeat(3)
来源：http://eyz.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://vmv.zhoulong.xyz

Ruby: "ab" * 3
来源：http://nmy.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eay.jinghuilouyu.cn

[E03] 截取子串
来源：http://yyg.aizwys.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uum.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mfl.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rvb.daria6918.cn

TS:   s.slice(1, 4)
来源：http://kgh.sysykeji.top

Java: s.substring(1, 4)
来源：http://vyv.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gmq.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://edh.yonumen.top

C#:   s.Substring(1, 3)
来源：http://ddb.zhoulong.xyz

[E04] 查找子串位置
来源：http://akj.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://seg.sxryk.cn

PHP:  strpos($s, "x");
来源：http://xbb.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://elb.jinqigufen.top

TS:   s.indexOf("x")
来源：http://vrt.nanxuanxn.top

Java: s.indexOf("x")
来源：http://dib.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://esk.hnqzz.top

Ruby: s.index("x")
来源：http://gbi.yj202588.top

C#:   s.IndexOf("x")
来源：http://iho.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://jgr.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://muz.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ycr.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wpz.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gkd.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wjj.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://otf.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ekh.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kvq.ivvv.top

[E06] 替换子串
来源：http://epz.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ikr.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://cct.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ydm.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://hdh.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://und.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tvs.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aqq.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://ojs.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://jtz.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qde.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://emf.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://soa.xziqi.cn

TS:   s.split(",")
来源：http://xli.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://prl.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bte.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://scu.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://szi.fktsv.cn

[E08] 数组按分隔符合并
来源：http://qqr.ydzc1.top

Py:   ",".join(items)
来源：http://hwf.smart0.xyz

PHP:  implode(",", $items);
来源：http://ezf.jqgfzy.top

JS:   items.join(",")
来源：http://ysc.jyoumei.cn

TS:   items.join(",")
来源：http://wrv.wangshuangyany.cn

Java: String.join(",", items)
来源：http://tcg.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://fhz.daxiang520.top

Ruby: items.join(",")
来源：http://mmk.pycfn.com

C#:   string.Join(",", items)
来源：http://hhl.tanke756.top

[E09] 去除所有空白字符
来源：http://czf.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mui.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gqu.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://jpo.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://nys.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://gwx.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jvx.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://wyy.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wkb.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://dmz.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://daa.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xsw.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://gov.sweek.top

TS:   "7".padStart(3, "0")
来源：http://ppn.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://ocv.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ldj.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aen.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://puu.pengpengdd.cyou

[E11] 反转字符串
来源：http://uhv.sufxvd.cn

Py:   s[::-1]
来源：http://fak.tanke756.top

PHP:  strrev($s);
来源：http://ewr.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://yda.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://ofy.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xrf.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lqr.chenjidiqi.icu

Ruby: s.reverse
来源：http://dio.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://goc.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://hdj.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://tpl.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://utd.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://won.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://hhb.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://khb.tarul.cn

Go:   strings.Count(s, "a")
来源：http://ovq.vehdjk.com

Ruby: s.count("a")
来源：http://iqy.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://czv.jinqigfzy.top

[E13] 逐字符遍历
来源：http://tft.tanke756.top

Py:   for ch in s: print(ch)
来源：http://ldy.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dwv.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iei.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hxo.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jwc.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fqc.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bmr.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jpd.fktsv.cn

[E14] URL 编码与 Base64
来源：http://wcd.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zet.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gvh.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kxz.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ssw.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txh.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vas.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://isi.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tik.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://yjn.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wav.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tut.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yzt.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://fek.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gis.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kbv.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fhm.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cjh.yj20258.top

[E16] 数字千分位
来源：http://kvz.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://jwr.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://tzw.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kem.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ptd.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uek.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sea.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nkh.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://ccs.yj20258.top

[E17] 首字母大写
来源：http://gta.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tij.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://irq.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://erw.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qfm.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tnw.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hjq.birdmap.top

Ruby: s.capitalize
来源：http://vmw.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qaw.jqgufenzy.top

[E18] 模板占位符替换
来源：http://bxb.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fbe.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wyl.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gyq.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mpd.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://njg.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wik.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://swo.ivvv.top


<!-- 参考信息 -->