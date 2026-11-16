代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aqi.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://dke.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lxr.bbcook.cn

TS:   nested.flat();
来源：http://dyk.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gru.0kj1m.cn

Go:   // 手写双层循环
来源：http://ktk.52xcode.cn

Ruby: nested.flatten
来源：http://kun.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://pdg.gaohongyu789.top

[D19] 按字段分组
来源：http://qrn.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fcx.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://slr.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dps.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zqy.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://svq.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://pwf.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dxt.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uxf.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://gcu.yj20258.top

Py:   Counter(arr)
来源：http://kna.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://mlg.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dfz.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://odw.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ldk.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://nsw.dianchejie.cn

Ruby: arr.tally
来源：http://btq.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ytz.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://xac.cdnleiting.top

Py:   x in arr
来源：http://szt.fzhhl.top

PHP:  in_array($x, $arr, true);
来源：http://etx.dianchejie.cn

JS:   arr.includes(x)
来源：http://ccn.gaohongyu789.top

TS:   arr.includes(x)
来源：http://zhb.quarkkingdee.top

Java: list.contains(x)
来源：http://ctf.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://lbe.jqgfzy.top

Ruby: arr.include?(x)
来源：http://ola.aizwys.cn

C#:   list.Contains(x)
来源：http://zsf.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://kss.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://elm.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mrd.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nul.cdnleiting.top

TS:   [...arr];
来源：http://lnp.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://xwc.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://thj.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://zvv.vehdjk.com

C#:   new List<int>(list);
来源：http://fid.yuanzhike.top

[D23] reduce 累积计算
来源：http://frb.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gji.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hvv.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lci.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tgx.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tzd.yvedp.cn

Go:   // 手写循环
来源：http://tpo.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iyz.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://plc.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://hvp.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sdd.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ygj.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nxy.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qnu.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qdi.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://apg.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lcy.ybcxt.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qti.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://ctm.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://scj.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sbi.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eig.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://adb.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tqv.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dok.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ucx.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hmc.ppjwa.cn

[D26] 数组转字符串
来源：http://hej.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://izl.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://yct.pycfn.com

JS:   arr.join(", ")
来源：http://fwf.smart0.xyz

TS:   arr.join(", ")
来源：http://pxa.hcnkem.com

Java: String.join(", ", list)
来源：http://ohh.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://bme.vehdjk.com

Ruby: arr.join(", ")
来源：http://ewp.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://uaf.yuxming.cn

================================================================================
来源：http://rfc.yj20258888.top

E. 字符串处理
来源：http://eqv.nanxinkj.top

================================================================================
来源：http://bxo.sxryk.cn

[E01] 拼接字符串
来源：http://jhh.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kbp.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qbe.0kj1m.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cyj.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://taq.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ryy.shangyingyoupin.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://msv.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gtz.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dfe.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://eqk.gotoacloud.top

Py:   "ab" * 3
来源：http://ibm.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://kvg.tanke756.top

JS:   "ab".repeat(3)
来源：http://ouz.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://kyb.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://log.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://qku.zdqjudy.top

Ruby: "ab" * 3
来源：http://ads.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zxb.snrcjt.cn

[E03] 截取子串
来源：http://rdx.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mio.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kbl.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xri.yj202588.top

TS:   s.slice(1, 4)
来源：http://mrz.fengsongda.top

Java: s.substring(1, 4)
来源：http://ciy.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sbq.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://okh.yj202588.top

C#:   s.Substring(1, 3)
来源：http://pvr.gzhubu.top

[E04] 查找子串位置
来源：http://lib.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://shb.bjfxy.top

PHP:  strpos($s, "x");
来源：http://nyc.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zzp.yj202588.top

TS:   s.indexOf("x")
来源：http://ifl.vqdsnc.cn

Java: s.indexOf("x")
来源：http://rou.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://obo.yueranfly.top

Ruby: s.index("x")
来源：http://yoy.fzhhl.top

C#:   s.IndexOf("x")
来源：http://ylm.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ykr.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvl.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wvb.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzo.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hya.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fyr.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://beg.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sry.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lcd.jinqigufen.top

[E06] 替换子串
来源：http://ubt.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vtv.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://hra.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysv.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://jhg.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mwk.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ywm.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bmm.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://gie.jyoumei.cn

[E07] 按分隔符拆分
来源：http://vdm.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://onz.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://shl.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://ujp.gogol.net.cn

TS:   s.split(",")
来源：http://puo.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://rsm.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://toy.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://gks.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://byz.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://tso.fengsongda.top

