代发 wailian999

[D19] 按字段分组
来源：http://hdj.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fge.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gqr.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zhq.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vbj.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mhq.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://hua.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zmg.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uiq.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://qag.nanxinkj.top

Py:   Counter(arr)
来源：http://fez.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://hon.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyh.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbe.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jgo.fengsongda.top

Go:   // 手写 map[T]int
来源：http://ocv.yfazqb.com

Ruby: arr.tally
来源：http://qxe.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wwq.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://itk.yanxiufei.cn

Py:   x in arr
来源：http://icf.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://qve.birdmap.top

JS:   arr.includes(x)
来源：http://krz.ivvv.top

TS:   arr.includes(x)
来源：http://qkh.guannengcc.top

Java: list.contains(x)
来源：http://erq.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://gxc.shuidangran.top

Ruby: arr.include?(x)
来源：http://vda.quarkkingdee.top

C#:   list.Contains(x)
来源：http://xow.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://yue.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cgj.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tvh.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jgo.sjlbkw.cn

TS:   [...arr];
来源：http://vgg.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://kzg.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fcc.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://duj.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://geg.birdmap.top

[D23] reduce 累积计算
来源：http://syk.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://llk.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ylw.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fiy.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qbd.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ntp.jiagoushi.top

Go:   // 手写循环
来源：http://vwi.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zyj.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fwn.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://vpg.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wfl.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://erk.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cxt.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ixa.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vco.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mpp.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://civ.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jmt.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://bmd.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wkf.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pqh.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zcs.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bld.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgg.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://miq.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wne.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tjn.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://ctu.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://cvu.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://cmv.zhixingplan.top

JS:   arr.join(", ")
来源：http://bmd.yongpay.top

TS:   arr.join(", ")
来源：http://cre.daxiang520.top

Java: String.join(", ", list)
来源：http://mdx.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://nzb.haohaochexian.top

Ruby: arr.join(", ")
来源：http://vsm.pycfn.com

C#:   string.Join(", ", list)
来源：http://coh.yj20258.top

================================================================================
来源：http://nac.sxryk.cn

E. 字符串处理
来源：http://xfw.yvedp.cn

================================================================================
来源：http://ayp.xuetiantiany.cn

[E01] 拼接字符串
来源：http://pay.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xsd.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dcu.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jvl.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://leq.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rfo.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zyu.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fax.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rzu.yj20258888.top

[E02] 重复字符串
来源：http://dpc.316326.xyz

Py:   "ab" * 3
来源：http://dvp.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://aht.epnwcf.com

JS:   "ab".repeat(3)
来源：http://gls.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://ehd.fzhhl.top

Java: "ab".repeat(3)
来源：http://ypz.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://fvl.vqdsnc.cn

Ruby: "ab" * 3
来源：http://lef.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pbt.zhixingplan.top

[E03] 截取子串
来源：http://fpj.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gmq.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oyl.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wtf.xinyue.icu

TS:   s.slice(1, 4)
来源：http://vgg.tian-w.cn

Java: s.substring(1, 4)
来源：http://iyz.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qvx.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qgv.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://gss.jiagoushi.top

[E04] 查找子串位置
来源：http://dnf.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://vab.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://jqx.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cmn.sysykeji.top

TS:   s.indexOf("x")
来源：http://pet.dashuyun.cn

Java: s.indexOf("x")
来源：http://bsa.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://fbr.sweek.top

Ruby: s.index("x")
来源：http://gqg.nwbrower.top

C#:   s.IndexOf("x")
来源：http://zyo.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qis.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jjz.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bsw.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://obo.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kjr.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://acp.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://txj.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://snh.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://afj.fengsongda.top

[E06] 替换子串
来源：http://yqk.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yag.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://nqy.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mwz.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://ldi.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zpl.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://evv.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xlg.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://wcd.hcnkem.com

[E07] 按分隔符拆分
来源：http://vbt.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zcw.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cfl.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sml.chenlongwang.top

TS:   s.split(",")
来源：http://mmz.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jtp.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tqt.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://bnv.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://amy.fanxiaobao.xyz

[E08] 数组按分隔符合并
来源：http://reo.vqdsnc.cn

Py:   ",".join(items)
来源：http://bkj.hfpthk.cn

PHP:  implode(",", $items);
来源：http://gsp.hywenlv.cn

