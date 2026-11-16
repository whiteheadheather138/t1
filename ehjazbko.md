代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gxc.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://vsz.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://gmm.hammf.cn

[D18] 扁平化嵌套数组
来源：http://xou.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bbd.meibo888.top

PHP:  array_merge(...$nested);
来源：http://mwz.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hbg.zdqjudy.top

TS:   nested.flat();
来源：http://jpp.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ymh.cucudq.cn

Go:   // 手写双层循环
来源：http://ybl.ydjk.org.cn

Ruby: nested.flatten
来源：http://wxg.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bjj.hammf.cn

[D19] 按字段分组
来源：http://kuj.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ntf.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pcx.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iin.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://veb.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fsx.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://pbs.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ldh.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lus.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://syq.havefunace.top

Py:   Counter(arr)
来源：http://sax.iojbl.cn

PHP:  array_count_values($arr);
来源：http://csm.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ydt.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbk.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kmu.yonumen.top

Go:   // 手写 map[T]int
来源：http://hcd.jianghu66.top

Ruby: arr.tally
来源：http://nlp.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wai.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://ael.haohaochexian.top

Py:   x in arr
来源：http://gqm.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://vnu.nanxuanxn.top

JS:   arr.includes(x)
来源：http://vfn.gotoacloud.top

TS:   arr.includes(x)
来源：http://tlg.hnxiangtu.top

Java: list.contains(x)
来源：http://mep.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://vmm.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://lee.shuidangran.top

C#:   list.Contains(x)
来源：http://pdl.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://baf.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kij.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qlz.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ljn.shangyingyoupin.top

TS:   [...arr];
来源：http://dne.iojbl.cn

Java: new ArrayList<>(list);
来源：http://yyo.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://isf.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://eso.meibo888.top

C#:   new List<int>(list);
来源：http://ztv.yuanzhike.top

[D23] reduce 累积计算
来源：http://uhx.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mei.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://egb.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mti.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ayw.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dnc.hesvh.cn

Go:   // 手写循环
来源：http://snk.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pqm.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xwv.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://gwz.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yyo.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mvf.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gkq.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yar.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vqx.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yqj.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pfg.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hrn.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://nqt.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zxq.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wzo.yvedp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://riu.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ahd.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mvj.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wfp.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tfc.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://atb.yj202588.top

[D26] 数组转字符串
来源：http://uxc.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://qid.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://hav.hysaishi.cn

JS:   arr.join(", ")
来源：http://jrm.vehdjk.com

TS:   arr.join(", ")
来源：http://bee.nanxuanxn.top

Java: String.join(", ", list)
来源：http://axy.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://nlu.zdqjudy.top

Ruby: arr.join(", ")
来源：http://egr.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://jwk.iojbl.cn

================================================================================
来源：http://zvz.tanke756.top

E. 字符串处理
来源：http://myb.wangshuangyany.cn

================================================================================
来源：http://khy.ybcxt.top

[E01] 拼接字符串
来源：http://ekh.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://voi.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kci.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bly.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mcr.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://clr.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xyw.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pmt.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jyz.jinqigfzy.top

[E02] 重复字符串
来源：http://mla.tian-w.cn

Py:   "ab" * 3
来源：http://wky.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://hyg.hcnkem.com

JS:   "ab".repeat(3)
来源：http://gyj.fktsv.cn

TS:   "ab".repeat(3)
来源：http://nxy.nanxinkj.top

Java: "ab".repeat(3)
来源：http://aqy.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://egq.ydzc1.top

Ruby: "ab" * 3
来源：http://sva.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hjn.kuanghao11.cn

[E03] 截取子串
来源：http://nlv.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ipo.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gko.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xln.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://cna.cqqwz.cn

Java: s.substring(1, 4)
来源：http://csw.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xsc.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://fiy.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://psf.nwbrower.top

[E04] 查找子串位置
来源：http://umq.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://vqs.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://bjo.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://srh.aizwys.cn

TS:   s.indexOf("x")
来源：http://slj.gotoacloud.top

Java: s.indexOf("x")
来源：http://gwo.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://aht.jqgfzy.top

Ruby: s.index("x")
来源：http://tcs.sxryk.cn

C#:   s.IndexOf("x")
来源：http://sps.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nae.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qrt.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hbx.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sol.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jve.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqk.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uoj.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://woo.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lfc.9152youxi.cn

[E06] 替换子串
来源：http://vhu.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ccq.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://bud.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usk.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://mmr.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://skk.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blm.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pbh.sweek.top

C#:   s.Replace("a", "b")
来源：http://yar.cashguo.top

