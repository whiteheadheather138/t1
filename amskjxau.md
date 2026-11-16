代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kea.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://pcz.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kuj.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aib.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ywt.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qqg.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qoa.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eqm.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aqb.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lry.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://iwb.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bmy.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://crl.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wjg.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mxj.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://szv.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uuu.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://slp.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vyu.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://bcz.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://rpy.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://wpq.cdnleiting.top

JS:   arr.join(", ")
来源：http://ufc.jinqigufen.top

TS:   arr.join(", ")
来源：http://cpv.cucudq.cn

Java: String.join(", ", list)
来源：http://vmy.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://lbl.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://vmq.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://hro.yangfankeji.com

================================================================================
来源：http://hxt.guowangkeji.top

E. 字符串处理
来源：http://joz.hammf.cn

================================================================================
来源：http://bxu.hongshengwenyu.top

[E01] 拼接字符串
来源：http://ygh.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oxu.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://edj.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bxy.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tyw.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sqy.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qit.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dcr.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hdq.hammf.cn

[E02] 重复字符串
来源：http://ekw.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://dtm.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://qsf.hcnkem.com

JS:   "ab".repeat(3)
来源：http://hit.yfazqb.com

TS:   "ab".repeat(3)
来源：http://rgq.yj202588.top

Java: "ab".repeat(3)
来源：http://ncp.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://tbj.hywenlv.cn

Ruby: "ab" * 3
来源：http://tgw.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kel.wangdashe.top

[E03] 截取子串
来源：http://yxf.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://afx.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wgx.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gpw.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://rri.yongpay.top

Java: s.substring(1, 4)
来源：http://kgo.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jze.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://mfo.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://njg.gzhubu.top

[E04] 查找子串位置
来源：http://nbj.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://ers.yfazqb.com

PHP:  strpos($s, "x");
来源：http://ahx.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wco.fehbvm.com

TS:   s.indexOf("x")
来源：http://ppn.ydzc1.top

Java: s.indexOf("x")
来源：http://nke.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://wuy.andypj.xyz

Ruby: s.index("x")
来源：http://der.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://ppz.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fov.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kjx.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uts.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pxz.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cqn.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qxl.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wsn.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://slm.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ddv.aibaodan.cn

[E06] 替换子串
来源：http://the.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jpv.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://yce.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dhj.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://iim.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpe.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ttp.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://srm.hammf.cn

C#:   s.Replace("a", "b")
来源：http://vkp.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://hep.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fes.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ioa.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wqh.sxryk.cn

TS:   s.split(",")
来源：http://nxd.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ktp.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://opo.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://mfp.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ytx.hammf.cn

[E08] 数组按分隔符合并
来源：http://ucm.ehwqpu.com

Py:   ",".join(items)
来源：http://qrh.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://red.sxryk.cn

JS:   items.join(",")
来源：http://gqy.tianlin.xyz

TS:   items.join(",")
来源：http://lup.316326.xyz

Java: String.join(",", items)
来源：http://xhm.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://bkw.yongpay.top

Ruby: items.join(",")
来源：http://rzt.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://vum.guowangkeji.top

[E09] 去除所有空白字符
来源：http://cfy.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xzq.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vdy.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://rzs.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://csk.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://vno.haohaochexian.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qoj.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://fko.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pal.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://xwd.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xfe.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://chy.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://gfa.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://nnb.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://wzp.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://oiy.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ben.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hka.wangshuangyany.cn

[E11] 反转字符串
来源：http://unp.bbcook.cn

Py:   s[::-1]
来源：http://qic.dashuyun.cn

PHP:  strrev($s);
来源：http://lji.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://ggv.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://aqb.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jxm.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://pzr.sysykeji.top

Ruby: s.reverse
来源：http://gin.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://ujx.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://tjy.guannengcc.top

Py:   s.count("a")
来源：http://igc.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://uss.andypj.xyz

