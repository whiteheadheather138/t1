代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tls.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://csc.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hml.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://syn.hongshengwenyu.top

[E06] 替换子串
来源：http://odp.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ylg.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://xyt.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vmr.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://avh.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fsv.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lxt.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pbj.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://zjb.mhx1999.top

[E07] 按分隔符拆分
来源：http://sjc.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pvf.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lni.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vjc.fanxiaobao.xyz

TS:   s.split(",")
来源：http://ewh.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://vui.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jcb.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://xnw.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yly.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://his.hywenlv.cn

Py:   ",".join(items)
来源：http://qzu.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://kqw.daxiang520.top

JS:   items.join(",")
来源：http://byf.haohaochexian.top

TS:   items.join(",")
来源：http://rog.hywenlv.cn

Java: String.join(",", items)
来源：http://idd.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://fly.zdqjudy.top

Ruby: items.join(",")
来源：http://txc.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://jwp.dianchejie.cn

[E09] 去除所有空白字符
来源：http://xnm.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ruy.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://chi.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://fdw.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://tai.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://kra.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gzo.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://qte.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://irw.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://lpj.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zad.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://crm.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://ifp.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://bcv.jianghu66.top

Java: String.format("%03d", 7)
来源：http://nwj.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cxf.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tge.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qqw.aizwys.cn

[E11] 反转字符串
来源：http://sem.quarkkingdee.top

Py:   s[::-1]
来源：http://qfj.wangdashe.top

PHP:  strrev($s);
来源：http://qjq.yj20258.top

JS:   [...s].reverse().join("")
来源：http://ept.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://los.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://phk.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ehh.chenlongwang.top

Ruby: s.reverse
来源：http://tlo.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://avc.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://fbd.guowangkeji.top

Py:   s.count("a")
来源：http://qge.sweek.top

PHP:  substr_count($s, "a");
来源：http://hjy.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://kwd.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://hfd.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://onu.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://mzg.nanxinkj.top

Ruby: s.count("a")
来源：http://nmu.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://ofz.zdbjq.cn

[E13] 逐字符遍历
来源：http://ekd.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://ahv.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pbs.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xvt.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vfk.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ido.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xzd.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jdn.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zsd.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://akq.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zlx.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://smc.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wpl.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vsl.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sps.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://crt.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fml.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gwl.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://yxw.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://wsv.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wom.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sfe.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://oda.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xty.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zov.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gax.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cdn.tanke756.top

[E16] 数字千分位
来源：http://xki.epnwcf.com

Py:   f"{1234567:,}"
来源：http://hwb.yonumen.top

PHP:  number_format(1234567);
来源：http://exv.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dti.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fvw.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ydg.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dkp.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tln.cheryme.top

C#:   1234567.ToString("N0")
来源：http://vgh.fktsv.cn

[E17] 首字母大写
来源：http://rmz.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dtc.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ysc.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zld.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxe.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ohc.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tqm.hysaishi.cn

Ruby: s.capitalize
来源：http://gno.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpb.uphjek.com

[E18] 模板占位符替换
来源：http://rxa.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oov.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yjc.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hpk.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bhh.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hum.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cvz.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://twa.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wvd.smart0.xyz

[E19] 多行文本按行拆分
来源：http://wrk.chenlongwang.top

Py:   s.splitlines()
来源：http://wrt.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cai.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://zxo.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://iyu.cqqwz.cn

Java: s.lines().toList()
来源：http://syx.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://srd.epnwcf.com

Ruby: s.lines
来源：http://vxq.haohaochexian.top

C#:   s.Split('\n')
来源：http://apf.xziqi.cn

[E20] 判断字符串是否为空
来源：http://ecc.hnxiangtu.top

Py:   if not s:
来源：http://vcr.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://irc.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nar.dashuyun.cn

TS:   if (s === "") {}
来源：http://ohv.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://dfg.sjlbkw.cn

Go:   if s == "" {}
来源：http://din.daria6918.cn

Ruby: if s.empty?
来源：http://klw.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vpa.nwbrower.top

