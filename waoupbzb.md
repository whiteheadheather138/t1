代发 wailian999

[D23] reduce 累积计算
来源：http://ffn.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://swe.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rne.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://utk.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhr.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eod.sxryk.cn

Go:   // 手写循环
来源：http://ucu.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cqd.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://prh.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://rqf.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zwk.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kxp.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sjr.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zgz.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://irj.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vtx.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cgv.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lxr.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://jkk.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nlz.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wiq.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hnw.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zkt.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qxk.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sgm.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ruy.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pft.fehbvm.com

[D26] 数组转字符串
来源：http://xvg.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://lvc.tarul.cn

PHP:  implode(", ", $arr);
来源：http://jaf.birdmap.top

JS:   arr.join(", ")
来源：http://hbu.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://ujc.yj202588.top

Java: String.join(", ", list)
来源：http://zbv.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://prh.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://mrd.cucudq.cn

C#:   string.Join(", ", list)
来源：http://raj.chenjidiqi.icu

================================================================================
来源：http://jyr.daria6918.cn

E. 字符串处理
来源：http://tsl.jlsjyb.cn

================================================================================
来源：http://qpq.hnqzz.top

[E01] 拼接字符串
来源：http://wkq.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lha.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iqp.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qnt.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lcy.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oqq.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rsc.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://opp.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://auc.jinqigfzy.top

[E02] 重复字符串
来源：http://vpj.yj20258.top

Py:   "ab" * 3
来源：http://azf.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://bks.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://gqf.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://gai.daria6918.cn

Java: "ab".repeat(3)
来源：http://kzz.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://hvw.vqdsnc.cn

Ruby: "ab" * 3
来源：http://lef.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ave.hammf.cn

[E03] 截取子串
来源：http://fbm.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bvu.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yan.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://krn.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://fqw.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://fyt.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jzz.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://fao.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://lsm.zhixingplan.top

[E04] 查找子串位置
来源：http://yqh.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://ron.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://gwq.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://noi.haohaochexian.top

TS:   s.indexOf("x")
来源：http://ecn.hfpthk.cn

Java: s.indexOf("x")
来源：http://yrv.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://pqf.cdnleiting.top

Ruby: s.index("x")
来源：http://olz.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://mco.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mqb.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yks.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iqi.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uif.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ghf.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lre.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dip.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hku.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bsu.hnqzz.top

[E06] 替换子串
来源：http://xbn.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rym.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://mmx.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usd.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://xqa.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ryg.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kfp.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rpw.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://hmd.sweek.top

[E07] 按分隔符拆分
来源：http://hyl.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cmv.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hvx.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tyo.nwbrower.top

TS:   s.split(",")
来源：http://umi.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://lvr.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://djt.yongpay.top

Ruby: s.split(",");  s.split
来源：http://ibv.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vsp.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://rpt.52xcode.cn

Py:   ",".join(items)
来源：http://flr.snrcjt.cn

PHP:  implode(",", $items);
来源：http://grt.xziqi.cn

JS:   items.join(",")
来源：http://nmq.dianchejie.cn

TS:   items.join(",")
来源：http://msa.sweek.top

Java: String.join(",", items)
来源：http://lmz.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://rzv.ivvv.top

Ruby: items.join(",")
来源：http://qsf.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://rvt.redwolf501.top

[E09] 去除所有空白字符
来源：http://vjo.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ylc.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ray.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://rau.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://ulw.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://uie.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jaa.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://zhx.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hdc.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://aka.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kxq.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dde.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://gaa.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://aqi.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://fss.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nds.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ksc.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qxk.xziqi.cn

[E11] 反转字符串
来源：http://bzf.hnqzz.top

Py:   s[::-1]
来源：http://xdl.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://zrg.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://gab.tanke756.top

TS:   [...s].reverse().join("")
来源：http://tda.yuanzhike.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pvl.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://opb.svipenyu.cn

