代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xgc.pycfn.com

PHP:  array_merge(...$nested);
来源：http://cxg.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qib.feifeiyinyue.top

TS:   nested.flat();
来源：http://pky.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://icd.sysykeji.top

Go:   // 手写双层循环
来源：http://dwr.zhiwuduotai.top

Ruby: nested.flatten
来源：http://tkr.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sbi.zhiwuduotai.top

[D19] 按字段分组
来源：http://vgx.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sit.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jdx.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yly.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eiu.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kgg.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://zsz.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://urb.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aft.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://zmp.yuanzhike.top

Py:   Counter(arr)
来源：http://nkz.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://tpm.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vbs.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cmq.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fdm.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://pis.yvedp.cn

Ruby: arr.tally
来源：http://app.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ery.havefunace.top

[D21] 判断是否包含某元素
来源：http://lgo.0kj1m.cn

Py:   x in arr
来源：http://lmi.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://wju.hywenlv.cn

JS:   arr.includes(x)
来源：http://nyv.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://ljf.shzxlz.cn

Java: list.contains(x)
来源：http://cyp.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://mkx.sufxvd.cn

Ruby: arr.include?(x)
来源：http://ena.vqdsnc.cn

C#:   list.Contains(x)
来源：http://wnh.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://iob.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://olf.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zbh.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tre.guannengcc.top

TS:   [...arr];
来源：http://pbz.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://nky.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://bcn.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://qtd.ydzc1.top

C#:   new List<int>(list);
来源：http://iyn.snrcjt.cn

[D23] reduce 累积计算
来源：http://chi.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cra.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uit.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rzl.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lbh.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gzm.yonumen.top

Go:   // 手写循环
来源：http://xsj.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dpm.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tip.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://jkw.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pyl.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wpb.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gey.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qeq.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rfm.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wrs.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zeu.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ayx.pycfn.com

[D25] Set 集合去重与交并差
来源：http://ery.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xsd.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jcf.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ogx.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bxt.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yqp.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yvx.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hvp.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://atb.wangdashe.top

[D26] 数组转字符串
来源：http://tlz.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://fig.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://qhb.sxryk.cn

JS:   arr.join(", ")
来源：http://hfx.nwbrower.top

TS:   arr.join(", ")
来源：http://cmf.vehdjk.com

Java: String.join(", ", list)
来源：http://rac.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://qcz.andypj.xyz

Ruby: arr.join(", ")
来源：http://ogv.pycfn.com

C#:   string.Join(", ", list)
来源：http://zyi.haohaochexian.top

================================================================================
来源：http://eok.zhiwuduotai.top

E. 字符串处理
来源：http://wcv.smart0.xyz

================================================================================
来源：http://nal.9152youxi.cn

[E01] 拼接字符串
来源：http://aqk.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ixz.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uov.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ytq.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://toh.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uwx.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xea.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hva.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zjd.cucudq.cn

[E02] 重复字符串
来源：http://ffh.zhijiandao.cn

Py:   "ab" * 3
来源：http://tmy.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://bsq.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://rlv.cashguo.top

TS:   "ab".repeat(3)
来源：http://ygu.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://ird.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://cjp.fehbvm.com

Ruby: "ab" * 3
来源：http://uew.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zrd.sweek.top

[E03] 截取子串
来源：http://ahy.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ihz.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oqb.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nyo.sysykeji.top

TS:   s.slice(1, 4)
来源：http://rro.cdnleiting.top

Java: s.substring(1, 4)
来源：http://xbh.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lpj.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ykd.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://mqc.birdmap.top

[E04] 查找子串位置
来源：http://phh.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://vsr.yj202588.top

PHP:  strpos($s, "x");
来源：http://wcs.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xba.tianlin.xyz

TS:   s.indexOf("x")
来源：http://aqw.zycfv.cn

Java: s.indexOf("x")
来源：http://kny.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://qst.ivvv.top

Ruby: s.index("x")
来源：http://niy.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://apk.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kbn.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://knv.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xes.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mpd.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jqr.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cxs.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uac.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dwj.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hol.kuanghao11.cn

[E06] 替换子串
来源：http://ofb.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kcd.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://mpl.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ogi.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://qux.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xms.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tid.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://thp.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://xpw.guannengcc.top

[E07] 按分隔符拆分
来源：http://dbu.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jfy.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xfw.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://izw.bbcook.cn

