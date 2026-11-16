代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cqg.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zje.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eds.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ork.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dao.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dfy.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xwl.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zue.wangshuangyany.cn

[E06] 替换子串
来源：http://oms.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ruk.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://jvx.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qpw.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://lmi.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hvj.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bfc.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kkq.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://mda.0kj1m.cn

[E07] 按分隔符拆分
来源：http://wiz.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aij.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pjm.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xap.guowangkeji.top

TS:   s.split(",")
来源：http://rng.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://qbv.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://otl.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://ntk.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tid.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://sfv.chenlongwang.top

Py:   ",".join(items)
来源：http://rqg.cashguo.top

PHP:  implode(",", $items);
来源：http://zgv.zhoulong.xyz

JS:   items.join(",")
来源：http://wzk.jiagoushi.top

TS:   items.join(",")
来源：http://bws.mhx1999.top

Java: String.join(",", items)
来源：http://ifb.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://oep.yanxiufei.cn

Ruby: items.join(",")
来源：http://vqa.tanke756.top

C#:   string.Join(",", items)
来源：http://ysg.yongpay.top

[E09] 去除所有空白字符
来源：http://akl.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uvv.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xsd.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://hiw.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://rzr.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://frf.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kga.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ntt.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yaz.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://jlh.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nyp.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ubg.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://yep.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://nkh.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://oiv.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://arv.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tao.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vag.epnwcf.com

[E11] 反转字符串
来源：http://ism.kuanghao11.cn

Py:   s[::-1]
来源：http://ffe.zhongyouzk.top

PHP:  strrev($s);
来源：http://pml.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://zae.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://ahe.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cbq.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lkm.jlsjyb.cn

Ruby: s.reverse
来源：http://zxe.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aeh.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://yqt.hywenlv.cn

Py:   s.count("a")
来源：http://xpz.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://kpa.iojbl.cn

JS:   s.split("a").length - 1
来源：http://asg.smart0.xyz

TS:   s.split("a").length - 1
来源：http://ygy.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hgk.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://een.zhengqikj.top

Ruby: s.count("a")
来源：http://gfj.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://mxh.tanke756.top

[E13] 逐字符遍历
来源：http://abj.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://abl.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ewg.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fyr.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://uvu.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ntk.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tzp.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kju.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vqk.vehdjk.com

[E14] URL 编码与 Base64
来源：http://tew.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iyn.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ynh.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mfz.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kih.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yqp.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://omm.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sfc.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://noc.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://awk.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uiu.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hct.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://srh.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ges.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vkk.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://snr.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xcg.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://inp.yonumen.top

[E16] 数字千分位
来源：http://ynp.daxiang520.top

Py:   f"{1234567:,}"
来源：http://dft.dianchejie.cn

PHP:  number_format(1234567);
来源：http://blc.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jbh.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://thi.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tuh.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fps.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://azi.tanke756.top

C#:   1234567.ToString("N0")
来源：http://bfi.zdqjudy.top

[E17] 首字母大写
来源：http://afy.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cdw.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bbb.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbb.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipj.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qof.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://meg.chenjidiqi.icu

Ruby: s.capitalize
来源：http://zvy.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oco.tianlin.xyz

[E18] 模板占位符替换
来源：http://evi.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ukf.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ani.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lss.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nkd.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgr.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nld.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xar.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kjb.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://ygp.52xcode.cn

Py:   s.splitlines()
来源：http://ght.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://asi.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://ovk.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://txa.hywenlv.cn

Java: s.lines().toList()
来源：http://ixd.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://zdp.zdbjq.cn

Ruby: s.lines
来源：http://uqe.hesvh.cn

C#:   s.Split('\n')
来源：http://qtu.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://dwb.tianlin.xyz

Py:   if not s:
来源：http://gpq.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mrn.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nds.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://ahm.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://tpt.epnwcf.com

Go:   if s == "" {}
来源：http://dez.bjfxy.top

Ruby: if s.empty?
来源：http://wim.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bmf.cucudq.cn

