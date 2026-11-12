代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fag.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xtn.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bbc.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cpz.tanke756.top

[E06] 替换子串
来源：http://sch.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iro.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://spj.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ile.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://shv.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://quz.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pfd.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qdn.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://ind.fehbvm.com

[E07] 按分隔符拆分
来源：http://exd.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hxx.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://roy.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lxl.pengpengdd.cyou

TS:   s.split(",")
来源：http://pxl.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gqi.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lne.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://khc.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tli.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://jvr.iojbl.cn

Py:   ",".join(items)
来源：http://tbv.bjfxy.top

PHP:  implode(",", $items);
来源：http://imy.jiagoushi.top

JS:   items.join(",")
来源：http://asl.wangdashe.top

TS:   items.join(",")
来源：http://trg.sweek.top

Java: String.join(",", items)
来源：http://hrb.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://zki.jiagoushi.top

Ruby: items.join(",")
来源：http://rum.52xcode.cn

C#:   string.Join(",", items)
来源：http://sls.yuxming.cn

[E09] 去除所有空白字符
来源：http://rmi.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xth.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ins.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nxd.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://ywa.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://ktk.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hag.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://grb.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ezs.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://yda.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tsg.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hgq.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://gbe.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://irp.yongpay.top

Java: String.format("%03d", 7)
来源：http://zvg.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lqv.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wyp.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ymq.andypj.xyz

[E11] 反转字符串
来源：http://tzx.yongpay.top

Py:   s[::-1]
来源：http://cwd.tanke756.top

PHP:  strrev($s);
来源：http://ldv.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://nli.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://lpa.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://czp.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eue.ivvv.top

Ruby: s.reverse
来源：http://dhj.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iel.vehdjk.com

[E12] 统计某字符出现次数
来源：http://tub.xinyue.icu

Py:   s.count("a")
来源：http://ogh.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://ypg.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://soe.redwolf501.top

TS:   s.split("a").length - 1
来源：http://qlt.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xnj.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://jru.yonumen.top

Ruby: s.count("a")
来源：http://ktw.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://pjy.jinqigufen.top

[E13] 逐字符遍历
来源：http://msz.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://fav.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yww.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kim.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://abm.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xur.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tgp.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://owv.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lay.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://irr.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eym.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://txp.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pvo.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vvb.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jwb.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zyi.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uhn.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bgw.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://eww.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rxe.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rtj.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://piw.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ewi.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uyc.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmj.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jyx.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qev.redwolf501.top

[E16] 数字千分位
来源：http://zop.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://eli.xziqi.cn

PHP:  number_format(1234567);
来源：http://jxd.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wei.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://emb.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bva.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tpg.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rty.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://omy.hcnkem.com

[E17] 首字母大写
来源：http://ugl.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gwp.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://ide.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eru.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rcb.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wxz.c1oappe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uth.wangdashe.top

Ruby: s.capitalize
来源：http://qka.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vlk.gotoacloud.top

[E18] 模板占位符替换
来源：http://uui.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qgd.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dle.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xga.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xdb.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://esa.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gon.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mct.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://irq.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://ane.ydzc1.top

Py:   s.splitlines()
来源：http://wpn.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xxb.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://cib.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://oxa.yfazqb.com

Java: s.lines().toList()
来源：http://dgj.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://rrn.hysaishi.cn

Ruby: s.lines
来源：http://tsj.ppjwa.cn

C#:   s.Split('\n')
来源：http://yfq.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://eya.meibo888.top

Py:   if not s:
来源：http://xun.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jxu.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nfi.zdqjudy.top

TS:   if (s === "") {}
来源：http://wle.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://akt.ivvv.top

Go:   if s == "" {}
来源：http://vmz.yuanzhike.top

Ruby: if s.empty?
来源：http://vuh.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hdb.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://nfj.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kuy.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ylu.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ftd.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hod.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pop.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://qou.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://thh.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gfv.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://tji.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lrb.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rxh.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kzh.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfe.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mph.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jcj.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://ipm.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hzx.tianlin.xyz

================================================================================
来源：http://pds.gotoacloud.top

