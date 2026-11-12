代发 wailian999

[D23] reduce 累积计算
来源：http://qqi.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ioz.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zie.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szh.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://loo.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pmd.cashguo.top

Go:   // 手写循环
来源：http://adx.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sti.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vig.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://gnx.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://naj.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ics.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zrl.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zhw.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lpw.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vds.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qtl.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rcj.yonumen.top

[D25] Set 集合去重与交并差
来源：http://ljo.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lsv.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pyt.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vrw.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xdp.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vfg.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zin.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pxt.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gsm.redwolf501.top

[D26] 数组转字符串
来源：http://phx.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://uou.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://rwm.yvedp.cn

JS:   arr.join(", ")
来源：http://qjs.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://xoe.cucudq.cn

Java: String.join(", ", list)
来源：http://hrn.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://isf.zdbjq.cn

Ruby: arr.join(", ")
来源：http://tax.uphjek.com

C#:   string.Join(", ", list)
来源：http://ktd.jyoumei.cn

================================================================================
来源：http://bnr.hysaishi.cn

E. 字符串处理
来源：http://hpn.yueranfly.top

================================================================================
来源：http://nic.xziqi.cn

[E01] 拼接字符串
来源：http://zuw.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cqq.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xtt.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kpq.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwf.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://toc.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tws.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tue.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ipo.bjfxy.top

[E02] 重复字符串
来源：http://ipp.yj20258888.top

Py:   "ab" * 3
来源：http://ddf.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://qcf.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://ekc.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://xui.yj20258888.top

Java: "ab".repeat(3)
来源：http://cbc.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://bfk.ehwqpu.com

Ruby: "ab" * 3
来源：http://dqt.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pga.daria6918.cn

[E03] 截取子串
来源：http://mgy.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qta.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iqw.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zhj.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://zfj.jinqigufen.top

Java: s.substring(1, 4)
来源：http://ygn.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cvf.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hxs.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://tlu.zhixingplan.top

[E04] 查找子串位置
来源：http://dnq.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://xaz.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://prk.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nhx.bbcook.cn

TS:   s.indexOf("x")
来源：http://xmp.jqgfzy.top

Java: s.indexOf("x")
来源：http://gzr.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://wqz.fktsv.cn

Ruby: s.index("x")
来源：http://jku.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://fmx.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pfg.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sgc.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zri.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xab.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hzc.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edc.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://plh.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mrn.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aur.xinyue.icu

[E06] 替换子串
来源：http://fqn.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vwo.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://oso.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wbi.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://kam.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wsw.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lll.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ibw.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://rbc.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://akm.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nrq.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vam.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rfi.guowangkeji.top

TS:   s.split(",")
来源：http://zho.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zus.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kvu.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://fsc.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xcv.smart0.xyz

[E08] 数组按分隔符合并
来源：http://rjl.dianchejie.cn

Py:   ",".join(items)
来源：http://hhs.yj20258.top

PHP:  implode(",", $items);
来源：http://kgc.jianghu66.top

JS:   items.join(",")
来源：http://zqj.hnqzz.top

TS:   items.join(",")
来源：http://qiy.pengpengdd.cyou

Java: String.join(",", items)
来源：http://jqf.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://aja.andypj.xyz

Ruby: items.join(",")
来源：http://idc.yangfankeji.com

C#:   string.Join(",", items)
来源：http://jde.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://qqx.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blx.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aot.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://siu.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://yas.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://wpi.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cit.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://llh.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyq.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://lti.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vdq.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nhc.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://htc.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://isi.xinyue.icu

Java: String.format("%03d", 7)
来源：http://swv.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yik.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xth.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uug.cashguo.top

[E11] 反转字符串
来源：http://qmc.bbcook.cn

Py:   s[::-1]
来源：http://biw.yangfankeji.com

PHP:  strrev($s);
来源：http://hmh.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://nth.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://vaz.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tzc.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wil.tanke756.top

