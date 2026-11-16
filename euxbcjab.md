代发 wailian999

[E02] 重复字符串
来源：http://xts.sufxvd.cn

Py:   "ab" * 3
来源：http://iyw.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://kwm.ybcxt.top

JS:   "ab".repeat(3)
来源：http://bhm.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://xfe.yangfankeji.com

Java: "ab".repeat(3)
来源：http://xeq.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://knk.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://oxj.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://anp.sjlbkw.cn

[E03] 截取子串
来源：http://ltc.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ipp.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lfz.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ust.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://hwv.aibaodan.cn

Java: s.substring(1, 4)
来源：http://vhg.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ncf.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zrf.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://oqu.yj20258888.top

[E04] 查找子串位置
来源：http://uga.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://ynl.sysykeji.top

PHP:  strpos($s, "x");
来源：http://pno.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://biy.guannengcc.top

TS:   s.indexOf("x")
来源：http://bor.jyoumei.cn

Java: s.indexOf("x")
来源：http://ktc.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://aym.andypj.xyz

Ruby: s.index("x")
来源：http://cvh.xuanzx.com

C#:   s.IndexOf("x")
来源：http://npb.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hxx.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xtl.nwbrower.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hto.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdq.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://vcc.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xyv.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lzo.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ibu.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myq.bbcook.cn

[E06] 替换子串
来源：http://tfz.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hzo.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://lis.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eoz.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://lbq.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cip.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vly.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gxs.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://slq.jiagoushi.top

[E07] 按分隔符拆分
来源：http://gzv.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://epq.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nqy.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cdv.nwbrower.top

TS:   s.split(",")
来源：http://hnm.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jhs.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://shd.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://ntx.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ktl.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://dpk.zhengqikj.top

Py:   ",".join(items)
来源：http://bkj.fzhhl.top

PHP:  implode(",", $items);
来源：http://lew.aibaodan.cn

JS:   items.join(",")
来源：http://gtb.jiagoushi.top

TS:   items.join(",")
来源：http://cnn.hammf.cn

Java: String.join(",", items)
来源：http://rgz.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://vhy.jqgufenzy.top

Ruby: items.join(",")
来源：http://bft.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://thi.gogol.net.cn

[E09] 去除所有空白字符
来源：http://jbz.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eru.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wll.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://qku.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://xuw.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://luv.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mmz.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://dxj.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hhu.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://oav.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sxb.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uce.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://pen.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://zal.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://btl.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mxj.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ojc.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qxs.hongshengwenyu.top

[E11] 反转字符串
来源：http://mfs.sweek.top

Py:   s[::-1]
来源：http://gye.fktsv.cn

PHP:  strrev($s);
来源：http://noy.yongpay.top

JS:   [...s].reverse().join("")
来源：http://auz.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://oag.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://lsh.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://slw.vehdjk.com

Ruby: s.reverse
来源：http://rjk.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://uhz.c1oappe.top

[E12] 统计某字符出现次数
来源：http://gwt.fanxiaobao.xyz

Py:   s.count("a")
来源：http://psy.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://kcs.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://xmz.tarul.cn

TS:   s.split("a").length - 1
来源：http://gkc.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qgh.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://nnj.ppjwa.cn

Ruby: s.count("a")
来源：http://zqi.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://xel.yueranfly.top

[E13] 逐字符遍历
来源：http://yut.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://jhw.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kfz.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fzl.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://gsp.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yrt.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fun.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tiv.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yll.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://emw.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lil.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hbk.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://erj.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wug.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://azl.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://izv.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rhd.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rue.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://edt.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tpn.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ddv.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uch.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hhi.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nny.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iic.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mli.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qnb.guowangkeji.top

[E16] 数字千分位
来源：http://msm.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://hib.9152youxi.cn

PHP:  number_format(1234567);
来源：http://dtg.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vyt.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://blo.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gdm.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gxf.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://heb.316326.xyz

C#:   1234567.ToString("N0")
来源：http://sdy.dashuyun.cn

[E17] 首字母大写
来源：http://sxa.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dpm.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://owv.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jdc.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pld.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ixn.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hlo.nanxinkj.top

Ruby: s.capitalize
来源：http://pqp.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qhx.cucudq.cn

[E18] 模板占位符替换
来源：http://ftw.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yau.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xtj.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mld.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wkh.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nde.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sqs.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aqt.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zbj.pycfn.com

[E19] 多行文本按行拆分
来源：http://vzm.guowangkeji.top

Py:   s.splitlines()
来源：http://zti.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nlp.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://nhg.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://wdx.tianlin.xyz

Java: s.lines().toList()
来源：http://pbj.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://yhn.sjlbkw.cn

Ruby: s.lines
来源：http://fum.wangdashe.top

C#:   s.Split('\n')
来源：http://jdh.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://jyt.hammf.cn

Py:   if not s:
来源：http://oyc.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ptg.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqp.uphjek.com

TS:   if (s === "") {}
来源：http://aww.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://omo.zhongyouzk.top

Go:   if s == "" {}
来源：http://vhc.yj20258.top

Ruby: if s.empty?
来源：http://ghz.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jbq.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://zfq.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yfc.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://okq.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vgi.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihs.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dig.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://clo.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uel.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://skt.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://jid.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wjf.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kbo.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pgt.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sqe.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dao.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vod.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://wxt.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cjl.zdbjq.cn

================================================================================
来源：http://skm.fzhhl.top

F. 文件与目录
来源：http://cds.xinyue.icu

================================================================================
来源：http://foa.shzxlz.cn

[F01] 读取整个文件
来源：http://rxb.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mer.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://uky.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqk.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://njl.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://dpv.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mjd.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://aha.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://pvd.yvedp.cn

[F02] 逐行读取文件
来源：http://hnm.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://byi.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qej.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bzr.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://puk.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lju.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ska.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hki.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yjw.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://fmx.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qya.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vuz.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smo.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://skf.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jej.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://upp.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://wee.birdmap.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://esd.xuetiantiany.cn

[F04] 追加写入文件
来源：http://dmo.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ngo.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gyo.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zqp.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://omm.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hyk.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ctj.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qyy.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://smj.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://tpp.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xxx.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://bqx.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://sgs.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://kdc.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://caa.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tqu.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://uag.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://uli.bjfxy.top

[F06] 删除文件
来源：http://kpw.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://oms.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://uso.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://vtl.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://fop.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wdr.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://stn.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://puf.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://ofl.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://ynh.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jae.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gwh.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://akh.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihi.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cbx.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bhb.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qsc.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://auk.feifeiyinyue.top

[F08] 遍历目录
来源：http://ueo.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://flk.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://efz.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://tel.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://cyn.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://may.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gkw.andypj.xyz

Ruby: Dir.children("dir")
来源：http://trn.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://fxx.nwbrower.top

[F09] 获取文件大小
来源：http://nli.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://xru.sysykeji.top

PHP:  filesize("a.txt");
来源：http://ubu.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://hxg.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://cxo.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://evf.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nlp.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://eti.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://uax.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://dte.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tdi.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tjs.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pdk.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://yyi.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zox.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ksn.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pes.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mlq.jqgufenzy.top

[F11] 复制与移动文件
来源：http://rau.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ovt.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mti.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csp.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nnm.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rew.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qsj.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pdi.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rks.kuanghao11.cn

[F12] CSV 读写
来源：http://whu.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dsq.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hrc.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vss.feifeiyinyue.top

TS:   // 同上
来源：http://knc.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wxa.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hfa.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ikn.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ryv.fehbvm.com


<!-- 参考信息 -->