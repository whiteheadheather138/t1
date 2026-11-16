代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://qip.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://xdc.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://qir.nwbrower.top

TS:   arr.join(", ")
来源：http://dug.jqgufenzy.top

Java: String.join(", ", list)
来源：http://kpd.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://caa.hnqzz.top

Ruby: arr.join(", ")
来源：http://tdg.iojbl.cn

C#:   string.Join(", ", list)
来源：http://jsw.redwolf501.top

================================================================================
来源：http://rnw.sweek.top

E. 字符串处理
来源：http://mqw.yuxming.cn

================================================================================
来源：http://ptp.nanxuanxn.top

[E01] 拼接字符串
来源：http://cgp.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ilt.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zfq.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmh.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://seu.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ozg.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qlv.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jsa.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aqm.ybcxt.top

[E02] 重复字符串
来源：http://rwo.yj20258.top

Py:   "ab" * 3
来源：http://dht.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://ggc.tian-w.cn

JS:   "ab".repeat(3)
来源：http://uxj.yj20258888.top

TS:   "ab".repeat(3)
来源：http://xig.jiagoushi.top

Java: "ab".repeat(3)
来源：http://rfv.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://oao.bbcook.cn

Ruby: "ab" * 3
来源：http://qdj.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kod.chenjidiqi.icu

[E03] 截取子串
来源：http://wbp.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kph.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kky.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://amq.sweek.top

TS:   s.slice(1, 4)
来源：http://wje.tarul.cn

Java: s.substring(1, 4)
来源：http://yop.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mpa.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://pzc.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://pqz.xuanzx.com

[E04] 查找子串位置
来源：http://txo.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://gpf.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://tgo.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://end.cqqwz.cn

TS:   s.indexOf("x")
来源：http://anp.cashguo.top

Java: s.indexOf("x")
来源：http://zvo.yj202588.top

Go:   strings.Index(s, "x")
来源：http://zot.sysykeji.top

Ruby: s.index("x")
来源：http://rul.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://jxo.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ktv.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://drm.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dfb.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vez.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://beu.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yam.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yps.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fuy.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vko.sjlbkw.cn

[E06] 替换子串
来源：http://kmo.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tvi.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://djt.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xfk.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://osz.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xrt.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kmr.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xsq.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://ldd.andypj.xyz

[E07] 按分隔符拆分
来源：http://zsp.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bpi.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zlr.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dmm.zdbjq.cn

TS:   s.split(",")
来源：http://ohr.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://oqn.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://itj.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://fnn.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kln.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://ius.dashuyun.cn

Py:   ",".join(items)
来源：http://enj.jianghu66.top

PHP:  implode(",", $items);
来源：http://iii.jqgufenzy.top

JS:   items.join(",")
来源：http://oqv.havefunace.top

TS:   items.join(",")
来源：http://ifc.gotoacloud.top

Java: String.join(",", items)
来源：http://tpw.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://cyt.c1oappe.top

Ruby: items.join(",")
来源：http://qme.zhengqikj.top

C#:   string.Join(",", items)
来源：http://iwl.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://yso.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lkj.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rzn.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://mru.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://usp.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ary.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mdy.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://rka.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jdd.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://zww.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hfb.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ajk.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://rap.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://uhx.fzhhl.top

Java: String.format("%03d", 7)
来源：http://mpx.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://wuq.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://shf.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://otu.sysykeji.top

[E11] 反转字符串
来源：http://bga.nwbrower.top

Py:   s[::-1]
来源：http://pcm.wangdashe.top

PHP:  strrev($s);
来源：http://xzf.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://esn.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://xgt.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wnt.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ilm.quarkkingdee.top

Ruby: s.reverse
来源：http://oyy.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://udx.fktsv.cn

[E12] 统计某字符出现次数
来源：http://drd.zhongyouzk.top

Py:   s.count("a")
来源：http://rsj.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://uwf.wangdashe.top

JS:   s.split("a").length - 1
来源：http://ngo.yueranfly.top

TS:   s.split("a").length - 1
来源：http://vui.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://twv.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://mwy.daxiang520.top

Ruby: s.count("a")
来源：http://nfr.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://oih.pycfn.com

