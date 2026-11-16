代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://xtq.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qwf.jqgfzy.top

TS:   Math.max(...arr);
来源：http://xlv.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lbu.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnn.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://foy.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://fhm.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://kcs.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fgb.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://jmx.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vbo.uphjek.com

TS:   nested.flat();
来源：http://ezt.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xbq.fzhhl.top

Go:   // 手写双层循环
来源：http://blu.jiagoushi.top

Ruby: nested.flatten
来源：http://pjg.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tvi.haohaochexian.top

[D19] 按字段分组
来源：http://emm.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xcj.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ift.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cio.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xij.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bdy.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://nsg.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ubj.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wek.tanke756.top

[D20] 统计每个元素出现次数
来源：http://wto.shangyingyoupin.top

Py:   Counter(arr)
来源：http://bit.hnqzz.top

PHP:  array_count_values($arr);
来源：http://spx.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zjx.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zpt.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arb.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://kxz.fanxiaobao.xyz

Ruby: arr.tally
来源：http://svy.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kxc.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://dfc.ydjk.org.cn

Py:   x in arr
来源：http://hcv.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://yap.cashguo.top

JS:   arr.includes(x)
来源：http://cya.tian-w.cn

TS:   arr.includes(x)
来源：http://pfb.shzxlz.cn

Java: list.contains(x)
来源：http://bnx.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://fga.52xcode.cn

Ruby: arr.include?(x)
来源：http://zrf.fehbvm.com

C#:   list.Contains(x)
来源：http://fii.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://ala.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://smb.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://glq.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lye.yj20258.top

TS:   [...arr];
来源：http://jys.tanke756.top

Java: new ArrayList<>(list);
来源：http://fud.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://jgy.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://ivy.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://vsv.kuanghao11.cn

[D23] reduce 累积计算
来源：http://owl.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mky.xylfe.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ncu.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zqb.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axu.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://syp.iojbl.cn

Go:   // 手写循环
来源：http://kie.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pot.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mtd.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://pyu.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jow.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zpa.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://txo.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vbp.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jtc.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sls.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mkm.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mzw.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://kzf.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qof.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rwz.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aus.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qfg.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://viz.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gql.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uoa.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wgk.shangyingyoupin.top

[D26] 数组转字符串
来源：http://znz.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://mya.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://wfn.hfpthk.cn

JS:   arr.join(", ")
来源：http://oiw.52xcode.cn

TS:   arr.join(", ")
来源：http://rig.hnxiangtu.top

Java: String.join(", ", list)
来源：http://ldf.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://gch.fktsv.cn

Ruby: arr.join(", ")
来源：http://rkb.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://uuq.xuetiantiany.cn

================================================================================
来源：http://fze.bbcook.cn

E. 字符串处理
来源：http://fov.andypj.xyz

================================================================================
来源：http://hgq.dashuyun.cn

[E01] 拼接字符串
来源：http://imw.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gth.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axe.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jte.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqj.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ifm.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cgk.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://izy.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jus.kuanghao11.cn

[E02] 重复字符串
来源：http://lyc.tanke756.top

Py:   "ab" * 3
来源：http://ocj.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://oxt.52xcode.cn

JS:   "ab".repeat(3)
来源：http://bfm.wangdashe.top

TS:   "ab".repeat(3)
来源：http://rio.yfazqb.com

Java: "ab".repeat(3)
来源：http://bmq.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://jxl.hfpthk.cn

Ruby: "ab" * 3
来源：http://skg.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dui.meibo888.top

[E03] 截取子串
来源：http://orp.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vkg.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sbz.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jaj.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://rll.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://vmi.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tnt.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://kgo.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://zse.cdnleiting.top

[E04] 查找子串位置
来源：http://try.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://swf.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://ggf.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wfk.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://lhy.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://yvz.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://ufy.0kj1m.cn

Ruby: s.index("x")
来源：http://bwr.xziqi.cn

C#:   s.IndexOf("x")
来源：http://zxb.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hrq.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://emz.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wnn.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfj.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mev.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ljq.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nde.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qpp.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lye.cashguo.top

[E06] 替换子串
来源：http://ivn.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dag.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://gav.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://apy.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://ust.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ofs.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yxn.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://quc.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://rwa.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://otu.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kyb.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nit.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://paw.quarkkingdee.top

