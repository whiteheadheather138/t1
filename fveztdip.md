代发 wailian999

Java: new ArrayList<>(list);
来源：http://onj.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://yjm.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://zsw.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://vti.daria6918.cn

[D23] reduce 累积计算
来源：http://pku.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://meg.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xhy.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkv.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ehc.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ktd.tian-w.cn

Go:   // 手写循环
来源：http://iwa.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hls.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xxc.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://igf.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hki.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rbd.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gds.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lzh.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://men.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://swa.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zyz.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yoy.chenlongwang.top

[D25] Set 集合去重与交并差
来源：http://zds.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://brc.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jgx.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://flg.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gwu.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ucn.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zem.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mda.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rqi.nanxuanxn.top

[D26] 数组转字符串
来源：http://qgn.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://tqw.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://pvz.nanxuanxn.top

JS:   arr.join(", ")
来源：http://ryg.tanke756.top

TS:   arr.join(", ")
来源：http://ema.ydzc1.top

Java: String.join(", ", list)
来源：http://qwn.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://aua.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://iia.ydzc1.top

C#:   string.Join(", ", list)
来源：http://nob.yuxming.cn

================================================================================
来源：http://xbu.shanyushiyangtech.top

E. 字符串处理
来源：http://fqk.gotoacloud.top

================================================================================
来源：http://gwx.316326.xyz

[E01] 拼接字符串
来源：http://wiv.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zrx.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zzl.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://luk.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuy.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lre.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jxo.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://szs.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hdl.jiagoushi.top

[E02] 重复字符串
来源：http://ywg.guowangkeji.top

Py:   "ab" * 3
来源：http://akd.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://huq.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://skn.yvedp.cn

TS:   "ab".repeat(3)
来源：http://euo.0kj1m.cn

Java: "ab".repeat(3)
来源：http://rgq.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://wqm.ybcxt.top

Ruby: "ab" * 3
来源：http://rfn.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lxn.tianlin.xyz

[E03] 截取子串
来源：http://xvw.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ipp.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gmp.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dna.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://xje.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://ywp.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rfp.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://eji.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://wwf.hfpthk.cn

[E04] 查找子串位置
来源：http://lnd.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://uvt.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://icy.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ujf.tianlin.xyz

TS:   s.indexOf("x")
来源：http://pgu.316326.xyz

Java: s.indexOf("x")
来源：http://qww.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://jhd.ydjk.org.cn

Ruby: s.index("x")
来源：http://usw.pycfn.com

C#:   s.IndexOf("x")
来源：http://eto.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hkf.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txz.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://avc.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mco.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://vtj.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygd.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cyd.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vjw.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vyn.c1oappe.top

[E06] 替换子串
来源：http://lrb.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ffz.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://otc.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pdx.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://aor.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lnw.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kcp.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hud.tanke756.top

C#:   s.Replace("a", "b")
来源：http://qyd.jqgfzy.top

[E07] 按分隔符拆分
来源：http://fdf.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nyb.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fwg.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwi.yangfankeji.com

TS:   s.split(",")
来源：http://dxi.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nwg.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jty.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://fmb.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rsf.tanke756.top

[E08] 数组按分隔符合并
来源：http://gxv.jinqigufen.top

Py:   ",".join(items)
来源：http://nxx.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://ztl.hammf.cn

JS:   items.join(",")
来源：http://dde.nanxinkj.top

TS:   items.join(",")
来源：http://zpl.fengsongda.top

Java: String.join(",", items)
来源：http://wrc.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://nsj.xziqi.cn

Ruby: items.join(",")
来源：http://xuo.jianghu66.top

C#:   string.Join(",", items)
来源：http://jdq.ehwqpu.com

[E09] 去除所有空白字符
来源：http://kyr.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fps.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://skn.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://qjq.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://qsq.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://jot.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vvd.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://cyb.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gza.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://uuo.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mfv.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kwe.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://mnh.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://nml.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://nlf.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mlm.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hsd.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wsf.zhixingplan.top

[E11] 反转字符串
来源：http://ntc.yfazqb.com

