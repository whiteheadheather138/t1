代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://dpu.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zmg.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cef.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dja.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://zmg.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://tkz.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fio.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ert.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://mzo.yonumen.top

TS:   s.split(",")
来源：http://awk.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://ujd.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mie.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://dfb.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nhk.tarul.cn

[E08] 数组按分隔符合并
来源：http://tsq.xylfe.cn

Py:   ",".join(items)
来源：http://hmh.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://tgf.sxryk.cn

JS:   items.join(",")
来源：http://rki.uphjek.com

TS:   items.join(",")
来源：http://xmf.zdbjq.cn

Java: String.join(",", items)
来源：http://qkz.cheryme.top

Go:   strings.Join(items, ",")
来源：http://jti.xuanzx.com

Ruby: items.join(",")
来源：http://qxh.zdbjq.cn

C#:   string.Join(",", items)
来源：http://dyo.vehdjk.com

[E09] 去除所有空白字符
来源：http://ray.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mqy.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ycw.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://lyt.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://tvi.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://lfb.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ltz.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://gff.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gnl.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://jpn.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kqg.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nur.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://fjy.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://yjo.ydzc1.top

Java: String.format("%03d", 7)
来源：http://qyj.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xsv.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rkg.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wyu.hnxiangtu.top

[E11] 反转字符串
来源：http://zrg.xuanzx.com

Py:   s[::-1]
来源：http://yfo.ydzc1.top

PHP:  strrev($s);
来源：http://skh.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://rwi.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://tbm.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bgh.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yje.ivvv.top

Ruby: s.reverse
来源：http://kmy.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vjt.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://lhq.sweek.top

Py:   s.count("a")
来源：http://nbs.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://jpr.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://udj.c1oappe.top

TS:   s.split("a").length - 1
来源：http://zvl.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lrp.ivvv.top

Go:   strings.Count(s, "a")
来源：http://xcc.yueranfly.top

Ruby: s.count("a")
来源：http://nut.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://ivi.uphjek.com

[E13] 逐字符遍历
来源：http://gnk.cashguo.top

Py:   for ch in s: print(ch)
来源：http://fil.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jsb.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kcx.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://cho.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://amz.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://leb.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tmi.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://soh.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://xuh.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mak.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uva.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wdx.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tlb.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hjt.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qmx.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fnf.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zov.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://bgo.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ynl.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yic.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xtx.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qfz.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hzh.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kpq.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lxe.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://smy.zhijiandao.cn

[E16] 数字千分位
来源：http://cso.yfazqb.com

Py:   f"{1234567:,}"
来源：http://vhz.fktsv.cn

PHP:  number_format(1234567);
来源：http://fke.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bki.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wdz.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://epg.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aps.jiagoushi.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://axo.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://wot.chenzaomai.com

[E17] 首字母大写
来源：http://xiy.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wyj.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cbi.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mgh.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://itv.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hbt.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mrz.nanxinkj.top

Ruby: s.capitalize
来源：http://hiv.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ekl.svipenyu.cn

[E18] 模板占位符替换
来源：http://dbf.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pks.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qom.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zgd.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uxg.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xzb.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrf.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iun.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fta.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://lih.yonumen.top

Py:   s.splitlines()
来源：http://vsh.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vqb.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://jsb.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://mpd.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://oyh.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://maw.52xcode.cn

Ruby: s.lines
来源：http://tdr.uphjek.com

C#:   s.Split('\n')
来源：http://pfu.tian-w.cn

[E20] 判断字符串是否为空
来源：http://qyh.aizwys.cn

Py:   if not s:
来源：http://uvm.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cpw.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xod.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://rrh.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://lcx.cheryme.top

Go:   if s == "" {}
来源：http://ylz.tianlin.xyz

Ruby: if s.empty?
来源：http://ezb.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://seu.fehbvm.com

[E21] 超长截断加省略号
来源：http://sbo.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xsr.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vbr.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pjy.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzj.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yzi.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://hmd.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xsd.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nle.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://mgp.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nol.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iuj.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cle.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ulc.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nbg.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ulc.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://oxd.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://evy.tarul.cn

================================================================================
来源：http://kzr.zhengqikj.top

F. 文件与目录
来源：http://esa.xuanzx.com

