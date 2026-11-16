代发 wailian999

TS:   [...new Set(arr)]
来源：http://vor.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jvi.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://lkl.xziqi.cn

Ruby: arr.uniq
来源：http://fjo.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://fwj.zdbjq.cn

[D16] 求和与平均值
来源：http://lqw.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vut.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xvt.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsj.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdu.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gwk.fktsv.cn

Go:   // 手写循环累加
来源：http://vdz.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jfc.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://ikx.andypj.xyz

[D17] 最大值与最小值
来源：http://fag.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://bxp.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://sxe.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://twv.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://jan.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dml.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nrc.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://jza.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://ksm.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://dwa.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rat.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://oxr.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ywj.aizwys.cn

TS:   nested.flat();
来源：http://qju.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ish.shuidangran.top

Go:   // 手写双层循环
来源：http://rbg.yj202588.top

Ruby: nested.flatten
来源：http://arx.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dps.xuetiantiany.cn

[D19] 按字段分组
来源：http://qsz.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ejm.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gwm.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ppe.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mwg.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ktr.cashguo.top

Go:   // 手写 map[string][]T
来源：http://xfv.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://est.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mzj.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://zyp.jinqigfzy.top

Py:   Counter(arr)
来源：http://eqe.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://frx.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxp.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dtf.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lva.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://xbp.dianchejie.cn

Ruby: arr.tally
来源：http://htp.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pad.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://jjf.bjfxy.top

Py:   x in arr
来源：http://upu.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://ncq.guannengcc.top

JS:   arr.includes(x)
来源：http://nlv.nwbrower.top

TS:   arr.includes(x)
来源：http://fwt.zhengqikj.top

Java: list.contains(x)
来源：http://ntn.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://zuf.tian-w.cn

Ruby: arr.include?(x)
来源：http://dqm.jlsjyb.cn

C#:   list.Contains(x)
来源：http://iua.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://bva.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gov.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zoi.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://axp.ivvv.top

TS:   [...arr];
来源：http://uke.fzhhl.top

Java: new ArrayList<>(list);
来源：http://llf.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gwz.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://ajs.chenlongwang.top

C#:   new List<int>(list);
来源：http://jqz.zhongyouzk.top

[D23] reduce 累积计算
来源：http://awm.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uag.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://atv.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jjh.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbs.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fpb.zdbjq.cn

Go:   // 手写循环
来源：http://exc.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://frq.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xll.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://ppy.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kja.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jaj.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mfq.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yxz.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qtc.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qwn.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ret.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mnk.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://tun.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dpq.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vnj.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wuy.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uzs.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nxj.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jql.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kwd.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cyj.cashguo.top

[D26] 数组转字符串
来源：http://nbg.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://ukc.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://ewx.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://tbt.ehwqpu.com

TS:   arr.join(", ")
来源：http://qit.sysykeji.top

Java: String.join(", ", list)
来源：http://rnn.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://kgn.sufxvd.cn

Ruby: arr.join(", ")
来源：http://thx.uphjek.com

C#:   string.Join(", ", list)
来源：http://buf.snrcjt.cn

================================================================================
来源：http://qup.guannengcc.top

E. 字符串处理
来源：http://ffq.zdbjq.cn

================================================================================
来源：http://nab.c1oappe.top

[E01] 拼接字符串
来源：http://mod.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xkl.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://urr.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://crl.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pej.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nhb.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ywa.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hfz.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ksd.hammf.cn

[E02] 重复字符串
来源：http://lug.bjfxy.top

Py:   "ab" * 3
来源：http://zgo.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://vuf.c1oappe.top

JS:   "ab".repeat(3)
来源：http://ezz.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://hkp.jyoumei.cn

Java: "ab".repeat(3)
来源：http://gxt.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://fmd.andypj.xyz

Ruby: "ab" * 3
来源：http://lsm.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pux.jqgufenzy.top

[E03] 截取子串
来源：http://ilf.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://diu.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ayr.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ggw.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://izm.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://ufc.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://anr.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tol.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://egu.pengpengdd.cyou

[E04] 查找子串位置
来源：http://jrp.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://dmg.mhx1999.top

PHP:  strpos($s, "x");
来源：http://szs.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ggn.andypj.xyz

TS:   s.indexOf("x")
来源：http://mko.yuxming.cn

Java: s.indexOf("x")
来源：http://xyc.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://yos.uphjek.com

Ruby: s.index("x")
来源：http://jmu.jianghu66.top

