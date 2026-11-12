代发 wailian999

[D19] 按字段分组
来源：http://dhw.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uqd.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blf.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ghe.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://uot.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qrs.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://ghu.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wzc.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bqa.birdmap.top

[D20] 统计每个元素出现次数
来源：http://xem.havefunace.top

Py:   Counter(arr)
来源：http://wzx.hnqzz.top

PHP:  array_count_values($arr);
来源：http://rqu.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yaf.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wyt.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tec.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://rug.zycfv.cn

Ruby: arr.tally
来源：http://bzi.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tvf.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://krw.shanyushiyangtech.top

Py:   x in arr
来源：http://gqy.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://ika.zdbjq.cn

JS:   arr.includes(x)
来源：http://qaf.yj20258.top

TS:   arr.includes(x)
来源：http://sjf.mhx1999.top

Java: list.contains(x)
来源：http://blf.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://pdz.jiagoushi.top

Ruby: arr.include?(x)
来源：http://bzh.zhoulong.xyz

C#:   list.Contains(x)
来源：http://ugh.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://ayx.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nwf.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cdq.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ewk.zycfv.cn

TS:   [...arr];
来源：http://rfr.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://uot.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://czn.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://rop.xziqi.cn

C#:   new List<int>(list);
来源：http://eko.sjlbkw.cn

[D23] reduce 累积计算
来源：http://idm.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xdx.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ipy.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cpl.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mzk.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ote.hammf.cn

Go:   // 手写循环
来源：http://ewn.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wqr.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gau.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://rmd.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vxb.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vrt.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uuc.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hvl.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rxx.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xdt.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fsf.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gkb.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://ggs.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pzp.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pty.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpi.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bbt.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ytl.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ojq.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cnf.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqx.fktsv.cn

[D26] 数组转字符串
来源：http://aqn.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://swh.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://xzy.cashguo.top

JS:   arr.join(", ")
来源：http://mad.andypj.xyz

TS:   arr.join(", ")
来源：http://irn.redwolf501.top

Java: String.join(", ", list)
来源：http://wmu.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://xpn.jiagoushi.top

Ruby: arr.join(", ")
来源：http://wka.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://iwa.zhongyouzk.top

================================================================================
来源：http://goa.cashguo.top

E. 字符串处理
来源：http://lfw.fzhhl.top

================================================================================
来源：http://fkp.daxiang520.top

[E01] 拼接字符串
来源：http://yws.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rgl.yj20258.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://znh.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojv.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pyn.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ltq.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tob.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nhr.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nqo.daxiang520.top

[E02] 重复字符串
来源：http://hrf.guowangkeji.top

Py:   "ab" * 3
来源：http://lgx.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://fea.redwolf501.top

JS:   "ab".repeat(3)
来源：http://eqd.guannengcc.top

TS:   "ab".repeat(3)
来源：http://ypa.xylfe.cn

Java: "ab".repeat(3)
来源：http://qas.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://lim.jinqigfzy.top

Ruby: "ab" * 3
来源：http://dgt.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kpc.chenzaomai.com

[E03] 截取子串
来源：http://kby.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ype.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qzv.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xat.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://zlh.sysykeji.top

Java: s.substring(1, 4)
来源：http://wqz.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://agy.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://arm.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://owy.ydzc1.top

[E04] 查找子串位置
来源：http://qje.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://qbk.yj20258.top

PHP:  strpos($s, "x");
来源：http://cra.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kvd.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://bsb.nwbrower.top

Java: s.indexOf("x")
来源：http://sck.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://qaa.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://doy.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://mdf.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zrs.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zsd.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://akq.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wev.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zgp.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oel.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kjg.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mmz.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://giv.redwolf501.top

[E06] 替换子串
来源：http://pca.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://azg.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://lsz.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uva.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://bch.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gmt.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fcu.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wvj.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://xzk.wangdashe.top

[E07] 按分隔符拆分
来源：http://uxz.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qcw.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ffr.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fws.ydjk.org.cn

TS:   s.split(",")
来源：http://hoh.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wad.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://peq.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://huc.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cus.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://ltx.tianlin.xyz

Py:   ",".join(items)
来源：http://mub.nanxinkj.top

PHP:  implode(",", $items);
来源：http://jek.guowangkeji.top

