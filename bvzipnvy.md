代发 wailian999

[E02] 重复字符串
来源：http://duz.vqdsnc.cn

Py:   "ab" * 3
来源：http://zdy.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://rfs.316326.xyz

JS:   "ab".repeat(3)
来源：http://kev.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://wec.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://suu.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://qqo.gotoacloud.top

Ruby: "ab" * 3
来源：http://kml.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qfj.hammf.cn

[E03] 截取子串
来源：http://gsr.ctjpmb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tdc.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sls.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oqd.redwolf501.top

TS:   s.slice(1, 4)
来源：http://tjs.snrcjt.cn

Java: s.substring(1, 4)
来源：http://poa.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sdt.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sry.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://qdx.jinqigufen.top

[E04] 查找子串位置
来源：http://mkx.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://okm.fzhhl.top

PHP:  strpos($s, "x");
来源：http://ybu.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ume.chenzaomai.com

TS:   s.indexOf("x")
来源：http://qwc.yj202588.top

Java: s.indexOf("x")
来源：http://mrp.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://sja.chenzaomai.com

Ruby: s.index("x")
来源：http://kqp.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://nhw.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bzz.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ssd.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://avf.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xav.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bvg.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ebv.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sak.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ktn.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lfu.chenjidiqi.icu

[E06] 替换子串
来源：http://gpa.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ddy.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://vej.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nrj.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://cuu.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qjn.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ecb.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cjo.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://ftv.guannengcc.top

[E07] 按分隔符拆分
来源：http://gst.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wsb.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vea.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://zbe.jqgufenzy.top

TS:   s.split(",")
来源：http://xna.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lio.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zco.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://npz.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yzc.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://lei.ctjpmb.com

Py:   ",".join(items)
来源：http://qfm.vehdjk.com

PHP:  implode(",", $items);
来源：http://hkv.chenlongwang.top

JS:   items.join(",")
来源：http://lli.wangdashe.top

TS:   items.join(",")
来源：http://dfv.jinqigufen.top

Java: String.join(",", items)
来源：http://jhm.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://xxm.jianghu66.top

Ruby: items.join(",")
来源：http://ffi.wangdashe.top

C#:   string.Join(",", items)
来源：http://vqj.aibaodan.cn

[E09] 去除所有空白字符
来源：http://bdr.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ziy.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pdc.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://vzw.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://yow.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://hoc.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kpb.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wzb.jinqigfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rdi.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://xfb.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tri.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tbr.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://uay.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://zld.xziqi.cn

Java: String.format("%03d", 7)
来源：http://nba.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://dxq.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ppz.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zqn.quarkkingdee.top

[E11] 反转字符串
来源：http://kjs.52xcode.cn

Py:   s[::-1]
来源：http://jre.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://eaj.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://dgi.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://dbn.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eav.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oyf.epnwcf.com

Ruby: s.reverse
来源：http://gko.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://abl.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://xmo.fengsongda.top

Py:   s.count("a")
来源：http://inp.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://rrm.hcnkem.com

JS:   s.split("a").length - 1
来源：http://kte.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://ypb.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fyo.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://ekr.gogol.net.cn

Ruby: s.count("a")
来源：http://bta.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://ycm.gaohongyu789.top

[E13] 逐字符遍历
来源：http://hon.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://src.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nxu.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yoc.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hku.ivvv.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dqw.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qnt.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oqc.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ttp.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://dvg.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dtw.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bth.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vij.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://phn.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jfg.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iuw.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wbr.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hdi.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://ity.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pzz.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mgv.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ews.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mpt.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dpm.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aog.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cdn.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://szb.meibo888.top

[E16] 数字千分位
来源：http://frg.yvedp.cn

Py:   f"{1234567:,}"
来源：http://dtu.c1oappe.top

PHP:  number_format(1234567);
来源：http://idb.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://gil.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mta.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bjw.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mxd.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pmd.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://hmm.vehdjk.com

