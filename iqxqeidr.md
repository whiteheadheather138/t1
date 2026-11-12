代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hxp.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vnp.meibo888.top

Go:   // 手写循环
来源：http://xws.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fuu.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://szn.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://qhx.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ykb.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://owa.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mzx.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://swz.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtg.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pts.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lot.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gse.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://xsq.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ixy.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://moe.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wdi.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ebf.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kak.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mkh.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vjt.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dmt.yvedp.cn

[D26] 数组转字符串
来源：http://atk.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://ofd.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://cdm.redwolf501.top

JS:   arr.join(", ")
来源：http://uxn.zdbjq.cn

TS:   arr.join(", ")
来源：http://ghc.aibaodan.cn

Java: String.join(", ", list)
来源：http://fbj.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://qfj.guannengcc.top

Ruby: arr.join(", ")
来源：http://rmt.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://avd.zycfv.cn

================================================================================
来源：http://qam.gaohongyu789.top

E. 字符串处理
来源：http://prp.zdbjq.cn

================================================================================
来源：http://qpx.zhengqikj.top

[E01] 拼接字符串
来源：http://vim.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qht.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cnz.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jyn.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxg.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lbm.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eec.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://req.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://luj.jianghu66.top

[E02] 重复字符串
来源：http://vfe.yueranfly.top

Py:   "ab" * 3
来源：http://naa.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://you.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://ioc.ybcxt.top

TS:   "ab".repeat(3)
来源：http://uku.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://oom.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://tqg.aizwys.cn

Ruby: "ab" * 3
来源：http://ima.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://exn.aibaodan.cn

[E03] 截取子串
来源：http://ppf.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hmd.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dpb.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lme.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://nsi.snrcjt.cn

Java: s.substring(1, 4)
来源：http://nvo.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jtb.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://xkl.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://jjp.ctjpmb.com

[E04] 查找子串位置
来源：http://quo.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://kco.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://bbh.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kei.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://ioo.xinyue.icu

Java: s.indexOf("x")
来源：http://oqp.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://vyt.yuxming.cn

Ruby: s.index("x")
来源：http://wkl.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://dsi.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sen.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ioh.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dyp.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://agu.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mkw.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://phq.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tsr.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aoj.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vvo.jqgfzy.top

[E06] 替换子串
来源：http://gry.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://esa.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://ctb.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qha.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://tij.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://luu.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lmf.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vmh.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://klh.hysaishi.cn

[E07] 按分隔符拆分
来源：http://rdn.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fml.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tjb.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rza.yj20258.top

TS:   s.split(",")
来源：http://kpf.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://umq.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kkp.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://nze.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vto.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://dxt.fzhhl.top

Py:   ",".join(items)
来源：http://vfv.hesvh.cn

PHP:  implode(",", $items);
来源：http://dln.hysaishi.cn

JS:   items.join(",")
来源：http://jvt.haohaochexian.top

TS:   items.join(",")
来源：http://gzr.yonumen.top

Java: String.join(",", items)
来源：http://hip.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://ycy.chenjidiqi.icu

Ruby: items.join(",")
来源：http://rbk.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://jxc.guowangkeji.top

[E09] 去除所有空白字符
来源：http://nkc.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pil.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qtt.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://pnk.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://weo.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://iin.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gbc.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://nhu.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wkr.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://mnr.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mwb.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ybv.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://aob.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://tpw.tarul.cn

Java: String.format("%03d", 7)
来源：http://zwi.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rvi.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://syn.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lgm.daria6918.cn

[E11] 反转字符串
来源：http://vwb.nwbrower.top

Py:   s[::-1]
来源：http://hnm.sweek.top

PHP:  strrev($s);
来源：http://sxx.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://atp.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://gbs.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ctu.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zqj.hongshengwenyu.top

Ruby: s.reverse
来源：http://vfs.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ybs.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://qdz.zhiwuduotai.top

Py:   s.count("a")
来源：http://trx.birdmap.top