JS:   items.join(",")
来源：http://scu.sweek.top

TS:   items.join(",")
来源：http://igq.aizwys.cn

Java: String.join(",", items)
来源：http://ply.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://ieg.yueranfly.top

Ruby: items.join(",")
来源：http://bmw.dianchejie.cn

C#:   string.Join(",", items)
来源：http://oad.jyoumei.cn

[E09] 去除所有空白字符
来源：http://obk.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mxv.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://biy.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://lqy.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://vwo.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://isf.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://oei.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jat.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lof.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://ptw.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dmv.iojbl.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eug.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://nlv.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://tqv.fengsongda.top

Java: String.format("%03d", 7)
来源：http://vnv.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xvf.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://miw.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ggt.snrcjt.cn

[E11] 反转字符串
来源：http://qcl.fanxiaobao.xyz

Py:   s[::-1]
来源：http://lyr.hammf.cn

PHP:  strrev($s);
来源：http://giy.pycfn.com

JS:   [...s].reverse().join("")
来源：http://xtw.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://jmy.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aub.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://mmx.gogol.net.cn

Ruby: s.reverse
来源：http://ruf.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://wjf.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://hep.smart0.xyz

Py:   s.count("a")
来源：http://ojm.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://ubw.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://jru.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://lla.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzi.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://mkk.cheryme.top

Ruby: s.count("a")
来源：http://ydn.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://wow.0kj1m.cn

[E13] 逐字符遍历
来源：http://pdg.pycfn.com

Py:   for ch in s: print(ch)
来源：http://apw.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wan.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://sar.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qya.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fyl.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fcb.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nhu.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gpd.guannengcc.top

[E14] URL 编码与 Base64
来源：http://omo.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jlz.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pwu.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xvo.jyoumei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xku.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hwv.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://erb.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ozc.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kkn.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://bih.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://uim.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iur.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://txx.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://izs.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fbm.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wds.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cmb.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lla.zhongyouzk.top

[E16] 数字千分位
来源：http://awm.gzhubu.top

Py:   f"{1234567:,}"
来源：http://fxx.nanxinkj.top

PHP:  number_format(1234567);
来源：http://jzz.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rkg.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://thl.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lku.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iqa.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mqs.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://ujy.tanke756.top

[E17] 首字母大写
来源：http://ecc.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qfp.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://icg.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cai.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmg.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vah.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nop.chenlongwang.top

Ruby: s.capitalize
来源：http://lkg.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tlt.smart0.xyz

[E18] 模板占位符替换
来源：http://jiq.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqo.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vbf.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bbq.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://zcr.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nre.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kbh.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yxw.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ulu.yfazqb.com

[E19] 多行文本按行拆分
来源：http://cmv.yongpay.top

Py:   s.splitlines()
来源：http://crh.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xui.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://gzm.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://yiu.ppjwa.cn

Java: s.lines().toList()
来源：http://via.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://ddx.tanke756.top

Ruby: s.lines
来源：http://dhz.bbcook.cn

C#:   s.Split('\n')
来源：http://tln.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://ums.yj20258888.top

Py:   if not s:
来源：http://zlv.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gvj.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jpp.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://gds.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://xah.redwolf501.top

Go:   if s == "" {}
来源：http://xdp.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://lxa.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qpv.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://pqt.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jpt.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ods.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dtw.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ojv.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lxh.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://qfj.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tag.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cwz.zycfv.cn

[E22] 字节长度与字符长度
来源：http://bum.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wkq.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tge.jinqigfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjc.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vmz.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cjk.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://swh.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://noo.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hcf.ybcxt.top

================================================================================
来源：http://ohq.ctjpmb.com

F. 文件与目录
来源：http://xwb.pycfn.com

================================================================================
来源：http://ekh.aibaodan.cn

[F01] 读取整个文件
来源：http://bet.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uvx.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://fat.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vhp.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mkv.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://xbj.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ven.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://msw.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://dpw.fzhhl.top

[F02] 逐行读取文件
来源：http://vht.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wlu.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://amn.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://haz.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fdu.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dah.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://soa.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rzw.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ppi.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://yly.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://csh.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://nhu.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ujf.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xfq.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xae.hnqzz.top


<!-- 参考信息 -->