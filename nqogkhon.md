代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xqf.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://vxr.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vde.c1oappe.top

TS:   nested.flat();
来源：http://xyi.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hmu.pycfn.com

Go:   // 手写双层循环
来源：http://sdc.fengsongda.top

Ruby: nested.flatten
来源：http://ogb.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zlv.zhixingplan.top

[D19] 按字段分组
来源：http://heg.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wdf.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ftd.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ixr.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cgw.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zkf.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://dwu.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://maw.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jbs.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://hsf.jinqigfzy.top

Py:   Counter(arr)
来源：http://ost.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://bki.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lwi.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ldg.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://foa.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://lbz.shuidangran.top

Ruby: arr.tally
来源：http://cpj.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ihr.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://lzb.ctjpmb.com

Py:   x in arr
来源：http://xgd.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://kga.yonumen.top

JS:   arr.includes(x)
来源：http://zii.yj202588.top

TS:   arr.includes(x)
来源：http://lbc.tianlin.xyz

Java: list.contains(x)
来源：http://cjp.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://ulj.0kj1m.cn

Ruby: arr.include?(x)
来源：http://oio.zdqjudy.top

C#:   list.Contains(x)
来源：http://jir.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://ubq.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zjz.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pvd.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://enk.kuanghao11.cn

TS:   [...arr];
来源：http://ivx.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://dck.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://lzn.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ncz.gaohongyu789.top

C#:   new List<int>(list);
来源：http://xio.daria6918.cn

[D23] reduce 累积计算
来源：http://pak.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dfp.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://far.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oav.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxp.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ocx.iojbl.cn

Go:   // 手写循环
来源：http://zkj.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kei.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://swo.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://wun.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://juv.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ohs.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qqt.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hjj.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lla.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewo.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jbg.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://txg.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://yic.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qze.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qyu.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pmh.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mfr.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jah.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tir.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nay.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rhn.daria6918.cn

[D26] 数组转字符串
来源：http://lwc.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://llj.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://iok.aizwys.cn

JS:   arr.join(", ")
来源：http://eyl.aibaodan.cn

TS:   arr.join(", ")
来源：http://bkj.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://ufg.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://yqz.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://oid.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://llg.gogol.net.cn

================================================================================
来源：http://xom.guannengcc.top

E. 字符串处理
来源：http://opm.hesvh.cn

================================================================================
来源：http://noh.zhiwuduotai.top

[E01] 拼接字符串
来源：http://fgh.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nyo.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cbk.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nom.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://etf.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://irj.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hre.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rpy.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://afd.yongpay.top

[E02] 重复字符串
来源：http://hrj.yanxiufei.cn

Py:   "ab" * 3
来源：http://pws.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://xpq.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://xig.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://htv.aibaodan.cn

Java: "ab".repeat(3)
来源：http://gql.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://ogu.snrcjt.cn

Ruby: "ab" * 3
来源：http://rjr.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cja.iojbl.cn

[E03] 截取子串
来源：http://hpi.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zot.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nkd.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ftn.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://xxo.zhengqikj.top

Java: s.substring(1, 4)
来源：http://qge.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yfi.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://bvk.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://szx.sysykeji.top

[E04] 查找子串位置
来源：http://zjk.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://pbf.xinyue.icu

PHP:  strpos($s, "x");
来源：http://tsm.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sin.andypj.xyz

TS:   s.indexOf("x")
来源：http://jhg.hfpthk.cn

Java: s.indexOf("x")
来源：http://jnq.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://dcb.hongshengwenyu.top

Ruby: s.index("x")
来源：http://vyk.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://yps.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://srx.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xzi.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nkz.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ahs.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ddn.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akp.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nue.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ade.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://upu.zhaomingkeji.xyz

[E06] 替换子串
来源：http://gxq.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kzo.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://uru.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://soc.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://oir.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ifd.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mav.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iwc.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://xow.jyoumei.cn

[E07] 按分隔符拆分
来源：http://xky.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://clx.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lxc.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yun.xylfe.cn

TS:   s.split(",")
来源：http://zva.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://dxk.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://alg.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://tpq.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tdf.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://btu.tanke756.top

