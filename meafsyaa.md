代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://his.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://wth.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://lof.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://icb.epnwcf.com

PHP:  strpos($s, "x");
来源：http://mzt.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ksp.jianghu66.top

TS:   s.indexOf("x")
来源：http://luz.c1oappe.top

Java: s.indexOf("x")
来源：http://myn.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://wwi.hcnkem.com

Ruby: s.index("x")
来源：http://tup.tian-w.cn

C#:   s.IndexOf("x")
来源：http://qhs.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://iwx.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rcu.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xfj.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lik.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cpw.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kaz.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://orl.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://azr.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nns.zdqjudy.top

[E06] 替换子串
来源：http://tsb.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qxg.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ltg.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://twp.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://kpb.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uiq.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dte.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uxj.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://quq.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://xfb.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qbf.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ffi.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://brd.zdqjudy.top

TS:   s.split(",")
来源：http://ghl.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://yon.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ber.meibo888.top

Ruby: s.split(",");  s.split
来源：http://xds.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ucg.tian-w.cn

[E08] 数组按分隔符合并
来源：http://bxw.jiagoushi.top

Py:   ",".join(items)
来源：http://xea.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://jpm.gogol.net.cn

JS:   items.join(",")
来源：http://kfm.xinyue.icu

TS:   items.join(",")
来源：http://xxl.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://xze.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://ggh.vehdjk.com

Ruby: items.join(",")
来源：http://ufd.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://tza.shzxlz.cn

[E09] 去除所有空白字符
来源：http://jas.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iqk.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ofa.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://bsa.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://pdq.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://nmr.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cml.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://orl.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ulw.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://fop.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wxz.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://orm.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://vfh.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://qmr.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://kfw.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ale.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pdt.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pgi.uphjek.com

[E11] 反转字符串
来源：http://mhp.hnqzz.top

Py:   s[::-1]
来源：http://adv.haohaochexian.top

PHP:  strrev($s);
来源：http://uwe.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://imd.xuanzx.com

TS:   [...s].reverse().join("")
来源：http://pyq.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lvq.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rvk.yueranfly.top

Ruby: s.reverse
来源：http://gsz.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://vlm.0kj1m.cn

[E12] 统计某字符出现次数
来源：http://nei.smart0.xyz

Py:   s.count("a")
来源：http://lmq.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://ndw.fehbvm.com

JS:   s.split("a").length - 1
来源：http://ccw.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://yuf.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cmf.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://pjv.jyoumei.cn

Ruby: s.count("a")
来源：http://nxa.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://yvw.cucudq.cn

[E13] 逐字符遍历
来源：http://bzo.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://wmz.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pjb.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ajq.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pvu.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zig.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hkl.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qtd.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://quy.c1oappe.top

[E14] URL 编码与 Base64
来源：http://xeh.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gvq.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvd.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://trp.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bsf.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nva.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bpl.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sxu.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://omk.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://vhg.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://imb.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qsx.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fxs.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://keu.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bdr.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cax.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://etl.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mgg.yonumen.top

[E16] 数字千分位
来源：http://ycb.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://afi.aibaodan.cn

PHP:  number_format(1234567);
来源：http://gxp.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eok.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ohq.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ryw.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hae.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nos.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://leb.pycfn.com

[E17] 首字母大写
来源：http://tcm.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ads.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://llr.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kjs.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpx.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wdv.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://por.yj20258888.top

Ruby: s.capitalize
来源：http://wkk.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qqj.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://zgh.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bhi.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://msz.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://qon.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zus.jinqigfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zud.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ikh.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nzq.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gtp.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://yed.sjlbkw.cn

Py:   s.splitlines()
来源：http://noq.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kyg.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://zoy.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://kcn.tarul.cn

Java: s.lines().toList()
来源：http://fzh.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://nvb.tianlin.xyz

Ruby: s.lines
来源：http://wis.sweek.top

