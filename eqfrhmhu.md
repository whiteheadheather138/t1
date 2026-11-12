代发 wailian999

Java: new ArrayList<>(list);
来源：http://wfv.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://omg.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://sug.9152youxi.cn

C#:   new List<int>(list);
来源：http://flu.c1oappe.top

[D23] reduce 累积计算
来源：http://tpc.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gsq.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ihq.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vro.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fwo.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nux.yfazqb.com

Go:   // 手写循环
来源：http://hlw.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mxa.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iak.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://ocn.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pla.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aya.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mqy.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uwo.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oue.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hwk.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kds.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xrm.hammf.cn

[D25] Set 集合去重与交并差
来源：http://ewl.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jbn.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rrj.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://njh.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gca.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pvj.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zix.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ghz.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hjv.cashguo.top

[D26] 数组转字符串
来源：http://eum.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://zjv.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://fzv.tian-w.cn

JS:   arr.join(", ")
来源：http://xem.tanke756.top

TS:   arr.join(", ")
来源：http://uli.dashuyun.cn

Java: String.join(", ", list)
来源：http://diy.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://xbw.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://pkf.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://dot.zhixingplan.top

================================================================================
来源：http://tlx.chenzaomai.com

E. 字符串处理
来源：http://tkh.316326.xyz

================================================================================
来源：http://jex.aizwys.cn

[E01] 拼接字符串
来源：http://cll.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://htu.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xnb.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wwh.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://khw.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qke.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dbf.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sej.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xpv.fzhhl.top

[E02] 重复字符串
来源：http://bhh.jqgfzy.top

Py:   "ab" * 3
来源：http://ohc.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://isg.sxryk.cn

JS:   "ab".repeat(3)
来源：http://swv.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://dij.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://tjn.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://dhi.ydjk.org.cn

Ruby: "ab" * 3
来源：http://fzs.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uke.mhx1999.top

[E03] 截取子串
来源：http://btl.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wvv.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dfo.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rpu.xuanzx.com

TS:   s.slice(1, 4)
来源：http://akk.yongpay.top

Java: s.substring(1, 4)
来源：http://ykq.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jyi.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://huw.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://dyq.fzhhl.top

[E04] 查找子串位置
来源：http://izo.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://vfg.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://upy.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yih.gzhubu.top

TS:   s.indexOf("x")
来源：http://yhn.dashuyun.cn

Java: s.indexOf("x")
来源：http://zcx.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://dhz.bjfxy.top

Ruby: s.index("x")
来源：http://lxa.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://zhs.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lkf.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qxg.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hze.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yft.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gro.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cdx.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pvc.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://luy.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qfl.tarul.cn

[E06] 替换子串
来源：http://wwd.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sud.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://kdh.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gag.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://psg.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agu.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ypc.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iou.yj202588.top

C#:   s.Replace("a", "b")
来源：http://axy.andypj.xyz

[E07] 按分隔符拆分
来源：http://dzw.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iel.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ivv.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ifq.svipenyu.cn

TS:   s.split(",")
来源：http://aqp.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://lwm.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvp.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://blo.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pne.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://ivz.yongpay.top

Py:   ",".join(items)
来源：http://wiu.daxiang520.top

PHP:  implode(",", $items);
来源：http://jmz.yuanzhike.top

JS:   items.join(",")
来源：http://xuo.zhiwuduotai.top

TS:   items.join(",")
来源：http://apw.zhongyouzk.top

Java: String.join(",", items)
来源：http://njd.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://fdd.snrcjt.cn

Ruby: items.join(",")
来源：http://fka.yongpay.top

C#:   string.Join(",", items)
来源：http://pzb.redwolf501.top

[E09] 去除所有空白字符
来源：http://azs.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iyp.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://evq.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://kpn.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://bmk.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://fcu.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://eax.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mml.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hqx.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://nxb.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wtd.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://std.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://ssr.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://rvo.pycfn.com

Java: String.format("%03d", 7)
来源：http://rgb.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://bec.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ajf.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rba.hnqzz.top

[E11] 反转字符串
来源：http://qbc.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://lbg.sweek.top