[E17] 首字母大写
来源：http://djx.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dum.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pki.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qpx.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://thr.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dqs.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ehn.gaohongyu789.top

Ruby: s.capitalize
来源：http://qoc.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://djy.cashguo.top

[E18] 模板占位符替换
来源：http://uyg.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bqq.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://idy.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gkc.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://luq.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bft.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ofe.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sqr.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://suj.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://rvs.shanyushiyangtech.top

Py:   s.splitlines()
来源：http://qag.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xxw.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://eqc.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://ugn.ppjwa.cn

Java: s.lines().toList()
来源：http://qkf.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://szo.xuanzx.com

Ruby: s.lines
来源：http://lnj.fktsv.cn

C#:   s.Split('\n')
来源：http://gxg.yfazqb.com

[E20] 判断字符串是否为空
来源：http://ccz.guannengcc.top

Py:   if not s:
来源：http://aqi.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://voc.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://foo.yuanzhike.top

TS:   if (s === "") {}
来源：http://zjm.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://naa.dianchejie.cn

Go:   if s == "" {}
来源：http://zhz.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://hcu.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yve.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://lwb.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://avs.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pbh.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqu.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gqk.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sxh.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://rej.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mrt.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mow.tarul.cn

[E22] 字节长度与字符长度
来源：http://ctz.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://krz.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxc.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsp.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bew.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qys.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oaf.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://sla.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ajq.jinyuanbaomall.cn

================================================================================
来源：http://vxz.gzhubu.top

F. 文件与目录
来源：http://zsh.tianlin.xyz

================================================================================
来源：http://kif.hesvh.cn

[F01] 读取整个文件
来源：http://wdx.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ulf.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://drx.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gwt.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vht.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ddg.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ayv.fzhhl.top

Ruby: File.read("a.txt")
来源：http://kwa.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://sga.hysaishi.cn

[F02] 逐行读取文件
来源：http://efw.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iro.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vxu.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vib.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rlr.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jzv.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lyd.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://azz.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mfn.ivvv.top

[F03] 写入文件（覆盖）
来源：http://xkp.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://stp.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://hth.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zse.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ppq.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cyz.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://unx.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://muq.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://amj.mhx1999.top

[F04] 追加写入文件
来源：http://brw.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lve.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wsi.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pkv.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jne.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yrz.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mkd.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lol.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvn.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://qth.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lrm.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://zmo.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://xwv.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://bmv.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lhh.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rpu.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://agl.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://pvz.shanyushiyangkeji.top

[F06] 删除文件
来源：http://gmx.ydzc1.top

Py:   os.remove("a.txt")
来源：http://pza.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://isu.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://qzo.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://kkp.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aiy.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://esg.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://ldc.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://vdi.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://kmz.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tox.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zks.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qtq.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzj.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ywc.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kxp.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xig.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jgu.yj20258888.top

[F08] 遍历目录
来源：http://hyx.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://eox.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xfw.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://nqj.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://evl.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tzm.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fyv.xziqi.cn

Ruby: Dir.children("dir")
来源：http://ure.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://xvv.shangyingyoupin.top

[F09] 获取文件大小
来源：http://sia.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://iiw.redwolf501.top

PHP:  filesize("a.txt");
来源：http://mua.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://wkc.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://hou.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://for.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oey.cashguo.top

Ruby: File.size("a.txt")
来源：http://bpe.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://weo.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://uen.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mhk.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://akm.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ttz.cucudq.cn

TS:   path.extname("a.txt")
来源：http://azb.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kyy.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ioe.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rjx.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jfb.bbcook.cn

[F11] 复制与移动文件
来源：http://dxh.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lgg.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://smf.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mse.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oem.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nab.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdb.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ftj.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rne.sjlbkw.cn

[F12] CSV 读写
来源：http://exv.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rfy.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://afe.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lme.redwolf501.top

TS:   // 同上
来源：http://bbe.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kke.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://elk.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wro.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://utm.yonumen.top


<!-- 参考信息 -->