Py:   ",".join(items)
来源：http://jcs.meibo888.top

PHP:  implode(",", $items);
来源：http://rdp.tarul.cn

JS:   items.join(",")
来源：http://omf.fanxiaobao.xyz

TS:   items.join(",")
来源：http://juz.ybcxt.top

Java: String.join(",", items)
来源：http://wra.cheryme.top

Go:   strings.Join(items, ",")
来源：http://zmt.xziqi.cn

Ruby: items.join(",")
来源：http://svp.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://fdy.chenzaomai.com

[E09] 去除所有空白字符
来源：http://fdq.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://asx.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hbh.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ppn.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://nqg.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://iwh.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cdf.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://noo.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://anq.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://jwq.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ezd.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lwv.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://yrr.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://ape.guannengcc.top

Java: String.format("%03d", 7)
来源：http://rsk.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bds.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ace.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://adi.xziqi.cn

[E11] 反转字符串
来源：http://pxd.feifeiyinyue.top

Py:   s[::-1]
来源：http://bpn.hywenlv.cn

PHP:  strrev($s);
来源：http://jri.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://afb.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://ifd.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://woj.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xhu.bbcook.cn

Ruby: s.reverse
来源：http://yka.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://ewm.bbcook.cn

[E12] 统计某字符出现次数
来源：http://jhm.xylfe.cn

Py:   s.count("a")
来源：http://hnh.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://jgu.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://mas.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://wru.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://slg.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://yfy.iojbl.cn

Ruby: s.count("a")
来源：http://uyb.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://oly.daxiang520.top

[E13] 逐字符遍历
来源：http://kjg.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://rbx.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qnc.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hsm.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hsd.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vnc.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gqd.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zuq.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dov.iojbl.cn

[E14] URL 编码与 Base64
来源：http://kzq.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kmk.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qfo.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kph.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iqw.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jzq.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uol.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tai.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ahx.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://nzi.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wrj.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qby.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pxn.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ege.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lrr.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xha.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ypq.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sql.hfpthk.cn

[E16] 数字千分位
来源：http://ihx.xinyue.icu

Py:   f"{1234567:,}"
来源：http://ljv.xziqi.cn

PHP:  number_format(1234567);
来源：http://dsg.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://czf.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mzc.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jox.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ioo.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vfp.316326.xyz

C#:   1234567.ToString("N0")
来源：http://ylh.chenjidiqi.icu

[E17] 首字母大写
来源：http://aah.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gtg.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://uem.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hvf.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aeo.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sih.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://acs.zhongyouzk.top

Ruby: s.capitalize
来源：http://xep.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eoj.daxiang520.top

[E18] 模板占位符替换
来源：http://bfy.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tqh.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://omh.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cqw.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://zek.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qap.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yoq.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qov.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zir.gzhubu.top

[E19] 多行文本按行拆分
来源：http://yod.yanxiufei.cn

Py:   s.splitlines()
来源：http://acj.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eth.sweek.top

JS:   s.split(/\r?\n/)
来源：http://vri.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://pbd.zhiwuduotai.top

Java: s.lines().toList()
来源：http://oza.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://fnx.guowangkeji.top

Ruby: s.lines
来源：http://ike.ppjwa.cn

C#:   s.Split('\n')
来源：http://yws.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://sod.jqgfzy.top

Py:   if not s:
来源：http://vik.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cxk.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://elj.bjfxy.top

TS:   if (s === "") {}
来源：http://mhf.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://vvi.redwolf501.top

Go:   if s == "" {}
来源：http://lnv.zhijiandao.cn

Ruby: if s.empty?
来源：http://rxd.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yzx.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://wpd.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gub.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uwn.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://npz.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hvg.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lzh.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://scj.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://htz.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ogh.316326.xyz

[E22] 字节长度与字符长度
来源：http://jth.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qpz.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fmd.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wfj.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pei.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hnx.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mbs.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://ckq.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tvz.xziqi.cn

================================================================================
来源：http://pyr.jlsjyb.cn

F. 文件与目录
来源：http://rmh.pengpengdd.cyou

================================================================================
来源：http://kfi.zhiwuduotai.top

[F01] 读取整个文件
来源：http://kbh.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vng.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://ljx.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fso.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zcx.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ruo.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vcb.sxryk.cn

Ruby: File.read("a.txt")
来源：http://lxd.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://jhc.cucudq.cn

[F02] 逐行读取文件
来源：http://ale.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ibz.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mor.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://arr.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mub.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jva.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pff.ivvv.top


<!-- 参考信息 -->