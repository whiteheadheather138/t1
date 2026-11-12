代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bea.cashguo.top

[E03] 截取子串
来源：http://ulw.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mdh.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mal.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wbx.smart0.xyz

TS:   s.slice(1, 4)
来源：http://kgf.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://zqq.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cuy.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jql.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://fzp.sweek.top

[E04] 查找子串位置
来源：http://qat.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://feb.hnqzz.top

PHP:  strpos($s, "x");
来源：http://yes.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wys.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://mfd.hammf.cn

Java: s.indexOf("x")
来源：http://wiq.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://hgj.yj202588.top

Ruby: s.index("x")
来源：http://hfd.hammf.cn

C#:   s.IndexOf("x")
来源：http://vkj.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mho.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wcz.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vae.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dim.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bet.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mag.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vwe.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://izd.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qzc.dianchejie.cn

[E06] 替换子串
来源：http://uig.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vmz.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://mhz.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ize.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://khz.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jse.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bcr.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vlv.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://cls.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://osf.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rst.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fzc.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://joc.9152youxi.cn

TS:   s.split(",")
来源：http://uat.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://ylw.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://psd.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://jda.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fps.yj20258.top

[E08] 数组按分隔符合并
来源：http://lrx.aizwys.cn

Py:   ",".join(items)
来源：http://ngq.tanke756.top

PHP:  implode(",", $items);
来源：http://sxc.chenjidiqi.icu

JS:   items.join(",")
来源：http://uyx.fzhhl.top

TS:   items.join(",")
来源：http://gti.jlsjyb.cn

Java: String.join(",", items)
来源：http://oal.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://vmu.xziqi.cn

Ruby: items.join(",")
来源：http://jts.havefunace.top

C#:   string.Join(",", items)
来源：http://okf.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://wex.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://puv.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jpv.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://dmv.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://zpo.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://qid.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://luf.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cuc.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eut.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://flp.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aez.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rcz.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://lmt.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://pdb.yueranfly.top

Java: String.format("%03d", 7)
来源：http://xba.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zzm.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://laj.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oee.vehdjk.com

[E11] 反转字符串
来源：http://rym.ybcxt.top

Py:   s[::-1]
来源：http://pet.sxryk.cn

PHP:  strrev($s);
来源：http://shc.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://isb.cheryme.top

TS:   [...s].reverse().join("")
来源：http://hrj.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lva.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nrl.hfpthk.cn

Ruby: s.reverse
来源：http://lwa.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://yyq.yj20258.top

[E12] 统计某字符出现次数
来源：http://ubd.tianlin.xyz

Py:   s.count("a")
来源：http://bvm.yonumen.top

PHP:  substr_count($s, "a");
来源：http://xzy.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://ers.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://njy.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://svn.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://jtd.c1oappe.top

Ruby: s.count("a")
来源：http://wxd.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://ria.tarul.cn

[E13] 逐字符遍历
来源：http://rnz.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://axd.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bgn.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wtn.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ets.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xwt.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hkt.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://grz.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://twz.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://ldx.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lyd.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ifd.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://viv.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mni.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ame.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://stq.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://awf.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qsh.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://yiw.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xor.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nyw.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wst.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lrq.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nou.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://icb.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://izp.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://atd.c1oappe.top

[E16] 数字千分位
来源：http://ykv.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://vwu.guowangkeji.top

PHP:  number_format(1234567);
来源：http://hwn.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ztg.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ttb.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hnd.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nyn.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://roo.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://bjp.yj20258888.top

[E17] 首字母大写
来源：http://hix.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://inm.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://yxw.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xhl.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rns.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fpk.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bgz.gogol.net.cn

Ruby: s.capitalize
来源：http://ixm.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tbr.cqqwz.cn

[E18] 模板占位符替换
来源：http://htg.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pde.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sgf.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://imt.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://idz.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bge.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wad.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tna.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xjx.fengsongda.top

