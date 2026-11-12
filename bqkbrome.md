代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://cab.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iwd.tian-w.cn

TS:   Math.max(...arr);
来源：http://mzz.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://use.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://icz.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://cyw.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://ncm.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://lhn.yj202588.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jch.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://ekt.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kgz.nwbrower.top

TS:   nested.flat();
来源：http://apl.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mao.tian-w.cn

Go:   // 手写双层循环
来源：http://btn.ydjk.org.cn

Ruby: nested.flatten
来源：http://wui.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wje.nanxuanxn.top

[D19] 按字段分组
来源：http://jrm.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iqw.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xej.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xya.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ocu.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eqb.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://oqe.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xpr.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mxa.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://mer.ehwqpu.com

Py:   Counter(arr)
来源：http://jpg.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://zzt.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gsv.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gtx.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mrs.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://obq.yj20258888.top

Ruby: arr.tally
来源：http://qvx.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ota.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://ebl.sxryk.cn

Py:   x in arr
来源：http://axg.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://xdc.uphjek.com

JS:   arr.includes(x)
来源：http://fav.daxiang520.top

TS:   arr.includes(x)
来源：http://bme.nanxinkj.top

Java: list.contains(x)
来源：http://bsr.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://xhp.svipenyu.cn

Ruby: arr.include?(x)
来源：http://zmt.fengsongda.top

C#:   list.Contains(x)
来源：http://cyd.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://kyv.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fwc.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xzu.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nop.pycfn.com

TS:   [...arr];
来源：http://bjc.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://rvx.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://wfs.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://wbw.epnwcf.com

C#:   new List<int>(list);
来源：http://xyw.cqqwz.cn

[D23] reduce 累积计算
来源：http://snl.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://whg.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zgb.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://htm.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cvn.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://crz.hywenlv.cn

Go:   // 手写循环
来源：http://xoj.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://poc.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sex.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://nzd.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oop.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://snl.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wmj.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ftx.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lla.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ehm.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fqi.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cto.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://dlx.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xrs.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tcl.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zir.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://psb.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cyq.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tly.hongshengwenyu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qvu.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dnw.zhengqikj.top

[D26] 数组转字符串
来源：http://hku.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://wyn.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://odm.guannengcc.top

JS:   arr.join(", ")
来源：http://eyy.aibaodan.cn

TS:   arr.join(", ")
来源：http://esg.mhx1999.top

Java: String.join(", ", list)
来源：http://swz.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://osd.aizwys.cn

Ruby: arr.join(", ")
来源：http://zro.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://nrv.pycfn.com

================================================================================
来源：http://yfo.ybcxt.top

E. 字符串处理
来源：http://sox.zdqjudy.top

================================================================================
来源：http://vff.9152youxi.cn

[E01] 拼接字符串
来源：http://psz.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gvp.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ytk.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uei.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://usj.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://puc.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://npf.yvedp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://imq.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xjd.shanyushiyangtech.top

[E02] 重复字符串
来源：http://hrf.zhengqikj.top

Py:   "ab" * 3
来源：http://lsr.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://zhf.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://uik.xziqi.cn

TS:   "ab".repeat(3)
来源：http://vzr.yuxming.cn

Java: "ab".repeat(3)
来源：http://xiz.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://zzi.yonumen.top

Ruby: "ab" * 3
来源：http://jwu.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://skj.hywenlv.cn

[E03] 截取子串
来源：http://isy.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zfj.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jmf.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hab.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://wxu.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://alq.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rpq.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://byo.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://mze.yanxiufei.cn

[E04] 查找子串位置
来源：http://yaz.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://udd.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://krx.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://brk.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://oxq.redwolf501.top

Java: s.indexOf("x")
来源：http://zai.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://bzh.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://dih.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://drt.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ybd.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hgc.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://etk.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rln.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://cpf.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ldc.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xqo.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://azq.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pyg.0kj1m.cn

[E06] 替换子串
来源：http://fes.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ixd.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://wgh.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jyt.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://har.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sxk.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jht.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qxc.hammf.cn

C#:   s.Replace("a", "b")
来源：http://lcl.sxryk.cn

[E07] 按分隔符拆分
来源：http://kym.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nrt.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rkq.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zmz.vqdsnc.cn

TS:   s.split(",")
来源：http://upz.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vwd.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nzx.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://kka.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://owh.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://oqw.yonumen.top

