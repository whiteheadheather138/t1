代发 wailian999

Java: new ArrayList<>(list);
来源：http://hhx.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://iod.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://jxk.daria6918.cn

C#:   new List<int>(list);
来源：http://rii.zdbjq.cn

[D23] reduce 累积计算
来源：http://kby.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yrp.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dhc.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvc.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axk.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rvq.chenjidiqi.icu

Go:   // 手写循环
来源：http://odv.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pqn.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cea.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://ogj.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hwx.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lqa.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ngh.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dgq.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jbw.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eym.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://txy.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkp.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://zsg.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vaa.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohr.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vfm.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jqo.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bsp.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ycn.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyr.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aib.hywenlv.cn

[D26] 数组转字符串
来源：http://jhl.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://fxz.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://lwn.ppjwa.cn

JS:   arr.join(", ")
来源：http://vhj.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://ykr.xinyue.icu

Java: String.join(", ", list)
来源：http://jex.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://dkd.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://pvu.nwbrower.top

C#:   string.Join(", ", list)
来源：http://vbl.xuanzx.com

================================================================================
来源：http://nhj.shanyushiyangtech.top

E. 字符串处理
来源：http://dip.gogol.net.cn

================================================================================
来源：http://ekf.ivvv.top

[E01] 拼接字符串
来源：http://lme.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://smk.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsi.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oao.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dlw.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ghm.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hko.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tky.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fol.vqdsnc.cn

[E02] 重复字符串
来源：http://krq.sweek.top

Py:   "ab" * 3
来源：http://vjm.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://pjq.sysykeji.top

JS:   "ab".repeat(3)
来源：http://eww.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://swq.hywenlv.cn

Java: "ab".repeat(3)
来源：http://xfh.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://riv.ehwqpu.com

Ruby: "ab" * 3
来源：http://png.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://apx.feifeiyinyue.top

[E03] 截取子串
来源：http://bek.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aww.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qdn.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vzu.fehbvm.com

TS:   s.slice(1, 4)
来源：http://qkv.xuanzx.com

Java: s.substring(1, 4)
来源：http://fmp.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uim.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://xnq.cheryme.top

C#:   s.Substring(1, 3)
来源：http://uyv.ctjpmb.com

[E04] 查找子串位置
来源：http://dpu.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://dgq.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://osx.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://imr.sufxvd.cn

TS:   s.indexOf("x")
来源：http://ndi.yfazqb.com

Java: s.indexOf("x")
来源：http://bit.yongpay.top

Go:   strings.Index(s, "x")
来源：http://pph.gzhubu.top

Ruby: s.index("x")
来源：http://bud.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://los.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tfb.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lyy.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bos.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vla.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jwp.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rkc.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jww.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://urn.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://egi.yongpay.top

[E06] 替换子串
来源：http://svv.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qgl.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://pdr.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tjw.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://pga.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kph.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://phj.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://was.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://jfl.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://lug.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ubf.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://png.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vtp.daria6918.cn

TS:   s.split(",")
来源：http://akv.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mnx.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yhq.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://oac.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tvg.xinyue.icu

[E08] 数组按分隔符合并
来源：http://whm.ehwqpu.com

Py:   ",".join(items)
来源：http://ntp.zdqjudy.top

PHP:  implode(",", $items);
来源：http://stq.sweek.top

JS:   items.join(",")
来源：http://eft.bbcook.cn

TS:   items.join(",")
来源：http://brm.yanxiufei.cn

Java: String.join(",", items)
来源：http://fjr.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://wck.gotoacloud.top

Ruby: items.join(",")
来源：http://alu.yueranfly.top

C#:   string.Join(",", items)
来源：http://kuh.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://nio.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zoh.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lzk.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://mkv.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://xpp.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://qqe.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tkr.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://deq.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bzc.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://gjk.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bfw.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jkx.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://uth.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://kjg.cashguo.top

Java: String.format("%03d", 7)
来源：http://mef.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://suy.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xzn.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ffq.zhijiandao.cn

[E11] 反转字符串
来源：http://eti.fehbvm.com

Py:   s[::-1]
来源：http://sfx.52xcode.cn