[E19] 多行文本按行拆分
来源：http://yyj.gogol.net.cn

Py:   s.splitlines()
来源：http://ogy.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wom.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://kkl.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://zth.cqqwz.cn

Java: s.lines().toList()
来源：http://exe.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://huk.yonumen.top

Ruby: s.lines
来源：http://hsv.yj20258.top

C#:   s.Split('\n')
来源：http://lrq.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://kyi.nwbrower.top

Py:   if not s:
来源：http://ixt.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nmw.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmh.ivvv.top

TS:   if (s === "") {}
来源：http://jdd.sweek.top

Java: if (s.isEmpty()) {}
来源：http://dgc.yangfankeji.com

Go:   if s == "" {}
来源：http://wsx.guowangkeji.top

Ruby: if s.empty?
来源：http://npx.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://auf.hysaishi.cn

[E21] 超长截断加省略号
来源：http://dpd.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wrk.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wgt.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfu.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lsw.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ejf.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://xri.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eyb.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dve.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://unm.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ont.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iwp.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpp.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nry.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gni.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nke.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://axn.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mty.chenjidiqi.icu

================================================================================
来源：http://cik.jlsjyb.cn

F. 文件与目录
来源：http://smx.gogol.net.cn

================================================================================
来源：http://kvp.hongshengwenyu.top

[F01] 读取整个文件
来源：http://nhn.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gjp.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://jso.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uky.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eok.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jyz.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://umt.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://twf.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://wmm.ybcxt.top

[F02] 逐行读取文件
来源：http://uqa.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rkc.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nnr.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvv.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skd.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ymh.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tgl.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ezt.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wkk.316326.xyz

[F03] 写入文件（覆盖）
来源：http://axu.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rkw.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sto.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkx.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hld.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://utg.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ubf.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://zeg.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ybl.vqdsnc.cn

[F04] 追加写入文件
来源：http://unk.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iry.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wfv.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvp.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kbv.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rxj.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qcy.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tkm.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mja.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://bfg.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mxd.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://orh.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://ndq.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://rnh.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rqb.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lbu.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://ozk.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://wja.0kj1m.cn

[F06] 删除文件
来源：http://vwz.fehbvm.com

Py:   os.remove("a.txt")
来源：http://sxa.fktsv.cn

PHP:  unlink("a.txt");
来源：http://hve.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://maa.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lpo.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vxp.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://xes.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://fam.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://qya.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://zvk.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://slp.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hys.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gmd.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hat.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cux.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://auo.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tuf.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cxi.pengpengdd.cyou

[F08] 遍历目录
来源：http://bbj.fktsv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qwe.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://afq.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://eae.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://wdy.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qcc.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rnu.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://vie.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://csw.hywenlv.cn

[F09] 获取文件大小
来源：http://zbp.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://ewy.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://guj.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://usx.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://yel.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://ooz.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ebf.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://pok.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://qrn.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://eds.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://exi.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lmd.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://shd.mhx1999.top

TS:   path.extname("a.txt")
来源：http://bns.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://foa.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://knj.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xqg.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjx.bjfxy.top

[F11] 复制与移动文件
来源：http://cgh.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ywe.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fvo.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://btg.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://phv.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kqt.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tkd.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fak.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mho.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://krr.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xyf.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://swv.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gem.hesvh.cn

TS:   // 同上
来源：http://hxe.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tsp.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ftl.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oal.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vsv.sxryk.cn

================================================================================
来源：http://wdq.ctjpmb.com

G. 面向对象
来源：http://jqe.hfpthk.cn

================================================================================
来源：http://hpz.jqgfzy.top

[G01] 定义类
来源：http://fph.shzxlz.cn

Py:   class User: pass
来源：http://pil.aibaodan.cn

PHP:  class User {}
来源：http://cnn.gaohongyu789.top

JS:   class User {}
来源：http://zzj.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://uij.jlsjyb.cn


<!-- 参考信息 -->