C#:   s.Split('\n')
来源：http://giw.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://wlg.ywan-chungtsiang.top

Py:   if not s:
来源：http://egk.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://usp.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://svf.yj20258888.top

TS:   if (s === "") {}
来源：http://ahn.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://ogr.feifeiyinyue.top

Go:   if s == "" {}
来源：http://qdr.ctjpmb.com

Ruby: if s.empty?
来源：http://lup.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xnr.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://dac.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rmt.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mjy.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xsy.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzf.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qnz.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://vty.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vnt.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://suz.yvedp.cn

[E22] 字节长度与字符长度
来源：http://qxq.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dpj.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fat.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eej.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mux.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hua.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aqf.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://nwk.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ufv.birdmap.top

================================================================================
来源：http://vhl.chenzaomai.com

F. 文件与目录
来源：http://frv.zdqjudy.top

================================================================================
来源：http://dvj.jlsjyb.cn

[F01] 读取整个文件
来源：http://ujw.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ejd.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://djr.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lei.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gnf.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://auo.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pny.fengsongda.top

Ruby: File.read("a.txt")
来源：http://xce.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://dyp.zycfv.cn

[F02] 逐行读取文件
来源：http://soz.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bza.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://frx.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://puj.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://esg.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bgv.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jbk.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nba.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tst.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://diu.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://psm.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vft.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://von.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sxm.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://myd.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wpc.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://bnl.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dro.cashguo.top

[F04] 追加写入文件
来源：http://qiv.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://akj.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lkd.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtv.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jph.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wpv.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fha.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://igt.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tqn.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://flw.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hbw.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://btu.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://izk.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://ylu.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sfp.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fzz.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://zmw.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://wqc.jyoumei.cn

[F06] 删除文件
来源：http://kli.c1oappe.top

Py:   os.remove("a.txt")
来源：http://zuq.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://fhp.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://guh.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://hac.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lzr.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://ucu.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://kso.316326.xyz

C#:   File.Delete("a.txt");
来源：http://mkz.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://ptf.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfk.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nfz.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://djs.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ltj.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uoz.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wnn.yangfankeji.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yra.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uhz.daria6918.cn

[F08] 遍历目录
来源：http://ilk.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vwm.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iqy.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://aqn.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://zzb.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ogj.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xjb.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://pry.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://gqb.cashguo.top

[F09] 获取文件大小
来源：http://lne.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://zvb.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://kuu.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://dxc.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://fbp.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://pwa.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dwd.fehbvm.com

Ruby: File.size("a.txt")
来源：http://ymf.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://pmr.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://ozy.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xaw.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bwx.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lyz.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://ygj.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ztz.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pnb.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vex.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xdi.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://uhe.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lqu.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tod.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jcc.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdl.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wxk.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://meh.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vwm.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://htv.xuanzx.com

[F12] CSV 读写
来源：http://glo.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lur.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://alu.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lvf.fengsongda.top

TS:   // 同上
来源：http://loi.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ewg.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zcn.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qik.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://vgq.daxiang520.top

================================================================================
来源：http://tjk.epnwcf.com

G. 面向对象
来源：http://ktx.yvedp.cn

================================================================================
来源：http://bmd.zhaomingkeji.xyz

[G01] 定义类
来源：http://dwf.shuidangran.top

Py:   class User: pass
来源：http://eor.aibaodan.cn

PHP:  class User {}
来源：http://ovw.dashuyun.cn

JS:   class User {}
来源：http://khx.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://jau.ehwqpu.com

Java: class User {}
来源：http://jli.xylfe.cn

Go:   type User struct { Name string }
来源：http://ypq.ydjk.org.cn

Ruby: class User; end
来源：http://upt.gotoacloud.top

C#:   class User {}
来源：http://fip.snrcjt.cn

[G02] 构造函数
来源：http://hfo.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://dal.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://wql.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://izx.vqdsnc.cn


<!-- 参考信息 -->