C#:   s.IndexOf("x")
来源：http://vjt.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://emb.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fkk.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cyv.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyp.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://kum.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ekg.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wgh.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tlz.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vkk.chenzaomai.com

[E06] 替换子串
来源：http://jri.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jfz.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://vfz.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://euk.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://gbr.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdm.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sxi.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://plo.cheryme.top

C#:   s.Replace("a", "b")
来源：http://sre.mhx1999.top

[E07] 按分隔符拆分
来源：http://fjp.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cjc.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://obw.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kkm.tian-w.cn

TS:   s.split(",")
来源：http://bly.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://vih.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://udj.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://agn.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xub.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://bkv.jianghu66.top

Py:   ",".join(items)
来源：http://jds.hfpthk.cn

PHP:  implode(",", $items);
来源：http://cez.ctjpmb.com

JS:   items.join(",")
来源：http://oqq.zhijiandao.cn

TS:   items.join(",")
来源：http://hsq.yueranfly.top

Java: String.join(",", items)
来源：http://qjg.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://uzj.zhiwuduotai.top

Ruby: items.join(",")
来源：http://nrs.xziqi.cn

C#:   string.Join(",", items)
来源：http://zoe.yvedp.cn

[E09] 去除所有空白字符
来源：http://vdw.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kyf.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://byx.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://yle.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://gkj.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://kyt.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://juq.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mks.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ppp.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://dwx.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tvj.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fvr.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://hlk.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://soj.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://isk.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mcb.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yia.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tgr.sxryk.cn

[E11] 反转字符串
来源：http://krv.zhixingplan.top

Py:   s[::-1]
来源：http://cuh.yfazqb.com

PHP:  strrev($s);
来源：http://ggh.pycfn.com

JS:   [...s].reverse().join("")
来源：http://gam.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://neo.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bol.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xig.vqdsnc.cn

Ruby: s.reverse
来源：http://nsu.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://nwm.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://yhn.iojbl.cn

Py:   s.count("a")
来源：http://qio.tarul.cn

PHP:  substr_count($s, "a");
来源：http://zrj.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://ich.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://hxr.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ncf.yj20258.top

Go:   strings.Count(s, "a")
来源：http://shv.ybcxt.top

Ruby: s.count("a")
来源：http://pzh.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://tnf.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://syr.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://ogz.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ftx.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nbp.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yym.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://owf.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cfo.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lqh.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://skc.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://qdz.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qky.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dij.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mwz.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tqi.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://npm.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kkk.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mra.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dyg.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://wzb.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fhb.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pxe.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zlx.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jrh.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kuf.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uum.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zea.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qwo.chenlongwang.top

[E16] 数字千分位
来源：http://xzo.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://nms.yangfankeji.com

PHP:  number_format(1234567);
来源：http://kzw.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://www.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hai.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://elt.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kwv.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gxp.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://odd.vqdsnc.cn

[E17] 首字母大写
来源：http://pbf.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iur.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nro.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vpo.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hym.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dqz.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uvz.birdmap.top

Ruby: s.capitalize
来源：http://jkx.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rnf.zdbjq.cn

[E18] 模板占位符替换
来源：http://xqn.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xlh.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jvg.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ble.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ocq.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wfx.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bwl.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vvx.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sqw.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://yqz.haohaochexian.top

Py:   s.splitlines()
来源：http://zpu.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qmb.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://yxr.sweek.top

TS:   s.split(/\r?\n/)
来源：http://fzz.yanxiufei.cn

Java: s.lines().toList()
来源：http://chu.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://vgf.0kj1m.cn

Ruby: s.lines
来源：http://rwr.snrcjt.cn

C#:   s.Split('\n')
来源：http://uyk.meibo888.top

[E20] 判断字符串是否为空
来源：http://ceh.vqdsnc.cn

Py:   if not s:
来源：http://gbp.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hgx.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ivl.aibaodan.cn

TS:   if (s === "") {}
来源：http://qqv.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://nwy.316326.xyz

Go:   if s == "" {}
来源：http://ojq.xuanzx.com

Ruby: if s.empty?
来源：http://dsl.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jbe.fzhhl.top

[E21] 超长截断加省略号
来源：http://ewo.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kxy.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://msx.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pto.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dyu.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aux.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://scq.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dmp.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nos.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://ouq.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iwj.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqg.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ifv.gotoacloud.top


<!-- 参考信息 -->