JS:   s.split("a").length - 1
来源：http://kmn.bbcook.cn

TS:   s.split("a").length - 1
来源：http://san.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bzh.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://kwd.hywenlv.cn

Ruby: s.count("a")
来源：http://sig.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://sha.andypj.xyz

[E13] 逐字符遍历
来源：http://gst.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://xdd.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cyt.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gws.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dec.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pyh.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ykv.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rfh.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://khh.fzhhl.top

[E14] URL 编码与 Base64
来源：http://lkh.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://igy.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qar.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukk.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iho.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://api.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vkw.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://seg.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kdj.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://szy.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lqd.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tio.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tbj.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xci.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ikz.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yqk.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://clx.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jbf.sufxvd.cn

[E16] 数字千分位
来源：http://qqz.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://cqm.fktsv.cn

PHP:  number_format(1234567);
来源：http://fdj.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bif.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fgp.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://niv.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zdv.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://axc.yongpay.top

C#:   1234567.ToString("N0")
来源：http://cuq.shzxlz.cn

[E17] 首字母大写
来源：http://rno.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pnk.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hyl.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ftz.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dhq.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vli.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ikk.chenzaomai.com

Ruby: s.capitalize
来源：http://vgd.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jyh.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://cjn.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xqi.vehdjk.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zrj.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gxc.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ryj.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mki.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ccx.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gja.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rdj.tanke756.top

[E19] 多行文本按行拆分
来源：http://xqp.jiagoushi.top

Py:   s.splitlines()
来源：http://erb.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gmj.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://ani.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://rfh.yj20258888.top

Java: s.lines().toList()
来源：http://zyj.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://fru.gogol.net.cn

Ruby: s.lines
来源：http://rda.nanxinkj.top

C#:   s.Split('\n')
来源：http://qzk.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://tup.fzhhl.top

Py:   if not s:
来源：http://voi.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wbn.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tat.hysaishi.cn

TS:   if (s === "") {}
来源：http://uvr.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://cgq.yj202588.top

Go:   if s == "" {}
来源：http://jvl.hongshengwenyu.top

Ruby: if s.empty?
来源：http://vpj.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oxo.smart0.xyz

[E21] 超长截断加省略号
来源：http://yct.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rku.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mwe.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ppu.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nqn.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ysm.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://lug.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ycy.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iuc.redwolf501.top

[E22] 字节长度与字符长度
来源：http://zot.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xca.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bxc.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rzp.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://raj.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tkp.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nsb.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://imm.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uzb.bbcook.cn

================================================================================
来源：http://bog.shangyingyoupin.top

F. 文件与目录
来源：http://yct.gotoacloud.top

================================================================================
来源：http://lnm.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://zrm.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bmo.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://oss.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bjw.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gzx.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uyp.xingfuxueyuan.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wdj.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://cey.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://hqk.xuanzx.com

[F02] 逐行读取文件
来源：http://oya.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dud.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bba.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgb.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xhn.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xcw.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aoe.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mrv.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yfz.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://yyq.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mgp.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jjw.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nxo.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sie.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gul.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://phh.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://qqe.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://orq.gaohongyu789.top

[F04] 追加写入文件
来源：http://eyt.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dzn.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nxu.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ukr.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebu.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bet.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vqr.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qkv.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rcq.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://arj.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cqd.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://aua.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://cww.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://fbx.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ufb.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vni.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://jng.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://vcw.xuanzx.com

[F06] 删除文件
来源：http://uql.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://bbq.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://gci.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oov.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://nji.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ngb.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://thv.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://pgr.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://dve.yonumen.top

[F07] 创建目录（含多级）
来源：http://xwv.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zzo.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hll.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ktj.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jnl.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kzu.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cly.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ndf.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://brz.zhijiandao.cn

[F08] 遍历目录
来源：http://hvw.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mna.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ckg.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://qut.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://rcw.yonumen.top


<!-- 参考信息 -->