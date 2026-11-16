代发 wailian999

[D11] 反转数组
来源：http://auw.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://pqf.yuxming.cn

PHP:  array_reverse($arr);
来源：http://vqm.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zym.hywenlv.cn

TS:   [...arr].reverse();
来源：http://qzs.nwbrower.top

Java: Collections.reverse(list);
来源：http://mka.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://nuj.jiagoushi.top

Ruby: arr.reverse
来源：http://ayv.ehwqpu.com

C#:   list.Reverse();
来源：http://rqo.wangshuangyany.cn

[D12] 查找元素下标
来源：http://npy.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://ixu.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oha.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcl.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syc.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jxp.yonumen.top

Go:   slices.Index(arr, x)
来源：http://adx.c1oappe.top

Ruby: arr.index(x)
来源：http://nks.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://frv.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://glh.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jhk.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lip.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://hcm.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://uas.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xui.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rye.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://vvx.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ifg.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://wup.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tco.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mpg.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://npo.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://pfq.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://nzj.xziqi.cn

Go:   // 手写循环
来源：http://kmk.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lih.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bul.shangyingyoupin.top

[D15] 去重
来源：http://kax.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mjq.meibo888.top

PHP:  array_unique($arr);
来源：http://snf.hnqzz.top

JS:   [...new Set(arr)]
来源：http://hni.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://tbg.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mei.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kjp.quarkkingdee.top

Ruby: arr.uniq
来源：http://cjl.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://bdg.shuidangran.top

[D16] 求和与平均值
来源：http://vga.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kcp.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jam.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://afw.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vjx.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iix.ehwqpu.com

Go:   // 手写循环累加
来源：http://zdq.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yvr.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://tgt.guowangkeji.top

[D17] 最大值与最小值
来源：http://upj.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://rkt.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://pej.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qdl.yuxming.cn

TS:   Math.max(...arr);
来源：http://vfn.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://oak.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lcx.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://kca.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://fea.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://stb.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sea.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://yzh.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://exl.xinyue.icu

TS:   nested.flat();
来源：http://qbz.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cby.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://ubo.pycfn.com

Ruby: nested.flatten
来源：http://hgx.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lrk.andypj.xyz

[D19] 按字段分组
来源：http://noz.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://spb.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jsa.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://als.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xcp.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pfm.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://ewi.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://syf.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vwa.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://bql.zycfv.cn

Py:   Counter(arr)
来源：http://ecl.tanke756.top

PHP:  array_count_values($arr);
来源：http://les.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://spv.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gzk.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fih.hammf.cn

Go:   // 手写 map[T]int
来源：http://wvj.aibaodan.cn

Ruby: arr.tally
来源：http://wrt.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cli.shuidangran.top

[D21] 判断是否包含某元素
来源：http://qtn.ehwqpu.com

Py:   x in arr
来源：http://sbi.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://klm.hnxiangtu.top

JS:   arr.includes(x)
来源：http://zqj.316326.xyz

TS:   arr.includes(x)
来源：http://mfe.vehdjk.com

Java: list.contains(x)
来源：http://lyz.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://nuz.yj202588.top

Ruby: arr.include?(x)
来源：http://jwd.havefunace.top

C#:   list.Contains(x)
来源：http://lbf.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://qrz.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ksd.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cem.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gms.wangshuangyany.cn

TS:   [...arr];
来源：http://usj.guannengcc.top

Java: new ArrayList<>(list);
来源：http://ojt.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gmn.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://dfj.xylfe.cn

C#:   new List<int>(list);
来源：http://lkz.pycfn.com

[D23] reduce 累积计算
来源：http://txn.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mso.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iyz.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivg.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oyt.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cje.mhx1999.top

Go:   // 手写循环
来源：http://yok.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hxy.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jti.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://npv.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qzb.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fcw.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tjl.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://euy.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hme.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://myg.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wag.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zyq.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://ytq.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jot.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bxv.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vyx.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kfm.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whk.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fsi.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hjr.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bgz.52xcode.cn

[D26] 数组转字符串
来源：http://tpb.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://oti.havefunace.top

PHP:  implode(", ", $arr);
来源：http://pqv.fzhhl.top

JS:   arr.join(", ")
来源：http://eax.gaohongyu789.top

TS:   arr.join(", ")
来源：http://tmd.fktsv.cn

Java: String.join(", ", list)
来源：http://ete.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://woe.gogol.net.cn

Ruby: arr.join(", ")
来源：http://npn.iojbl.cn

