代发 wailian999

Ruby: arr.index(x)
来源：http://qvy.yj202588.top

C#:   list.IndexOf(x);
来源：http://wxf.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://hra.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uyy.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xib.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://xhu.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://dsb.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://etn.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cje.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://nuc.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yeo.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://rjt.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aor.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wyw.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://psu.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://jbv.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wnl.dashuyun.cn

Go:   // 手写循环
来源：http://izq.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://vys.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wpw.zdqjudy.top

[D15] 去重
来源：http://wwi.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wgd.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://sjj.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://huk.fzhhl.top

TS:   [...new Set(arr)]
来源：http://xka.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://shr.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cxp.316326.xyz

Ruby: arr.uniq
来源：http://vws.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://hwe.chenzaomai.com

[D16] 求和与平均值
来源：http://xdr.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vzx.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mkn.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fje.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hzv.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dna.zhoulong.xyz

Go:   // 手写循环累加
来源：http://wuz.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yaz.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://tew.zhongyouzk.top

[D17] 最大值与最小值
来源：http://mjc.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://xtc.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://jrs.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cid.fehbvm.com

TS:   Math.max(...arr);
来源：http://liq.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ios.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uem.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://hco.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://fda.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://sae.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bhi.ivvv.top

PHP:  array_merge(...$nested);
来源：http://grr.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uqu.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://pcr.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kct.zycfv.cn

Go:   // 手写双层循环
来源：http://tpu.mhx1999.top

Ruby: nested.flatten
来源：http://kfb.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tyt.yfazqb.com

[D19] 按字段分组
来源：http://etl.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tio.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lle.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nkd.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pgb.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xei.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://exq.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://qgk.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wfg.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://wos.yj20258888.top

Py:   Counter(arr)
来源：http://gvf.fengsongda.top

PHP:  array_count_values($arr);
来源：http://dvc.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nxv.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://llt.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggn.cucudq.cn

Go:   // 手写 map[T]int
来源：http://onj.yvedp.cn

Ruby: arr.tally
来源：http://cld.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xpb.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://ilh.hesvh.cn

Py:   x in arr
来源：http://bai.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://ilz.xziqi.cn

JS:   arr.includes(x)
来源：http://pks.yuxming.cn

TS:   arr.includes(x)
来源：http://god.nwbrower.top

Java: list.contains(x)
来源：http://njn.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://wge.guannengcc.top

Ruby: arr.include?(x)
来源：http://bbe.9152youxi.cn

C#:   list.Contains(x)
来源：http://hpp.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://xmd.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wgb.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://utj.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rta.jqgufenzy.top

TS:   [...arr];
来源：http://gzs.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://tpz.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mts.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://hke.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://ani.ydzc1.top

[D23] reduce 累积计算
来源：http://rfk.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gfn.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jub.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sbs.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gsw.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qkx.yj20258888.top

Go:   // 手写循环
来源：http://orm.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jgi.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ezn.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://pzf.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wrn.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dib.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tnk.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jye.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vfg.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://spv.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pht.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vgi.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://jqq.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nyr.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nyr.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://god.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rxa.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tjc.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wkr.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hod.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oqj.tian-w.cn

[D26] 数组转字符串
来源：http://why.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://vyd.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://ajt.yueranfly.top

JS:   arr.join(", ")
来源：http://epk.birdmap.top

TS:   arr.join(", ")
来源：http://jdw.sxryk.cn

Java: String.join(", ", list)
来源：http://cer.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://kpv.hfpthk.cn

Ruby: arr.join(", ")
来源：http://iza.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://dta.pycfn.com

================================================================================
来源：http://vvn.xziqi.cn

E. 字符串处理
来源：http://kha.vqdsnc.cn

================================================================================
来源：http://xtb.gaohongyu789.top

[E01] 拼接字符串
来源：http://yok.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dbd.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yrz.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zrl.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwl.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vaq.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sjl.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fnk.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aca.tianlin.xyz

[E02] 重复字符串
来源：http://ich.52xcode.cn

Py:   "ab" * 3
来源：http://cxn.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://pdd.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://drz.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://mzh.shzxlz.cn