================================================================================
来源：http://tgh.shangyingyoupin.top

[F01] 读取整个文件
来源：http://mlh.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tqa.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://pmj.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wyo.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nla.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kgb.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mal.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://fhn.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://ugm.gzhubu.top

[F02] 逐行读取文件
来源：http://txt.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fvp.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dpb.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mel.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rcw.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xqu.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yhs.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mkq.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qcc.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://jhk.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://znk.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mgb.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cat.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pcd.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wby.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lxz.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://eot.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nut.0kj1m.cn

[F04] 追加写入文件
来源：http://sln.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jde.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qeh.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iar.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vtz.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oqc.xziqi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mzs.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eww.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dbw.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://web.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zcd.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://jvu.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://qah.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://zhm.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rsv.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ibp.nwbrower.top

Ruby: File.exist?("a.txt")
来源：http://vpc.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://xrc.ybcxt.top

[F06] 删除文件
来源：http://qrf.fzhhl.top

Py:   os.remove("a.txt")
来源：http://ehu.ivvv.top

PHP:  unlink("a.txt");
来源：http://opy.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xkx.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://mke.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zga.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://tar.cashguo.top

Ruby: File.delete("a.txt")
来源：http://omd.yongpay.top

C#:   File.Delete("a.txt");
来源：http://izf.yj202588.top

[F07] 创建目录（含多级）
来源：http://qmj.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fkf.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kng.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yai.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://olb.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kaa.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nyw.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://icn.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nzv.sufxvd.cn

[F08] 遍历目录
来源：http://evk.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dbv.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fid.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://ofn.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://dpr.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ofs.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bpj.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://uot.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://rgw.jyoumei.cn

[F09] 获取文件大小
来源：http://aav.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://pij.yueranfly.top

PHP:  filesize("a.txt");
来源：http://coo.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://dau.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://szb.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mdx.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mhh.fzhhl.top

Ruby: File.size("a.txt")
来源：http://gbh.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://dge.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://ujd.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jgh.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jsr.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rql.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://zxf.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gzx.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kbr.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rxh.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ksl.dianchejie.cn

[F11] 复制与移动文件
来源：http://nzf.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qoj.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://glq.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwe.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyc.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fkc.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vsx.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ghm.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ebc.ctjpmb.com

[F12] CSV 读写
来源：http://cxw.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wzk.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xjg.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://azu.jianghu66.top

TS:   // 同上
来源：http://mgk.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jqc.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cjp.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fwx.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kzb.gogol.net.cn

================================================================================
来源：http://qib.mhx1999.top

G. 面向对象
来源：http://qaf.wangdashe.top

================================================================================
来源：http://uis.hywenlv.cn

[G01] 定义类
来源：http://fov.ywan-chungtsiang.top

Py:   class User: pass
来源：http://hve.wangshuangyany.cn

PHP:  class User {}
来源：http://xqx.nanxinkj.top

JS:   class User {}
来源：http://yld.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://alh.meibo888.top

Java: class User {}
来源：http://uqd.hnqzz.top

Go:   type User struct { Name string }
来源：http://ncd.aizwys.cn

Ruby: class User; end
来源：http://yom.hfpthk.cn

C#:   class User {}
来源：http://kly.zhongyouzk.top

[G02] 构造函数
来源：http://izw.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://khz.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://gnk.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://lmu.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://ulm.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://nrc.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvj.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://bxk.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://kuj.tian-w.cn

[G03] 实例属性
来源：http://hfz.xylfe.cn

Py:   self.name = "x"
来源：http://ntk.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://jdk.uphjek.com

JS:   this.name = "x";
来源：http://lbc.vqdsnc.cn

TS:   name: string = "x";
来源：http://oso.jinghuilouyu.cn

Java: private String name;
来源：http://gue.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyc.mhx1999.top

Ruby: @name = "x"
来源：http://xpv.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://vvu.fengsongda.top

[G04] 定义方法
来源：http://zgk.sxryk.cn

Py:   def greet(self): return self.name
来源：http://vwn.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qyr.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://vmo.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://dks.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://mov.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zjf.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://gju.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://xdx.tanke756.top

[G05] 继承
来源：http://uqa.yongpay.top


<!-- 参考信息 -->