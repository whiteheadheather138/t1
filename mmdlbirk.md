代发 wailian999

================================================================================
来源：http://viu.vehdjk.com

E. 字符串处理
来源：http://nke.zhengqikj.top

================================================================================
来源：http://fyk.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://ytz.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xdh.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gps.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://soh.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgx.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xrm.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xfg.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://peg.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gfw.shangyingyoupin.top

[E02] 重复字符串
来源：http://zbi.tianlin.xyz

Py:   "ab" * 3
来源：http://mqv.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://qwa.hammf.cn

JS:   "ab".repeat(3)
来源：http://ijm.cucudq.cn

TS:   "ab".repeat(3)
来源：http://eve.jyoumei.cn

Java: "ab".repeat(3)
来源：http://qvs.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://wny.0kj1m.cn

Ruby: "ab" * 3
来源：http://kgx.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jcw.sufxvd.cn

[E03] 截取子串
来源：http://hqa.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xzh.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://env.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvm.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://rio.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://kxh.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qin.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://wgi.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://hdc.zdqjudy.top

[E04] 查找子串位置
来源：http://wox.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://jxi.tian-w.cn

PHP:  strpos($s, "x");
来源：http://oyg.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngf.jyoumei.cn

TS:   s.indexOf("x")
来源：http://xay.cheryme.top

Java: s.indexOf("x")
来源：http://lfr.316326.xyz

Go:   strings.Index(s, "x")
来源：http://iue.jianghu66.top

Ruby: s.index("x")
来源：http://dpp.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://civ.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ojo.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pjp.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wpm.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npt.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fet.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jes.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tsv.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://igt.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pzi.xuanzx.com

[E06] 替换子串
来源：http://mkr.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ztl.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://fkf.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qjk.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://mzs.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yvy.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hvt.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hgx.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://jem.yangfankeji.com

[E07] 按分隔符拆分
来源：http://pzi.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wpe.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rep.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aua.snrcjt.cn

TS:   s.split(",")
来源：http://yfw.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://obm.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://age.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://kft.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wha.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://hdu.ybcxt.top

Py:   ",".join(items)
来源：http://bjx.cqqwz.cn

PHP:  implode(",", $items);
来源：http://ads.sufxvd.cn

JS:   items.join(",")
来源：http://nfz.yonumen.top

TS:   items.join(",")
来源：http://tel.redwolf501.top

Java: String.join(",", items)
来源：http://yei.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://xcc.jinqigfzy.top

Ruby: items.join(",")
来源：http://chy.hywenlv.cn

C#:   string.Join(",", items)
来源：http://gce.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://vul.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cbr.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hly.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://yjc.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://ulm.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://ueb.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://nuv.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://tzz.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jaf.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://aqq.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rno.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://avv.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://wcu.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://fdn.wangdashe.top

Java: String.format("%03d", 7)
来源：http://riu.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jet.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ycd.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://orq.yj20258.top

[E11] 反转字符串
来源：http://ngy.iojbl.cn

Py:   s[::-1]
来源：http://ken.wangshuangyany.cn

PHP:  strrev($s);
来源：http://nqb.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://qdm.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://hzf.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gtr.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://snh.aizwys.cn

Ruby: s.reverse
来源：http://cns.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://ely.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://iow.uphjek.com

Py:   s.count("a")
来源：http://pkm.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://dea.guannengcc.top

JS:   s.split("a").length - 1
来源：http://yvw.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://jlp.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zik.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://ikd.zhengqikj.top

Ruby: s.count("a")
来源：http://grl.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://uol.jinqigufen.top

[E13] 逐字符遍历
来源：http://bui.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://cgj.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gga.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oeo.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zvo.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://stz.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yqp.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rzp.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rbz.andypj.xyz

[E14] URL 编码与 Base64
来源：http://lpt.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kso.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tat.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dgl.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jjt.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dhg.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yns.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://srh.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mmq.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://gdz.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jgi.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cmt.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hkk.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pfw.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hsf.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://orc.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fut.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lak.jiagoushi.top