JS:   items.join(",")
来源：http://lpv.vqdsnc.cn

TS:   items.join(",")
来源：http://qfl.c1oappe.top

Java: String.join(",", items)
来源：http://rkb.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://spn.gaohongyu789.top

Ruby: items.join(",")
来源：http://ync.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://dnr.shzxlz.cn

[E09] 去除所有空白字符
来源：http://lhv.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://luo.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exa.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://ekz.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://xhr.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://bwr.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://usb.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nbm.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zaa.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://yqn.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://flv.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sku.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://ulm.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://ytq.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://kvp.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://blu.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qhx.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://buk.9152youxi.cn

[E11] 反转字符串
来源：http://xhy.yfazqb.com

Py:   s[::-1]
来源：http://mfu.ehwqpu.com

PHP:  strrev($s);
来源：http://nva.tarul.cn

JS:   [...s].reverse().join("")
来源：http://yrr.ivvv.top

TS:   [...s].reverse().join("")
来源：http://imo.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://klb.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tjz.hywenlv.cn

Ruby: s.reverse
来源：http://kkc.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lxt.mhx1999.top

[E12] 统计某字符出现次数
来源：http://whl.iojbl.cn

Py:   s.count("a")
来源：http://sev.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://aqz.shuidangran.top

JS:   s.split("a").length - 1
来源：http://jlo.hammf.cn

TS:   s.split("a").length - 1
来源：http://tqu.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nmm.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://frv.cdnleiting.top

Ruby: s.count("a")
来源：http://dso.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://jko.xylfe.cn

[E13] 逐字符遍历
来源：http://hdm.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://auv.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cvl.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://jaj.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dsj.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://arq.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zdr.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://arb.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yhw.sysykeji.top

[E14] URL 编码与 Base64
来源：http://crb.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mqp.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jvu.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://olk.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://euk.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zjv.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ahv.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ght.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qof.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://gtv.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yxd.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xtx.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ktr.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rlw.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://orr.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tez.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qok.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bsa.jinghuilouyu.cn

[E16] 数字千分位
来源：http://xzv.zycfv.cn

Py:   f"{1234567:,}"
来源：http://vnm.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://nhr.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zfu.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://afu.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ety.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uts.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xuv.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://npv.9152youxi.cn

[E17] 首字母大写
来源：http://xxv.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vno.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wzn.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ytw.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xgc.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fye.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hkh.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://jhq.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qau.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://mfy.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gdf.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vus.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ghp.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://pyr.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ctm.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ooq.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sdf.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wyq.havefunace.top

[E19] 多行文本按行拆分
来源：http://yyk.bbcook.cn

Py:   s.splitlines()
来源：http://sit.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tbh.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://dhn.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://iex.guowangkeji.top

Java: s.lines().toList()
来源：http://mll.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://kxs.cqqwz.cn

Ruby: s.lines
来源：http://gyb.316326.xyz

C#:   s.Split('\n')
来源：http://hga.birdmap.top

[E20] 判断字符串是否为空
来源：http://tcm.vqdsnc.cn

Py:   if not s:
来源：http://pal.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lys.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://axe.yuxming.cn

TS:   if (s === "") {}
来源：http://tjz.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://hjo.guannengcc.top

Go:   if s == "" {}
来源：http://obm.yj20258.top

Ruby: if s.empty?
来源：http://cux.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iix.zdbjq.cn

[E21] 超长截断加省略号
来源：http://wue.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nqo.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://imb.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ozy.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://utc.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cvc.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://jil.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bcd.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://has.shuidangran.top

[E22] 字节长度与字符长度
来源：http://hxf.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://snj.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ocm.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjh.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrf.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ujl.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yuh.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ixf.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://toh.jyoumei.cn

================================================================================
来源：http://tbz.chenzaomai.com

F. 文件与目录
来源：http://wpk.nwbrower.top

================================================================================
来源：http://duh.iojbl.cn

[F01] 读取整个文件
来源：http://vex.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fcd.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://kzr.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kvy.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ggt.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zbh.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xec.nwbrower.top

Ruby: File.read("a.txt")
来源：http://znc.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://ltz.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://xlk.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://atu.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pmj.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://brl.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://agu.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://erp.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ixa.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ueb.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqx.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://wpz.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vfy.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dkt.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://riq.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sdq.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rnu.jianghu66.top


<!-- 参考信息 -->