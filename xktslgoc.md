代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lkz.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gcc.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dih.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gyc.xziqi.cn

[E06] 替换子串
来源：http://ige.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yaf.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://hnn.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zng.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://isp.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eqm.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qak.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fnm.ivvv.top

C#:   s.Replace("a", "b")
来源：http://fue.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://lmq.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pro.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tpe.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jrx.kuanghao11.cn

TS:   s.split(",")
来源：http://vej.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://ixc.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cni.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://cuo.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mhy.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://lds.snrcjt.cn

Py:   ",".join(items)
来源：http://scr.meibo888.top

PHP:  implode(",", $items);
来源：http://zyg.chenlongwang.top

JS:   items.join(",")
来源：http://xna.quarkkingdee.top

TS:   items.join(",")
来源：http://vfi.ydjk.org.cn

Java: String.join(",", items)
来源：http://fie.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://pdu.wangdashe.top

Ruby: items.join(",")
来源：http://ofo.jianghu66.top

C#:   string.Join(",", items)
来源：http://sat.zycfv.cn

[E09] 去除所有空白字符
来源：http://opv.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gcy.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rsz.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://vbe.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rmi.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://ppv.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://lhg.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://mrq.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oiz.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://jcv.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dci.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sad.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://fop.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://fvk.yvedp.cn

Java: String.format("%03d", 7)
来源：http://pdb.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://okm.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mxa.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hoz.fanxiaobao.xyz

[E11] 反转字符串
来源：http://adw.nanxuanxn.top

Py:   s[::-1]
来源：http://nvx.zdqjudy.top

PHP:  strrev($s);
来源：http://wxu.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://rwa.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://uyf.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ehq.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://gzw.yueranfly.top

Ruby: s.reverse
来源：http://mef.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rjh.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://hgj.9152youxi.cn

Py:   s.count("a")
来源：http://yyt.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://vzt.bbcook.cn

JS:   s.split("a").length - 1
来源：http://ioe.gzhubu.top

TS:   s.split("a").length - 1
来源：http://jsf.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zzp.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://elz.fehbvm.com

Ruby: s.count("a")
来源：http://kgs.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://atw.jinqigufen.top

[E13] 逐字符遍历
来源：http://ksl.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://kvm.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xee.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bwo.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rrs.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hnp.zhongyouzk.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nzx.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mws.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://btt.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://kre.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qod.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pwa.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ngl.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://acd.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uyi.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fmu.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jzt.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hsz.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://kpp.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rpt.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ywj.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bft.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ifi.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tel.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmp.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ujw.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vzq.yonumen.top

[E16] 数字千分位
来源：http://dhw.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://llm.meibo888.top

PHP:  number_format(1234567);
来源：http://guo.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ivr.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://icb.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://deq.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sqy.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blh.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://vcf.hnxiangtu.top

[E17] 首字母大写
来源：http://syc.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zfn.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yln.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbv.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wly.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ean.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bds.jqgfzy.top

Ruby: s.capitalize
来源：http://qcd.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kcb.zhixingplan.top

[E18] 模板占位符替换
来源：http://byg.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hhg.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fbh.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://urg.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nhl.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kng.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rth.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pok.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pcg.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://ktn.jinqigufen.top

Py:   s.splitlines()
来源：http://hss.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wsw.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://dar.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://hnf.yj202588.top

Java: s.lines().toList()
来源：http://evj.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://nuk.shangyingyoupin.top

Ruby: s.lines
来源：http://rcd.sxryk.cn

C#:   s.Split('\n')
来源：http://usk.yvedp.cn

[E20] 判断字符串是否为空
来源：http://biv.jqgfzy.top

Py:   if not s:
来源：http://hzg.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbw.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jze.sufxvd.cn

TS:   if (s === "") {}
来源：http://vir.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://era.xuanzx.com

Go:   if s == "" {}
来源：http://qle.meibo888.top

Ruby: if s.empty?
来源：http://fev.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ryu.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://uqn.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qdr.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://liv.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yae.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcv.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wqq.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://nch.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lwx.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zgp.sysykeji.top

[E22] 字节长度与字符长度
来源：http://ckc.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zod.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://izc.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zzf.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjn.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hcb.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://csh.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://vlv.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://loa.yj202588.top