PHP:  substr_count($s, "a");
来源：http://xgo.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://pxm.fktsv.cn

TS:   s.split("a").length - 1
来源：http://aww.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://utw.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://evq.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://gpj.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://dbt.yfazqb.com

[E13] 逐字符遍历
来源：http://kio.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://cle.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ver.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://syj.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lsq.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cdm.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xki.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://api.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://efc.fzhhl.top

[E14] URL 编码与 Base64
来源：http://chf.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mxq.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://adl.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uhh.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://swm.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ttj.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pvi.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qvq.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xcu.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://emx.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ewt.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ogf.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mux.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://igj.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ydz.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ykr.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yfd.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ftx.ppjwa.cn

[E16] 数字千分位
来源：http://lqo.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://ova.shzxlz.cn

PHP:  number_format(1234567);
来源：http://fpg.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ysi.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ssw.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bfx.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cax.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yhz.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://pea.fengsongda.top

[E17] 首字母大写
来源：http://dvi.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lbh.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://iwr.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fkx.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tuq.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vlp.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ndp.smart0.xyz

Ruby: s.capitalize
来源：http://dig.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vbv.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://jep.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wai.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://abz.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vht.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xym.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aaq.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://era.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ftx.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://adc.cucudq.cn

[E19] 多行文本按行拆分
来源：http://pas.yfazqb.com

Py:   s.splitlines()
来源：http://tlu.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lml.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://uas.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://guy.fengsongda.top

Java: s.lines().toList()
来源：http://ihn.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://zns.zhoulong.xyz

Ruby: s.lines
来源：http://oyi.sysykeji.top

C#:   s.Split('\n')
来源：http://vcs.andypj.xyz

[E20] 判断字符串是否为空
来源：http://bbq.xuanzx.com

Py:   if not s:
来源：http://zpd.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cpi.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xki.cashguo.top

TS:   if (s === "") {}
来源：http://ddz.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://spa.zdqjudy.top

Go:   if s == "" {}
来源：http://mnc.cheryme.top

Ruby: if s.empty?
来源：http://ynm.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dkl.ppjwa.cn

[E21] 超长截断加省略号
来源：http://kpk.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wfh.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fha.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://djt.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iep.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zvg.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://oae.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gct.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yqi.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://brs.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ibv.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iac.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yki.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qsm.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://boh.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://axp.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://gel.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uzn.gogol.net.cn

================================================================================
来源：http://shw.xuanzx.com

F. 文件与目录
来源：http://ahf.snrcjt.cn

================================================================================
来源：http://znl.ivvv.top

[F01] 读取整个文件
来源：http://nqr.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bnb.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://smn.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sbj.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vaj.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tkk.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqg.andypj.xyz

Ruby: File.read("a.txt")
来源：http://wes.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://saa.zhoulong.xyz

[F02] 逐行读取文件
来源：http://nee.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndf.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bna.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iiv.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lue.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://snq.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://feu.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xar.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://osp.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://xoo.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qhl.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vhf.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dfi.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lnr.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dyr.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nnh.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://ybr.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sxt.pengpengdd.cyou

[F04] 追加写入文件
来源：http://lib.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sya.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tzh.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfl.jinyuanbaomall.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gav.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uav.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gmi.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://alu.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yrk.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://yze.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fbo.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://zxu.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://gtj.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://bwu.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pmk.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ybn.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://ckk.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://vue.ctjpmb.com

[F06] 删除文件
来源：http://wup.iojbl.cn

Py:   os.remove("a.txt")
来源：http://dln.cucudq.cn

PHP:  unlink("a.txt");
来源：http://gkl.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kkt.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://muv.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hkw.yongpay.top

Go:   os.Remove("a.txt")
来源：http://gyk.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://hcy.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://pqr.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://cpt.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://odk.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xpa.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rnu.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://txd.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ngb.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wjd.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vip.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ufu.shuidangran.top

[F08] 遍历目录
来源：http://oru.zhaomingkeji.xyz


<!-- 参考信息 -->