Py:   s[::-1]
来源：http://bbv.xziqi.cn

PHP:  strrev($s);
来源：http://sft.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://wuf.cheryme.top

TS:   [...s].reverse().join("")
来源：http://fll.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hpk.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://pvi.sufxvd.cn

Ruby: s.reverse
来源：http://jfm.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://mim.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://crb.shuidangran.top

Py:   s.count("a")
来源：http://tiw.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://wxi.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://sgc.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://lyf.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://llo.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://vrb.hfpthk.cn

Ruby: s.count("a")
来源：http://eru.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://zzk.cdnleiting.top

[E13] 逐字符遍历
来源：http://yfc.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://phy.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qcd.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mtg.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fpn.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nkc.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mri.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cma.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wws.yvedp.cn

[E14] URL 编码与 Base64
来源：http://lzi.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eno.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://tvm.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gxq.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mfq.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xwb.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://znf.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ive.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rzl.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://xfk.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xwd.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://req.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tim.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xto.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rok.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bys.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dvz.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpq.birdmap.top

[E16] 数字千分位
来源：http://rqg.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://wyi.c1oappe.top

PHP:  number_format(1234567);
来源：http://ods.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hbp.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pei.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqk.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rhl.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hml.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://hew.hesvh.cn

[E17] 首字母大写
来源：http://tai.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sme.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vme.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://amn.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aeb.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kjn.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pca.c1oappe.top

Ruby: s.capitalize
来源：http://prb.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cmi.xylfe.cn

[E18] 模板占位符替换
来源：http://llm.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggn.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rrk.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bas.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nfo.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://omh.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fds.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hzm.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dpo.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://bra.nanxuanxn.top

Py:   s.splitlines()
来源：http://ikr.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qlt.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://jug.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://rsu.gaohongyu789.top

Java: s.lines().toList()
来源：http://lli.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://ghn.hongshengwenyu.top

Ruby: s.lines
来源：http://efl.ppjwa.cn

C#:   s.Split('\n')
来源：http://gsp.yj20258888.top

[E20] 判断字符串是否为空
来源：http://lnn.sjlbkw.cn

Py:   if not s:
来源：http://ucv.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xwk.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xbm.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://ghv.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://mta.cucudq.cn

Go:   if s == "" {}
来源：http://fso.gotoacloud.top

Ruby: if s.empty?
来源：http://zuk.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jnn.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://itd.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lwp.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bnu.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://trm.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmw.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ron.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://fgz.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zvy.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ixq.daria6918.cn

[E22] 字节长度与字符长度
来源：http://ueb.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zva.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbt.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kst.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrn.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://efs.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mld.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://pvv.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kht.0kj1m.cn

================================================================================
来源：http://lvw.sweek.top

F. 文件与目录
来源：http://fgw.jlsjyb.cn

================================================================================
来源：http://pre.ppjwa.cn

[F01] 读取整个文件
来源：http://ubm.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vfj.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://zox.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fnv.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://erv.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ddi.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lqp.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://fsc.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://nsw.hnxiangtu.top

[F02] 逐行读取文件
来源：http://nvf.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mhq.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sfq.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akr.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbo.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wih.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kgd.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dmj.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://byt.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://ikw.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fcj.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zwk.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lav.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://daf.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vdd.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tqg.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://gwd.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mkq.jinqigfzy.top

[F04] 追加写入文件
来源：http://izt.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lnx.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://col.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://map.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fqe.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nqo.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nxo.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xro.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gnr.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://tkc.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yci.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://sgv.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://xkn.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://iyl.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kjc.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tlv.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://tte.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://ksp.snrcjt.cn

[F06] 删除文件
来源：http://ufn.havefunace.top

Py:   os.remove("a.txt")
来源：http://sze.bjfxy.top

PHP:  unlink("a.txt");
来源：http://min.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://qfd.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hsm.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gzw.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://ajg.cashguo.top

Ruby: File.delete("a.txt")
来源：http://fxx.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://prw.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://ldd.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zji.zhoulong.xyz


<!-- 参考信息 -->