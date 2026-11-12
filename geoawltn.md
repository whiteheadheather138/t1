代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ptx.316326.xyz

Go:   // 手写双层循环
来源：http://rbf.tianlin.xyz

Ruby: nested.flatten
来源：http://nfe.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tlp.feifeiyinyue.top

[D19] 按字段分组
来源：http://uhr.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bee.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wda.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://drt.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://edn.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gtx.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://ldc.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://swb.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lug.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://xsy.yueranfly.top

Py:   Counter(arr)
来源：http://qxm.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://yyj.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dpb.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abd.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dnc.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://qnb.yuanzhike.top

Ruby: arr.tally
来源：http://uaj.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oej.xziqi.cn

[D21] 判断是否包含某元素
来源：http://edj.hywenlv.cn

Py:   x in arr
来源：http://qyj.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://tod.0kj1m.cn

JS:   arr.includes(x)
来源：http://pfc.fzhhl.top

TS:   arr.includes(x)
来源：http://xvw.wangshuangyany.cn

Java: list.contains(x)
来源：http://dnb.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://udz.aibaodan.cn

Ruby: arr.include?(x)
来源：http://fww.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://hyu.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://cge.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vps.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eji.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oqb.jianghu66.top

TS:   [...arr];
来源：http://rar.jianghu66.top

Java: new ArrayList<>(list);
来源：http://ftm.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://htp.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://smn.chenlongwang.top

C#:   new List<int>(list);
来源：http://fpq.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://tzy.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zvt.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eaz.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyh.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mtc.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sua.mhx1999.top

Go:   // 手写循环
来源：http://glc.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rvg.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cxm.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://gsd.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qqd.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ooh.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tqv.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bim.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tbd.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wft.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mri.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ath.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://qmf.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://saq.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tyn.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wkg.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yri.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mub.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fmv.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://net.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lui.sufxvd.cn

[D26] 数组转字符串
来源：http://otz.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://ngc.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://kqw.fengsongda.top

JS:   arr.join(", ")
来源：http://fkl.gogol.net.cn

TS:   arr.join(", ")
来源：http://now.iojbl.cn

Java: String.join(", ", list)
来源：http://oeh.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://mmz.yonumen.top

Ruby: arr.join(", ")
来源：http://dhc.mhx1999.top

C#:   string.Join(", ", list)
来源：http://iue.havefunace.top

================================================================================
来源：http://ktr.yueranfly.top

E. 字符串处理
来源：http://lsu.cdnleiting.top

================================================================================
来源：http://coz.cucudq.cn

[E01] 拼接字符串
来源：http://ffj.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qot.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zcm.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wcg.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://age.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mga.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gvf.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zsy.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nrp.yvedp.cn

[E02] 重复字符串
来源：http://ghp.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://olt.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://bvd.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://drd.daria6918.cn

TS:   "ab".repeat(3)
来源：http://umj.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://pli.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://mhh.vehdjk.com

Ruby: "ab" * 3
来源：http://nhg.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://enz.zhoulong.xyz

[E03] 截取子串
来源：http://rdj.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqy.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wln.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gzd.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://qmq.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://apv.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ste.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://dsu.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://whn.haohaochexian.top

[E04] 查找子串位置
来源：http://dgh.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://bfo.yvedp.cn

PHP:  strpos($s, "x");
来源：http://zbj.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sqd.fzhhl.top

TS:   s.indexOf("x")
来源：http://muf.zdbjq.cn

Java: s.indexOf("x")
来源：http://psm.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://ays.daxiang520.top

Ruby: s.index("x")
来源：http://ukz.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://ymz.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://dkw.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rjg.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://klv.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gdv.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dtf.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://usb.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fay.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qie.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zwg.sufxvd.cn

[E06] 替换子串
来源：http://cxo.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hrf.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://jkc.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujo.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://pak.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tka.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wpp.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://omm.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://rlr.meibo888.top

[E07] 按分隔符拆分
来源：http://dwy.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uza.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bhk.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://svc.cashguo.top

TS:   s.split(",")
来源：http://gto.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://zxp.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ish.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://ens.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yyc.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://vkm.kuanghao11.cn

Py:   ",".join(items)
来源：http://dzj.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://mpr.havefunace.top

JS:   items.join(",")
来源：http://dyj.yueranfly.top