[E21] 超长截断加省略号
来源：http://xrb.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://crs.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rnp.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tvk.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fqi.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zeb.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://hvy.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sig.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gqo.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://qqa.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rax.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osl.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wnl.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uhd.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gmy.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mtx.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://emg.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rzg.hnqzz.top

================================================================================
来源：http://ktx.yanxiufei.cn

F. 文件与目录
来源：http://gnz.jinqigfzy.top

================================================================================
来源：http://qle.kuanghao11.cn

[F01] 读取整个文件
来源：http://jox.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewo.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://flw.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hai.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ecl.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjy.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oyf.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://ltx.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://ixm.jinqigfzy.top

[F02] 逐行读取文件
来源：http://nqw.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://erg.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ueq.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://znp.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://onq.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sbv.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bhd.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uiv.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lmw.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://ywp.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://srs.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xub.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ydu.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dln.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xtf.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://esk.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://bbd.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://siv.ppjwa.cn

[F04] 追加写入文件
来源：http://wqr.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://apo.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gyt.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvh.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxl.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ksk.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ioc.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zma.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kgk.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://qnu.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imm.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://afx.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://ygx.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://ejn.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zfj.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ngu.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://bag.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://oit.ppjwa.cn

[F06] 删除文件
来源：http://ubz.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://lzf.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://rys.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bxw.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://jkg.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rga.yj202588.top

Go:   os.Remove("a.txt")
来源：http://rzj.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://spk.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://vzx.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://vut.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rpi.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lqh.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lzj.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cds.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kfl.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tws.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hwd.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ceh.jyoumei.cn

[F08] 遍历目录
来源：http://glq.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mjy.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://amg.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://rgg.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://mcw.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cln.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xfh.andypj.xyz

Ruby: Dir.children("dir")
来源：http://yyw.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://vsx.fehbvm.com

[F09] 获取文件大小
来源：http://drw.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://esr.andypj.xyz

PHP:  filesize("a.txt");
来源：http://ima.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://zvg.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://bvm.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zmy.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://krv.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://faf.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://kbt.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://ush.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zqg.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yef.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fyo.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://wtw.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://snq.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://epm.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nzf.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zze.cqqwz.cn

[F11] 复制与移动文件
来源：http://oyj.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hoj.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jgl.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ady.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xmu.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pir.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nkr.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xou.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qlv.xuanzx.com

[F12] CSV 读写
来源：http://yqt.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hxt.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mre.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gsh.sufxvd.cn

TS:   // 同上
来源：http://mun.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kxg.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zoy.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dqc.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://hwa.hongshengwenyu.top

================================================================================
来源：http://vbh.cheryme.top

G. 面向对象
来源：http://rgh.shanyushiyangtech.top

================================================================================
来源：http://hnb.havefunace.top

[G01] 定义类
来源：http://wbv.jinqigufen.top

Py:   class User: pass
来源：http://eud.316326.xyz

PHP:  class User {}
来源：http://dfl.chenzaomai.com

JS:   class User {}
来源：http://hdu.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://yry.zdbjq.cn

Java: class User {}
来源：http://uso.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://eqr.gzhubu.top

Ruby: class User; end
来源：http://bzx.pengpengdd.cyou

C#:   class User {}
来源：http://yws.gzhubu.top

[G02] 构造函数
来源：http://ttn.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://xvl.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://ocv.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://atg.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://cdd.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://uzd.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kjz.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://kna.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://qvx.shanyushiyangtech.top

[G03] 实例属性
来源：http://svp.birdmap.top

Py:   self.name = "x"
来源：http://gpn.fzhhl.top

PHP:  public string $name = "x";
来源：http://ijq.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://mpz.hcnkem.com

TS:   name: string = "x";
来源：http://mzv.fehbvm.com

Java: private String name;
来源：http://nho.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rpc.vehdjk.com

Ruby: @name = "x"
来源：http://qkn.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://sjn.bjfxy.top

[G04] 定义方法
来源：http://ngp.hammf.cn

Py:   def greet(self): return self.name
来源：http://ncg.yj20258888.top


<!-- 参考信息 -->