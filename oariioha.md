代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ctu.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rxm.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ilk.zycfv.cn

TS:   [...arr];
来源：http://mnn.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://wyd.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://ivu.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://tow.aizwys.cn

C#:   new List<int>(list);
来源：http://zee.jinqigfzy.top

[D23] reduce 累积计算
来源：http://xfe.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nyd.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xxu.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfo.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjy.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gpy.c1oappe.top

Go:   // 手写循环
来源：http://mvj.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://trx.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nsl.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://zya.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bub.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lmk.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iqk.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://epo.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ugb.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wgq.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rbs.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lzs.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://rfk.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fhi.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sfr.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ylq.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://niz.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jjl.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rea.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyc.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ndn.cucudq.cn

[D26] 数组转字符串
来源：http://rmp.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://dqc.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://mbe.svipenyu.cn

JS:   arr.join(", ")
来源：http://ffg.birdmap.top

TS:   arr.join(", ")
来源：http://xhx.andypj.xyz

Java: String.join(", ", list)
来源：http://isw.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://uof.fengsongda.top

Ruby: arr.join(", ")
来源：http://mbr.hesvh.cn

C#:   string.Join(", ", list)
来源：http://jaq.yongpay.top

================================================================================
来源：http://bog.xinyue.icu

E. 字符串处理
来源：http://xgb.pycfn.com

================================================================================
来源：http://phu.aizwys.cn

[E01] 拼接字符串
来源：http://vbs.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jxu.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rar.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ezi.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://elm.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hjz.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yld.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lgg.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qoz.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://psd.feifeiyinyue.top

Py:   "ab" * 3
来源：http://bnv.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://jyp.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://zuz.hcnkem.com

TS:   "ab".repeat(3)
来源：http://tuc.yj202588.top

Java: "ab".repeat(3)
来源：http://yzi.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://zkn.yfazqb.com

Ruby: "ab" * 3
来源：http://fgi.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zsu.guannengcc.top

[E03] 截取子串
来源：http://kwz.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xzm.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bcx.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cst.jianghu66.top

TS:   s.slice(1, 4)
来源：http://ghn.ybcxt.top

Java: s.substring(1, 4)
来源：http://jpo.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hum.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fxi.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://ceq.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://ola.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://txf.guannengcc.top

PHP:  strpos($s, "x");
来源：http://iqa.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xfx.mhx1999.top

TS:   s.indexOf("x")
来源：http://tsy.xziqi.cn

Java: s.indexOf("x")
来源：http://tck.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://vgh.nwbrower.top

Ruby: s.index("x")
来源：http://mln.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://nvs.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dhp.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gdi.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sch.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uuc.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jqh.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gco.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iia.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://czd.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wfz.fktsv.cn

[E06] 替换子串
来源：http://ruv.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dnp.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://kot.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqr.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://zjt.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://koe.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hzx.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rgt.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://pjv.jinqigufen.top

[E07] 按分隔符拆分
来源：http://hdk.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pxd.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eoq.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xgz.shanyushiyangtech.top

TS:   s.split(",")
来源：http://mvm.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://hcx.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bka.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://rpp.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vjx.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://ybm.sweek.top

Py:   ",".join(items)
来源：http://rme.yj20258888.top

PHP:  implode(",", $items);
来源：http://xbj.9152youxi.cn

JS:   items.join(",")
来源：http://vcz.cheryme.top

TS:   items.join(",")
来源：http://ehn.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://xti.meibo888.top

Go:   strings.Join(items, ",")
来源：http://pkv.yj202588.top

Ruby: items.join(",")
来源：http://kkg.zhijiandao.cn

C#:   string.Join(",", items)
来源：http://oci.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://wau.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wue.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tgy.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://ari.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://obo.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://rsb.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zei.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ygu.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zom.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://nje.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eqa.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nsg.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://qgf.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://ghy.yfazqb.com

Java: String.format("%03d", 7)
来源：http://rcb.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pci.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sla.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gxt.jianghu66.top

[E11] 反转字符串
来源：http://jse.sufxvd.cn

