代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uym.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://cox.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mks.tarul.cn

TS:   nested.flat();
来源：http://sdd.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wec.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://ctx.aizwys.cn

Ruby: nested.flatten
来源：http://elw.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wsd.hammf.cn

[D19] 按字段分组
来源：http://qar.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edl.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zfy.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oki.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cwv.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wzr.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://wqh.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://php.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wlj.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://qus.sjlbkw.cn

Py:   Counter(arr)
来源：http://rpe.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://aex.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://shh.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pbf.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xew.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://twf.yfazqb.com

Ruby: arr.tally
来源：http://skb.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mkj.yuxming.cn

[D21] 判断是否包含某元素
来源：http://rri.feifeiyinyue.top

Py:   x in arr
来源：http://elb.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://vll.aizwys.cn

JS:   arr.includes(x)
来源：http://zdh.sxryk.cn

TS:   arr.includes(x)
来源：http://szr.smart0.xyz

Java: list.contains(x)
来源：http://boj.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://ryx.0kj1m.cn

Ruby: arr.include?(x)
来源：http://uki.zhoulong.xyz

C#:   list.Contains(x)
来源：http://ete.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://arp.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yew.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kro.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jqv.yuanzhike.top

TS:   [...arr];
来源：http://jfy.316326.xyz

Java: new ArrayList<>(list);
来源：http://ncc.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://xds.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://fak.hywenlv.cn

C#:   new List<int>(list);
来源：http://edx.haohaochexian.top

[D23] reduce 累积计算
来源：http://pzq.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zwg.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mwz.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tjf.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bde.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cni.ybcxt.top

Go:   // 手写循环
来源：http://dzt.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tzw.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zaj.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://enq.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://agd.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ivt.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skx.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mfr.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://unr.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vzo.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://njt.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fpk.hammf.cn

[D25] Set 集合去重与交并差
来源：http://xby.quarkkingdee.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uer.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xel.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xey.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://njf.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dol.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dal.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bzw.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zyl.jianghu66.top

[D26] 数组转字符串
来源：http://kur.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://sov.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://zsb.gzhubu.top

JS:   arr.join(", ")
来源：http://aey.mhx1999.top

TS:   arr.join(", ")
来源：http://mex.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://fhe.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://wcy.snrcjt.cn

Ruby: arr.join(", ")
来源：http://pxi.fktsv.cn

C#:   string.Join(", ", list)
来源：http://ixa.hcnkem.com

================================================================================
来源：http://urx.gotoacloud.top

E. 字符串处理
来源：http://gri.shanyushiyangkeji.top

================================================================================
来源：http://dsf.haohaochexian.top

[E01] 拼接字符串
来源：http://vkl.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gaf.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ytk.haohaochexian.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zew.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxr.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oxg.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lvq.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ysq.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jcd.hysaishi.cn

[E02] 重复字符串
来源：http://whl.yfazqb.com

Py:   "ab" * 3
来源：http://rwp.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://zua.iojbl.cn

JS:   "ab".repeat(3)
来源：http://sxr.nwbrower.top

TS:   "ab".repeat(3)
来源：http://ivd.svipenyu.cn

Java: "ab".repeat(3)
来源：http://ptm.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://iqh.haohaochexian.top

Ruby: "ab" * 3
来源：http://spk.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cgg.hongshengwenyu.top

[E03] 截取子串
来源：http://gds.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iri.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lzu.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gzp.xylfe.cn

TS:   s.slice(1, 4)
来源：http://rcs.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://rpr.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lnr.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://tvx.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://pgl.mhx1999.top

[E04] 查找子串位置
来源：http://zhm.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://eaw.birdmap.top

PHP:  strpos($s, "x");
来源：http://wcm.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://srz.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://wgi.daria6918.cn

Java: s.indexOf("x")
来源：http://anz.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://iah.zhiwuduotai.top

Ruby: s.index("x")
来源：http://cki.iojbl.cn

C#:   s.IndexOf("x")
来源：http://ciz.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://icy.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bjn.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fii.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sds.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://war.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akh.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://txx.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ink.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ezt.gzhubu.top

[E06] 替换子串
来源：http://qvc.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yyv.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://qdn.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yrb.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://rwc.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jsk.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hxr.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jhx.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://dtk.yfazqb.com

