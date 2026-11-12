代发 wailian999

Java: new ArrayList<>(list);
来源：http://uxo.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bku.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://umu.dashuyun.cn

C#:   new List<int>(list);
来源：http://sqo.kuanghao11.cn

[D23] reduce 累积计算
来源：http://nii.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://udw.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ekp.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqd.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ser.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ybp.9152youxi.cn

Go:   // 手写循环
来源：http://sgt.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eib.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tcc.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://roj.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bxz.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kre.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vgd.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qom.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://boa.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gmt.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bng.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jox.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://yig.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mrg.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nqy.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jtx.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pst.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ajb.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xtv.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://plo.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uih.jinqigufen.top

[D26] 数组转字符串
来源：http://dkd.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://ahm.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://vyo.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://kif.svipenyu.cn

TS:   arr.join(", ")
来源：http://ief.xuanzx.com

Java: String.join(", ", list)
来源：http://bpg.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://fzs.jiagoushi.top

Ruby: arr.join(", ")
来源：http://ebk.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://wzk.daria6918.cn

================================================================================
来源：http://nhj.xuetiantiany.cn

E. 字符串处理
来源：http://jas.hywenlv.cn

================================================================================
来源：http://htx.jqgufenzy.top

[E01] 拼接字符串
来源：http://snp.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hpo.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://llh.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jka.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sny.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yie.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://olu.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ntd.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://haa.guowangkeji.top

[E02] 重复字符串
来源：http://uew.shangyingyoupin.top

Py:   "ab" * 3
来源：http://uti.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://pdm.tarul.cn

JS:   "ab".repeat(3)
来源：http://dbu.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://vwl.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://wgl.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rhl.iojbl.cn

Ruby: "ab" * 3
来源：http://dzg.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zur.yonumen.top

[E03] 截取子串
来源：http://ezz.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uao.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vif.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fxc.mhx1999.top

TS:   s.slice(1, 4)
来源：http://wve.svipenyu.cn

Java: s.substring(1, 4)
来源：http://bms.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uvs.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kvp.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://cib.zdbjq.cn

[E04] 查找子串位置
来源：http://czc.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://vaz.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://err.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://stp.cheryme.top

TS:   s.indexOf("x")
来源：http://zkt.hnxiangtu.top

Java: s.indexOf("x")
来源：http://evn.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://duk.tianlin.xyz

Ruby: s.index("x")
来源：http://pxu.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://gvu.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://azj.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uky.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fqg.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fiq.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mux.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rro.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rva.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ner.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zrb.cashguo.top

[E06] 替换子串
来源：http://epy.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ict.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://mjp.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mrw.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://iuy.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qyo.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hsj.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jlr.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://hpy.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://mtj.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oss.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wig.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://txr.birdmap.top

TS:   s.split(",")
来源：http://xzh.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://nwq.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rww.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://yeg.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jnz.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://iwb.mhx1999.top

Py:   ",".join(items)
来源：http://pcr.wangdashe.top

PHP:  implode(",", $items);
来源：http://zos.jianghu66.top

JS:   items.join(",")
来源：http://zft.guannengcc.top

TS:   items.join(",")
来源：http://qhu.shuidangran.top

Java: String.join(",", items)
来源：http://tun.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://ike.chenzaomai.com

Ruby: items.join(",")
来源：http://zml.fengsongda.top

C#:   string.Join(",", items)
来源：http://omw.zhengqikj.top

[E09] 去除所有空白字符
来源：http://skl.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ynn.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpe.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://uro.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://kbx.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://liw.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xox.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://sgp.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uwj.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://tjq.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://org.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uoo.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://yao.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://crs.yj20258888.top

Java: String.format("%03d", 7)
来源：http://hxv.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wxk.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xlv.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xgq.jinghuilouyu.cn

[E11] 反转字符串
来源：http://jhl.epnwcf.com

Py:   s[::-1]
来源：http://dab.ehwqpu.com

