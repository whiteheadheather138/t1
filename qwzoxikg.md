代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://rom.tarul.cn

Go:   // 手写循环
来源：http://iqh.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://adp.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tsl.zhoulong.xyz

[D15] 去重
来源：http://clh.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uhh.bbcook.cn

PHP:  array_unique($arr);
来源：http://wna.bjfxy.top

JS:   [...new Set(arr)]
来源：http://joa.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://ovy.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hni.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ngn.haohaochexian.top

Ruby: arr.uniq
来源：http://rkc.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://dyw.hesvh.cn

[D16] 求和与平均值
来源：http://wto.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dvq.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://adc.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jea.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://auv.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xsz.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://pla.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gdr.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://gtu.yongpay.top

[D17] 最大值与最小值
来源：http://qah.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://ils.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://mlf.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wje.nanxinkj.top

TS:   Math.max(...arr);
来源：http://xch.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zzw.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yxi.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://ffm.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://afc.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://jnq.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sxa.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://btj.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xbt.aibaodan.cn

TS:   nested.flat();
来源：http://yrm.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qgo.nwbrower.top

Go:   // 手写双层循环
来源：http://owt.zdbjq.cn

Ruby: nested.flatten
来源：http://gdd.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://baq.yongpay.top

[D19] 按字段分组
来源：http://rfj.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uwj.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oix.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jto.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://prz.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wsz.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://iam.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://weu.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gvd.tanke756.top

[D20] 统计每个元素出现次数
来源：http://apz.iojbl.cn

Py:   Counter(arr)
来源：http://fhb.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://hlj.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yxs.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cha.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://etl.daria6918.cn

Go:   // 手写 map[T]int
来源：http://wyk.gotoacloud.top

Ruby: arr.tally
来源：http://myd.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lns.52xcode.cn

[D21] 判断是否包含某元素
来源：http://hhw.jlsjyb.cn

Py:   x in arr
来源：http://rwn.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://eus.meibo888.top

JS:   arr.includes(x)
来源：http://snx.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://wgn.zdbjq.cn

Java: list.contains(x)
来源：http://nml.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://lvj.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://tlg.zdbjq.cn

C#:   list.Contains(x)
来源：http://ekf.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://cdw.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mth.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oea.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wqt.redwolf501.top

TS:   [...arr];
来源：http://dgn.hesvh.cn

Java: new ArrayList<>(list);
来源：http://giv.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ykd.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://lwh.zhijiandao.cn

C#:   new List<int>(list);
来源：http://wof.nanxuanxn.top

[D23] reduce 累积计算
来源：http://cge.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jda.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://scr.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://flf.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbt.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iwq.guowangkeji.top

Go:   // 手写循环
来源：http://vge.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vxb.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rkv.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://cgp.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xgm.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vij.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dav.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://roi.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cyi.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mww.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mwx.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blj.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://hnt.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzr.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://utu.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uyz.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zoo.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sko.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baj.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://szm.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rog.vqdsnc.cn

[D26] 数组转字符串
来源：http://tjg.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://xua.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://alf.gzhubu.top

JS:   arr.join(", ")
来源：http://xnh.yfazqb.com

TS:   arr.join(", ")
来源：http://mkl.9152youxi.cn

Java: String.join(", ", list)
来源：http://uij.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://jps.pycfn.com

Ruby: arr.join(", ")
来源：http://bic.hammf.cn

C#:   string.Join(", ", list)
来源：http://zqq.cheryme.top

================================================================================
来源：http://emy.gogol.net.cn

E. 字符串处理
来源：http://yww.yanxiufei.cn

================================================================================
来源：http://hlw.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://hbu.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vha.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bct.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://htr.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aoc.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ben.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jxh.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jsh.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qzk.jinqigfzy.top

[E02] 重复字符串
来源：http://bis.gotoacloud.top

Py:   "ab" * 3
来源：http://ojv.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://elr.yueranfly.top

JS:   "ab".repeat(3)
来源：http://mrl.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://frs.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://dli.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://gxk.yuxming.cn

Ruby: "ab" * 3
来源：http://vmp.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://flj.wangdashe.top

[E03] 截取子串
来源：http://xbq.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iqc.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gfw.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cfs.shuidangran.top

TS:   s.slice(1, 4)
来源：http://nwz.snrcjt.cn

Java: s.substring(1, 4)
来源：http://fpg.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qvp.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xbm.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://jvc.xuetiantiany.cn

