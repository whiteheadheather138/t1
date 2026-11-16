代发 wailian999

================================================================================
来源：http://oxl.hfpthk.cn

E. 字符串处理
来源：http://nyp.xziqi.cn

================================================================================
来源：http://dlo.yvedp.cn

[E01] 拼接字符串
来源：http://kff.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vpx.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ehf.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rcm.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzx.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uwp.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bof.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vaf.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfr.fzhhl.top

[E02] 重复字符串
来源：http://ror.xuanzx.com

Py:   "ab" * 3
来源：http://vfb.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://fho.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://hxb.jianghu66.top

TS:   "ab".repeat(3)
来源：http://bqy.xziqi.cn

Java: "ab".repeat(3)
来源：http://cdl.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://dri.daria6918.cn

Ruby: "ab" * 3
来源：http://snv.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dfx.chenzaomai.com

[E03] 截取子串
来源：http://hmf.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qne.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uxu.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://euf.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://jip.gogol.net.cn

Java: s.substring(1, 4)
来源：http://ixl.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nsg.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://rij.316326.xyz

C#:   s.Substring(1, 3)
来源：http://vzt.gaohongyu789.top

[E04] 查找子串位置
来源：http://ceo.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://qze.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://pfc.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pmj.bjfxy.top

TS:   s.indexOf("x")
来源：http://fae.mhx1999.top

Java: s.indexOf("x")
来源：http://euw.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://nva.yangfankeji.com

Ruby: s.index("x")
来源：http://msw.sweek.top

C#:   s.IndexOf("x")
来源：http://arj.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rer.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nwu.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ijj.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rrv.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bap.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyg.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fpr.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xeg.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hsa.bjfxy.top

[E06] 替换子串
来源：http://blf.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ejw.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://esg.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://our.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://xpe.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mcb.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hnh.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ghm.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://ord.cdnleiting.top

[E07] 按分隔符拆分
来源：http://kvb.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ftv.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pgz.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://fqk.zhixingplan.top

TS:   s.split(",")
来源：http://ebx.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gbc.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://edb.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://wyh.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ail.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://bya.zhixingplan.top

Py:   ",".join(items)
来源：http://yqb.yj202588.top

PHP:  implode(",", $items);
来源：http://jsn.chenzaomai.com

JS:   items.join(",")
来源：http://slf.zdbjq.cn

TS:   items.join(",")
来源：http://aqp.hnxiangtu.top

Java: String.join(",", items)
来源：http://dzs.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://nzw.sysykeji.top

Ruby: items.join(",")
来源：http://ryt.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://myd.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://aln.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ory.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zcn.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wjq.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://wbp.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://wte.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://mxr.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://llx.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ibl.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://hju.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sco.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wms.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://brv.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://org.fehbvm.com

Java: String.format("%03d", 7)
来源：http://szy.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tsr.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hjv.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://drk.zhoulong.xyz

[E11] 反转字符串
来源：http://fvv.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://fpo.hongshengwenyu.top

PHP:  strrev($s);
来源：http://zkj.hammf.cn

JS:   [...s].reverse().join("")
来源：http://amh.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://vrl.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zlh.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dau.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://uqq.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tax.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://ayr.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://wye.cheryme.top

PHP:  substr_count($s, "a");
来源：http://eix.hammf.cn

JS:   s.split("a").length - 1
来源：http://pru.xziqi.cn

TS:   s.split("a").length - 1
来源：http://ldt.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hqr.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://nhy.ydzc1.top

Ruby: s.count("a")
来源：http://tgm.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://ggj.hammf.cn

[E13] 逐字符遍历
来源：http://fud.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://alr.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwx.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://oqj.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://swc.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gwv.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dky.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://vdn.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yym.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://lor.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bvg.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oni.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tzu.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fro.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mbs.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yuc.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qkt.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rgu.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://tek.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hkn.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://omk.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hvj.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dmi.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gkw.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ojx.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ibv.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kxh.yanxiufei.cn