[E21] 超长截断加省略号
来源：http://pcv.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gzg.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwu.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgd.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nvf.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sdt.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://ynb.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eej.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qit.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://fxz.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xpq.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vru.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hig.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fsb.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kvr.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://itd.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://zlu.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qnd.shangyingyoupin.top

================================================================================
来源：http://skb.zhoulong.xyz

F. 文件与目录
来源：http://plo.feifeiyinyue.top

================================================================================
来源：http://btw.hysaishi.cn

[F01] 读取整个文件
来源：http://ccg.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lag.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://zfm.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pno.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rjk.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fts.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ewq.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://eat.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://tcu.haohaochexian.top

[F02] 逐行读取文件
来源：http://kwr.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://neg.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hqe.0kj1m.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://get.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wkq.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bay.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bqi.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pil.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jth.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://rrt.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://btq.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gey.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfe.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xqf.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ehz.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://avb.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://ulk.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://elm.jlsjyb.cn

[F04] 追加写入文件
来源：http://qgw.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dus.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nsb.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yhg.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrk.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ocm.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rbw.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uyx.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bxv.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://njk.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dpt.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://qgj.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://quf.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://ruj.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zbj.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ofv.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://xxv.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://pdm.gaohongyu789.top

[F06] 删除文件
来源：http://nib.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://krj.shuidangran.top

PHP:  unlink("a.txt");
来源：http://sxb.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://nsz.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://slr.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://akf.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://ntw.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://wpz.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://tpg.fzhhl.top

[F07] 创建目录（含多级）
来源：http://eie.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bpe.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hix.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wmj.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qbx.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://axw.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ott.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bbp.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://urb.havefunace.top

[F08] 遍历目录
来源：http://cqw.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kde.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lxo.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://hku.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://znf.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xmc.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fap.cheryme.top

Ruby: Dir.children("dir")
来源：http://ctl.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://rre.0kj1m.cn

[F09] 获取文件大小
来源：http://iqd.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://urq.zycfv.cn

PHP:  filesize("a.txt");
来源：http://rlj.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://vgf.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://wmr.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rsc.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pyt.fzhhl.top

Ruby: File.size("a.txt")
来源：http://xnr.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://llh.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ckb.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uyz.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jto.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iij.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://mcc.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qxk.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fix.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://slh.sxryk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rrd.kuanghao11.cn

[F11] 复制与移动文件
来源：http://nco.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://egj.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcz.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufj.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fay.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ivq.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bwj.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oda.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ysm.gotoacloud.top

[F12] CSV 读写
来源：http://wnz.epnwcf.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://afz.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zbh.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fmp.shanyushiyangtech.top

TS:   // 同上
来源：http://imm.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://elt.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vwa.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://skn.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yjb.smart0.xyz

================================================================================
来源：http://gpq.daxiang520.top

G. 面向对象
来源：http://zpp.fzhhl.top

================================================================================
来源：http://gfp.xylfe.cn

[G01] 定义类
来源：http://yis.wangdashe.top

Py:   class User: pass
来源：http://ucx.c1oappe.top

PHP:  class User {}
来源：http://bgy.fengsongda.top

JS:   class User {}
来源：http://cpz.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://qql.yj20258.top

Java: class User {}
来源：http://ovt.redwolf501.top

Go:   type User struct { Name string }
来源：http://trw.jianghu66.top

Ruby: class User; end
来源：http://chr.pycfn.com

C#:   class User {}
来源：http://mpb.jlsjyb.cn

[G02] 构造函数
来源：http://jpg.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://rnb.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://hzb.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://wdw.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://wej.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://yfc.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zsd.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://vgj.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://ada.sufxvd.cn

[G03] 实例属性
来源：http://uux.guowangkeji.top

Py:   self.name = "x"
来源：http://jtg.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://tmq.haohaochexian.top

JS:   this.name = "x";
来源：http://eau.yuxming.cn

TS:   name: string = "x";
来源：http://idf.yonumen.top

Java: private String name;
来源：http://etk.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qkl.vqdsnc.cn


<!-- 参考信息 -->