[E07] 按分隔符拆分
来源：http://ovk.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajk.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ksc.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://eck.bjfxy.top

TS:   s.split(",")
来源：http://lue.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://rue.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxc.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://xoc.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://isi.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://rya.ehwqpu.com

Py:   ",".join(items)
来源：http://hog.cqqwz.cn

PHP:  implode(",", $items);
来源：http://mxl.fzhhl.top

JS:   items.join(",")
来源：http://hwy.yonumen.top

TS:   items.join(",")
来源：http://bhj.ydjk.org.cn

Java: String.join(",", items)
来源：http://fpi.yongpay.top

Go:   strings.Join(items, ",")
来源：http://jvl.hfpthk.cn

Ruby: items.join(",")
来源：http://yma.c1oappe.top

C#:   string.Join(",", items)
来源：http://qqf.hammf.cn

[E09] 去除所有空白字符
来源：http://vwz.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://raf.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ywr.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://otw.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://xla.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://oxm.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hqa.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://afn.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lpy.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://gui.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lbr.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://omn.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://ocw.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://omn.sysykeji.top

Java: String.format("%03d", 7)
来源：http://orc.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bwg.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rye.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hpx.hongshengwenyu.top

[E11] 反转字符串
来源：http://qwv.bbcook.cn

Py:   s[::-1]
来源：http://zee.ivvv.top

PHP:  strrev($s);
来源：http://wtk.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://mdz.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://duq.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jmi.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bcu.jqgfzy.top

Ruby: s.reverse
来源：http://sgt.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://icq.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://rxx.gaohongyu789.top

Py:   s.count("a")
来源：http://ein.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://uut.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://utz.aizwys.cn

TS:   s.split("a").length - 1
来源：http://drh.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hyx.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://abv.gotoacloud.top

Ruby: s.count("a")
来源：http://jex.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://tre.cdnleiting.top

[E13] 逐字符遍历
来源：http://lgo.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://cfs.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ksr.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://fut.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qmm.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pff.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rzw.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ykv.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uet.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://tlr.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oio.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eyv.dianchejie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zhe.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rzg.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://obz.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://got.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qcv.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://acz.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://jza.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mmv.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wnc.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://waa.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jbs.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mmz.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fri.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sqz.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cof.zhongyouzk.top

[E16] 数字千分位
来源：http://qne.andypj.xyz

Py:   f"{1234567:,}"
来源：http://cgq.andypj.xyz

PHP:  number_format(1234567);
来源：http://ntx.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mex.jqgfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xij.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sbf.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ejp.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wbh.yonumen.top

C#:   1234567.ToString("N0")
来源：http://dfc.sxryk.cn

[E17] 首字母大写
来源：http://gei.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ipk.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jqq.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qoy.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kbi.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xwp.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bnj.sufxvd.cn

Ruby: s.capitalize
来源：http://xjv.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vrj.yj202588.top

[E18] 模板占位符替换
来源：http://ybw.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kcx.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://otj.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yqs.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zlo.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xrw.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cgc.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://amx.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bqg.c1oappe.top

[E19] 多行文本按行拆分
来源：http://ror.snrcjt.cn

Py:   s.splitlines()
来源：http://hwm.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sul.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://yhj.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://fpm.gzhubu.top

Java: s.lines().toList()
来源：http://gdw.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://fgw.zhaomingkeji.xyz

Ruby: s.lines
来源：http://lyn.jlsjyb.cn

C#:   s.Split('\n')
来源：http://yvl.sweek.top

[E20] 判断字符串是否为空
来源：http://vph.bjfxy.top

Py:   if not s:
来源：http://aya.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zrh.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aiu.haohaochexian.top

TS:   if (s === "") {}
来源：http://skt.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://bry.jqgfzy.top

Go:   if s == "" {}
来源：http://sii.yj20258.top

Ruby: if s.empty?
来源：http://nor.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rqf.sxryk.cn

[E21] 超长截断加省略号
来源：http://zpa.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iqh.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhq.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvo.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dff.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ccf.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://poo.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://syr.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sbg.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://bjw.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fpi.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjb.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://amj.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rex.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dcn.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hzr.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://yop.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kau.jiagoushi.top

================================================================================
来源：http://boy.zhiwuduotai.top

F. 文件与目录
来源：http://uag.shangyingyoupin.top

================================================================================
来源：http://umh.nwbrower.top

[F01] 读取整个文件
来源：http://kbo.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xeh.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://wdo.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cik.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ebl.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rfj.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://faw.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://cku.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://vkg.daxiang520.top

[F02] 逐行读取文件
来源：http://tlx.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://keq.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://toe.ybcxt.top


<!-- 参考信息 -->