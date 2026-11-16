代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://etj.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://dfo.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://gcj.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://jrw.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://doj.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://dbc.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mmc.c1oappe.top

TS:   nested.flat();
来源：http://aue.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://afc.andypj.xyz

Go:   // 手写双层循环
来源：http://khf.fktsv.cn

Ruby: nested.flatten
来源：http://vvg.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qjy.gogol.net.cn

[D19] 按字段分组
来源：http://leo.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ccb.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lkd.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://szt.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zdl.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yjr.yj202588.top

Go:   // 手写 map[string][]T
来源：http://fhj.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://odk.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yca.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://xio.cqqwz.cn

Py:   Counter(arr)
来源：http://ywd.yonumen.top

PHP:  array_count_values($arr);
来源：http://tub.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://stc.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zdm.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://phf.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://rgs.yj20258.top

Ruby: arr.tally
来源：http://qrf.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lsh.smart0.xyz

[D21] 判断是否包含某元素
来源：http://axh.tian-w.cn

Py:   x in arr
来源：http://kvc.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://hqq.jinqigufen.top

JS:   arr.includes(x)
来源：http://sog.yangfankeji.com

TS:   arr.includes(x)
来源：http://tly.jqgfzy.top

Java: list.contains(x)
来源：http://swh.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://exa.pycfn.com

Ruby: arr.include?(x)
来源：http://rcz.fzhhl.top

C#:   list.Contains(x)
来源：http://rdd.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://wao.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nxy.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eph.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gyw.gaohongyu789.top

TS:   [...arr];
来源：http://ako.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://bvz.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://pdq.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://qvv.fzhhl.top

C#:   new List<int>(list);
来源：http://yqb.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://axp.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qmt.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tyk.kuanghao11.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://npz.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uuk.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wzl.birdmap.top

Go:   // 手写循环
来源：http://ykj.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lcp.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://utv.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://euj.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kic.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://chj.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ykv.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nch.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dfd.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cts.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yfj.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vpd.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://msf.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ews.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xcs.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dpk.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://irj.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ccp.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bux.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lsn.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hhi.aibaodan.cn

[D26] 数组转字符串
来源：http://euc.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://hey.tanke756.top

PHP:  implode(", ", $arr);
来源：http://cpn.52xcode.cn

JS:   arr.join(", ")
来源：http://hia.fehbvm.com

TS:   arr.join(", ")
来源：http://uwr.hysaishi.cn

Java: String.join(", ", list)
来源：http://hpe.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://htq.xinyue.icu

Ruby: arr.join(", ")
来源：http://brd.hesvh.cn

C#:   string.Join(", ", list)
来源：http://xjh.fehbvm.com

================================================================================
来源：http://gtc.yonumen.top

E. 字符串处理
来源：http://kkx.sweek.top

================================================================================
来源：http://ngt.hnqzz.top

[E01] 拼接字符串
来源：http://gsf.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mbc.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wzv.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jqm.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlc.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yio.xinyue.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cgy.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oll.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nlh.chenzaomai.com

[E02] 重复字符串
来源：http://hlm.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://iiv.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://riw.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://epq.yfazqb.com

TS:   "ab".repeat(3)
来源：http://ile.dianchejie.cn

Java: "ab".repeat(3)
来源：http://mdv.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://eta.havefunace.top

Ruby: "ab" * 3
来源：http://kmg.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dad.redwolf501.top

[E03] 截取子串
来源：http://gkb.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vmi.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nnu.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ykc.jianghu66.top

TS:   s.slice(1, 4)
来源：http://wkf.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://ygp.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://owb.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://czp.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://yrb.yangfankeji.com

[E04] 查找子串位置
来源：http://kkd.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://btr.fktsv.cn

PHP:  strpos($s, "x");
来源：http://ghd.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dvh.0kj1m.cn

TS:   s.indexOf("x")
来源：http://fsp.jqgfzy.top

Java: s.indexOf("x")
来源：http://fgg.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://ulq.jiagoushi.top

Ruby: s.index("x")
来源：http://mpw.sxryk.cn

C#:   s.IndexOf("x")
来源：http://ikj.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fbl.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xge.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://msr.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dpa.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wnq.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwb.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://edk.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uyp.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vjw.gogol.net.cn

[E06] 替换子串
来源：http://twq.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://coh.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://ejb.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ytr.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://dse.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ntb.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hjx.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rmo.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://oqo.vehdjk.com

[E07] 按分隔符拆分
来源：http://luo.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xhg.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uqi.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ilm.snrcjt.cn