[E07] 按分隔符拆分
来源：http://hxa.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lua.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://voq.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uqj.guowangkeji.top

TS:   s.split(",")
来源：http://vuk.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ami.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zfb.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://bsx.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://viy.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://phi.yonumen.top

Py:   ",".join(items)
来源：http://iwl.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://jlu.jqgufenzy.top

JS:   items.join(",")
来源：http://dvm.xziqi.cn

TS:   items.join(",")
来源：http://qgl.shzxlz.cn

Java: String.join(",", items)
来源：http://pcr.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://vhu.nanxinkj.top

Ruby: items.join(",")
来源：http://ynt.ydzc1.top

C#:   string.Join(",", items)
来源：http://zwm.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://hxy.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rkr.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yus.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://jyd.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://vur.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://mdz.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://trp.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://htp.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nph.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://gig.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://efn.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xzk.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://pxl.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://eso.havefunace.top

Java: String.format("%03d", 7)
来源：http://avm.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rru.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxi.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pzb.yanxiufei.cn

[E11] 反转字符串
来源：http://ocw.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://cse.chenlongwang.top

PHP:  strrev($s);
来源：http://ohf.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://jei.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://haf.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ifu.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zaa.cqqwz.cn

Ruby: s.reverse
来源：http://ioc.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://vnr.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://jcz.yueranfly.top

Py:   s.count("a")
来源：http://bwd.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://wgj.zycfv.cn

JS:   s.split("a").length - 1
来源：http://rvd.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://tku.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qep.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://qlm.hesvh.cn

Ruby: s.count("a")
来源：http://mmf.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://rod.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://lsy.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://xcn.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ovr.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mit.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ekp.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jkh.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ldz.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://xzc.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://leh.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://fua.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://paw.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ksb.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tqn.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rjb.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tap.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sys.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ero.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gly.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://zia.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cbv.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iop.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pxy.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kgj.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lmw.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rvi.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wfc.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://faj.ydjk.org.cn

[E16] 数字千分位
来源：http://mai.sweek.top

Py:   f"{1234567:,}"
来源：http://ylg.ybcxt.top

PHP:  number_format(1234567);
来源：http://ivw.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kzc.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ekw.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vvp.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nwh.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ftq.yonumen.top

C#:   1234567.ToString("N0")
来源：http://mmy.jianghu66.top

[E17] 首字母大写
来源：http://yro.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hqs.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hvq.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evk.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kwd.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zec.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iue.meibo888.top

Ruby: s.capitalize
来源：http://yir.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vif.fktsv.cn

[E18] 模板占位符替换
来源：http://tfm.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://djz.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://reg.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xho.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rmz.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ita.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dgm.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aqm.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uwz.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://dnd.jqgufenzy.top

Py:   s.splitlines()
来源：http://gce.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://svd.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://yzk.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://bhx.fehbvm.com

Java: s.lines().toList()
来源：http://jsd.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://rzy.cqqwz.cn

Ruby: s.lines
来源：http://ghe.cqqwz.cn

C#:   s.Split('\n')
来源：http://jte.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://oag.iojbl.cn

Py:   if not s:
来源：http://juu.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tvo.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://txl.gotoacloud.top

TS:   if (s === "") {}
来源：http://loi.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://qng.yongpay.top

Go:   if s == "" {}
来源：http://upi.vehdjk.com

Ruby: if s.empty?
来源：http://ojo.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ubi.yj202588.top

[E21] 超长截断加省略号
来源：http://fol.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://toc.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pbe.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptl.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ume.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qof.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://iab.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nzo.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ulx.shuidangran.top

[E22] 字节长度与字符长度
来源：http://hin.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://shk.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nma.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rww.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vcl.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wzr.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pzt.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://kwx.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fya.tarul.cn

================================================================================
来源：http://cdj.52xcode.cn

F. 文件与目录
来源：http://mbx.cheryme.top

================================================================================
来源：http://gay.ehwqpu.com

[F01] 读取整个文件
来源：http://ikg.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ato.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://eer.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://chg.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tui.jqgufenzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cyu.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ihx.zycfv.cn

Ruby: File.read("a.txt")
来源：http://saw.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://sgx.sufxvd.cn

[F02] 逐行读取文件
来源：http://yof.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gyt.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cty.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tru.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tvn.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xar.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qwb.yanxiufei.cn


<!-- 参考信息 -->