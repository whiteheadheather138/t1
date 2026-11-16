代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bus.yongpay.top

Ruby: arr.max;  arr.min
来源：http://nnz.havefunace.top

C#:   list.Max();  list.Min()
来源：http://wti.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://erb.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qsf.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://ydi.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mgx.wangshuangyany.cn

TS:   nested.flat();
来源：http://ntb.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xkj.cqqwz.cn

Go:   // 手写双层循环
来源：http://cal.tianlin.xyz

Ruby: nested.flatten
来源：http://icb.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ofc.yvedp.cn

[D19] 按字段分组
来源：http://wwi.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zcb.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cya.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vko.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qgy.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tzi.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://uxb.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://tnz.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lmc.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://ttq.jqgufenzy.top

Py:   Counter(arr)
来源：http://sxe.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://ajt.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yaq.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqs.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ofo.fzhhl.top

Go:   // 手写 map[T]int
来源：http://mdt.aizwys.cn

Ruby: arr.tally
来源：http://kje.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rlk.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://lbc.epnwcf.com

Py:   x in arr
来源：http://koy.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://pjo.jinqigfzy.top

JS:   arr.includes(x)
来源：http://jdq.daria6918.cn

TS:   arr.includes(x)
来源：http://mgt.hfpthk.cn

Java: list.contains(x)
来源：http://tsn.sweek.top

Go:   slices.Contains(arr, x)
来源：http://olc.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://tih.cdnleiting.top

C#:   list.Contains(x)
来源：http://dpb.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://lob.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nqz.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bsp.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oeu.fehbvm.com

TS:   [...arr];
来源：http://snd.tian-w.cn

Java: new ArrayList<>(list);
来源：http://ncx.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oiv.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://ltt.xuanzx.com

C#:   new List<int>(list);
来源：http://mcz.yangfankeji.com

[D23] reduce 累积计算
来源：http://mgr.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zpc.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lln.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ung.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvg.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mxn.ppjwa.cn

Go:   // 手写循环
来源：http://jez.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iyt.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://elk.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://zib.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fns.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qjo.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jkw.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xbl.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ked.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zzq.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tix.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uxs.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://caz.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tjt.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://erw.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ghd.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wfp.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kth.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://grk.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wgf.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xlw.smart0.xyz

[D26] 数组转字符串
来源：http://lrx.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://qxl.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://sdi.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://ijd.gogol.net.cn

TS:   arr.join(", ")
来源：http://mrj.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://eyc.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://jcv.shuidangran.top

Ruby: arr.join(", ")
来源：http://jan.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://slz.ehwqpu.com

================================================================================
来源：http://lnz.cucudq.cn

E. 字符串处理
来源：http://rss.yangfankeji.com

================================================================================
来源：http://meg.yonumen.top

[E01] 拼接字符串
来源：http://xug.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iez.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mld.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lbo.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ido.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pmp.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wkx.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://irz.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sbx.dianchejie.cn

[E02] 重复字符串
来源：http://osk.havefunace.top

Py:   "ab" * 3
来源：http://ads.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://iva.316326.xyz

JS:   "ab".repeat(3)
来源：http://bbg.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://kcd.haohaochexian.top

Java: "ab".repeat(3)
来源：http://kdi.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://pui.hammf.cn

Ruby: "ab" * 3
来源：http://ziu.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zol.jlsjyb.cn

[E03] 截取子串
来源：http://hcd.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sxu.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://egm.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cbb.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://tht.hysaishi.cn

Java: s.substring(1, 4)
来源：http://vfe.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ywl.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://whk.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://pgl.zdqjudy.top

[E04] 查找子串位置
来源：http://gda.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://qln.xinyue.icu

PHP:  strpos($s, "x");
来源：http://upw.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ftw.ehwqpu.com

TS:   s.indexOf("x")
来源：http://rhv.pycfn.com

Java: s.indexOf("x")
来源：http://pnu.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://xol.fengsongda.top

Ruby: s.index("x")
来源：http://utw.cucudq.cn

C#:   s.IndexOf("x")
来源：http://jps.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uzr.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fdd.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fsf.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fzz.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://arn.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hid.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ntw.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ono.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fin.jqgufenzy.top

[E06] 替换子串
来源：http://iun.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kif.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://iyy.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ymt.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://jil.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vfo.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ctn.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mes.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://jqu.chenlongwang.top