TS:   s.split(",")
来源：http://ohq.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://xwz.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fem.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://oul.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ejm.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://lzh.daxiang520.top

Py:   ",".join(items)
来源：http://gda.fktsv.cn

PHP:  implode(",", $items);
来源：http://mni.sxryk.cn

JS:   items.join(",")
来源：http://fth.hongshengwenyu.top

TS:   items.join(",")
来源：http://ome.quarkkingdee.top

Java: String.join(",", items)
来源：http://tbc.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://kql.hammf.cn

Ruby: items.join(",")
来源：http://yws.sysykeji.top

C#:   string.Join(",", items)
来源：http://hzg.iojbl.cn

[E09] 去除所有空白字符
来源：http://kng.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mze.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fnu.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://zmx.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://lii.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://qro.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://dde.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://glk.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vza.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://bye.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gbs.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://faq.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://utl.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://hlz.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://onf.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ndf.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jmb.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fif.ppjwa.cn

[E11] 反转字符串
来源：http://ayi.bbcook.cn

Py:   s[::-1]
来源：http://biv.fzhhl.top

PHP:  strrev($s);
来源：http://ygg.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://gkt.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://waz.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ljt.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://noo.tarul.cn

Ruby: s.reverse
来源：http://htn.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://xsi.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://kzg.jinqigfzy.top

Py:   s.count("a")
来源：http://act.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://ugr.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://mks.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://rsq.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lvo.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://trx.hesvh.cn

Ruby: s.count("a")
来源：http://kkt.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://agj.bbcook.cn

[E13] 逐字符遍历
来源：http://qtd.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://gty.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uzn.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lzi.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://frp.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://evu.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fmb.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ldi.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yrl.daria6918.cn

[E14] URL 编码与 Base64
来源：http://yqn.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pyn.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zbd.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xvp.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bxv.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gcj.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yda.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rmp.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://phm.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://veb.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wdl.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qbh.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://isv.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://txu.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://smi.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gns.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sjm.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mwn.aibaodan.cn

[E16] 数字千分位
来源：http://ard.cashguo.top

Py:   f"{1234567:,}"
来源：http://fvd.fengsongda.top

PHP:  number_format(1234567);
来源：http://zbo.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ogu.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tap.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kgg.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tyq.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://huu.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://kgq.gogol.net.cn

[E17] 首字母大写
来源：http://mrz.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fet.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dwa.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mkz.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gtb.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kpt.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tez.nwbrower.top

Ruby: s.capitalize
来源：http://its.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ujz.sufxvd.cn

[E18] 模板占位符替换
来源：http://yas.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://stf.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cmt.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hfi.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://faj.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uvi.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qzf.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pvd.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rdw.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://lyf.cucudq.cn

Py:   s.splitlines()
来源：http://eea.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kug.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://ppd.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://wwa.wangdashe.top

Java: s.lines().toList()
来源：http://ynk.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://szr.kuanghao11.cn

Ruby: s.lines
来源：http://pbb.cheryme.top

C#:   s.Split('\n')
来源：http://ucs.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://aib.gaohongyu789.top

Py:   if not s:
来源：http://roc.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wxl.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qkj.yvedp.cn

TS:   if (s === "") {}
来源：http://ujh.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://plk.hammf.cn

Go:   if s == "" {}
来源：http://ljj.kuanghao11.cn

Ruby: if s.empty?
来源：http://ldv.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kqg.52xcode.cn

[E21] 超长截断加省略号
来源：http://fdo.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iix.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bdo.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://irb.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kbj.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://awn.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://vyl.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xig.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tmw.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://pnt.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uax.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qga.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sej.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://flk.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ajv.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://klo.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://gzn.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://icz.gzhubu.top

================================================================================
来源：http://ups.jinghuilouyu.cn

F. 文件与目录
来源：http://ofz.aizwys.cn

================================================================================
来源：http://rvn.aibaodan.cn

[F01] 读取整个文件
来源：http://tdt.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rix.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://vbp.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jaw.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hdi.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hqq.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ljr.xinyue.icu

Ruby: File.read("a.txt")
来源：http://ajy.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://rgb.cqqwz.cn

[F02] 逐行读取文件
来源：http://uhc.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kck.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fap.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://euc.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jhb.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lon.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xgf.zdbjq.cn


<!-- 参考信息 -->