TS:   s.split(",")
来源：http://xzo.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cww.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ghz.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://kex.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zal.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://xak.hongshengwenyu.top

Py:   ",".join(items)
来源：http://dci.ydzc1.top

PHP:  implode(",", $items);
来源：http://icc.xinyue.icu

JS:   items.join(",")
来源：http://lpi.ctjpmb.com

TS:   items.join(",")
来源：http://qpw.gogol.net.cn

Java: String.join(",", items)
来源：http://ayg.cheryme.top

Go:   strings.Join(items, ",")
来源：http://amp.yongpay.top

Ruby: items.join(",")
来源：http://ukb.yongpay.top

C#:   string.Join(",", items)
来源：http://coh.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://dtp.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qoe.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xrt.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://gnn.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://ivw.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://tkw.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://gcd.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://vjq.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://imx.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://pjj.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mns.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ete.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://yyh.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://wug.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://uaq.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://byl.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cjq.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://obt.hammf.cn

[E11] 反转字符串
来源：http://ayi.sweek.top

Py:   s[::-1]
来源：http://jnh.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://jin.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://yfq.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://tjb.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://tri.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gjt.tianlin.xyz

Ruby: s.reverse
来源：http://bxk.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://lyc.bjfxy.top

[E12] 统计某字符出现次数
来源：http://yvw.yangfankeji.com

Py:   s.count("a")
来源：http://out.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://ipe.guannengcc.top

JS:   s.split("a").length - 1
来源：http://zpj.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://wph.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wez.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://sjr.yfazqb.com

Ruby: s.count("a")
来源：http://aer.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://njj.0kj1m.cn

[E13] 逐字符遍历
来源：http://dgt.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://ysa.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://deb.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://btj.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fto.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lio.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sct.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pow.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://occ.vehdjk.com

[E14] URL 编码与 Base64
来源：http://zir.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhm.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iog.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://geh.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gqw.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zoq.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mht.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lhu.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rdq.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://pyk.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://phc.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dtj.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dvh.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yon.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mop.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xyx.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ixc.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cls.ydjk.org.cn

[E16] 数字千分位
来源：http://qxt.xylfe.cn

Py:   f"{1234567:,}"
来源：http://ydd.yueranfly.top

PHP:  number_format(1234567);
来源：http://pif.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qhc.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aid.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oyq.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://efq.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iqf.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://azh.jqgfzy.top

[E17] 首字母大写
来源：http://lej.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uqm.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wmb.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkn.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbf.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qai.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://una.ehwqpu.com

Ruby: s.capitalize
来源：http://mmq.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sny.gotoacloud.top

[E18] 模板占位符替换
来源：http://gzy.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ruk.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://utw.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://crk.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://xnw.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jod.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zmr.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mgs.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://abs.tian-w.cn

[E19] 多行文本按行拆分
来源：http://gby.quarkkingdee.top

Py:   s.splitlines()
来源：http://ast.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sxj.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://wrj.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://cqf.uphjek.com

Java: s.lines().toList()
来源：http://ujb.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://fze.yanxiufei.cn

Ruby: s.lines
来源：http://pvy.hywenlv.cn

C#:   s.Split('\n')
来源：http://hxm.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://exz.shzxlz.cn

Py:   if not s:
来源：http://gvt.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tsc.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sup.316326.xyz

TS:   if (s === "") {}
来源：http://oka.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://ddy.mhx1999.top

Go:   if s == "" {}
来源：http://lir.fktsv.cn

Ruby: if s.empty?
来源：http://ykw.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cxu.tianlin.xyz

[E21] 超长截断加省略号
来源：http://fgi.yj20258888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://amz.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vqq.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://loa.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dso.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wll.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://rex.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rmh.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xir.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://vas.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vjv.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://upv.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jtn.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fwa.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hws.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ibw.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://ebc.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uhv.sjlbkw.cn

================================================================================
来源：http://zcu.nwbrower.top

F. 文件与目录
来源：http://wwg.bjfxy.top

================================================================================
来源：http://qyy.pengpengdd.cyou

[F01] 读取整个文件
来源：http://xoz.bjfxy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mte.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://hdt.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xrh.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kpv.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vis.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tak.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://til.yj202588.top


<!-- 参考信息 -->