Ruby: s.reverse
来源：http://fqt.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://gua.tanke756.top

[E12] 统计某字符出现次数
来源：http://wsn.wangshuangyany.cn

Py:   s.count("a")
来源：http://vce.tarul.cn

PHP:  substr_count($s, "a");
来源：http://hsm.bjfxy.top

JS:   s.split("a").length - 1
来源：http://kds.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://icq.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dqs.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://hem.ctjpmb.com

Ruby: s.count("a")
来源：http://hoy.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://sjf.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://puj.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://wnn.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nrw.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ois.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://swn.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qfe.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://czb.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uay.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jbh.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://mjk.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dli.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nhx.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ntl.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iwv.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://riv.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tpy.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pag.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qnn.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://jke.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lle.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://smq.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://euk.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://znt.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jmb.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wzw.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yqz.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gpv.ivvv.top

[E16] 数字千分位
来源：http://gqn.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://gvg.jiagoushi.top

PHP:  number_format(1234567);
来源：http://xnw.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://uhf.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ntl.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yeg.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ecv.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cns.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://xdf.yueranfly.top

[E17] 首字母大写
来源：http://aus.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://inb.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gsp.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://des.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drp.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lma.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ahn.jiagoushi.top

Ruby: s.capitalize
来源：http://zca.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gym.yj20258888.top

[E18] 模板占位符替换
来源：http://rad.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lhx.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vbf.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mgj.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://msi.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dmj.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xfq.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xpg.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uca.gzhubu.top

[E19] 多行文本按行拆分
来源：http://zfe.316326.xyz

Py:   s.splitlines()
来源：http://xds.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vdg.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://hde.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://axt.cqqwz.cn

Java: s.lines().toList()
来源：http://hll.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://xjq.dashuyun.cn

Ruby: s.lines
来源：http://ner.yonumen.top

C#:   s.Split('\n')
来源：http://nah.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://mlr.gogol.net.cn

Py:   if not s:
来源：http://egk.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://emn.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sdn.hnqzz.top

TS:   if (s === "") {}
来源：http://vng.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://udb.xylfe.cn

Go:   if s == "" {}
来源：http://mwj.ydzc1.top

Ruby: if s.empty?
来源：http://ctd.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bmu.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://roo.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llw.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://elo.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://asw.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ctq.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hor.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://cgp.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fso.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bnf.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://vhq.xuetiantiany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://chm.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zti.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qud.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hls.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aza.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lla.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://esa.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pae.jianghu66.top

================================================================================
来源：http://lmh.yuanzhike.top

F. 文件与目录
来源：http://mnh.316326.xyz

================================================================================
来源：http://rrq.chenjidiqi.icu

[F01] 读取整个文件
来源：http://xsx.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://chq.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://rjd.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jmr.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwn.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tdh.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lcs.tanke756.top

Ruby: File.read("a.txt")
来源：http://upq.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://ksj.daxiang520.top

[F02] 逐行读取文件
来源：http://dmr.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://frt.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qrl.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://okx.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iam.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sze.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nat.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ita.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vij.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://ytb.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oah.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ltm.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cvp.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cnr.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://olj.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jxo.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://uys.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ley.cheryme.top

[F04] 追加写入文件
来源：http://ldw.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qoc.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://chb.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gzq.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oac.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://naw.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nqd.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tus.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://opt.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://rxl.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ati.meibo888.top

PHP:  file_exists("a.txt");
来源：http://qem.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://aqr.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://tux.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://tny.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://odn.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://dxh.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://bbj.pengpengdd.cyou

[F06] 删除文件
来源：http://zlw.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://nkv.fehbvm.com

PHP:  unlink("a.txt");
来源：http://jaf.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vyz.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://dte.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qls.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://bqt.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://xpq.tarul.cn

C#:   File.Delete("a.txt");
来源：http://olv.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://jas.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pza.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gfd.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rib.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ebb.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uxg.xziqi.cn


<!-- 参考信息 -->