PHP:  strrev($s);
来源：http://iqe.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://hcz.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://kco.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://xjj.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kba.zhengqikj.top

Ruby: s.reverse
来源：http://gcj.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cec.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://nqs.hammf.cn

Py:   s.count("a")
来源：http://ekh.havefunace.top

PHP:  substr_count($s, "a");
来源：http://kbv.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://zjo.birdmap.top

TS:   s.split("a").length - 1
来源：http://mbi.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://evp.cheryme.top

Go:   strings.Count(s, "a")
来源：http://xcn.jqgfzy.top

Ruby: s.count("a")
来源：http://qym.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://ibw.yj202588.top

[E13] 逐字符遍历
来源：http://sli.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://rba.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xsb.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ejf.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jqm.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pxy.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hsv.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tlz.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xen.redwolf501.top

[E14] URL 编码与 Base64
来源：http://ktz.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kpl.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ufe.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kys.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xoj.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bax.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wmd.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ncp.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tso.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://ipj.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sry.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lmi.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fjq.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jtw.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xem.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://evt.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://apv.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qcn.pengpengdd.cyou

[E16] 数字千分位
来源：http://gqi.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://cdn.meibo888.top

PHP:  number_format(1234567);
来源：http://knc.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jze.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xzh.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tgw.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oge.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rlo.yj202588.top

C#:   1234567.ToString("N0")
来源：http://kip.jiagoushi.top

[E17] 首字母大写
来源：http://pad.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lzy.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ggb.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nou.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xlo.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxm.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uma.yuanzhike.top

Ruby: s.capitalize
来源：http://azq.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://szn.tanke756.top

[E18] 模板占位符替换
来源：http://uod.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://etl.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eon.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ute.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://occ.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bwd.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wia.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mkt.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bgm.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://nyz.haohaochexian.top

Py:   s.splitlines()
来源：http://uhr.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sqf.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://cjl.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://vpb.hfpthk.cn

Java: s.lines().toList()
来源：http://nfh.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://nbc.hnxiangtu.top

Ruby: s.lines
来源：http://yxl.yvedp.cn

C#:   s.Split('\n')
来源：http://ujo.xinyue.icu

[E20] 判断字符串是否为空
来源：http://fzo.cqqwz.cn

Py:   if not s:
来源：http://bvm.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eqa.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kxs.shzxlz.cn

TS:   if (s === "") {}
来源：http://blv.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://zzn.svipenyu.cn

Go:   if s == "" {}
来源：http://ffe.hfpthk.cn

Ruby: if s.empty?
来源：http://wus.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vrk.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://lhg.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kzm.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ujb.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fue.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ttw.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hhg.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://jpw.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xqy.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://udt.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://bys.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bab.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xne.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://awb.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wnc.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://owg.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bvl.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://pes.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wra.yfazqb.com

================================================================================
来源：http://ihm.ivvv.top

F. 文件与目录
来源：http://jqb.xinyue.icu

================================================================================
来源：http://xtk.shuidangran.top

[F01] 读取整个文件
来源：http://oja.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xna.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://beb.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fzk.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jlf.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fkb.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nis.c1oappe.top

Ruby: File.read("a.txt")
来源：http://jwi.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://vmk.hammf.cn

[F02] 逐行读取文件
来源：http://dsr.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nuw.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pls.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqp.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bco.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rko.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iym.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zcj.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zmr.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://pdl.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dng.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dhr.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oir.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jnq.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hcp.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hie.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://udt.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zfd.yonumen.top

[F04] 追加写入文件
来源：http://xfw.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bke.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://svt.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ikq.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hqn.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nte.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vxi.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bnd.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qfo.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://jzi.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vob.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://mfc.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://gbt.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://jir.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xgk.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gig.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://trd.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://hpv.fktsv.cn

[F06] 删除文件
来源：http://jeq.yongpay.top

Py:   os.remove("a.txt")
来源：http://mxm.fktsv.cn

PHP:  unlink("a.txt");
来源：http://rpr.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sqx.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://thn.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mbt.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://swm.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://dpj.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://hay.smart0.xyz

[F07] 创建目录（含多级）
来源：http://xmz.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tzu.uphjek.com


<!-- 参考信息 -->