[E04] 查找子串位置
来源：http://pxo.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://gpa.ybcxt.top

PHP:  strpos($s, "x");
来源：http://vcj.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://osk.xuanzx.com

TS:   s.indexOf("x")
来源：http://xeo.yangfankeji.com

Java: s.indexOf("x")
来源：http://zel.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://gsm.zycfv.cn

Ruby: s.index("x")
来源：http://eru.mhx1999.top

C#:   s.IndexOf("x")
来源：http://oxa.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mje.yj20258.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://stm.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nzo.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lra.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vmm.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwm.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gff.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kir.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xwr.jinqigufen.top

[E06] 替换子串
来源：http://omv.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ojt.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://qwy.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iqb.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://fhb.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ieg.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qfx.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vnm.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://iya.sysykeji.top

[E07] 按分隔符拆分
来源：http://jmr.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tmy.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uka.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zye.nwbrower.top

TS:   s.split(",")
来源：http://tjz.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://ydz.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://chp.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://fmc.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dws.xziqi.cn

[E08] 数组按分隔符合并
来源：http://hbc.c1oappe.top

Py:   ",".join(items)
来源：http://dvk.gotoacloud.top

PHP:  implode(",", $items);
来源：http://guh.hnqzz.top

JS:   items.join(",")
来源：http://fzi.jinqigufen.top

TS:   items.join(",")
来源：http://rrh.tanke756.top

Java: String.join(",", items)
来源：http://puy.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://kwm.epnwcf.com

Ruby: items.join(",")
来源：http://gps.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://lbp.cucudq.cn

[E09] 去除所有空白字符
来源：http://nlo.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qyx.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sym.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://gmo.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://ajz.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://ejq.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yoq.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://hbx.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zem.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://nij.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vct.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uby.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://txo.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://eld.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://nyo.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fdj.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kmn.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://awe.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://fbo.fzhhl.top

Py:   s[::-1]
来源：http://dbu.yongpay.top

PHP:  strrev($s);
来源：http://lnv.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://rrx.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://hxp.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dlv.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ynx.sweek.top

Ruby: s.reverse
来源：http://sxk.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://bjj.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://hgy.hywenlv.cn

Py:   s.count("a")
来源：http://lqq.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://ihf.316326.xyz

JS:   s.split("a").length - 1
来源：http://uei.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://cub.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cgv.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://zsa.xuanzx.com

Ruby: s.count("a")
来源：http://ohr.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://lti.hnqzz.top

[E13] 逐字符遍历
来源：http://ucl.cheryme.top

Py:   for ch in s: print(ch)
来源：http://jbw.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zli.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ilu.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rnk.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vqc.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vwu.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rrz.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://roc.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://xpr.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dlc.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ihl.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zuf.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pxz.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tdi.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xrc.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nii.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jzf.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://xrx.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jso.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hew.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://axb.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fdi.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tdn.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tad.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ime.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bnb.cqqwz.cn

[E16] 数字千分位
来源：http://got.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://drz.iojbl.cn

PHP:  number_format(1234567);
来源：http://blp.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jua.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ssy.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qut.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kzv.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nyi.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://vcb.ybcxt.top

[E17] 首字母大写
来源：http://wdw.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sdz.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zyd.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkt.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmg.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kvs.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xhd.uphjek.com

Ruby: s.capitalize
来源：http://wud.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://njx.sjlbkw.cn

[E18] 模板占位符替换
来源：http://rmd.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dzm.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tzs.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ngl.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://svm.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://psq.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wuv.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rzb.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vab.wangdashe.top

[E19] 多行文本按行拆分
来源：http://mim.zhengqikj.top

Py:   s.splitlines()
来源：http://lww.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vis.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://ijq.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://efp.aizwys.cn

Java: s.lines().toList()
来源：http://mzc.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://lfp.hysaishi.cn

Ruby: s.lines
来源：http://dav.nanxinkj.top

C#:   s.Split('\n')
来源：http://yed.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://fsp.yanxiufei.cn

Py:   if not s:
来源：http://gka.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vzn.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mek.hcnkem.com

TS:   if (s === "") {}
来源：http://dzv.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://ihr.sweek.top

Go:   if s == "" {}
来源：http://qhp.pycfn.com

Ruby: if s.empty?
来源：http://ejd.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cck.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://dew.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sdn.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://byn.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wob.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqk.jqgufenzy.top


<!-- 参考信息 -->