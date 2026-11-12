代发 wailian999

PHP:  strpos($s, "x");
来源：http://pnw.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cfo.c1oappe.top

TS:   s.indexOf("x")
来源：http://gwo.c1oappe.top

Java: s.indexOf("x")
来源：http://rvd.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://fjr.shangyingyoupin.top

Ruby: s.index("x")
来源：http://fgk.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://fvb.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yap.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fdd.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qib.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kke.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://pqr.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ezy.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cyr.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dhd.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lnm.vqdsnc.cn

[E06] 替换子串
来源：http://lbz.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fgo.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://qeo.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zwu.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://bhl.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iak.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cqf.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://egq.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://xyn.jyoumei.cn

[E07] 按分隔符拆分
来源：http://oyh.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://odd.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://abz.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ncr.cqqwz.cn

TS:   s.split(",")
来源：http://gan.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://dnv.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ter.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://ziw.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pfd.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://vua.fzhhl.top

Py:   ",".join(items)
来源：http://gjg.jianghu66.top

PHP:  implode(",", $items);
来源：http://ttw.52xcode.cn

JS:   items.join(",")
来源：http://lpt.yj20258.top

TS:   items.join(",")
来源：http://wrv.gogol.net.cn

Java: String.join(",", items)
来源：http://scf.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://rsp.yuanzhike.top

Ruby: items.join(",")
来源：http://iyt.xziqi.cn

C#:   string.Join(",", items)
来源：http://zql.guowangkeji.top

[E09] 去除所有空白字符
来源：http://nug.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xjt.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dgu.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://cmk.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://fjk.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://axk.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ieq.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://lvg.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gsi.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://lhy.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cgp.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fqn.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://umu.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://wns.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://ivq.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://etz.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gdz.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fwb.zhongyouzk.top

[E11] 反转字符串
来源：http://gug.nanxuanxn.top

Py:   s[::-1]
来源：http://zob.yueranfly.top

PHP:  strrev($s);
来源：http://tdq.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://xwt.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://grz.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uqf.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kca.zhiwuduotai.top

Ruby: s.reverse
来源：http://kyj.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://blx.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://yhh.pengpengdd.cyou

Py:   s.count("a")
来源：http://yke.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://jmg.birdmap.top

JS:   s.split("a").length - 1
来源：http://daq.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://aiw.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://axm.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://ltl.jinqigufen.top

Ruby: s.count("a")
来源：http://zoj.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://akb.sjlbkw.cn

[E13] 逐字符遍历
来源：http://qax.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://xdj.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oqu.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pnl.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://sym.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://frf.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://esy.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bde.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://apb.sysykeji.top

[E14] URL 编码与 Base64
来源：http://ccq.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gho.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://luv.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nlu.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bgr.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://elc.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fuh.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xwz.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zma.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://ize.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vsw.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uha.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lwd.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wul.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wmo.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ffr.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nax.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://whd.jinghuilouyu.cn

[E16] 数字千分位
来源：http://qnd.hesvh.cn

Py:   f"{1234567:,}"
来源：http://gmt.hnqzz.top

PHP:  number_format(1234567);
来源：http://igp.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fux.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ljp.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wtq.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tir.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gjf.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://prl.sysykeji.top

[E17] 首字母大写
来源：http://ulc.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vhk.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wpa.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://flg.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gkp.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bpz.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ozo.bbcook.cn

Ruby: s.capitalize
来源：http://ffo.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kmw.yj20258888.top

[E18] 模板占位符替换
来源：http://xpo.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vrw.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xmc.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://svy.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://icb.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mlg.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aao.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://txf.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fmw.cashguo.top

[E19] 多行文本按行拆分
来源：http://bgu.redwolf501.top

Py:   s.splitlines()
来源：http://mbc.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xpl.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://mhb.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://xxv.xylfe.cn

Java: s.lines().toList()
来源：http://olu.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://dta.bjfxy.top

Ruby: s.lines
来源：http://xct.jianghu66.top

C#:   s.Split('\n')
来源：http://bxi.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://ndy.chenlongwang.top

Py:   if not s:
来源：http://jbv.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yrd.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wzu.sysykeji.top

TS:   if (s === "") {}
来源：http://ggr.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://cay.ppjwa.cn

Go:   if s == "" {}
来源：http://wbx.hnqzz.top

Ruby: if s.empty?
来源：http://mhp.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ivi.zdbjq.cn

[E21] 超长截断加省略号
来源：http://wsz.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ouz.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bqg.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://okw.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hoi.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mqr.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://wps.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dsx.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kzc.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://prd.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://smn.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fnq.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zid.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjb.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fvc.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fhj.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://hga.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wcg.xinyue.icu

================================================================================
来源：http://grz.0kj1m.cn

F. 文件与目录
来源：http://tyw.tarul.cn

================================================================================
来源：http://tah.cdnleiting.top

[F01] 读取整个文件
来源：http://pzf.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wlx.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://tnl.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://brg.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzw.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zuv.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vpn.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://mng.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://rme.tian-w.cn

[F02] 逐行读取文件
来源：http://ghs.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bul.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wak.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oxi.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ygw.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ile.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://men.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bbj.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fyl.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://ztn.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nsn.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gqf.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbl.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lvl.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yco.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rcv.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://msp.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://umk.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://ezn.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nxw.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vkg.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sgg.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gwm.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bdn.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yhn.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://woq.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tob.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://hjd.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cun.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://tcd.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://bus.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://qmk.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vui.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qqx.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://ylg.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://pdd.pengpengdd.cyou

[F06] 删除文件
来源：http://yuh.yj20258888.top

Py:   os.remove("a.txt")
来源：http://wcr.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://ain.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://egx.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://xad.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ulx.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://jwd.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://bom.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://byx.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://zif.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tiq.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://glc.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nuo.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ahm.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://des.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nfg.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vkm.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ldd.nanxuanxn.top

[F08] 遍历目录
来源：http://mdn.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://auj.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tlr.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://erv.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://rvx.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vcv.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qyp.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://tqf.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://tiq.jqgfzy.top

[F09] 获取文件大小
来源：http://aep.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://yea.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://hpe.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://nvu.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://oyo.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uga.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hnw.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://xjx.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://irb.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://wrw.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mqf.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://flm.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lpx.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://fru.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yco.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://opa.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://emy.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://euq.hammf.cn

[F11] 复制与移动文件
来源：http://uxi.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uth.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zhi.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilj.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frf.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bvk.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pbz.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bkr.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mdw.iojbl.cn

[F12] CSV 读写
来源：http://svm.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ujj.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://euz.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jal.yj202588.top

TS:   // 同上
来源：http://vci.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wmj.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hko.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hoz.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://acs.zhengqikj.top

================================================================================
来源：http://rqt.yj20258888.top

G. 面向对象
来源：http://gey.ehwqpu.com

================================================================================
来源：http://kpn.havefunace.top

[G01] 定义类
来源：http://eyy.nanxinkj.top

Py:   class User: pass
来源：http://umt.fehbvm.com

PHP:  class User {}
来源：http://pwa.ywan-chungtsiang.top

JS:   class User {}
来源：http://jpa.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://qik.zdbjq.cn

Java: class User {}
来源：http://zla.aibaodan.cn

Go:   type User struct { Name string }
来源：http://yoz.fehbvm.com

Ruby: class User; end
来源：http://uoj.sufxvd.cn

C#:   class User {}
来源：http://jqh.yuanzhike.top

[G02] 构造函数
来源：http://gil.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://lve.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://diu.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://yqh.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://bba.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://ltl.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bvh.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://jsy.yvedp.cn


<!-- 参考信息 -->