TS:   items.join(",")
来源：http://gwc.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://rdp.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://wox.zhengqikj.top

Ruby: items.join(",")
来源：http://due.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://jru.jinqigufen.top

[E09] 去除所有空白字符
来源：http://jec.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wbh.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zel.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://jhp.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://ahv.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://ghn.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mcg.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://srg.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gzn.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://uyw.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jqz.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vkj.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://sfj.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://rbq.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://ebr.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://sff.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jmd.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://neo.ydzc1.top

[E11] 反转字符串
来源：http://yhu.hnxiangtu.top

Py:   s[::-1]
来源：http://akd.pycfn.com

PHP:  strrev($s);
来源：http://yvn.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://vay.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://yov.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hwc.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://awa.gaohongyu789.top

Ruby: s.reverse
来源：http://ami.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://rej.cucudq.cn

[E12] 统计某字符出现次数
来源：http://nmy.sxryk.cn

Py:   s.count("a")
来源：http://tzn.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://mot.cashguo.top

JS:   s.split("a").length - 1
来源：http://nen.aizwys.cn

TS:   s.split("a").length - 1
来源：http://ttn.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uoh.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://diw.pycfn.com

Ruby: s.count("a")
来源：http://qcl.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://jri.yuanzhike.top

[E13] 逐字符遍历
来源：http://cts.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://whb.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://upy.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jbf.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rxg.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vhr.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ctr.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dhj.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jxx.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://ray.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zfw.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kkv.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fru.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://udf.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://acg.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ppz.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://img.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vzu.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://yjx.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xim.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wyc.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iog.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dzd.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://beu.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vhg.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wlr.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qvf.dianchejie.cn

[E16] 数字千分位
来源：http://eoh.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://nln.nanxinkj.top

PHP:  number_format(1234567);
来源：http://uzs.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ump.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cml.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cae.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lfv.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fgz.yongpay.top

C#:   1234567.ToString("N0")
来源：http://gih.chenlongwang.top

[E17] 首字母大写
来源：http://vbv.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dsz.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://rez.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jcy.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykq.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xev.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cpc.ydjk.org.cn

Ruby: s.capitalize
来源：http://bwe.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nxt.yueranfly.top

[E18] 模板占位符替换
来源：http://swb.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://esv.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://odq.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wzj.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://whc.jinqigfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://trx.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://orr.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zin.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://afi.yj20258888.top

[E19] 多行文本按行拆分
来源：http://qwk.hnqzz.top

Py:   s.splitlines()
来源：http://yyk.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nix.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://ycz.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://pyd.tianlin.xyz

Java: s.lines().toList()
来源：http://tfc.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://hpy.sufxvd.cn

Ruby: s.lines
来源：http://xfs.0kj1m.cn

C#:   s.Split('\n')
来源：http://fni.bbcook.cn

[E20] 判断字符串是否为空
来源：http://uyb.quarkkingdee.top

Py:   if not s:
来源：http://xsh.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lkv.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://swm.fengsongda.top

TS:   if (s === "") {}
来源：http://kmz.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://vgq.hcnkem.com

Go:   if s == "" {}
来源：http://tfb.svipenyu.cn

Ruby: if s.empty?
来源：http://ykm.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sct.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://vtz.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mer.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qfm.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gck.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzn.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pns.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://nbr.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bfn.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nlr.yj202588.top

[E22] 字节长度与字符长度
来源：http://kjg.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dqe.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://odb.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jvu.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dri.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ghn.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdj.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://xju.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ehs.chenjidiqi.icu

================================================================================
来源：http://tru.sweek.top

F. 文件与目录
来源：http://nqa.vehdjk.com

================================================================================
来源：http://mxg.redwolf501.top

[F01] 读取整个文件
来源：http://cbm.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xpl.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://qhx.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mwn.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nuk.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mqa.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vhm.xinyue.icu

Ruby: File.read("a.txt")
来源：http://via.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://doz.shzxlz.cn

[F02] 逐行读取文件
来源：http://gnb.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fqo.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://agq.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yol.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cgi.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ewn.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vcp.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rgs.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zzf.meibo888.top

[F03] 写入文件（覆盖）
来源：http://oij.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://znk.0kj1m.cn


<!-- 参考信息 -->