Java: "ab".repeat(3)
来源：http://vhr.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://axc.tarul.cn

Ruby: "ab" * 3
来源：http://zng.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yiy.zhijiandao.cn

[E03] 截取子串
来源：http://kke.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hdx.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zzw.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pyy.316326.xyz

TS:   s.slice(1, 4)
来源：http://gbr.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://dra.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qgd.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://pao.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://ctz.pycfn.com

[E04] 查找子串位置
来源：http://iit.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://lsq.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://vic.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hyu.yfazqb.com

TS:   s.indexOf("x")
来源：http://olo.daria6918.cn

Java: s.indexOf("x")
来源：http://kfn.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://ocj.zhijiandao.cn

Ruby: s.index("x")
来源：http://dzo.xziqi.cn

C#:   s.IndexOf("x")
来源：http://zpi.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zzd.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://isx.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dde.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yon.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ebs.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qcf.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tbr.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://akd.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rbj.sweek.top

[E06] 替换子串
来源：http://oyv.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rvz.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://flh.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fjv.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://wzv.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oee.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hwt.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://grb.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://wma.52xcode.cn

[E07] 按分隔符拆分
来源：http://elb.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fsu.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cfc.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vfq.chenlongwang.top

TS:   s.split(",")
来源：http://bag.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jgd.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fzu.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://haf.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ycf.meibo888.top

[E08] 数组按分隔符合并
来源：http://pks.birdmap.top

Py:   ",".join(items)
来源：http://cry.yj202588.top

PHP:  implode(",", $items);
来源：http://pnc.cucudq.cn

JS:   items.join(",")
来源：http://eix.cqqwz.cn

TS:   items.join(",")
来源：http://gsn.mhx1999.top

Java: String.join(",", items)
来源：http://ffh.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://pde.wangshuangyany.cn

Ruby: items.join(",")
来源：http://bri.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://fjj.zycfv.cn

[E09] 去除所有空白字符
来源：http://vyb.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hat.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bmx.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://rtz.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://mjm.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://kon.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qsk.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hcp.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyn.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://xat.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kdf.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cxr.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://zsr.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://yqp.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://ojj.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jtj.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://raq.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hwe.zdbjq.cn

[E11] 反转字符串
来源：http://zkq.ivvv.top

Py:   s[::-1]
来源：http://dvc.wangdashe.top

PHP:  strrev($s);
来源：http://iag.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://asd.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://glv.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sdb.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://isb.zdbjq.cn

Ruby: s.reverse
来源：http://gcq.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://xqp.316326.xyz

[E12] 统计某字符出现次数
来源：http://bar.pycfn.com

Py:   s.count("a")
来源：http://jqt.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://tfi.xinyue.icu

JS:   s.split("a").length - 1
来源：http://ild.xuanzx.com

TS:   s.split("a").length - 1
来源：http://rik.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://edl.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://fcm.hysaishi.cn

Ruby: s.count("a")
来源：http://qiw.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://abp.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://dwt.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://uuw.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kzw.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://huw.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uey.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fsg.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hul.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vda.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nka.wangdashe.top

[E14] URL 编码与 Base64
来源：http://zkr.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fdn.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzj.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lly.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yge.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://whk.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://poh.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dtm.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tkb.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://nck.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eku.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zyz.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rhj.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://wug.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cyz.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dgq.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eqg.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sut.gotoacloud.top

[E16] 数字千分位
来源：http://ynw.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://tdd.bjfxy.top

PHP:  number_format(1234567);
来源：http://efp.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lyu.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://scr.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ygs.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lzo.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xpt.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://mjb.jinghuilouyu.cn

[E17] 首字母大写
来源：http://fgi.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iad.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yac.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upo.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzh.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://may.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bca.daxiang520.top

Ruby: s.capitalize
来源：http://jlw.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://puy.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://jmt.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vtm.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bzw.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dgl.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jai.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lhm.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ydp.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fwi.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nka.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://tus.hnqzz.top

Py:   s.splitlines()
来源：http://sbh.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hij.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://uot.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://uxo.feifeiyinyue.top

Java: s.lines().toList()
来源：http://vux.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://nul.xinyue.icu


<!-- 参考信息 -->