Ruby: s.reverse
来源：http://kcd.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lkl.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://vqg.zhongyouzk.top

Py:   s.count("a")
来源：http://kdv.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://eau.316326.xyz

JS:   s.split("a").length - 1
来源：http://reg.meibo888.top

TS:   s.split("a").length - 1
来源：http://bus.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tup.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://ntq.hesvh.cn

Ruby: s.count("a")
来源：http://emi.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://opk.nwbrower.top

[E13] 逐字符遍历
来源：http://mta.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://qyv.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uir.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://aqd.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gih.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ugr.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ueb.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pel.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ciq.xuanzx.com

[E14] URL 编码与 Base64
来源：http://zhk.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xyi.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://otm.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pby.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wle.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nmn.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ask.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rzh.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vhz.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://oei.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qrk.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kle.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://des.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ncv.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wjv.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kib.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kpm.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xus.pycfn.com

[E16] 数字千分位
来源：http://swu.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://kbm.fengsongda.top

PHP:  number_format(1234567);
来源：http://irf.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ljv.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nls.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lvs.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rka.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dot.uphjek.com

C#:   1234567.ToString("N0")
来源：http://yfc.ctjpmb.com

[E17] 首字母大写
来源：http://lch.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zwg.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dpp.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jnc.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://atx.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dlj.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ljx.quarkkingdee.top

Ruby: s.capitalize
来源：http://poi.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eaa.52xcode.cn

[E18] 模板占位符替换
来源：http://ccu.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://noc.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uyg.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://dxt.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ghy.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wty.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://amq.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvn.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oza.yvedp.cn

[E19] 多行文本按行拆分
来源：http://wjk.sysykeji.top

Py:   s.splitlines()
来源：http://mag.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dcs.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://nnk.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://gvh.yangfankeji.com

Java: s.lines().toList()
来源：http://wzx.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://ghe.xuetiantiany.cn

Ruby: s.lines
来源：http://xpu.yuanzhike.top

C#:   s.Split('\n')
来源：http://hvn.tian-w.cn

[E20] 判断字符串是否为空
来源：http://fer.jyoumei.cn

Py:   if not s:
来源：http://tih.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zju.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hfj.52xcode.cn

TS:   if (s === "") {}
来源：http://uxc.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://jtz.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://kxh.vehdjk.com

Ruby: if s.empty?
来源：http://bwr.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pnv.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://fhw.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ujq.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vhy.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fed.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xri.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dbg.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://onc.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tse.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tdn.fktsv.cn

[E22] 字节长度与字符长度
来源：http://yvx.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pda.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://itp.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kuw.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tnh.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://elb.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tii.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://xyi.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jco.cdnleiting.top

================================================================================
来源：http://ydk.shzxlz.cn

F. 文件与目录
来源：http://gad.yfazqb.com

================================================================================
来源：http://bnz.sysykeji.top

[F01] 读取整个文件
来源：http://flv.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jib.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://zgu.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dwp.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bhh.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fsv.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rwb.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://ugv.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://mth.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://ymn.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://biv.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jkf.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://inu.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ewl.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hbk.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://shm.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bkw.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://peq.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://xxf.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://exh.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oxk.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fdv.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dha.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cte.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jik.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://umx.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yvo.xuanzx.com

[F04] 追加写入文件
来源：http://vmj.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xjv.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wbr.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxm.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zdl.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uxx.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://efa.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cub.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iie.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://zxo.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iwh.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://zuw.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://qgx.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://vxs.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kxe.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hpv.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://wsj.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://qah.xuanzx.com

[F06] 删除文件
来源：http://vdt.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://sqt.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://mtn.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://joh.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://smf.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gnh.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://xyj.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://jpm.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://otc.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://gab.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qgn.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://stx.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://urc.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yax.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eaw.guowangkeji.top


<!-- 参考信息 -->