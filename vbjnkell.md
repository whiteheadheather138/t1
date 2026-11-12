代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nhk.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hat.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://usq.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://zva.yj20258888.top

Ruby: arr.index(x)
来源：http://ohb.xylfe.cn

C#:   list.IndexOf(x);
来源：http://cgy.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://wht.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gmc.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lsp.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://ejt.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://mvs.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://woi.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wsc.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://axi.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oyl.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://usq.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cnk.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhr.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://hfz.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://yxe.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uji.tianlin.xyz

Go:   // 手写循环
来源：http://kqd.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yxs.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vfy.zhaomingkeji.xyz

[D15] 去重
来源：http://szd.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jyp.daxiang520.top

PHP:  array_unique($arr);
来源：http://omu.shuidangran.top

JS:   [...new Set(arr)]
来源：http://bkd.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://bmo.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sxc.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://svd.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://vjw.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://pyl.yvedp.cn

[D16] 求和与平均值
来源：http://dwi.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvp.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ygr.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wkh.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rox.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://epi.xziqi.cn

Go:   // 手写循环累加
来源：http://kyj.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sai.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://zyd.snrcjt.cn

[D17] 最大值与最小值
来源：http://miy.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://srd.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://qlw.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wbg.fehbvm.com

TS:   Math.max(...arr);
来源：http://kpp.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kbi.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://isw.havefunace.top

Ruby: arr.max;  arr.min
来源：http://shr.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://ujt.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://lre.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://izh.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://bjm.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ybw.jianghu66.top

TS:   nested.flat();
来源：http://ney.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vel.ehwqpu.com

Go:   // 手写双层循环
来源：http://inv.sjlbkw.cn

Ruby: nested.flatten
来源：http://rgp.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tfd.svipenyu.cn

[D19] 按字段分组
来源：http://kvg.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kpi.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vuw.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kri.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://seb.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ijb.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://osu.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ffl.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://epf.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://inz.zdbjq.cn

Py:   Counter(arr)
来源：http://jfo.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://qjh.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rzw.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pzf.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://krr.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://skp.0kj1m.cn

Ruby: arr.tally
来源：http://vjr.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pkz.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://lxm.ywan-chungtsiang.top

Py:   x in arr
来源：http://jgs.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://noc.yuxming.cn

JS:   arr.includes(x)
来源：http://jzg.svipenyu.cn

TS:   arr.includes(x)
来源：http://pwq.shanyushiyangtech.top

Java: list.contains(x)
来源：http://kze.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://lfa.xziqi.cn

Ruby: arr.include?(x)
来源：http://zkb.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://jtw.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://nqk.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nuf.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ujc.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aty.epnwcf.com

TS:   [...arr];
来源：http://jjv.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://fsv.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://nzg.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://jqz.hammf.cn

C#:   new List<int>(list);
来源：http://tyw.nwbrower.top

[D23] reduce 累积计算
来源：http://ber.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dwg.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://anv.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvv.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uay.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://won.sufxvd.cn

Go:   // 手写循环
来源：http://kik.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://red.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oyw.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://fyp.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eij.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jrv.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tng.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ntp.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bzd.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kaw.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vot.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cix.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://jaq.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://osc.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://avm.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wkd.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://flx.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dvc.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gys.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dpi.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nkt.jlsjyb.cn

[D26] 数组转字符串
来源：http://psg.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://zwa.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://mkb.pycfn.com

JS:   arr.join(", ")
来源：http://gex.yanxiufei.cn

TS:   arr.join(", ")
来源：http://oyf.aizwys.cn

Java: String.join(", ", list)
来源：http://cjk.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://oof.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://ita.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://sqa.birdmap.top

================================================================================
来源：http://fxf.vqdsnc.cn

E. 字符串处理
来源：http://jle.havefunace.top

================================================================================
来源：http://ojs.ydjk.org.cn

[E01] 拼接字符串
来源：http://ghi.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aip.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zzc.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://glf.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tbr.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jyl.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rct.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ypw.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ust.0kj1m.cn

[E02] 重复字符串
来源：http://bwb.cucudq.cn

Py:   "ab" * 3
来源：http://jbq.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://woo.yj20258.top

JS:   "ab".repeat(3)
来源：http://vum.cheryme.top

