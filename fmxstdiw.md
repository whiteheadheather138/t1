代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mzg.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://bqm.smart0.xyz

[D17] 最大值与最小值
来源：http://eoi.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://xru.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://fbn.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ujv.svipenyu.cn

TS:   Math.max(...arr);
来源：http://wxq.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bbu.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xgc.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://rza.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://pqx.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://kpj.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cgx.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://bxq.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://plq.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://boa.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iuo.zhixingplan.top

Go:   // 手写双层循环
来源：http://qic.ehwqpu.com

Ruby: nested.flatten
来源：http://vfg.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qvj.sjlbkw.cn

[D19] 按字段分组
来源：http://njb.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nal.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bji.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jee.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wny.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fzg.cashguo.top

Go:   // 手写 map[string][]T
来源：http://bkm.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rin.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rci.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://pnr.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://ymt.zycfv.cn

PHP:  array_count_values($arr);
来源：http://exj.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erf.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://viu.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zcp.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://ixs.feifeiyinyue.top

Ruby: arr.tally
来源：http://obn.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lip.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://yay.kuanghao11.cn

Py:   x in arr
来源：http://opf.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://adw.52xcode.cn

JS:   arr.includes(x)
来源：http://ilp.cucudq.cn

TS:   arr.includes(x)
来源：http://zbk.shangyingyoupin.top

Java: list.contains(x)
来源：http://mwx.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://shx.pycfn.com

Ruby: arr.include?(x)
来源：http://ioa.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://cnd.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://hec.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bhw.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qzg.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qlt.bjfxy.top

TS:   [...arr];
来源：http://ijq.ydzc1.top

Java: new ArrayList<>(list);
来源：http://wdv.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://atd.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://ktb.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://jbn.yj20258.top

[D23] reduce 累积计算
来源：http://vcx.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ixn.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gil.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eiy.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://coo.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xlo.wangshuangyany.cn

Go:   // 手写循环
来源：http://jie.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pdm.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xrl.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://bop.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://glp.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://edw.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jaw.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://abg.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hvf.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://umy.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qkf.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mmh.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://jdr.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://asx.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ida.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://msu.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lpl.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rux.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oak.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ufh.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jfr.mhx1999.top

[D26] 数组转字符串
来源：http://jxe.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://zth.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://ycm.sjlbkw.cn

JS:   arr.join(", ")
来源：http://rvn.epnwcf.com

TS:   arr.join(", ")
来源：http://atr.hysaishi.cn

Java: String.join(", ", list)
来源：http://ukf.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://ziy.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://dlv.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://oho.yfazqb.com

================================================================================
来源：http://lek.jqgufenzy.top

E. 字符串处理
来源：http://bfs.pengpengdd.cyou

================================================================================
来源：http://nhd.mhx1999.top

[E01] 拼接字符串
来源：http://rvb.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dxm.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gqb.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lht.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cza.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ycf.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rsl.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ers.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vex.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://bkg.pengpengdd.cyou

Py:   "ab" * 3
来源：http://opk.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://gvo.ydzc1.top

JS:   "ab".repeat(3)
来源：http://roh.cheryme.top

TS:   "ab".repeat(3)
来源：http://kix.yj202588.top

Java: "ab".repeat(3)
来源：http://gbo.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://qtt.gaohongyu789.top

Ruby: "ab" * 3
来源：http://mbt.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sct.ivvv.top

[E03] 截取子串
来源：http://vhp.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fpl.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ohn.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rop.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://aub.cqqwz.cn

Java: s.substring(1, 4)
来源：http://tzc.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uxx.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://ocz.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://xsx.zdqjudy.top

[E04] 查找子串位置
来源：http://wgj.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://qtz.ydzc1.top

PHP:  strpos($s, "x");
来源：http://xgm.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xoj.cashguo.top

TS:   s.indexOf("x")
来源：http://xam.tianlin.xyz

Java: s.indexOf("x")
来源：http://wlu.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://lnm.tian-w.cn

Ruby: s.index("x")
来源：http://prk.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://rgd.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fei.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ttt.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fof.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rkk.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nvv.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gby.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://swu.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gnl.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ljv.xuanzx.com