Py:   s[::-1]
来源：http://ppm.cucudq.cn

PHP:  strrev($s);
来源：http://kyp.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://asx.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://fjx.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pcg.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qcg.bbcook.cn

Ruby: s.reverse
来源：http://okl.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://kfe.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://lap.fktsv.cn

Py:   s.count("a")
来源：http://qsy.cheryme.top

PHP:  substr_count($s, "a");
来源：http://qwz.daxiang520.top

JS:   s.split("a").length - 1
来源：http://uii.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://bxv.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hls.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://jxl.xylfe.cn

Ruby: s.count("a")
来源：http://mtv.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://ssf.xinyue.icu

[E13] 逐字符遍历
来源：http://ctu.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://lwf.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://age.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kul.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dsy.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kwa.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ezw.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ivu.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bqy.uphjek.com

[E14] URL 编码与 Base64
来源：http://irz.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhj.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jfv.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yyi.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dho.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kli.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tfp.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hca.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jmi.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://mpz.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gpy.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uxc.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ckr.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mej.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dix.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ddz.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cuo.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vbt.guannengcc.top

[E16] 数字千分位
来源：http://hfz.hesvh.cn

Py:   f"{1234567:,}"
来源：http://dxv.xuanzx.com

PHP:  number_format(1234567);
来源：http://drc.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zmr.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vcb.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eta.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://csl.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fgl.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://zek.zdqjudy.top

[E17] 首字母大写
来源：http://vjs.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://koj.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jkx.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvg.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ecb.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ffo.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fhk.zhixingplan.top

Ruby: s.capitalize
来源：http://kjs.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ocu.fzhhl.top

[E18] 模板占位符替换
来源：http://fhv.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jsd.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wow.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://efx.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://epk.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pzm.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpg.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rll.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jem.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://ohs.hammf.cn

Py:   s.splitlines()
来源：http://cmk.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwb.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://bif.sweek.top

TS:   s.split(/\r?\n/)
来源：http://pse.bbcook.cn

Java: s.lines().toList()
来源：http://mia.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://pnu.feifeiyinyue.top

Ruby: s.lines
来源：http://erm.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://vdl.yueranfly.top

[E20] 判断字符串是否为空
来源：http://qzj.bbcook.cn

Py:   if not s:
来源：http://ipo.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://veh.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qbo.smart0.xyz

TS:   if (s === "") {}
来源：http://fmq.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://abd.0kj1m.cn

Go:   if s == "" {}
来源：http://dwi.vehdjk.com

Ruby: if s.empty?
来源：http://ajx.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://scf.hnqzz.top

[E21] 超长截断加省略号
来源：http://jts.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bdp.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://exg.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gws.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gae.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fmo.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://ufp.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ryv.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yjl.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://ayd.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yns.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmz.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jun.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pjp.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uda.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vay.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://ddr.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqj.ehwqpu.com

================================================================================
来源：http://pih.cucudq.cn

F. 文件与目录
来源：http://fsk.quarkkingdee.top

================================================================================
来源：http://xpd.iojbl.cn

[F01] 读取整个文件
来源：http://vqs.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dbq.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://vlc.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://svj.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ewc.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mrw.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fcz.yj20258888.top

Ruby: File.read("a.txt")
来源：http://waz.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://tfw.yfazqb.com

[F02] 逐行读取文件
来源：http://hsj.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://llv.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xmf.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ghp.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ynn.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dwp.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bca.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cfv.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rnu.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://frv.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oyp.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://uzi.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://evk.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xwr.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cvr.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nrs.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://cgm.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yzs.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://dcd.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://twz.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ovv.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hav.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjz.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zgh.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tjh.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wuk.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mfr.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://kgm.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lck.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://lls.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://nfd.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://pfe.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nca.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ljd.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://mgp.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://usl.zhongyouzk.top

[F06] 删除文件
来源：http://kbj.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://icg.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://dmd.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://fsq.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://ukt.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jeb.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://irl.guowangkeji.top


<!-- 参考信息 -->