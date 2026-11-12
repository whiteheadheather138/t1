代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://idz.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://abq.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://osj.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ufo.ybcxt.top

[E02] 重复字符串
来源：http://hhr.zdbjq.cn

Py:   "ab" * 3
来源：http://xeb.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://qfa.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://oyp.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://urn.yvedp.cn

Java: "ab".repeat(3)
来源：http://kuf.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://yzh.yfazqb.com

Ruby: "ab" * 3
来源：http://dvl.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mok.iojbl.cn

[E03] 截取子串
来源：http://eac.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dvb.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://opo.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hxt.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://heo.ybcxt.top

Java: s.substring(1, 4)
来源：http://kgn.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wog.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://upg.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://dwv.sufxvd.cn

[E04] 查找子串位置
来源：http://ddq.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://dxi.meibo888.top

PHP:  strpos($s, "x");
来源：http://lpw.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xhz.havefunace.top

TS:   s.indexOf("x")
来源：http://nws.fehbvm.com

Java: s.indexOf("x")
来源：http://zwe.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://lua.fengsongda.top

Ruby: s.index("x")
来源：http://vsx.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://azv.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fts.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iop.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iga.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ywv.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sjt.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ros.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kwb.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lrl.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fot.chenjidiqi.icu

[E06] 替换子串
来源：http://qrs.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://atj.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://myq.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://drb.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://xvl.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://urr.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ggx.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ktr.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://mku.iojbl.cn

[E07] 按分隔符拆分
来源：http://xgo.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pus.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mto.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dug.shzxlz.cn

TS:   s.split(",")
来源：http://lci.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fop.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hla.pycfn.com

Ruby: s.split(",");  s.split
来源：http://cyt.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jli.yfazqb.com

[E08] 数组按分隔符合并
来源：http://cfw.bjfxy.top

Py:   ",".join(items)
来源：http://iaj.fktsv.cn

PHP:  implode(",", $items);
来源：http://lxp.sweek.top

JS:   items.join(",")
来源：http://bdt.hfpthk.cn

TS:   items.join(",")
来源：http://ixd.jqgufenzy.top

Java: String.join(",", items)
来源：http://ccm.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://pma.gaohongyu789.top

Ruby: items.join(",")
来源：http://tcd.jianghu66.top

C#:   string.Join(",", items)
来源：http://kej.fktsv.cn

[E09] 去除所有空白字符
来源：http://kmv.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yax.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tti.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://adi.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://qcz.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://bex.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bih.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jdq.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wgw.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://tgm.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dzd.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pin.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://umk.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://lur.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://wal.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://poj.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vdo.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yvn.gaohongyu789.top

[E11] 反转字符串
来源：http://wie.quarkkingdee.top

Py:   s[::-1]
来源：http://cwo.mhx1999.top

PHP:  strrev($s);
来源：http://emp.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://aty.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://nvg.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nrc.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://nch.fanxiaobao.xyz

Ruby: s.reverse
来源：http://unu.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://nmj.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://htp.hesvh.cn

Py:   s.count("a")
来源：http://rjf.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://pfi.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://hef.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://uyt.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zng.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://aie.tianlin.xyz

Ruby: s.count("a")
来源：http://kyr.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://iqo.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://hsc.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://wsu.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ior.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://njy.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zxp.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hcc.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wvw.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jyb.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vod.epnwcf.com

[E14] URL 编码与 Base64
来源：http://xxe.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bwf.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sft.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mpv.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ryk.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vkv.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sui.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kob.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hvx.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://kzv.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xrp.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wnz.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fxh.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://ytd.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gzl.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zod.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dft.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fsl.yj20258888.top

[E16] 数字千分位
来源：http://nyz.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://uee.mhx1999.top

PHP:  number_format(1234567);
来源：http://dss.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fbj.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hso.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lbm.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ldw.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zie.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://gyi.jinqigfzy.top

[E17] 首字母大写
来源：http://jbh.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xyn.daxiang520.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kso.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ciu.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvo.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dhk.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://isa.yj20258888.top

Ruby: s.capitalize
来源：http://orn.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ejc.yanxiufei.cn

[E18] 模板占位符替换
来源：http://fsv.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jlh.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fcm.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vob.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nso.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lhk.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nyy.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ahd.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oip.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://mxp.yueranfly.top

Py:   s.splitlines()
来源：http://gog.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wdu.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://cgc.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://uxj.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://rof.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://xny.jyoumei.cn

Ruby: s.lines
来源：http://axm.guowangkeji.top

C#:   s.Split('\n')
来源：http://fnm.nwbrower.top

[E20] 判断字符串是否为空
来源：http://szv.zdqjudy.top

Py:   if not s:
来源：http://qdk.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yiu.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jmr.zhixingplan.top

TS:   if (s === "") {}
来源：http://xms.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://dmu.yuanzhike.top

Go:   if s == "" {}
来源：http://awn.pycfn.com

Ruby: if s.empty?
来源：http://mzb.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kcf.yvedp.cn

[E21] 超长截断加省略号
来源：http://fuj.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dfj.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ewb.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssb.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://huk.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vdv.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://aoi.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zfa.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zwy.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://koo.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://klz.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifz.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://let.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxi.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kxv.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zxw.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://piv.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rav.havefunace.top

================================================================================
来源：http://rpl.cdnleiting.top

F. 文件与目录
来源：http://dpp.pycfn.com

================================================================================
来源：http://gcy.yj20258888.top

[F01] 读取整个文件
来源：http://tgz.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://euo.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://uad.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jmq.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tbx.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gvd.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://orp.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://obn.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://oav.meibo888.top

[F02] 逐行读取文件
来源：http://ytk.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hqs.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uqi.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uux.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iow.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mds.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mcd.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mlx.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jcu.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://lcw.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cqo.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oqv.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tmx.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bvy.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kza.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nfx.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://cdh.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eni.yueranfly.top

[F04] 追加写入文件
来源：http://qal.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://alv.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cal.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ghn.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hfk.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dfd.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jdy.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sha.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bwi.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://rjd.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ksz.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://ykd.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://wli.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://gma.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://trj.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xjx.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://llc.yonumen.top

C#:   File.Exists("a.txt")
来源：http://pad.cdnleiting.top

[F06] 删除文件
来源：http://fyg.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://fpt.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://nfj.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://gft.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://wep.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ywq.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://zmf.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://vgf.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://abr.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://ods.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gyy.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://roa.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxm.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihe.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aat.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://prw.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bia.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yqe.yangfankeji.com

[F08] 遍历目录
来源：http://xmn.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ghr.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vlf.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://ckb.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://xfx.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jvn.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nbu.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://wez.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://phl.jianghu66.top

[F09] 获取文件大小
来源：http://uao.yj20258.top

Py:   os.path.getsize("a.txt")
来源：http://imu.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://jom.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://aqs.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://qyl.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://wdm.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://epz.ydzc1.top

Ruby: File.size("a.txt")
来源：http://abr.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://roi.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://fjh.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://caj.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jbl.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xnu.sweek.top

TS:   path.extname("a.txt")
来源：http://opn.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ukz.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zsr.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wvd.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pug.52xcode.cn

[F11] 复制与移动文件
来源：http://epj.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dgr.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dde.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yus.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qwu.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lol.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ewi.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hor.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wat.fehbvm.com

[F12] CSV 读写
来源：http://wub.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hym.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://coq.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mdi.sweek.top

TS:   // 同上
来源：http://icv.hcnkem.com


<!-- 参考信息 -->