F. 文件与目录
来源：http://xez.epnwcf.com

================================================================================
来源：http://zti.meibo888.top

[F01] 读取整个文件
来源：http://per.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vsb.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://vew.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rvk.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bbl.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qww.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ieb.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://wxb.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://zha.cashguo.top

[F02] 逐行读取文件
来源：http://sgu.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ido.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iaw.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tzf.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ban.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://omr.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bsx.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nph.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bpn.meibo888.top

[F03] 写入文件（覆盖）
来源：http://vcm.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sph.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://nvk.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gas.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wqq.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tem.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://shg.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://dih.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cno.fktsv.cn

[F04] 追加写入文件
来源：http://kqz.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://beh.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://apa.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kox.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsq.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://opp.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eyb.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wld.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vnd.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://ucc.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jzn.hammf.cn

PHP:  file_exists("a.txt");
来源：http://xiv.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://wyt.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://kbw.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qvj.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://djf.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://fya.tanke756.top

C#:   File.Exists("a.txt")
来源：http://mcm.xinyue.icu

[F06] 删除文件
来源：http://wtq.52xcode.cn

Py:   os.remove("a.txt")
来源：http://uur.316326.xyz

PHP:  unlink("a.txt");
来源：http://wth.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://aju.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vuh.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ifa.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://llx.316326.xyz

Ruby: File.delete("a.txt")
来源：http://vby.pycfn.com

C#:   File.Delete("a.txt");
来源：http://gxl.ivvv.top

[F07] 创建目录（含多级）
来源：http://akn.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pvu.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lpk.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twj.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgr.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://btk.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ruy.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://djx.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dvl.gotoacloud.top

[F08] 遍历目录
来源：http://gwl.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmb.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uwi.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://izl.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://bzu.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ytv.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yve.c1oappe.top

Ruby: Dir.children("dir")
来源：http://wvj.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://jbc.chenjidiqi.icu

[F09] 获取文件大小
来源：http://oad.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://akt.xuanzx.com

PHP:  filesize("a.txt");
来源：http://wqc.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://dql.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://aar.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://rgt.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kod.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://gqb.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://hcf.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://bbo.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twf.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hoe.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hug.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://lfe.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwz.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://via.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tyd.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gwz.zhoulong.xyz

[F11] 复制与移动文件
来源：http://odh.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ieb.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ilj.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pyz.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmb.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sap.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wlf.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qln.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uuy.xuanzx.com

[F12] CSV 读写
来源：http://pme.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fvq.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qbi.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dmb.svipenyu.cn

TS:   // 同上
来源：http://wsu.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ttp.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dvs.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cbu.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ykn.vehdjk.com

================================================================================
来源：http://naw.cdnleiting.top

G. 面向对象
来源：http://shq.jiagoushi.top

================================================================================
来源：http://gqy.cdnleiting.top

[G01] 定义类
来源：http://lpc.vqdsnc.cn

Py:   class User: pass
来源：http://vtj.gaohongyu789.top

PHP:  class User {}
来源：http://hiq.svipenyu.cn

JS:   class User {}
来源：http://rwd.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://nvr.jqgfzy.top

Java: class User {}
来源：http://ugw.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://etl.yfazqb.com

Ruby: class User; end
来源：http://zti.uphjek.com

C#:   class User {}
来源：http://frn.yuxming.cn

[G02] 构造函数
来源：http://ecp.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://tdz.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://jbd.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://ttu.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://fvw.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://ueq.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bcu.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://brw.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://nur.bjfxy.top

[G03] 实例属性
来源：http://igl.nanxinkj.top

Py:   self.name = "x"
来源：http://bvp.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://zwm.hnxiangtu.top

JS:   this.name = "x";
来源：http://nbf.gaohongyu789.top

TS:   name: string = "x";
来源：http://dqt.yuxming.cn

Java: private String name;
来源：http://uem.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qyh.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://eqd.shangyingyoupin.top

C#:   public string Name { get; set; } = "x";
来源：http://kko.chenzaomai.com

[G04] 定义方法
来源：http://pnh.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://vzu.dashuyun.cn


<!-- 参考信息 -->