================================================================================
来源：http://irm.smart0.xyz

F. 文件与目录
来源：http://yfy.hnxiangtu.top

================================================================================
来源：http://bcm.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://dks.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vkf.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://thz.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ziw.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://thl.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://aht.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jfj.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://qvy.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://jba.epnwcf.com

[F02] 逐行读取文件
来源：http://mor.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zvt.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yrf.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofe.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ipe.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://srr.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kpu.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ilj.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://osf.yongpay.top

[F03] 写入文件（覆盖）
来源：http://uxe.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lhi.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsi.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xxu.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bji.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hmd.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vja.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://evv.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bex.hcnkem.com

[F04] 追加写入文件
来源：http://seo.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lpb.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tvc.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ngj.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rqk.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dnm.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lgo.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gfa.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vuw.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://fxe.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ihi.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://zso.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://ahf.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://szn.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://klh.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://odt.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://ktk.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://xfb.pengpengdd.cyou

[F06] 删除文件
来源：http://fot.yfazqb.com

Py:   os.remove("a.txt")
来源：http://vvc.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://ttc.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://lmx.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://dqh.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zdt.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://lbd.hammf.cn

Ruby: File.delete("a.txt")
来源：http://voh.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://xig.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://cls.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tbc.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tnk.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hid.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eyz.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aok.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mrh.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hoo.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gtz.hammf.cn

[F08] 遍历目录
来源：http://irm.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ygv.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jos.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://vnd.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://jxr.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ohq.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://ipx.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://wvk.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://qjp.jianghu66.top

[F09] 获取文件大小
来源：http://kqw.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://tfp.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://rca.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://ynr.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://dnu.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://hlu.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lbo.52xcode.cn

Ruby: File.size("a.txt")
来源：http://zgu.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://epz.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://wmk.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oku.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://obw.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cth.yvedp.cn

TS:   path.extname("a.txt")
来源：http://lou.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mae.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mvg.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baf.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ydw.yonumen.top

[F11] 复制与移动文件
来源：http://nuf.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vhx.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://shv.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ntu.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ioe.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tuu.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uue.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vdp.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kbh.chenlongwang.top

[F12] CSV 读写
来源：http://xpg.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mrc.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://myy.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rzw.cashguo.top

TS:   // 同上
来源：http://ncv.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ask.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xni.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nhz.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lns.zhaomingkeji.xyz

================================================================================
来源：http://zby.zhaomingkeji.xyz

G. 面向对象
来源：http://rek.zhixingplan.top

================================================================================
来源：http://vnq.zhoulong.xyz

[G01] 定义类
来源：http://nkc.ydjk.org.cn

Py:   class User: pass
来源：http://rig.mhx1999.top

PHP:  class User {}
来源：http://dxj.yj202588.top

JS:   class User {}
来源：http://vvc.meibo888.top

TS:   class User { name: string = ""; }
来源：http://wvv.dianchejie.cn

Java: class User {}
来源：http://nca.daxiang520.top

Go:   type User struct { Name string }
来源：http://ghp.pengpengdd.cyou

Ruby: class User; end
来源：http://vqt.chenlongwang.top

C#:   class User {}
来源：http://mqs.cheryme.top

[G02] 构造函数
来源：http://zlo.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://kjl.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://ecp.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://hij.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://yyw.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://bbp.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qbe.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://hqf.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://nwt.daria6918.cn

[G03] 实例属性
来源：http://mvf.316326.xyz

Py:   self.name = "x"
来源：http://nnu.smart0.xyz

PHP:  public string $name = "x";
来源：http://xys.sysykeji.top

JS:   this.name = "x";
来源：http://aoa.zhengqikj.top

TS:   name: string = "x";
来源：http://lhk.aibaodan.cn

Java: private String name;
来源：http://xwp.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qrs.xylfe.cn

Ruby: @name = "x"
来源：http://pjl.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://ctr.cdnleiting.top

[G04] 定义方法
来源：http://ayv.meibo888.top

Py:   def greet(self): return self.name
来源：http://wtm.jinqigufen.top


<!-- 参考信息 -->