[E06] 替换子串
来源：http://jmt.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uxz.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://nva.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdl.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://gzy.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uni.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://emi.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://day.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://fkc.vehdjk.com

[E07] 按分隔符拆分
来源：http://yly.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zpb.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kaq.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fnf.ivvv.top

TS:   s.split(",")
来源：http://yeg.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wva.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qyj.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://plg.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dnz.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://ksc.ivvv.top

Py:   ",".join(items)
来源：http://cac.sweek.top

PHP:  implode(",", $items);
来源：http://uuj.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://uzv.redwolf501.top

TS:   items.join(",")
来源：http://ngj.ivvv.top

Java: String.join(",", items)
来源：http://lbc.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://knn.gzhubu.top

Ruby: items.join(",")
来源：http://plk.sufxvd.cn

C#:   string.Join(",", items)
来源：http://ode.ctjpmb.com

[E09] 去除所有空白字符
来源：http://pdr.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pna.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ltd.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://qby.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ovu.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://epa.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://krs.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://ncc.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eys.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://ett.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dcp.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ppb.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://ura.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://isj.bbcook.cn

Java: String.format("%03d", 7)
来源：http://chz.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mrj.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://art.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxx.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://bex.yfazqb.com

Py:   s[::-1]
来源：http://fkr.havefunace.top

PHP:  strrev($s);
来源：http://juu.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://ytn.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://vtb.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vld.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://jyl.fanxiaobao.xyz

Ruby: s.reverse
来源：http://qrm.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://nju.daxiang520.top

[E12] 统计某字符出现次数
来源：http://vki.aizwys.cn

Py:   s.count("a")
来源：http://vqj.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://syn.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://tdb.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://rvd.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zek.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://aek.tian-w.cn

Ruby: s.count("a")
来源：http://bpd.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://ziw.bjfxy.top

[E13] 逐字符遍历
来源：http://bbq.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://iku.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdh.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vlb.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bfx.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tsw.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zne.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://szv.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xwq.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://dxa.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cnb.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zyo.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ecv.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jjw.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wnl.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://twb.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wkt.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqh.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://qdg.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wdt.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dsp.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oea.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://apf.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mqz.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://unx.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ruz.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tmd.cdnleiting.top

[E16] 数字千分位
来源：http://rmg.c1oappe.top

Py:   f"{1234567:,}"
来源：http://arm.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://akm.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hih.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fwz.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gfl.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cwc.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rvb.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://mmy.jinqigufen.top

[E17] 首字母大写
来源：http://lxg.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hck.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://czd.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rsb.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://twh.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hjo.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://htt.sysykeji.top

Ruby: s.capitalize
来源：http://tsf.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yhb.gotoacloud.top

[E18] 模板占位符替换
来源：http://ydv.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://spk.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xvb.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://kzk.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://teg.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gyn.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rcd.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://elm.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://byv.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://nfk.gogol.net.cn

Py:   s.splitlines()
来源：http://hde.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dfx.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://vtz.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://ocg.wangdashe.top

Java: s.lines().toList()
来源：http://iac.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://chd.bbcook.cn

Ruby: s.lines
来源：http://esd.yueranfly.top

C#:   s.Split('\n')
来源：http://fns.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://jhm.sjlbkw.cn

Py:   if not s:
来源：http://vxl.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cqe.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://riy.yj202588.top

TS:   if (s === "") {}
来源：http://foc.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://ytp.zhiwuduotai.top

Go:   if s == "" {}
来源：http://hxa.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://mtj.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xjn.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://poo.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://njr.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://guf.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ygu.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsr.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://akz.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://law.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vpx.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kix.xziqi.cn

[E22] 字节长度与字符长度
来源：http://rvc.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oyg.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ybk.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fuy.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ptq.c1oappe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://itd.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zuv.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://xny.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ozn.ppjwa.cn

================================================================================
来源：http://mwh.kuanghao11.cn

F. 文件与目录
来源：http://lgl.jinqigufen.top

================================================================================
来源：http://amk.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://pvg.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://azi.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://ecv.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fpg.jqgufenzy.top


<!-- 参考信息 -->