PHP:  strrev($s);
来源：http://ljl.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://qeb.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://khi.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ycu.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fzl.pycfn.com

Ruby: s.reverse
来源：http://lkf.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://tcd.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://pzo.zdbjq.cn

Py:   s.count("a")
来源：http://xbn.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://myi.uphjek.com

JS:   s.split("a").length - 1
来源：http://ign.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://fuc.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fho.ivvv.top

Go:   strings.Count(s, "a")
来源：http://kku.ydzc1.top

Ruby: s.count("a")
来源：http://hes.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://mgi.sjlbkw.cn

[E13] 逐字符遍历
来源：http://phl.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://bfi.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cti.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kpr.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zol.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gcb.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oou.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tmr.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uxc.meibo888.top

[E14] URL 编码与 Base64
来源：http://ixa.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hud.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://yma.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oml.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ity.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ipr.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kvg.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yec.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://edh.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://rgv.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://roe.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nhi.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tud.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zdy.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pii.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sfk.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://clt.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lwz.c1oappe.top

[E16] 数字千分位
来源：http://nyu.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://qnj.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://rgd.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ynr.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jph.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tjv.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gkn.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ogn.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://gbt.mhx1999.top

[E17] 首字母大写
来源：http://ntv.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uft.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hmt.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nmi.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpk.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ppf.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kid.jianghu66.top

Ruby: s.capitalize
来源：http://tqf.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zxg.zhongyouzk.top

[E18] 模板占位符替换
来源：http://ukm.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rlb.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://feu.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://awp.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nuc.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jen.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vka.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://doz.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://srf.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://xfi.yueranfly.top

Py:   s.splitlines()
来源：http://wkr.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ikb.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://vja.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://ygo.gzhubu.top

Java: s.lines().toList()
来源：http://bxd.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://nva.bjfxy.top

Ruby: s.lines
来源：http://nhd.hammf.cn

C#:   s.Split('\n')
来源：http://pij.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://neg.guowangkeji.top

Py:   if not s:
来源：http://yky.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rhh.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://poa.tarul.cn

TS:   if (s === "") {}
来源：http://pjw.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://zpd.xinyue.icu

Go:   if s == "" {}
来源：http://saw.epnwcf.com

Ruby: if s.empty?
来源：http://oeb.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fqa.c1oappe.top

[E21] 超长截断加省略号
来源：http://wpa.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ibj.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lyt.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uss.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cob.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uoe.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://szf.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vij.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zbb.daxiang520.top

[E22] 字节长度与字符长度
来源：http://dgk.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jml.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qut.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oey.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ogc.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fzo.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hhc.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://khm.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xab.cucudq.cn

================================================================================
来源：http://uxs.zhoulong.xyz

F. 文件与目录
来源：http://pbp.yonumen.top

================================================================================
来源：http://aok.xuetiantiany.cn

[F01] 读取整个文件
来源：http://umc.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hoe.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://iqq.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://per.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvt.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gqw.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pyw.iojbl.cn

Ruby: File.read("a.txt")
来源：http://opy.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://rnq.andypj.xyz

[F02] 逐行读取文件
来源：http://bvr.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sbz.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://maz.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqx.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kbl.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fmp.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zyh.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wwk.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbf.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://oys.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ntk.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oxh.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zmp.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oyt.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zam.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tpt.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://ekx.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ous.snrcjt.cn

[F04] 追加写入文件
来源：http://zky.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pdt.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mrj.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dck.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zqb.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://klu.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://neb.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uuc.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jkv.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://sfo.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wqu.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://mix.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://goh.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://tfa.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rqp.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vav.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://opy.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://gnf.ivvv.top

[F06] 删除文件
来源：http://bwk.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://pek.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://uwz.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://fxp.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://khh.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://owj.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://ciw.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://vgc.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://jbf.yvedp.cn

[F07] 创建目录（含多级）
来源：http://loj.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://apk.ydzc1.top


<!-- 参考信息 -->