TS:   "ab".repeat(3)
来源：http://xam.ehwqpu.com

Java: "ab".repeat(3)
来源：http://ypj.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://rvr.sjlbkw.cn

Ruby: "ab" * 3
来源：http://trr.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nnx.cashguo.top

[E03] 截取子串
来源：http://hic.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zzq.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rya.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cbv.yonumen.top

TS:   s.slice(1, 4)
来源：http://wky.tian-w.cn

Java: s.substring(1, 4)
来源：http://udv.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gae.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://tuv.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://wbj.sufxvd.cn

[E04] 查找子串位置
来源：http://lcg.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://xph.yuxming.cn

PHP:  strpos($s, "x");
来源：http://gac.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kxj.svipenyu.cn

TS:   s.indexOf("x")
来源：http://uza.hammf.cn

Java: s.indexOf("x")
来源：http://hlg.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://avc.jinqigfzy.top

Ruby: s.index("x")
来源：http://suc.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://kbl.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xuj.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://phf.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xpb.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tii.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mea.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cmf.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yej.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rqv.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yqi.yj20258888.top

[E06] 替换子串
来源：http://kis.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gor.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://ymr.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oha.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://nzr.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://syg.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzx.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pvi.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://qcp.daxiang520.top

[E07] 按分隔符拆分
来源：http://oha.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vlq.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kqc.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ify.chenzaomai.com

TS:   s.split(",")
来源：http://ihn.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://fqx.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tjp.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://zws.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fiy.daria6918.cn

[E08] 数组按分隔符合并
来源：http://icm.hammf.cn

Py:   ",".join(items)
来源：http://ies.316326.xyz

PHP:  implode(",", $items);
来源：http://yeu.tanke756.top

JS:   items.join(",")
来源：http://ahu.yangfankeji.com

TS:   items.join(",")
来源：http://jbj.zhixingplan.top

Java: String.join(",", items)
来源：http://ibt.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://zsl.c1oappe.top

Ruby: items.join(",")
来源：http://wyr.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://nxj.dianchejie.cn

[E09] 去除所有空白字符
来源：http://cnq.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rch.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rya.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://fwv.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://nnc.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://rnb.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rqq.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lyv.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cwa.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://mbd.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lrv.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xvb.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://sni.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://qfz.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://gtn.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wxh.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kfy.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://byw.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://fmh.tanke756.top

Py:   s[::-1]
来源：http://mhz.ppjwa.cn

PHP:  strrev($s);
来源：http://fcd.havefunace.top

JS:   [...s].reverse().join("")
来源：http://jjk.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://ljr.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://otw.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rdr.sufxvd.cn

Ruby: s.reverse
来源：http://dyi.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://oak.yueranfly.top

[E12] 统计某字符出现次数
来源：http://ikd.epnwcf.com

Py:   s.count("a")
来源：http://udv.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://myt.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://vdy.316326.xyz

TS:   s.split("a").length - 1
来源：http://wdt.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qry.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://qwh.hcnkem.com

Ruby: s.count("a")
来源：http://ldm.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://vyh.zdbjq.cn

[E13] 逐字符遍历
来源：http://nwn.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://uye.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://syd.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hrr.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mlf.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gha.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yrc.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://son.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zuj.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://rpb.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jmk.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ule.dianchejie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qtj.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dqt.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vjp.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xuv.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ygr.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wwc.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://eyc.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tsd.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://idp.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gns.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zln.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qsc.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cbt.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xlz.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ena.vqdsnc.cn

[E16] 数字千分位
来源：http://tci.zycfv.cn

Py:   f"{1234567:,}"
来源：http://dvp.gzhubu.top

PHP:  number_format(1234567);
来源：http://ctt.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wub.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://yxb.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xsd.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sgq.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iqi.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://efx.ydjk.org.cn

[E17] 首字母大写
来源：http://zpa.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mgx.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jkr.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://izp.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sjy.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cer.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xzo.dashuyun.cn

Ruby: s.capitalize
来源：http://rso.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yog.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://icq.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eld.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qll.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://yat.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ppf.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zit.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tlj.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rtq.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xad.yvedp.cn

[E19] 多行文本按行拆分
来源：http://ewm.hywenlv.cn

Py:   s.splitlines()
来源：http://qjn.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vja.jqgfzy.top


<!-- 参考信息 -->