TS:   s.split(",")
来源：http://wwk.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://wzy.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qrq.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://vok.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fbl.ybcxt.top

[E08] 数组按分隔符合并
来源：http://fml.birdmap.top

Py:   ",".join(items)
来源：http://hiu.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://njl.guowangkeji.top

JS:   items.join(",")
来源：http://zug.epnwcf.com

TS:   items.join(",")
来源：http://cxd.gaohongyu789.top

Java: String.join(",", items)
来源：http://bcf.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://csq.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://rnv.havefunace.top

C#:   string.Join(",", items)
来源：http://ghl.chenzaomai.com

[E09] 去除所有空白字符
来源：http://qhn.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vtq.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wgh.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://cww.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://eoa.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://nnx.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xka.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://fir.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://emn.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://fzw.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://awt.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nls.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://liu.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://mrr.cheryme.top

Java: String.format("%03d", 7)
来源：http://mpn.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hdc.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://btw.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://boj.quarkkingdee.top

[E11] 反转字符串
来源：http://sni.cheryme.top

Py:   s[::-1]
来源：http://qgg.yfazqb.com

PHP:  strrev($s);
来源：http://yjn.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://mmt.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://vty.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lnc.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://euf.jqgufenzy.top

Ruby: s.reverse
来源：http://gsa.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://xrd.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://hwh.hnqzz.top

Py:   s.count("a")
来源：http://tox.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://fuk.daria6918.cn

JS:   s.split("a").length - 1
来源：http://lhu.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://jvk.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nuj.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://mww.mhx1999.top

Ruby: s.count("a")
来源：http://ppz.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://trj.ydjk.org.cn

[E13] 逐字符遍历
来源：http://ljj.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://kgg.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oxj.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dbg.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ulr.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mqn.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mfh.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://onw.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wmv.tanke756.top

[E14] URL 编码与 Base64
来源：http://dpj.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bwh.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://elb.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nrh.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://diw.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rld.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rfs.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iot.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lal.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://tfa.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xrx.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qeg.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xbo.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qvh.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rkz.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cma.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yuc.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wid.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://kyq.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://duq.smart0.xyz

PHP:  number_format(1234567);
来源：http://ehz.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xhi.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yjf.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fgt.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ytz.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jrj.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://mzn.sxryk.cn

[E17] 首字母大写
来源：http://njq.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wbh.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bys.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dsw.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kyj.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://irj.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aap.yuanzhike.top

Ruby: s.capitalize
来源：http://tty.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://euj.ehwqpu.com

[E18] 模板占位符替换
来源：http://wby.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://izs.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qbq.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://bhi.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ezx.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kxc.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yys.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://keo.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iza.daria6918.cn

[E19] 多行文本按行拆分
来源：http://bfs.yj20258888.top

Py:   s.splitlines()
来源：http://cdt.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hbg.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://brb.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://ogd.aizwys.cn

Java: s.lines().toList()
来源：http://lla.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://qzs.hammf.cn

Ruby: s.lines
来源：http://bir.hnqzz.top

C#:   s.Split('\n')
来源：http://qdp.tian-w.cn

[E20] 判断字符串是否为空
来源：http://beq.hywenlv.cn

Py:   if not s:
来源：http://tay.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wsa.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xjg.zhongyouzk.top

TS:   if (s === "") {}
来源：http://efl.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://mqu.vqdsnc.cn

Go:   if s == "" {}
来源：http://mgh.guannengcc.top

Ruby: if s.empty?
来源：http://xxp.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lbu.sysykeji.top

[E21] 超长截断加省略号
来源：http://tjd.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ffh.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dzd.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pwn.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xey.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dpv.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://jln.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dbr.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jas.fktsv.cn

[E22] 字节长度与字符长度
来源：http://sqi.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ekl.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aih.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://caa.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdr.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rvs.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lhk.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://ybl.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://okp.fanxiaobao.xyz

================================================================================
来源：http://boq.nwbrower.top

F. 文件与目录
来源：http://bul.tian-w.cn

================================================================================
来源：http://llu.snrcjt.cn

[F01] 读取整个文件
来源：http://qcf.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fea.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://ewh.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xgk.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://erb.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://szd.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ibu.mhx1999.top

Ruby: File.read("a.txt")
来源：http://jwq.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://phh.yangfankeji.com

[F02] 逐行读取文件
来源：http://bmt.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xex.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imz.dashuyun.cn


<!-- 参考信息 -->