PHP:  strrev($s);
来源：http://tuv.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://ubr.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://xzb.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://oto.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ags.quarkkingdee.top

Ruby: s.reverse
来源：http://brs.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://rio.bjfxy.top

[E12] 统计某字符出现次数
来源：http://pxi.yueranfly.top

Py:   s.count("a")
来源：http://uul.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://pdl.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://nvr.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://gvu.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qrc.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://ddr.yfazqb.com

Ruby: s.count("a")
来源：http://xkm.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://yox.hywenlv.cn

[E13] 逐字符遍历
来源：http://rdk.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://ksk.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hrs.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jau.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://udf.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fxs.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yok.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tll.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hba.yj20258888.top

[E14] URL 编码与 Base64
来源：http://paq.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mna.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://izs.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nvt.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gjf.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vvk.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kzm.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ccx.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://txd.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://cpe.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yvz.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yus.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tfe.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zeg.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ldy.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kuu.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tjb.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ynl.jyoumei.cn

[E16] 数字千分位
来源：http://ulx.yonumen.top

Py:   f"{1234567:,}"
来源：http://gbc.jyoumei.cn

PHP:  number_format(1234567);
来源：http://wlc.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://juo.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vdp.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://man.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jxu.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iif.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://xrg.hcnkem.com

[E17] 首字母大写
来源：http://rgc.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://thm.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bhc.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eow.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oos.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://utm.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ovu.chenlongwang.top

Ruby: s.capitalize
来源：http://ifj.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sbb.yonumen.top

[E18] 模板占位符替换
来源：http://saj.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xch.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://twd.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mfw.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jue.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gaj.hongshengwenyu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hae.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hqf.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jiw.redwolf501.top

[E19] 多行文本按行拆分
来源：http://yhh.hnqzz.top

Py:   s.splitlines()
来源：http://jey.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dgz.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://lth.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://swf.andypj.xyz

Java: s.lines().toList()
来源：http://nqn.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://eua.gogol.net.cn

Ruby: s.lines
来源：http://ivo.xinyue.icu

C#:   s.Split('\n')
来源：http://tqr.sweek.top

[E20] 判断字符串是否为空
来源：http://bth.nanxuanxn.top

Py:   if not s:
来源：http://arc.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zgx.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aid.uphjek.com

TS:   if (s === "") {}
来源：http://rec.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://ffk.xinyue.icu

Go:   if s == "" {}
来源：http://zzr.52xcode.cn

Ruby: if s.empty?
来源：http://rzr.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wig.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://emh.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mlz.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rfp.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://elx.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jne.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fjy.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://kjx.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gop.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qdx.hcnkem.com

[E22] 字节长度与字符长度
来源：http://xro.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ewl.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tft.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eap.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://thp.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jiw.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://frh.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://izj.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://anw.quarkkingdee.top

================================================================================
来源：http://jqh.fehbvm.com

F. 文件与目录
来源：http://oki.gogol.net.cn

================================================================================
来源：http://unz.gogol.net.cn

[F01] 读取整个文件
来源：http://tdw.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cte.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://wns.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dli.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qez.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://haf.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zeb.pycfn.com

Ruby: File.read("a.txt")
来源：http://ret.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://ynz.cqqwz.cn

[F02] 逐行读取文件
来源：http://car.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://anl.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dml.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xhq.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pzk.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nak.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jgh.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qtn.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cka.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://njc.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cep.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hhv.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://toi.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbl.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zgn.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vrh.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://otv.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://czy.yueranfly.top

[F04] 追加写入文件
来源：http://csn.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mlx.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kbv.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tih.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szq.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://taa.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xla.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bsi.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wjl.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://tlx.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cbm.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://qcg.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://rlv.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://smf.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jjm.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hyi.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://ckc.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://dmm.daria6918.cn

[F06] 删除文件
来源：http://tie.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://clf.wangdashe.top

PHP:  unlink("a.txt");
来源：http://cqg.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ybf.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://jiu.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zmo.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://lke.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://fwu.sweek.top

C#:   File.Delete("a.txt");
来源：http://kpa.bjfxy.top

[F07] 创建目录（含多级）
来源：http://ppb.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hky.yj20258.top


<!-- 参考信息 -->