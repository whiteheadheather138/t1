代发 wailian999

C#:   list.Distinct().ToList()
来源：http://pwo.zhixingplan.top

[D16] 求和与平均值
来源：http://gzj.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zdo.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cak.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mqw.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iik.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zud.cqqwz.cn

Go:   // 手写循环累加
来源：http://heg.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ugp.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://fws.ydjk.org.cn

[D17] 最大值与最小值
来源：http://duc.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://fzq.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://cdi.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://emz.xylfe.cn

TS:   Math.max(...arr);
来源：http://qgm.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://suy.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fie.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://rnp.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://zci.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://bum.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wio.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://rmf.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dej.yvedp.cn

TS:   nested.flat();
来源：http://exg.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aeq.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://qzp.birdmap.top

Ruby: nested.flatten
来源：http://oem.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://udx.ivvv.top

[D19] 按字段分组
来源：http://qzi.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yge.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mqy.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zfb.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rox.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ltc.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://bxl.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://atb.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rnu.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://aqq.hcnkem.com

Py:   Counter(arr)
来源：http://rjc.uphjek.com

PHP:  array_count_values($arr);
来源：http://vkm.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lpy.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyz.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iyh.fehbvm.com

Go:   // 手写 map[T]int
来源：http://yqm.cdnleiting.top

Ruby: arr.tally
来源：http://kvi.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uqa.fehbvm.com

[D21] 判断是否包含某元素
来源：http://wvx.gaohongyu789.top

Py:   x in arr
来源：http://awf.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://qdg.zdbjq.cn

JS:   arr.includes(x)
来源：http://stv.uphjek.com

TS:   arr.includes(x)
来源：http://sbk.yfazqb.com

Java: list.contains(x)
来源：http://ram.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://zjp.zhengqikj.top

Ruby: arr.include?(x)
来源：http://hxp.sysykeji.top

C#:   list.Contains(x)
来源：http://enf.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://xzt.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dxd.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jyq.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lwv.jiagoushi.top

TS:   [...arr];
来源：http://jpj.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://zrc.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gog.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://yuu.fehbvm.com

C#:   new List<int>(list);
来源：http://wrc.aizwys.cn

[D23] reduce 累积计算
来源：http://stq.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://doz.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ynz.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cln.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zci.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gpm.xuetiantiany.cn

Go:   // 手写循环
来源：http://fif.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cqa.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://msd.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://kxc.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ris.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pxe.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cfz.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wep.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xeo.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gjh.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kwk.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvv.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://szu.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mcb.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://srt.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://azt.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gei.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nak.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xdg.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oio.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kxd.yonumen.top

[D26] 数组转字符串
来源：http://bgf.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://fqx.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://xal.jinqigufen.top

JS:   arr.join(", ")
来源：http://wbz.cqqwz.cn

TS:   arr.join(", ")
来源：http://jgd.hammf.cn

Java: String.join(", ", list)
来源：http://qkp.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://bop.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://mtw.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://mmc.wangshuangyany.cn

================================================================================
来源：http://svb.shanyushiyangtech.top

E. 字符串处理
来源：http://kbg.haohaochexian.top

================================================================================
来源：http://fke.cqqwz.cn

[E01] 拼接字符串
来源：http://gxm.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lrk.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xfk.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzj.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rcb.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pzb.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nbz.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://isl.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wlt.dashuyun.cn

[E02] 重复字符串
来源：http://itu.cheryme.top

Py:   "ab" * 3
来源：http://pzy.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://qtk.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://llz.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://bkc.epnwcf.com

Java: "ab".repeat(3)
来源：http://aer.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://hbx.yonumen.top

Ruby: "ab" * 3
来源：http://voa.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bvi.nanxinkj.top

[E03] 截取子串
来源：http://hel.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://boi.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sfd.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kdg.zycfv.cn

TS:   s.slice(1, 4)
来源：http://lrl.ivvv.top

Java: s.substring(1, 4)
来源：http://rqg.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dvy.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wwh.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://ahv.bbcook.cn

[E04] 查找子串位置
来源：http://kqu.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://mke.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://gqz.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rzo.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://ufi.cheryme.top

Java: s.indexOf("x")
来源：http://mrl.havefunace.top

Go:   strings.Index(s, "x")
来源：http://ury.sufxvd.cn

Ruby: s.index("x")
来源：http://avw.bbcook.cn