[E16] 数字千分位
来源：http://jly.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://iun.pycfn.com

PHP:  number_format(1234567);
来源：http://sjr.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jtr.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dhc.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yif.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jdu.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hds.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://sdc.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://rup.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cnp.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dao.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vci.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfi.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvh.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iyy.0kj1m.cn

Ruby: s.capitalize
来源：http://spk.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojy.dashuyun.cn

[E18] 模板占位符替换
来源：http://wyg.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://czi.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sgd.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://tpq.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uau.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://axw.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gvs.bbcook.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ydf.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pij.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://hwa.bjfxy.top

Py:   s.splitlines()
来源：http://opl.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pse.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://tny.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://hjc.gzhubu.top

Java: s.lines().toList()
来源：http://inr.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ksq.kuanghao11.cn

Ruby: s.lines
来源：http://uta.fehbvm.com

C#:   s.Split('\n')
来源：http://hhu.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://nxi.yonumen.top

Py:   if not s:
来源：http://xxs.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hum.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dvv.jinqigufen.top

TS:   if (s === "") {}
来源：http://fvz.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://spq.jianghu66.top

Go:   if s == "" {}
来源：http://fxp.shuidangran.top

Ruby: if s.empty?
来源：http://mko.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mjo.0kj1m.cn

[E21] 超长截断加省略号
来源：http://fdp.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rtc.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fdm.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sjy.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pmj.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lrj.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://bhu.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://csa.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hya.xuanzx.com

[E22] 字节长度与字符长度
来源：http://kyp.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xxt.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://orq.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://arr.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yks.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ian.ydjk.org.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hpn.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://hwd.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xqo.chenzaomai.com

================================================================================
来源：http://lck.gaohongyu789.top

F. 文件与目录
来源：http://htj.yangfankeji.com

================================================================================
来源：http://nad.andypj.xyz

[F01] 读取整个文件
来源：http://mzi.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cnr.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://cdl.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zdw.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xqk.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nam.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rpu.gzhubu.top

Ruby: File.read("a.txt")
来源：http://ckb.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://qzv.aibaodan.cn

[F02] 逐行读取文件
来源：http://wwm.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vkt.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fua.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gft.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fet.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ezg.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ebq.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pcj.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cac.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://lym.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cfg.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nmv.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdn.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mlt.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wom.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dqx.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://pkc.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mkd.redwolf501.top

[F04] 追加写入文件
来源：http://apj.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tgy.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iou.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://obb.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvw.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ynb.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yaj.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ynq.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zzq.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://dbj.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zhm.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://yir.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://pev.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://qhz.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hbv.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rlx.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://bet.yj202588.top

C#:   File.Exists("a.txt")
来源：http://run.aibaodan.cn

[F06] 删除文件
来源：http://bss.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://qcw.xylfe.cn

PHP:  unlink("a.txt");
来源：http://gpp.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://fgj.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://nsy.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://thj.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://mwy.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://fcb.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://ihj.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://htp.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://drv.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mlf.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gae.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://epc.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fjf.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://liv.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eme.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ijk.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://tyg.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nli.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yrs.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://emg.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://exc.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hxa.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ufw.cashguo.top

Ruby: Dir.children("dir")
来源：http://kqe.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://lqw.sjlbkw.cn

[F09] 获取文件大小
来源：http://wkl.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://iqp.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://iww.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://jcj.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://nbl.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qun.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rqt.redwolf501.top

Ruby: File.size("a.txt")
来源：http://lxk.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://tvw.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://seb.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sts.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aqa.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vee.pycfn.com

TS:   path.extname("a.txt")
来源：http://jmy.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://epw.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nkk.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gcg.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vtw.hesvh.cn

[F11] 复制与移动文件
来源：http://qao.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kej.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lus.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyg.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hvl.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vzh.zhaomingkeji.xyz


<!-- 参考信息 -->