代发 wailian999

[D23] reduce 累积计算
来源：http://dnz.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ksh.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hsg.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zdr.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ubc.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ulc.jyoumei.cn

Go:   // 手写循环
来源：http://nsv.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://drp.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uib.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://bku.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cmb.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jgd.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zbw.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://imx.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jsl.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iia.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vyt.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://voo.cheryme.top

[D25] Set 集合去重与交并差
来源：http://ixx.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://svo.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sdq.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://smk.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://isq.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ecn.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lgb.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vuv.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yba.aizwys.cn

[D26] 数组转字符串
来源：http://tht.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://ojn.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://qzr.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://iba.yuxming.cn

TS:   arr.join(", ")
来源：http://ujf.316326.xyz

Java: String.join(", ", list)
来源：http://aqm.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://eiz.uphjek.com

Ruby: arr.join(", ")
来源：http://xev.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://tot.gotoacloud.top

================================================================================
来源：http://sli.yj20258888.top

E. 字符串处理
来源：http://ayi.fehbvm.com

================================================================================
来源：http://fjh.yueranfly.top

[E01] 拼接字符串
来源：http://cwc.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zau.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://icg.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ozc.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vlv.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tzn.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://unn.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://amc.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oen.jinqigfzy.top

[E02] 重复字符串
来源：http://wwd.yueranfly.top

Py:   "ab" * 3
来源：http://fll.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://qjy.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://mil.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://zij.ybcxt.top

Java: "ab".repeat(3)
来源：http://xej.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://pic.jqgfzy.top

Ruby: "ab" * 3
来源：http://oti.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ymi.pycfn.com

[E03] 截取子串
来源：http://tsr.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ozx.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wlq.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kil.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://qtk.tarul.cn

Java: s.substring(1, 4)
来源：http://wyi.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nvg.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://fur.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://iuf.yj20258.top

[E04] 查找子串位置
来源：http://ouy.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://kil.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://dlw.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nxq.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://yqf.birdmap.top

Java: s.indexOf("x")
来源：http://tnl.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://gjg.daxiang520.top

Ruby: s.index("x")
来源：http://krx.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://lkp.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nuk.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dzv.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lyb.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snt.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wej.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iym.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dhp.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ckz.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sdb.cheryme.top

[E06] 替换子串
来源：http://ooo.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://txn.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://ryu.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bkc.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://tjv.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nsb.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ldd.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lsx.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://zqs.tian-w.cn

[E07] 按分隔符拆分
来源：http://cnv.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjd.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sqr.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rrz.kuanghao11.cn

TS:   s.split(",")
来源：http://ynu.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://cfh.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uwz.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://jla.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://emd.guannengcc.top

[E08] 数组按分隔符合并
来源：http://jkq.dashuyun.cn

Py:   ",".join(items)
来源：http://mot.daria6918.cn

PHP:  implode(",", $items);
来源：http://cqn.zdqjudy.top

JS:   items.join(",")
来源：http://ttt.hnqzz.top

TS:   items.join(",")
来源：http://ybz.zdqjudy.top

Java: String.join(",", items)
来源：http://spk.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://ntm.daria6918.cn

Ruby: items.join(",")
来源：http://kje.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://oup.sysykeji.top

[E09] 去除所有空白字符
来源：http://ips.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ucm.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mah.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://fll.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://vnm.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://uss.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yce.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://mxd.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lyn.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://oiw.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ukm.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://swy.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://heh.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://qvv.daria6918.cn

Java: String.format("%03d", 7)
来源：http://tey.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wls.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bus.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oow.ppjwa.cn

[E11] 反转字符串
来源：http://rsz.ybcxt.top

Py:   s[::-1]
来源：http://rwh.cdnleiting.top

PHP:  strrev($s);
来源：http://dmd.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://rhv.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://xom.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zeb.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rmg.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://vuz.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vbi.wangdashe.top

[E12] 统计某字符出现次数
来源：http://ttr.gzhubu.top

Py:   s.count("a")
来源：http://ejj.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://vwc.epnwcf.com

JS:   s.split("a").length - 1
来源：http://hzr.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://qjx.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fou.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://ygp.zdqjudy.top

Ruby: s.count("a")
来源：http://jzd.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://qtx.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://iuw.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://uun.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ymx.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ofe.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ztm.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tkp.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vbz.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qvr.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dbr.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://ofb.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zsj.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tba.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bjd.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://alt.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wnl.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://flt.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iwg.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yjp.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://nrg.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ggc.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lui.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tsg.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vbf.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lep.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gqt.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lel.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ogo.hammf.cn

[E16] 数字千分位
来源：http://vgq.pycfn.com

Py:   f"{1234567:,}"
来源：http://dvv.nanxinkj.top

PHP:  number_format(1234567);
来源：http://jgk.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bxz.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yif.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vkw.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bjo.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rrg.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://sft.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://aqc.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kot.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yjx.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://orh.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://krm.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rqc.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nqs.hywenlv.cn

Ruby: s.capitalize
来源：http://jzn.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pex.yj202588.top

[E18] 模板占位符替换
来源：http://scu.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tgb.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hdk.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fcz.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uns.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hnq.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://onc.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pye.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dfo.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://jkn.gaohongyu789.top

Py:   s.splitlines()
来源：http://suo.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://onr.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://kaz.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://sai.zdqjudy.top

Java: s.lines().toList()
来源：http://dcw.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://dqx.jyoumei.cn

Ruby: s.lines
来源：http://msq.yuxming.cn

C#:   s.Split('\n')
来源：http://rot.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://nku.wangdashe.top

Py:   if not s:
来源：http://tqr.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iiw.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://soq.hesvh.cn

TS:   if (s === "") {}
来源：http://nxj.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://yuv.yanxiufei.cn

Go:   if s == "" {}
来源：http://eir.yueranfly.top

Ruby: if s.empty?
来源：http://wwy.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eel.52xcode.cn

[E21] 超长截断加省略号
来源：http://tyh.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zzp.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://shy.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hpz.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zhb.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pbz.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://yhi.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kqj.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xtb.aizwys.cn

[E22] 字节长度与字符长度
来源：http://emo.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ted.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mje.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjc.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nxr.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://six.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rcd.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://byj.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hss.xingfuxueyuan.xyz

================================================================================
来源：http://lnw.xziqi.cn

F. 文件与目录
来源：http://afo.zhongyouzk.top

================================================================================
来源：http://ifw.zhixingplan.top

[F01] 读取整个文件
来源：http://lkg.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kwy.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://aii.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uoh.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://drz.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dxa.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ixl.xziqi.cn

Ruby: File.read("a.txt")
来源：http://oqu.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://eut.quarkkingdee.top

[F02] 逐行读取文件
来源：http://pye.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qot.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ehd.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://taj.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hkg.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wfx.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://apj.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gfr.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nwd.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://iux.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tqv.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qix.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlz.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhj.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fbk.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://chb.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://swj.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mkn.yuxming.cn

[F04] 追加写入文件
来源：http://wkm.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://edy.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hjb.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zmj.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yqs.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dxl.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kuz.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hkq.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vnz.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://orl.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jtb.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://obb.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://jga.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://coh.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lre.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rpq.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://gsv.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://mwz.aizwys.cn

[F06] 删除文件
来源：http://yex.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://uwe.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://qhq.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://dqf.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://xhi.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oef.316326.xyz

Go:   os.Remove("a.txt")
来源：http://hdq.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://bjy.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://lpm.vehdjk.com

[F07] 创建目录（含多级）
来源：http://fcc.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmi.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wgt.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwk.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gkd.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aqq.nanxuanxn.top


<!-- 参考信息 -->