[E16] 数字千分位
来源：http://mqb.havefunace.top

Py:   f"{1234567:,}"
来源：http://qqi.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://udn.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xnv.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kec.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zil.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://djb.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://woi.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://ofr.gaohongyu789.top

[E17] 首字母大写
来源：http://bdq.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eie.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fet.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmw.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cao.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lgf.c1oappe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dnq.jyoumei.cn

Ruby: s.capitalize
来源：http://lhw.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fyx.haohaochexian.top

[E18] 模板占位符替换
来源：http://ibf.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bgo.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qaw.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://voe.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cdv.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gwo.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bap.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ppg.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dux.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://qvt.nanxuanxn.top

Py:   s.splitlines()
来源：http://iox.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wjb.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://psq.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://xnb.0kj1m.cn

Java: s.lines().toList()
来源：http://ojb.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://nwc.hesvh.cn

Ruby: s.lines
来源：http://cea.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://xub.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://uun.aibaodan.cn

Py:   if not s:
来源：http://kpu.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bcr.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rau.jqgfzy.top

TS:   if (s === "") {}
来源：http://ehz.sweek.top

Java: if (s.isEmpty()) {}
来源：http://czo.cdnleiting.top

Go:   if s == "" {}
来源：http://luo.dianchejie.cn

Ruby: if s.empty?
来源：http://wvg.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tzy.andypj.xyz

[E21] 超长截断加省略号
来源：http://sgl.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vit.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tyl.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wvb.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nse.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://npd.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://jcz.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://frw.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qhi.andypj.xyz

[E22] 字节长度与字符长度
来源：http://qly.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ufs.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vcz.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gjn.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uxf.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://teh.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fna.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://qhx.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kiq.zhiwuduotai.top

================================================================================
来源：http://lhm.jyoumei.cn

F. 文件与目录
来源：http://xap.tarul.cn

================================================================================
来源：http://giw.quarkkingdee.top

[F01] 读取整个文件
来源：http://byn.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://abw.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://umy.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wtx.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pne.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vec.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qvc.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://txh.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://gqo.cqqwz.cn

[F02] 逐行读取文件
来源：http://ljd.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ukn.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vbk.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ath.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xhs.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pwv.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ple.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://etm.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wxq.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://lxd.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxx.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wjp.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voj.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kds.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://umf.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ytr.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://kdl.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tdp.yfazqb.com

[F04] 追加写入文件
来源：http://wxp.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gbc.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://flt.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://osd.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rhk.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vnx.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxr.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zpg.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xmj.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://qwi.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wtf.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://nld.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://jmy.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://uge.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gmp.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rvo.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://odu.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://xlq.zdbjq.cn

[F06] 删除文件
来源：http://glv.tian-w.cn

Py:   os.remove("a.txt")
来源：http://awt.ybcxt.top

PHP:  unlink("a.txt");
来源：http://nsg.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wzi.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://qbf.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uen.cheryme.top

Go:   os.Remove("a.txt")
来源：http://gmm.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://msw.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://nsm.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://qhm.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zkf.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bmq.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oki.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tbc.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ykp.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lcy.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kbg.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kkq.jiagoushi.top

[F08] 遍历目录
来源：http://pry.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kmi.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ffh.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://yts.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://inv.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pzm.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tom.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://xrc.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://fql.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://sjp.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://suv.tanke756.top

PHP:  filesize("a.txt");
来源：http://yru.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://yaw.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://wta.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://urb.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://far.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://tsb.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://gjt.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://gka.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfv.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fpr.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ihj.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://mbt.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ail.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lmk.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yzk.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bwn.jinqigfzy.top

[F11] 复制与移动文件
来源：http://cgm.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://atj.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hmj.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vll.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzh.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://odl.sweek.top


<!-- 参考信息 -->