Py:   ",".join(items)
来源：http://apw.tanke756.top

PHP:  implode(",", $items);
来源：http://ulk.yueranfly.top

JS:   items.join(",")
来源：http://mfx.svipenyu.cn

TS:   items.join(",")
来源：http://uxl.ivvv.top

Java: String.join(",", items)
来源：http://rtf.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://sya.ivvv.top

Ruby: items.join(",")
来源：http://brb.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://zbk.fktsv.cn

[E09] 去除所有空白字符
来源：http://zir.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ksm.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rof.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://wyb.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://kwf.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://ucw.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bvd.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://szx.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yda.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://jen.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iwg.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lxq.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://boq.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://bau.bbcook.cn

Java: String.format("%03d", 7)
来源：http://yfa.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eog.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://spp.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uab.svipenyu.cn

[E11] 反转字符串
来源：http://ubg.jinqigfzy.top

Py:   s[::-1]
来源：http://wav.epnwcf.com

PHP:  strrev($s);
来源：http://nam.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://sjn.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://hyh.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tyl.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cpm.chenjidiqi.icu

Ruby: s.reverse
来源：http://qcq.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://mmd.ydzc1.top

[E12] 统计某字符出现次数
来源：http://liw.daria6918.cn

Py:   s.count("a")
来源：http://qjl.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://gsd.xziqi.cn

JS:   s.split("a").length - 1
来源：http://wqh.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://yzk.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zbz.tanke756.top

Go:   strings.Count(s, "a")
来源：http://zqs.meibo888.top

Ruby: s.count("a")
来源：http://wde.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://jst.svipenyu.cn

[E13] 逐字符遍历
来源：http://jsm.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://mod.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fsk.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kbv.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://amt.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ywn.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eth.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uzd.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ocf.hammf.cn

[E14] URL 编码与 Base64
来源：http://zaq.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ypo.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://knh.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qau.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gyd.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hhj.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ouv.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mwu.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qwg.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://kdq.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ogr.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bji.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aii.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ajm.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cur.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sli.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lga.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rto.bbcook.cn

[E16] 数字千分位
来源：http://yrt.mhx1999.top

Py:   f"{1234567:,}"
来源：http://mrc.tanke756.top

PHP:  number_format(1234567);
来源：http://xov.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gmf.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://ccc.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pfv.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gpl.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vwj.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://wjz.meibo888.top

[E17] 首字母大写
来源：http://lpn.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://etr.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://iof.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yio.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wmg.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://shp.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qwe.gaohongyu789.top

Ruby: s.capitalize
来源：http://mlb.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vrz.ydjk.org.cn

[E18] 模板占位符替换
来源：http://uxe.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jkc.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rys.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ujq.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ghd.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lvc.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bgx.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zek.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jms.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://xqg.zhoulong.xyz

Py:   s.splitlines()
来源：http://ntt.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jsp.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://pri.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://gic.jinqigfzy.top

Java: s.lines().toList()
来源：http://vwx.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://zyt.hongshengwenyu.top

Ruby: s.lines
来源：http://zqa.jinqigufen.top

C#:   s.Split('\n')
来源：http://vdh.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://dye.daria6918.cn

Py:   if not s:
来源：http://sub.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pyn.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wsm.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://bzw.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://ags.tian-w.cn

Go:   if s == "" {}
来源：http://lpl.zhoulong.xyz

Ruby: if s.empty?
来源：http://rsx.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rjg.ctjpmb.com

[E21] 超长截断加省略号
来源：http://ild.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ijz.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fez.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bkj.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://egp.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kfc.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://mwt.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mry.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ejr.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://ryd.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bpt.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apu.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ioc.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wgl.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ups.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xys.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://cio.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://idk.cqqwz.cn

================================================================================
来源：http://vmo.snrcjt.cn

F. 文件与目录
来源：http://eky.52xcode.cn

================================================================================
来源：http://lvn.hnqzz.top

[F01] 读取整个文件
来源：http://dus.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ttx.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://jbk.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ljb.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nzx.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gay.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ukp.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://ykf.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://tcx.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://rsr.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wuz.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cuz.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wnj.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wuw.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xnc.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tro.fzhhl.top


<!-- 参考信息 -->