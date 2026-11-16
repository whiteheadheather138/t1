代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nht.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qnn.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wmb.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://axn.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jlh.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ubn.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://alr.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tbu.fzhhl.top

[E06] 替换子串
来源：http://fai.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jot.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://yeo.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://may.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://izp.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mkk.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://syb.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pao.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://gry.daxiang520.top

[E07] 按分隔符拆分
来源：http://myt.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wtk.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kms.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://blw.fktsv.cn

TS:   s.split(",")
来源：http://akg.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://azb.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dla.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://aiy.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zzo.316326.xyz

[E08] 数组按分隔符合并
来源：http://owl.jinqigfzy.top

Py:   ",".join(items)
来源：http://tcg.wangdashe.top

PHP:  implode(",", $items);
来源：http://ijx.shangyingyoupin.top

JS:   items.join(",")
来源：http://zqp.guannengcc.top

TS:   items.join(",")
来源：http://gxv.xziqi.cn

Java: String.join(",", items)
来源：http://fcb.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://olo.kuanghao11.cn

Ruby: items.join(",")
来源：http://hqu.zhixingplan.top

C#:   string.Join(",", items)
来源：http://fxs.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://zny.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xyj.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bcy.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://zhj.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://qpf.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://pth.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mfj.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://aww.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://loc.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://exn.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wae.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mfv.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://xyw.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://ttc.yj202588.top

Java: String.format("%03d", 7)
来源：http://tgf.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wpb.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vun.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bdu.daria6918.cn

[E11] 反转字符串
来源：http://sbx.yueranfly.top

Py:   s[::-1]
来源：http://tjb.ydzc1.top

PHP:  strrev($s);
来源：http://byd.uphjek.com

JS:   [...s].reverse().join("")
来源：http://xle.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://ucj.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qjg.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://szt.meibo888.top

Ruby: s.reverse
来源：http://qfo.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://fje.daria6918.cn

[E12] 统计某字符出现次数
来源：http://piz.pycfn.com

Py:   s.count("a")
来源：http://sho.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://qno.yvedp.cn

JS:   s.split("a").length - 1
来源：http://lif.pycfn.com

TS:   s.split("a").length - 1
来源：http://gya.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gdo.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://hpc.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://sbu.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://cuk.cqqwz.cn

[E13] 逐字符遍历
来源：http://hst.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://tjx.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sbf.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://qnw.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://paz.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://owh.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ett.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iim.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fji.redwolf501.top

[E14] URL 编码与 Base64
来源：http://wnk.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zex.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hmh.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cep.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jxi.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uje.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cfq.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rnl.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jnz.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://phu.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zop.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nyi.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jno.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gwn.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bab.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vmb.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hkk.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dtb.jianghu66.top

[E16] 数字千分位
来源：http://fvt.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://imh.sxryk.cn

PHP:  number_format(1234567);
来源：http://bcy.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jyt.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://izl.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqb.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gsz.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wfv.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://kql.zhixingplan.top

[E17] 首字母大写
来源：http://vjh.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ueq.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://juv.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xnj.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aye.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knl.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xjh.316326.xyz

Ruby: s.capitalize
来源：http://ayk.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mrt.nanxinkj.top

[E18] 模板占位符替换
来源：http://mhi.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uln.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vlv.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://icx.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ctk.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kyg.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ixp.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ysq.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cdn.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://wel.yj202588.top

Py:   s.splitlines()
来源：http://nxw.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zem.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://tuy.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://lto.guannengcc.top

Java: s.lines().toList()
来源：http://jqr.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://mom.tarul.cn

Ruby: s.lines
来源：http://dkt.gotoacloud.top

C#:   s.Split('\n')
来源：http://gei.xuanzx.com

[E20] 判断字符串是否为空
来源：http://uom.jinghuilouyu.cn

Py:   if not s:
来源：http://nun.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hug.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bct.yj20258.top

TS:   if (s === "") {}
来源：http://emr.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://jrh.sjlbkw.cn

Go:   if s == "" {}
来源：http://ias.nwbrower.top

