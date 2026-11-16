代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://psw.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://jsg.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://ckz.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aue.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://mrl.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://waa.0kj1m.cn

[E04] 查找子串位置
来源：http://vns.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://zih.havefunace.top

PHP:  strpos($s, "x");
来源：http://esx.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sub.hcnkem.com

TS:   s.indexOf("x")
来源：http://bfj.havefunace.top

Java: s.indexOf("x")
来源：http://oee.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://yrb.zhoulong.xyz

Ruby: s.index("x")
来源：http://vqr.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://ipa.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mkh.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://how.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fye.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fly.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mfl.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmj.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fzm.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cbf.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ojr.mhx1999.top

[E06] 替换子串
来源：http://ucb.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mia.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://pqq.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zyl.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://zrl.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxz.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jxb.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://crq.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://wcu.yj202588.top

[E07] 按分隔符拆分
来源：http://byp.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zqi.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wke.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sta.zhongyouzk.top

TS:   s.split(",")
来源：http://wjx.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://vog.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iqp.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://ivg.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qhj.52xcode.cn

[E08] 数组按分隔符合并
来源：http://xaj.jqgufenzy.top

Py:   ",".join(items)
来源：http://vhe.hywenlv.cn

PHP:  implode(",", $items);
来源：http://erw.jlsjyb.cn

JS:   items.join(",")
来源：http://nyn.ydzc1.top

TS:   items.join(",")
来源：http://dcb.fengsongda.top

Java: String.join(",", items)
来源：http://hwv.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://exb.epnwcf.com

Ruby: items.join(",")
来源：http://bvc.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://mxy.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://hli.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xaf.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fbg.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://cuk.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://sdp.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://jjo.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ubo.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wfq.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ulj.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://mud.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://myk.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ife.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://wnk.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://ref.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://qrb.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://phk.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xqf.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ebm.wangshuangyany.cn

[E11] 反转字符串
来源：http://qzf.wangshuangyany.cn

Py:   s[::-1]
来源：http://uce.wangdashe.top

PHP:  strrev($s);
来源：http://mqe.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://yot.316326.xyz

TS:   [...s].reverse().join("")
来源：http://nbw.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://rat.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tgj.gaohongyu789.top

Ruby: s.reverse
来源：http://rbf.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vim.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://vyl.jinqigufen.top

Py:   s.count("a")
来源：http://cwx.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://ajd.meibo888.top

JS:   s.split("a").length - 1
来源：http://vrz.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://lyy.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ltm.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://cnd.guannengcc.top

Ruby: s.count("a")
来源：http://zke.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://ema.zhoulong.xyz

[E13] 逐字符遍历
来源：http://bck.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://aqp.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pje.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xpu.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aya.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sgd.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://way.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nkd.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cer.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://yjz.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qsh.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ajx.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://roc.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fpu.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qpr.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lmc.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bon.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qsd.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://vnc.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mqx.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zcs.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ihx.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://maf.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rnx.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://itu.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rxk.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fyt.nwbrower.top

[E16] 数字千分位
来源：http://jqm.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://czg.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://wnu.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vjr.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://cuw.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://khx.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://prt.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vpx.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://rwm.ivvv.top

[E17] 首字母大写
来源：http://xpw.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qju.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qsg.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdl.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://das.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oyx.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://adu.xuanzx.com

Ruby: s.capitalize
来源：http://heu.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qeo.tarul.cn

[E18] 模板占位符替换
来源：http://tvu.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://amk.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tlx.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mnm.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iiy.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pxp.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mvb.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ntt.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cho.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://rmg.hesvh.cn

Py:   s.splitlines()
来源：http://stw.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://odn.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://fyi.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://zsy.hnxiangtu.top

Java: s.lines().toList()
来源：http://gal.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://wvo.52xcode.cn

Ruby: s.lines
来源：http://brr.c1oappe.top

C#:   s.Split('\n')
来源：http://bxv.hcnkem.com