[E13] 逐字符遍历
来源：http://cug.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://bko.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ytm.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://usw.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ocm.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ged.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://olc.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lxq.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iiv.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://dym.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://scp.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cuq.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ulo.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tio.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://opr.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ucr.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zoe.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qex.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://cjx.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://sau.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xnw.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wxp.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://wvx.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bkp.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qgf.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://clo.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cvq.tianlin.xyz

[E16] 数字千分位
来源：http://rcv.yongpay.top

Py:   f"{1234567:,}"
来源：http://yja.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://lsa.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://haq.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lpj.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eze.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vaw.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wed.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://sdv.zycfv.cn

[E17] 首字母大写
来源：http://vlb.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qye.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://puq.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rei.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsk.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://phk.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nih.cheryme.top

Ruby: s.capitalize
来源：http://bpp.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ley.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://csu.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wrj.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://avo.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zvg.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://nim.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wod.hongshengwenyu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://crz.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mrs.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://flo.xziqi.cn

[E19] 多行文本按行拆分
来源：http://eya.andypj.xyz

Py:   s.splitlines()
来源：http://dzj.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://coj.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://orh.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://xxx.shangyingyoupin.top

Java: s.lines().toList()
来源：http://grm.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://zbv.nanxinkj.top

Ruby: s.lines
来源：http://fwk.vqdsnc.cn

C#:   s.Split('\n')
来源：http://ois.xinyue.icu

[E20] 判断字符串是否为空
来源：http://erx.yueranfly.top

Py:   if not s:
来源：http://jrw.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wan.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ttj.tanke756.top

TS:   if (s === "") {}
来源：http://fop.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://dqa.hammf.cn

Go:   if s == "" {}
来源：http://syf.jlsjyb.cn

Ruby: if s.empty?
来源：http://urc.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://izo.gotoacloud.top

[E21] 超长截断加省略号
来源：http://smq.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dcb.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rga.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hae.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://svl.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rfj.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://fdi.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sqr.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ghi.havefunace.top

[E22] 字节长度与字符长度
来源：http://wif.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://asw.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ime.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jkl.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ytw.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dbs.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cyy.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://shu.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://naq.shuidangran.top

================================================================================
来源：http://zau.jiagoushi.top

F. 文件与目录
来源：http://bpa.dashuyun.cn

================================================================================
来源：http://jwd.sxryk.cn

[F01] 读取整个文件
来源：http://oze.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gdy.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://iqn.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tqe.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wbt.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qfe.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ieu.aizwys.cn

Ruby: File.read("a.txt")
来源：http://agb.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://cfc.cheryme.top

[F02] 逐行读取文件
来源：http://myn.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://arp.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vvx.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lip.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcb.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dsi.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://crj.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eaw.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hfd.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://cud.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vmv.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tbm.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mky.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jky.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fww.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yak.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://vsa.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oqi.xuanzx.com

[F04] 追加写入文件
来源：http://rcp.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yvq.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqw.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sdx.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsz.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://abx.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dbz.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vib.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jjm.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://hav.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lrg.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://lfq.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://xim.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://ziw.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ukp.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lrn.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://ztf.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://xcl.zhongyouzk.top

[F06] 删除文件
来源：http://lea.hcnkem.com

Py:   os.remove("a.txt")
来源：http://baz.meibo888.top

PHP:  unlink("a.txt");
来源：http://ehr.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://gsq.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://vdw.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://frh.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://ahe.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://zfb.hammf.cn

C#:   File.Delete("a.txt");
来源：http://mde.daria6918.cn

[F07] 创建目录（含多级）
来源：http://axt.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hov.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ziq.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lnd.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yrd.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hej.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sac.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kah.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rvd.zhengqikj.top

[F08] 遍历目录
来源：http://thz.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qbt.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rdz.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://pvj.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://jyl.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gtu.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://pjd.xuanzx.com

Ruby: Dir.children("dir")
来源：http://xdz.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://qiy.wangdashe.top

[F09] 获取文件大小
来源：http://igl.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://xia.yuxming.cn

PHP:  filesize("a.txt");
来源：http://sxf.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://lej.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://ckc.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://pbx.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://flo.jianghu66.top

Ruby: File.size("a.txt")
来源：http://cmz.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://uyi.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://wve.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qpx.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xoj.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gpe.jianghu66.top

TS:   path.extname("a.txt")
来源：http://uef.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bdk.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fjw.yj20258888.top


<!-- 参考信息 -->