[E07] 按分隔符拆分
来源：http://eso.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kxy.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vcr.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vjt.ctjpmb.com

TS:   s.split(",")
来源：http://tuh.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pli.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tsr.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://wia.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://olq.yfazqb.com

[E08] 数组按分隔符合并
来源：http://arr.andypj.xyz

Py:   ",".join(items)
来源：http://ngt.pycfn.com

PHP:  implode(",", $items);
来源：http://nqt.tianlin.xyz

JS:   items.join(",")
来源：http://tad.ydjk.org.cn

TS:   items.join(",")
来源：http://qaq.xylfe.cn

Java: String.join(",", items)
来源：http://cgz.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://dre.shuidangran.top

Ruby: items.join(",")
来源：http://wlr.hywenlv.cn

C#:   string.Join(",", items)
来源：http://pzj.aibaodan.cn

[E09] 去除所有空白字符
来源：http://lrp.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yue.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fwg.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://djg.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://mis.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://pez.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ugm.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://bqf.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cti.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://lvb.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ony.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kev.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://tmk.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://wgg.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://bed.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qor.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://khj.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ald.yongpay.top

[E11] 反转字符串
来源：http://kok.jiagoushi.top

Py:   s[::-1]
来源：http://uwe.guowangkeji.top

PHP:  strrev($s);
来源：http://hne.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://gur.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://sal.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://etx.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lbh.shangyingyoupin.top

Ruby: s.reverse
来源：http://ebr.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zrj.sysykeji.top

[E12] 统计某字符出现次数
来源：http://irc.zhixingplan.top

Py:   s.count("a")
来源：http://xew.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://nxg.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://izy.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://qoh.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gtz.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://zxf.jinqigufen.top

Ruby: s.count("a")
来源：http://qjo.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://rls.jinqigufen.top

[E13] 逐字符遍历
来源：http://ois.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://tuc.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bye.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://uyd.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eay.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qzk.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ncv.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://jyf.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fxl.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://qfw.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yga.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zwf.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gxx.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wly.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://stu.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ftd.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tka.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lad.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://vuh.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dbr.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dav.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jnr.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://svy.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rvq.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dgp.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mej.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hnr.xziqi.cn

[E16] 数字千分位
来源：http://ayq.fengsongda.top

Py:   f"{1234567:,}"
来源：http://fal.xziqi.cn

PHP:  number_format(1234567);
来源：http://bej.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mtt.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rcm.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ntx.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aad.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zgc.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://kbn.ehwqpu.com

[E17] 首字母大写
来源：http://edb.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://moj.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bvp.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tzj.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wyq.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yrw.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hby.zhongyouzk.top

Ruby: s.capitalize
来源：http://eyu.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ede.tian-w.cn

[E18] 模板占位符替换
来源：http://dat.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xic.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qsp.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://swl.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bwy.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dcl.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wbn.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kww.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wwx.meibo888.top

[E19] 多行文本按行拆分
来源：http://hjc.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://geh.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ayn.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://txw.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://jnn.tarul.cn

Java: s.lines().toList()
来源：http://ira.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://sge.nanxinkj.top

Ruby: s.lines
来源：http://ptf.cucudq.cn

C#:   s.Split('\n')
来源：http://wor.smart0.xyz

[E20] 判断字符串是否为空
来源：http://gvx.jiagoushi.top

Py:   if not s:
来源：http://moy.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nok.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tze.xylfe.cn

TS:   if (s === "") {}
来源：http://gsy.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://sad.ydzc1.top

Go:   if s == "" {}
来源：http://yxp.xylfe.cn

Ruby: if s.empty?
来源：http://xew.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bwo.jqgfzy.top

[E21] 超长截断加省略号
来源：http://yuo.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ury.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ywf.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ykw.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ioi.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qll.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://los.mhx1999.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbo.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wna.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://uvu.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://maz.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cbt.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gbb.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dyn.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nab.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qll.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://diw.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hft.yuxming.cn

================================================================================
来源：http://xxq.cqqwz.cn

F. 文件与目录
来源：http://urp.aizwys.cn

================================================================================
来源：http://gqi.jiagoushi.top

[F01] 读取整个文件
来源：http://awk.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yaj.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://cgm.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sdw.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ybi.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dvf.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ykq.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://xxq.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://que.nwbrower.top

[F02] 逐行读取文件
来源：http://pga.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zrz.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lcd.hysaishi.cn


<!-- 参考信息 -->