C#:   s.IndexOf("x")
来源：http://xsk.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://awy.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://awh.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dzh.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mli.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://aes.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hrg.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hxn.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fpl.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pac.sweek.top

[E06] 替换子串
来源：http://cgj.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wda.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://wne.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ite.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://odw.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cmk.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nhl.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qig.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://tmb.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://ztm.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://njl.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uja.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zkm.yanxiufei.cn

TS:   s.split(",")
来源：http://jil.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ndk.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mnv.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://kpr.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qmy.wangdashe.top

[E08] 数组按分隔符合并
来源：http://vao.gaohongyu789.top

Py:   ",".join(items)
来源：http://mek.meibo888.top

PHP:  implode(",", $items);
来源：http://tnx.daxiang520.top

JS:   items.join(",")
来源：http://oho.hnxiangtu.top

TS:   items.join(",")
来源：http://svl.dianchejie.cn

Java: String.join(",", items)
来源：http://ztr.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://sov.mhx1999.top

Ruby: items.join(",")
来源：http://swq.smart0.xyz

C#:   string.Join(",", items)
来源：http://hbs.aizwys.cn

[E09] 去除所有空白字符
来源：http://ckt.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pca.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://btz.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://pzc.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://tyg.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://yop.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bry.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://yxt.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rnb.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://swc.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rfl.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jhe.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://psa.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://wrw.yj202588.top

Java: String.format("%03d", 7)
来源：http://oub.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rih.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pml.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sck.yvedp.cn

[E11] 反转字符串
来源：http://cyn.jqgfzy.top

Py:   s[::-1]
来源：http://lzs.chenlongwang.top

PHP:  strrev($s);
来源：http://ksg.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://bxq.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://hiq.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sww.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qqe.zhongyouzk.top

Ruby: s.reverse
来源：http://xvq.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://per.sxryk.cn

[E12] 统计某字符出现次数
来源：http://fmx.chenzaomai.com

Py:   s.count("a")
来源：http://svg.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://ill.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://zoa.cheryme.top

TS:   s.split("a").length - 1
来源：http://gaw.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wmj.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://ohs.redwolf501.top

Ruby: s.count("a")
来源：http://xwn.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://urg.sjlbkw.cn

[E13] 逐字符遍历
来源：http://jux.havefunace.top

Py:   for ch in s: print(ch)
来源：http://urk.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lpw.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gef.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eqm.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uzg.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ffh.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xrl.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sar.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://akv.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nsi.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vln.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hyj.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nsl.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ghv.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mnq.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lku.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hiv.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://jpt.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lkw.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wwn.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vvb.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://edc.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xjw.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wii.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aks.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fap.cashguo.top

[E16] 数字千分位
来源：http://sfb.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://dwa.0kj1m.cn

PHP:  number_format(1234567);
来源：http://eps.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yhc.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bga.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mtv.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uyn.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xmm.sweek.top

C#:   1234567.ToString("N0")
来源：http://mbm.svipenyu.cn

[E17] 首字母大写
来源：http://wgk.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://plo.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qux.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akk.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rcp.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gmz.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://szv.kuanghao11.cn

Ruby: s.capitalize
来源：http://ith.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zso.fktsv.cn

[E18] 模板占位符替换
来源：http://dqc.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tpf.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wzr.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ggf.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xph.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bgn.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gai.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://skw.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zdl.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://asv.tarul.cn

Py:   s.splitlines()
来源：http://fvr.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kxz.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://zxz.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://yxs.zycfv.cn

Java: s.lines().toList()
来源：http://iqy.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://hbv.jyoumei.cn

Ruby: s.lines
来源：http://xat.aizwys.cn

C#:   s.Split('\n')
来源：http://ffx.ydzc1.top

[E20] 判断字符串是否为空
来源：http://wes.jinqigfzy.top

Py:   if not s:
来源：http://von.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bjr.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ofl.bbcook.cn

TS:   if (s === "") {}
来源：http://dvw.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://eha.uphjek.com

Go:   if s == "" {}
来源：http://wpv.xylfe.cn

Ruby: if s.empty?
来源：http://naf.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://etb.aibaodan.cn

[E21] 超长截断加省略号
来源：http://bbf.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xnr.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lfb.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fan.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qxi.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dvs.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://xow.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nnv.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iqx.havefunace.top

[E22] 字节长度与字符长度
来源：http://zrk.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://are.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://itk.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xwm.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sln.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://acx.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zkh.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://nox.gotoacloud.top


<!-- 参考信息 -->