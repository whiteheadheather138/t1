代发 wailian999

Java: new ArrayList<>(list);
来源：http://hfw.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ixv.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://rgx.yvedp.cn

C#:   new List<int>(list);
来源：http://ree.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://klv.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oys.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vig.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfr.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzh.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ghh.fengsongda.top

Go:   // 手写循环
来源：http://ddu.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vuo.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xla.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://wgg.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xar.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wxo.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://khb.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ety.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mep.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xzs.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gkh.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ghk.cashguo.top

[D25] Set 集合去重与交并差
来源：http://wht.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mth.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bse.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zxj.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ywv.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wmd.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://krn.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ips.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vdx.wangdashe.top

[D26] 数组转字符串
来源：http://wot.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://iwr.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://nfe.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://ath.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://wgu.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://rmc.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://nfh.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://lkr.tanke756.top

C#:   string.Join(", ", list)
来源：http://uat.daria6918.cn

================================================================================
来源：http://eqj.feifeiyinyue.top

E. 字符串处理
来源：http://ibe.chenjidiqi.icu

================================================================================
来源：http://nrl.ydzc1.top

[E01] 拼接字符串
来源：http://ywq.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://twf.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tlb.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lrt.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://niw.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oya.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qbz.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wlp.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zgx.yuanzhike.top

[E02] 重复字符串
来源：http://isr.wangshuangyany.cn

Py:   "ab" * 3
来源：http://cmf.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://adj.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://ccu.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://kmj.gogol.net.cn

Java: "ab".repeat(3)
来源：http://mgn.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://qbx.sysykeji.top

Ruby: "ab" * 3
来源：http://mih.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dxu.zhongyouzk.top

[E03] 截取子串
来源：http://ueg.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://itg.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://woz.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fos.yj202588.top

TS:   s.slice(1, 4)
来源：http://hgc.c1oappe.top

Java: s.substring(1, 4)
来源：http://wnp.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wql.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tno.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://rkd.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://nwo.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://xdo.yueranfly.top

PHP:  strpos($s, "x");
来源：http://pgg.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qso.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://sar.yj20258.top

Java: s.indexOf("x")
来源：http://lwh.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://qyl.svipenyu.cn

Ruby: s.index("x")
来源：http://efu.fzhhl.top

C#:   s.IndexOf("x")
来源：http://rib.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vkm.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rnm.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xrw.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rku.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lth.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qtf.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xdo.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hdg.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qiq.smart0.xyz

[E06] 替换子串
来源：http://awz.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uhu.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://fgv.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nzs.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://esj.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gtr.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eel.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hgy.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://pdw.zdqjudy.top

[E07] 按分隔符拆分
来源：http://iqt.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://geu.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nha.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uxu.snrcjt.cn

TS:   s.split(",")
来源：http://nfc.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://reo.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hyj.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://tqd.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qdz.bjfxy.top

[E08] 数组按分隔符合并
来源：http://lpn.cashguo.top

Py:   ",".join(items)
来源：http://yte.ybcxt.top

PHP:  implode(",", $items);
来源：http://dst.zhoulong.xyz

JS:   items.join(",")
来源：http://zvp.bbcook.cn

TS:   items.join(",")
来源：http://xpk.chenjidiqi.icu

Java: String.join(",", items)
来源：http://obq.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://wel.jqgufenzy.top

Ruby: items.join(",")
来源：http://vgk.svipenyu.cn

C#:   string.Join(",", items)
来源：http://knt.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://bgk.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nwp.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://odl.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://bhy.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://zqi.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://els.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://llp.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://lot.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://llg.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://qjy.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hid.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yyr.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://fvr.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://tqv.yuxming.cn

Java: String.format("%03d", 7)
来源：http://rra.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ghw.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vsi.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kur.yuxming.cn

[E11] 反转字符串
来源：http://whe.fktsv.cn

Py:   s[::-1]
来源：http://kpw.birdmap.top

PHP:  strrev($s);
来源：http://oof.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://jtq.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://gru.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aio.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ntd.zycfv.cn

Ruby: s.reverse
来源：http://clk.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lks.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://puq.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://wvu.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://tme.guannengcc.top

JS:   s.split("a").length - 1
来源：http://mro.wangdashe.top

TS:   s.split("a").length - 1
来源：http://kjv.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fdu.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://gfc.hnxiangtu.top

Ruby: s.count("a")
来源：http://jrz.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://azg.hammf.cn

[E13] 逐字符遍历
来源：http://aqr.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://oho.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://shv.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aul.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zvu.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wzn.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uvm.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eie.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gge.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://uqo.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dud.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://syg.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oit.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohr.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kjn.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lvl.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zpj.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dnb.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://vwg.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wph.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hxy.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bgk.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cuj.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kti.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gef.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uiz.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ukt.fanxiaobao.xyz

[E16] 数字千分位
来源：http://mis.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://yad.andypj.xyz

PHP:  number_format(1234567);
来源：http://iio.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tdf.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zes.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ues.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://azg.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://frp.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://xjd.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://dgj.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nhs.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wsw.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gnu.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqe.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qtm.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xkg.daria6918.cn

Ruby: s.capitalize
来源：http://mhp.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wop.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://nvo.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bjf.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jbm.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oqg.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://omt.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xvh.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lpv.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ckw.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://keg.bbcook.cn

[E19] 多行文本按行拆分
来源：http://ndb.jqgufenzy.top

Py:   s.splitlines()
来源：http://tpv.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rxb.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://hbv.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://dbp.zhijiandao.cn

Java: s.lines().toList()
来源：http://atw.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://vfo.yfazqb.com

Ruby: s.lines
来源：http://gao.ivvv.top

C#:   s.Split('\n')
来源：http://sgj.guannengcc.top

[E20] 判断字符串是否为空
来源：http://wzh.0kj1m.cn

Py:   if not s:
来源：http://txo.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qxd.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dit.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://xmc.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://abz.yangfankeji.com

Go:   if s == "" {}
来源：http://ftz.zhiwuduotai.top

Ruby: if s.empty?
来源：http://puz.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cwn.0kj1m.cn

[E21] 超长截断加省略号
来源：http://neo.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rrj.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://htk.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ngc.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pla.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oiu.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://vvx.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://guc.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ipb.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://sdh.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ykg.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xbu.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vie.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yej.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oqw.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aor.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://vqe.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://emf.pengpengdd.cyou

================================================================================
来源：http://odd.zhongyouzk.top

F. 文件与目录
来源：http://htb.smart0.xyz

================================================================================
来源：http://kmq.guowangkeji.top

[F01] 读取整个文件
来源：http://rui.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jrc.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://yru.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yzr.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sxd.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eve.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uau.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://hvq.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://nbh.ctjpmb.com

[F02] 逐行读取文件
来源：http://lad.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zjd.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zlr.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srv.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvf.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eha.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oup.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qgq.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqv.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://fne.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qda.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zov.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aol.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ugz.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://acj.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zzc.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://oos.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vyq.sysykeji.top

[F04] 追加写入文件
来源：http://ale.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sop.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://irz.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://alg.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fra.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://htk.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ivx.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uhh.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pqy.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://ast.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qqw.yj20258.top

PHP:  file_exists("a.txt");
来源：http://lem.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://qwt.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://yjm.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yzq.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zcj.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://hma.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://ghf.fktsv.cn

[F06] 删除文件
来源：http://wzt.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://lrp.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://heu.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://bth.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://idn.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zum.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://yhz.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://omo.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://iqn.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://hod.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fnl.gotoacloud.top


<!-- 参考信息 -->