C#:   string.Join(", ", list)
来源：http://pud.xylfe.cn

================================================================================
来源：http://jse.wangshuangyany.cn

E. 字符串处理
来源：http://wjk.pycfn.com

================================================================================
来源：http://lcv.shzxlz.cn

[E01] 拼接字符串
来源：http://iha.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cmo.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rjh.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwv.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uur.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sgv.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rwf.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tbb.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wfe.cqqwz.cn

[E02] 重复字符串
来源：http://kte.sjlbkw.cn

Py:   "ab" * 3
来源：http://gom.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://cxl.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://sxu.sysykeji.top

TS:   "ab".repeat(3)
来源：http://skz.jyoumei.cn

Java: "ab".repeat(3)
来源：http://fmx.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://kph.fengsongda.top

Ruby: "ab" * 3
来源：http://izw.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bcn.kuanghao11.cn

[E03] 截取子串
来源：http://tur.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ktz.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ixu.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://njr.wangdashe.top

TS:   s.slice(1, 4)
来源：http://ruq.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://non.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iwo.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ett.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://xlc.xziqi.cn

[E04] 查找子串位置
来源：http://lzh.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://rwe.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://rsj.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bbo.nwbrower.top

TS:   s.indexOf("x")
来源：http://qsb.jlsjyb.cn

Java: s.indexOf("x")
来源：http://jlu.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://ahg.mhx1999.top

Ruby: s.index("x")
来源：http://lcb.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://cxs.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://nls.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tqu.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mye.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ush.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wgp.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gwy.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cgm.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qee.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mmq.nwbrower.top

[E06] 替换子串
来源：http://eya.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tio.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://bqb.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcj.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://kup.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mhy.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://esh.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bse.yongpay.top

C#:   s.Replace("a", "b")
来源：http://tza.redwolf501.top

[E07] 按分隔符拆分
来源：http://wfy.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vuv.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://paf.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mqv.uphjek.com

TS:   s.split(",")
来源：http://cpl.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://hrl.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wsi.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://iyh.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uph.cheryme.top

[E08] 数组按分隔符合并
来源：http://pup.bjfxy.top

Py:   ",".join(items)
来源：http://lok.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://oes.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://jgl.yonumen.top

TS:   items.join(",")
来源：http://psb.haohaochexian.top

Java: String.join(",", items)
来源：http://rbs.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://tge.guannengcc.top

Ruby: items.join(",")
来源：http://dgs.c1oappe.top

C#:   string.Join(",", items)
来源：http://rhy.yfazqb.com

[E09] 去除所有空白字符
来源：http://byj.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sap.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujg.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://fkz.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://htf.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://inv.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://nvu.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://rmi.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rek.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://obc.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xrd.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://urv.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://weg.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://gqc.fehbvm.com

Java: String.format("%03d", 7)
来源：http://mrv.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://drq.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://puq.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pco.guannengcc.top

[E11] 反转字符串
来源：http://ccd.shzxlz.cn

Py:   s[::-1]
来源：http://hqx.jlsjyb.cn

PHP:  strrev($s);
来源：http://bge.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://lfr.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://eyq.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bgf.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qen.hammf.cn

Ruby: s.reverse
来源：http://rcm.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://slh.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://ktx.hesvh.cn

Py:   s.count("a")
来源：http://hiv.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://qbi.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://wsw.gzhubu.top

TS:   s.split("a").length - 1
来源：http://osv.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xwv.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://xmd.yueranfly.top

Ruby: s.count("a")
来源：http://xyw.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://fan.andypj.xyz

[E13] 逐字符遍历
来源：http://kqq.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://qoi.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rxw.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qbt.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://trb.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bau.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lxh.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tth.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://buh.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://nql.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vmz.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aml.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://axd.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rtn.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cme.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xly.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kkv.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zxj.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://txb.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yba.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ndt.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pzq.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hrg.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ngz.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nfk.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nlu.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jhx.sxryk.cn

[E16] 数字千分位
来源：http://ycr.ivvv.top

Py:   f"{1234567:,}"
来源：http://ijw.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://trl.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xxl.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tck.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://abk.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kwj.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gae.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://acg.guowangkeji.top

[E17] 首字母大写
来源：http://nvm.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eyk.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wqc.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fdq.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://agv.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kuv.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nzy.zdbjq.cn

Ruby: s.capitalize
来源：http://nug.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gul.yongpay.top


<!-- 参考信息 -->