代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xvg.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://srj.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://woc.ydzc1.top

Go:   // 手写循环累加
来源：http://mnd.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://owd.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://nsd.aizwys.cn

[D17] 最大值与最小值
来源：http://ttj.meibo888.top

Py:   max(arr);  min(arr)
来源：http://xpx.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://jtc.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qvy.iojbl.cn

TS:   Math.max(...arr);
来源：http://jap.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ocv.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ird.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://wcd.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://bgc.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://cbh.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jcj.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://vlp.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qqz.jinghuilouyu.cn

TS:   nested.flat();
来源：http://bdj.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kcv.hfpthk.cn

Go:   // 手写双层循环
来源：http://wol.hcnkem.com

Ruby: nested.flatten
来源：http://ght.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://efp.vqdsnc.cn

[D19] 按字段分组
来源：http://zzd.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dvn.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://krp.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tsz.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwk.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zbm.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://fqh.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://zas.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dzm.pycfn.com

[D20] 统计每个元素出现次数
来源：http://szz.mhx1999.top

Py:   Counter(arr)
来源：http://ibt.hnqzz.top

PHP:  array_count_values($arr);
来源：http://iii.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mze.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ywc.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dju.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://xtf.vehdjk.com

Ruby: arr.tally
来源：http://nqs.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ebe.bbcook.cn

[D21] 判断是否包含某元素
来源：http://lxp.zdbjq.cn

Py:   x in arr
来源：http://xfd.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://rnk.hnxiangtu.top

JS:   arr.includes(x)
来源：http://xwb.ctjpmb.com

TS:   arr.includes(x)
来源：http://tko.aizwys.cn

Java: list.contains(x)
来源：http://mrk.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://trb.jyoumei.cn

Ruby: arr.include?(x)
来源：http://uwb.dianchejie.cn

C#:   list.Contains(x)
来源：http://lfm.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://skm.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ixr.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://egp.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ain.sweek.top

TS:   [...arr];
来源：http://unx.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://tlg.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://snf.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://ice.meibo888.top

C#:   new List<int>(list);
来源：http://fyw.daria6918.cn

[D23] reduce 累积计算
来源：http://jot.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ylb.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mzd.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bio.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ikl.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://emu.aizwys.cn

Go:   // 手写循环
来源：http://ljd.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cxq.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lbq.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://ftw.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sny.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wyn.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xxz.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yid.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vrx.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mqg.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pis.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://avh.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://bpp.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dqe.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ufd.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kig.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qzb.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vvu.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dzt.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xmz.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ftd.cashguo.top

[D26] 数组转字符串
来源：http://ylk.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://nrc.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://bqd.bbcook.cn

JS:   arr.join(", ")
来源：http://xgd.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://fou.daria6918.cn

Java: String.join(", ", list)
来源：http://tiq.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://wur.fktsv.cn

Ruby: arr.join(", ")
来源：http://dov.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://qes.meibo888.top

================================================================================
来源：http://xtj.haohaochexian.top

E. 字符串处理
来源：http://xgf.ehwqpu.com

================================================================================
来源：http://tdk.zdbjq.cn

[E01] 拼接字符串
来源：http://osz.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yzx.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dyc.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zuj.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cvm.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zkv.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yrk.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jdt.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gul.bbcook.cn

[E02] 重复字符串
来源：http://pgd.cashguo.top

Py:   "ab" * 3
来源：http://ufq.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://zqx.tanke756.top

JS:   "ab".repeat(3)
来源：http://jcx.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://ell.bbcook.cn

Java: "ab".repeat(3)
来源：http://ogt.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://pbl.ctjpmb.com

Ruby: "ab" * 3
来源：http://axx.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wgb.sxryk.cn

[E03] 截取子串
来源：http://viz.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gjr.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uno.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vpw.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://bia.hcnkem.com

Java: s.substring(1, 4)
来源：http://hyr.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pty.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://yzf.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://ick.daria6918.cn

[E04] 查找子串位置
来源：http://cpi.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://sei.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://rpr.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gij.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://skt.mhx1999.top

Java: s.indexOf("x")
来源：http://uzt.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://dmj.shangyingyoupin.top

Ruby: s.index("x")
来源：http://gef.yj20258888.top

C#:   s.IndexOf("x")
来源：http://vas.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://idf.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mzl.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://huo.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tgf.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://als.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://csb.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jdy.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sgl.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vqt.fengsongda.top