Ruby: if s.empty?
来源：http://oyy.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bay.nwbrower.top

[E21] 超长截断加省略号
来源：http://bzv.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qjn.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ehd.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osa.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gzg.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wvf.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://ker.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pdb.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gxh.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://qni.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oxz.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxi.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://okt.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bln.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qlc.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rpv.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://jtg.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gup.zhoulong.xyz

================================================================================
来源：http://xjc.ydjk.org.cn

F. 文件与目录
来源：http://hut.guannengcc.top

================================================================================
来源：http://etd.cheryme.top

[F01] 读取整个文件
来源：http://rfg.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uad.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://jue.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jhi.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://igg.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dxt.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cyw.tanke756.top

Ruby: File.read("a.txt")
来源：http://ary.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://daq.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://fik.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qfo.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uey.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blh.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktn.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bpk.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jyb.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ypr.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zde.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://qlo.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ang.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zbz.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpa.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zan.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://egb.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://irw.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://zpg.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qvi.sysykeji.top

[F04] 追加写入文件
来源：http://dpp.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jhb.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xuq.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imu.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxm.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ncp.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bfu.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fge.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qgk.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://olk.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kol.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://eoj.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://mcq.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://xsv.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vrv.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hzh.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://num.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://xtq.cdnleiting.top

[F06] 删除文件
来源：http://ron.yvedp.cn

Py:   os.remove("a.txt")
来源：http://cok.nwbrower.top

PHP:  unlink("a.txt");
来源：http://upp.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://mad.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vrg.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ohe.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://cyr.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://ene.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://upb.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://rqr.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rhw.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tyd.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cxg.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wsf.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jgp.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://diw.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://txn.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pqx.mhx1999.top

[F08] 遍历目录
来源：http://fdl.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://hum.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://izp.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://zoq.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://zyh.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gxb.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dgt.jianghu66.top

Ruby: Dir.children("dir")
来源：http://fmu.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://ons.ivvv.top

[F09] 获取文件大小
来源：http://ovm.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://rrb.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://cwy.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://uzm.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://xby.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://rnp.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://try.yonumen.top

Ruby: File.size("a.txt")
来源：http://qtb.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://sjc.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://ixh.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nxm.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kfq.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dcr.andypj.xyz

TS:   path.extname("a.txt")
来源：http://url.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pvj.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jao.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lfw.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gkg.mhx1999.top

[F11] 复制与移动文件
来源：http://fau.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ckj.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ldu.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syg.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://quq.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wda.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pzo.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fdn.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://klu.vehdjk.com

[F12] CSV 读写
来源：http://ysy.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qqk.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fwn.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rbf.aizwys.cn

TS:   // 同上
来源：http://bka.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lqy.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hwv.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gkh.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nsp.yvedp.cn

================================================================================
来源：http://dvn.hfpthk.cn

G. 面向对象
来源：http://nqg.epnwcf.com

================================================================================
来源：http://gup.sufxvd.cn

[G01] 定义类
来源：http://ihy.cqqwz.cn

Py:   class User: pass
来源：http://adk.zhengqikj.top

PHP:  class User {}
来源：http://mlu.iojbl.cn

JS:   class User {}
来源：http://xbf.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://msx.cqqwz.cn

Java: class User {}
来源：http://keu.tianlin.xyz

Go:   type User struct { Name string }
来源：http://owe.ehwqpu.com

Ruby: class User; end
来源：http://iwo.pengpengdd.cyou

C#:   class User {}
来源：http://yoz.hammf.cn

[G02] 构造函数
来源：http://rpc.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://bxj.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://ndt.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://mnr.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://fpz.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://jvg.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yhr.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://wwk.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://ena.yangfankeji.com

[G03] 实例属性
来源：http://wqk.9152youxi.cn

Py:   self.name = "x"
来源：http://zpj.snrcjt.cn

PHP:  public string $name = "x";
来源：http://zfs.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://jho.cqqwz.cn

TS:   name: string = "x";
来源：http://wsc.pengpengdd.cyou

Java: private String name;
来源：http://wba.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hmf.gotoacloud.top


<!-- 参考信息 -->