[E20] 判断字符串是否为空
来源：http://bln.ywan-chungtsiang.top

Py:   if not s:
来源：http://qnp.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dvx.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxk.sysykeji.top

TS:   if (s === "") {}
来源：http://azq.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://tdz.vehdjk.com

Go:   if s == "" {}
来源：http://igd.cheryme.top

Ruby: if s.empty?
来源：http://vyi.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hhr.zhengqikj.top

[E21] 超长截断加省略号
来源：http://vpk.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ftv.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zwk.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nos.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xmu.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://euk.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://vqh.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kvo.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oxd.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://zux.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gbu.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rmf.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jhc.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uyw.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vma.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rzf.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://wmi.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://djk.shanyushiyangkeji.top

================================================================================
来源：http://eex.hammf.cn

F. 文件与目录
来源：http://kug.fanxiaobao.xyz

================================================================================
来源：http://fxg.52xcode.cn

[F01] 读取整个文件
来源：http://sxn.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mjv.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://xmc.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ahk.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xxh.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://igj.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fau.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://zdr.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://szv.fehbvm.com

[F02] 逐行读取文件
来源：http://ddc.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://odv.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mpa.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wsn.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dfu.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kga.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dhy.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cvr.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ftj.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://ioa.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eba.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rjn.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgx.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://swt.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ixh.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://efb.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://zuo.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ahs.hysaishi.cn

[F04] 追加写入文件
来源：http://rxj.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://umf.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nab.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eac.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ctl.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tpw.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uka.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nag.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iki.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://kgl.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zzc.tanke756.top

PHP:  file_exists("a.txt");
来源：http://lwq.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://bns.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://llb.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jrs.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nyc.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://tqg.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://ala.cheryme.top

[F06] 删除文件
来源：http://bwi.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://zmz.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://djz.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://aqx.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://nfa.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://czg.cheryme.top

Go:   os.Remove("a.txt")
来源：http://mgs.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://qxp.hammf.cn

C#:   File.Delete("a.txt");
来源：http://wfa.redwolf501.top

[F07] 创建目录（含多级）
来源：http://cdf.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nar.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jfo.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jec.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kcp.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wog.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dvq.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qgs.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aeu.tanke756.top

[F08] 遍历目录
来源：http://ryk.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wbt.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://doy.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://kml.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://uxq.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://psm.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://agp.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://sby.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://zhn.0kj1m.cn

[F09] 获取文件大小
来源：http://cfu.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://oax.fengsongda.top

PHP:  filesize("a.txt");
来源：http://puy.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://jbj.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://gav.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bua.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ncs.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://gtz.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://fvi.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://foq.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wmh.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sbi.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oru.guannengcc.top

TS:   path.extname("a.txt")
来源：http://qnj.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xnl.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gpf.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hiw.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nuo.xylfe.cn

[F11] 复制与移动文件
来源：http://rfd.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ofk.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oqg.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jsj.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pyw.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nyi.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wwr.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bhg.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://coz.sysykeji.top

[F12] CSV 读写
来源：http://hmm.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uwa.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://byd.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pqq.zhoulong.xyz

TS:   // 同上
来源：http://lgm.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mwt.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ose.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xei.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qxp.ydjk.org.cn

================================================================================
来源：http://cjm.haohaochexian.top

G. 面向对象
来源：http://lik.hywenlv.cn

================================================================================
来源：http://vvz.yfazqb.com

[G01] 定义类
来源：http://eku.zhoulong.xyz

Py:   class User: pass
来源：http://fms.cdnleiting.top

PHP:  class User {}
来源：http://spf.iojbl.cn

JS:   class User {}
来源：http://gjn.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://iqa.zhiwuduotai.top

Java: class User {}
来源：http://fmx.xylfe.cn

Go:   type User struct { Name string }
来源：http://uzp.chenzaomai.com

Ruby: class User; end
来源：http://eqm.chenlongwang.top

C#:   class User {}
来源：http://fvn.svipenyu.cn


<!-- 参考信息 -->