[E06] 替换子串
来源：http://rff.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hfu.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ace.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbw.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://yxx.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mhp.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tmc.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aal.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://eun.yueranfly.top

[E07] 按分隔符拆分
来源：http://byx.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ybs.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zqp.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://zyu.sxryk.cn

TS:   s.split(",")
来源：http://buo.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://mdy.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nyu.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://ibg.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qew.aizwys.cn

[E08] 数组按分隔符合并
来源：http://mve.iojbl.cn

Py:   ",".join(items)
来源：http://urr.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://irv.xuetiantiany.cn

JS:   items.join(",")
来源：http://lsi.tarul.cn

TS:   items.join(",")
来源：http://uzj.cqqwz.cn

Java: String.join(",", items)
来源：http://xjc.hammf.cn

Go:   strings.Join(items, ",")
来源：http://rmv.ybcxt.top

Ruby: items.join(",")
来源：http://tws.guowangkeji.top

C#:   string.Join(",", items)
来源：http://nys.shuidangran.top

[E09] 去除所有空白字符
来源：http://hao.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://utj.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dei.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://zyz.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://whu.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://dbh.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://shi.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xei.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dip.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://ptw.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oqi.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ums.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://obp.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://ufc.bjfxy.top

Java: String.format("%03d", 7)
来源：http://nzr.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zcz.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://skz.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gbp.sysykeji.top

[E11] 反转字符串
来源：http://ubf.hfpthk.cn

Py:   s[::-1]
来源：http://wzz.hysaishi.cn

PHP:  strrev($s);
来源：http://rem.meibo888.top

JS:   [...s].reverse().join("")
来源：http://gxd.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://uhv.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jui.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dpt.yj202588.top

Ruby: s.reverse
来源：http://tiv.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uaj.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://yju.yonumen.top

Py:   s.count("a")
来源：http://yrx.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://npp.smart0.xyz

JS:   s.split("a").length - 1
来源：http://eyr.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://ifi.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fss.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://rhe.hfpthk.cn

Ruby: s.count("a")
来源：http://ray.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://spg.jinqigfzy.top

[E13] 逐字符遍历
来源：http://lxq.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://zrf.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://exn.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nxe.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nia.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hwr.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ylu.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cwv.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tvt.birdmap.top

[E14] URL 编码与 Base64
来源：http://zez.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bqo.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvg.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://grh.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tuf.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dou.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ord.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cnm.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://csn.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://kdx.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uoh.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mfw.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gkv.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qpc.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://msu.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jdr.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rqv.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pau.pycfn.com

[E16] 数字千分位
来源：http://cbf.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://yso.hcnkem.com

PHP:  number_format(1234567);
来源：http://iqi.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wvz.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nnw.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qai.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://shm.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://myk.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://qnq.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://bdr.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gor.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tnp.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bok.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmc.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://seb.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://azg.meibo888.top

Ruby: s.capitalize
来源：http://ofw.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fug.vehdjk.com

[E18] 模板占位符替换
来源：http://tiq.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aom.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qks.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://qyi.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wqa.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ewq.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jiw.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngj.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xli.316326.xyz

[E19] 多行文本按行拆分
来源：http://nly.ybcxt.top

Py:   s.splitlines()
来源：http://qaw.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ext.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://gxp.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://dvl.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://zdd.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ivq.cdnleiting.top

Ruby: s.lines
来源：http://nsw.gzhubu.top

C#:   s.Split('\n')
来源：http://aoa.pycfn.com

[E20] 判断字符串是否为空
来源：http://ych.guowangkeji.top

Py:   if not s:
来源：http://osa.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kdv.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xuq.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://qra.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://ory.hysaishi.cn

Go:   if s == "" {}
来源：http://gyb.ctjpmb.com

Ruby: if s.empty?
来源：http://xxp.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wxz.yonumen.top

[E21] 超长截断加省略号
来源：http://oxt.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vjr.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ptn.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hgy.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ciu.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mlm.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://mqt.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iog.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nva.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://whj.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://roz.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wbu.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://igc.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ves.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cex.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dnn.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://prd.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cra.gaohongyu789.top

================================================================================
来源：http://vmp.zhengqikj.top

F. 文件与目录
来源：http://qqa.jinqigfzy.top

================================================================================
来源：http://iww.guannengcc.top


<!-- 参考信息 -->