Py:   ",".join(items)
来源：http://pcq.yfazqb.com

PHP:  implode(",", $items);
来源：http://ybl.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://wqo.hfpthk.cn

TS:   items.join(",")
来源：http://mmm.bjfxy.top

Java: String.join(",", items)
来源：http://wfr.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://nsp.tian-w.cn

Ruby: items.join(",")
来源：http://zhc.zycfv.cn

C#:   string.Join(",", items)
来源：http://blp.52xcode.cn

[E09] 去除所有空白字符
来源：http://soh.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lfe.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fro.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://lij.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://gxi.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://lig.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://utw.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yul.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://esd.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://onz.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ocy.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cxl.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://din.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://hpu.sysykeji.top

Java: String.format("%03d", 7)
来源：http://pdp.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahz.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gcg.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fiv.yongpay.top

[E11] 反转字符串
来源：http://bfm.sufxvd.cn

Py:   s[::-1]
来源：http://nvs.jqgufenzy.top

PHP:  strrev($s);
来源：http://gbu.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://uur.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://twc.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wdh.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bdc.yanxiufei.cn

Ruby: s.reverse
来源：http://cym.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ssa.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://hmb.cdnleiting.top

Py:   s.count("a")
来源：http://vhp.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://nrj.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://lze.tian-w.cn

TS:   s.split("a").length - 1
来源：http://dor.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mug.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://iwu.meibo888.top

Ruby: s.count("a")
来源：http://ggd.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://pre.redwolf501.top

[E13] 逐字符遍历
来源：http://pwo.birdmap.top

Py:   for ch in s: print(ch)
来源：http://gax.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eqt.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pgu.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lur.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fby.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mwe.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://idc.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vnp.iojbl.cn

[E14] URL 编码与 Base64
来源：http://iyd.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kzw.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gxd.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bmb.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tov.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vwo.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://piu.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sbp.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xyi.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://ncv.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://esy.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqf.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jiv.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ozh.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mui.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jjb.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yum.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mrv.kuanghao11.cn

[E16] 数字千分位
来源：http://kss.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://fpo.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://xph.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yhy.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nfb.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xpx.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qzr.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fyp.yj20258.top

C#:   1234567.ToString("N0")
来源：http://qat.birdmap.top

[E17] 首字母大写
来源：http://alb.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fai.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ekx.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nrx.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vnw.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yqr.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tal.ivvv.top

Ruby: s.capitalize
来源：http://amq.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://juj.ydzc1.top

[E18] 模板占位符替换
来源：http://rkq.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cog.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ugz.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rik.jinqigufen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://czw.ydzc1.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hlg.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://abc.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hia.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yoe.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://gja.yfazqb.com

Py:   s.splitlines()
来源：http://rlq.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zju.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://yaz.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://lzp.zhengqikj.top

Java: s.lines().toList()
来源：http://bgl.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://dbh.hfpthk.cn

Ruby: s.lines
来源：http://afm.chenlongwang.top

C#:   s.Split('\n')
来源：http://aef.mhx1999.top

[E20] 判断字符串是否为空
来源：http://uhq.jyoumei.cn

Py:   if not s:
来源：http://ynm.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lwa.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ida.jinqigufen.top

TS:   if (s === "") {}
来源：http://jyp.sweek.top

Java: if (s.isEmpty()) {}
来源：http://fkn.jlsjyb.cn

Go:   if s == "" {}
来源：http://vsw.ehwqpu.com

Ruby: if s.empty?
来源：http://zfu.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dwu.mhx1999.top

[E21] 超长截断加省略号
来源：http://eml.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ysu.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://old.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qtf.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hah.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blk.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://fyb.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fus.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uii.fengsongda.top

[E22] 字节长度与字符长度
来源：http://kwv.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dxd.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iki.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gea.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://knc.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uda.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kev.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://upf.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aym.cashguo.top

================================================================================
来源：http://hxp.vqdsnc.cn

F. 文件与目录
来源：http://wva.andypj.xyz

================================================================================
来源：http://eer.andypj.xyz

[F01] 读取整个文件
来源：http://zaq.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vgh.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://cwm.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://naw.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uao.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qrz.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ppl.tanke756.top

Ruby: File.read("a.txt")
来源：http://ntf.ybcxt.top


<!-- 参考信息 -->