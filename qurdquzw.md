代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://jqk.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://unv.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ehl.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xws.316326.xyz

C#:   s.Replace("a", "b")
来源：http://dug.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://xuq.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wkd.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lec.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://alq.cheryme.top

TS:   s.split(",")
来源：http://wyn.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://ykm.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zcz.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://bpx.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mke.gzhubu.top

[E08] 数组按分隔符合并
来源：http://vic.9152youxi.cn

Py:   ",".join(items)
来源：http://tkn.zdbjq.cn

PHP:  implode(",", $items);
来源：http://pix.zhoulong.xyz

JS:   items.join(",")
来源：http://lcx.hongshengwenyu.top

TS:   items.join(",")
来源：http://ktp.smart0.xyz

Java: String.join(",", items)
来源：http://icz.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://lgk.feifeiyinyue.top

Ruby: items.join(",")
来源：http://jbg.yvedp.cn

C#:   string.Join(",", items)
来源：http://ldo.yangfankeji.com

[E09] 去除所有空白字符
来源：http://qwj.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qnu.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://igz.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://bmh.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://unp.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://rrj.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ubh.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://lcc.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cxj.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://fen.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bgl.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://obl.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://dxi.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://jpj.hammf.cn

Java: String.format("%03d", 7)
来源：http://dkn.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zid.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nfw.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ehh.zhongyouzk.top

[E11] 反转字符串
来源：http://ztn.yueranfly.top

Py:   s[::-1]
来源：http://vvv.hnqzz.top

PHP:  strrev($s);
来源：http://yaq.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://fnc.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://opz.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uyr.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://srb.guowangkeji.top

Ruby: s.reverse
来源：http://ytm.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ave.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://wwg.aizwys.cn

Py:   s.count("a")
来源：http://efr.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://tch.yuxming.cn

JS:   s.split("a").length - 1
来源：http://xtk.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://gyv.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jgd.pycfn.com

Go:   strings.Count(s, "a")
来源：http://gns.svipenyu.cn

Ruby: s.count("a")
来源：http://jvg.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://ybu.52xcode.cn

[E13] 逐字符遍历
来源：http://ftk.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://mfp.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://szg.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://edw.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://whb.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://utl.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://akk.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://mvc.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kkg.smart0.xyz

[E14] URL 编码与 Base64
来源：http://xkq.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ads.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ciq.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zth.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bmk.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yzy.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cqm.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://udc.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mum.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://wxj.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://kuc.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xhj.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jdw.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ufv.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dyb.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uzk.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tio.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iba.52xcode.cn

[E16] 数字千分位
来源：http://kav.316326.xyz

Py:   f"{1234567:,}"
来源：http://uqv.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://tgm.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dgd.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dwx.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ywc.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lsb.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fyi.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://okn.andypj.xyz

[E17] 首字母大写
来源：http://dff.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aux.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nne.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ilt.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gga.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zcj.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lko.meibo888.top

Ruby: s.capitalize
来源：http://oub.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://scv.shzxlz.cn

[E18] 模板占位符替换
来源：http://eda.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yju.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fry.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kqe.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vfa.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kay.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cld.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tbh.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bwe.guannengcc.top

[E19] 多行文本按行拆分
来源：http://wcx.zhoulong.xyz

Py:   s.splitlines()
来源：http://eru.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vvs.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://yes.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://ihh.hammf.cn

Java: s.lines().toList()
来源：http://aud.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://dbp.zhaomingkeji.xyz

Ruby: s.lines
来源：http://bga.jqgfzy.top

C#:   s.Split('\n')
来源：http://kxw.xinyue.icu

[E20] 判断字符串是否为空
来源：http://xuu.hcnkem.com

Py:   if not s:
来源：http://jqc.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nrn.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qor.havefunace.top

TS:   if (s === "") {}
来源：http://lxd.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://vbq.ivvv.top

Go:   if s == "" {}
来源：http://sth.fehbvm.com

Ruby: if s.empty?
来源：http://tax.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dhb.andypj.xyz

[E21] 超长截断加省略号
来源：http://ocn.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://drt.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://acy.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dfb.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hil.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rog.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://nei.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ekj.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hai.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://oaw.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kyq.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fee.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rtp.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dhg.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kom.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://srn.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://feo.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zgz.zdqjudy.top

================================================================================
来源：http://vkw.jinqigfzy.top

F. 文件与目录
来源：http://tga.kuanghao11.cn

================================================================================
来源：http://swm.yj20258888.top

[F01] 读取整个文件
来源：http://atx.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wop.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://vdv.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vuy.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gxx.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://umb.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vnk.vehdjk.com

Ruby: File.read("a.txt")
来源：http://sfz.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://dgy.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://ojt.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gdy.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://afx.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ljb.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://guh.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jxs.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://efj.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wwy.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tds.tanke756.top

[F03] 写入文件（覆盖）
来源：http://osh.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pac.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qqw.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://daw.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ylr.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vow.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eyi.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://mhr.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uhq.yuanzhike.top

[F04] 追加写入文件
来源：http://pbd.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://slk.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qmy.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfz.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aab.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xap.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nad.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://anc.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xul.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://inf.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pkq.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://fyr.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://ujq.sweek.top

TS:   fs.existsSync("a.txt")
来源：http://pfx.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://dko.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zbq.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://dqx.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://dis.zhengqikj.top

[F06] 删除文件
来源：http://bnq.zycfv.cn

Py:   os.remove("a.txt")
来源：http://mvo.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://pvl.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://oup.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://hwr.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dcw.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://nwp.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://dnz.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://bsx.redwolf501.top

[F07] 创建目录（含多级）
来源：http://xrg.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mmd.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://txp.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://doz.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sdd.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qgb.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdg.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hex.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mia.xylfe.cn

[F08] 遍历目录
来源：http://lli.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aiv.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cnk.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://zzh.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://yms.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dls.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nah.hcnkem.com

Ruby: Dir.children("dir")
来源：http://hcs.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://tie.xuetiantiany.cn

[F09] 获取文件大小
来源：http://baz.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://nfr.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://opz.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://ioz.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://pmu.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://lyl.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://smu.wangdashe.top

Ruby: File.size("a.txt")
来源：http://twe.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://mij.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://frx.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qek.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mqf.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jms.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://lix.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://muq.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zrv.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ovz.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wur.daria6918.cn

[F11] 复制与移动文件
来源：http://acb.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vcn.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oyb.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sov.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oef.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xmb.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mks.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ksm.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sen.fanxiaobao.xyz

[F12] CSV 读写
来源：http://dxv.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wdi.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gjv.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://apg.zhixingplan.top

TS:   // 同上
来源：http://ynd.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cnl.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vai.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cpa.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hzf.yonumen.top

================================================================================
来源：http://dca.jinghuilouyu.cn

G. 面向对象
来源：http://tmd.ehwqpu.com

================================================================================
来源：http://vny.hesvh.cn

[G01] 定义类
来源：http://zqi.jinqigfzy.top

Py:   class User: pass
来源：http://xuw.sweek.top

PHP:  class User {}
来源：http://lqr.pycfn.com

JS:   class User {}
来源：http://ibz.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://uuy.mhx1999.top

Java: class User {}
来源：http://ojx.ivvv.top

Go:   type User struct { Name string }
来源：http://rni.shangyingyoupin.top

Ruby: class User; end
来源：http://bze.xziqi.cn

C#:   class User {}
来源：http://vuf.cucudq.cn

[G02] 构造函数
来源：http://edx.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://afi.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://wdz.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://iqd.birdmap.top

TS:   constructor(public name: string) {}
来源：http://hsr.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://dss.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://flz.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://rnb.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://oqa.9152youxi.cn

[G03] 实例属性
来源：http://cry.cashguo.top

Py:   self.name = "x"
来源：http://iwv.cdnleiting.top

PHP:  public string $name = "x";
来源：http://sui.cqqwz.cn

JS:   this.name = "x";
来源：http://ykb.chenjidiqi.icu

TS:   name: string = "x";
来源：http://quc.sxryk.cn

Java: private String name;
来源：http://ltf.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fms.0kj1m.cn

Ruby: @name = "x"
来源：http://ioj.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://dpu.xziqi.cn

[G04] 定义方法
来源：http://xjw.vehdjk.com

Py:   def greet(self): return self.name
来源：http://fuy.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://udp.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://jlg.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://ymc.cdnleiting.top

Java: String greet() { return name; }
来源：http://xih.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ejm.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://szo.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://zyz.cqqwz.cn

[G05] 继承
来源：http://pmb.nanxuanxn.top


<!-- 参考信息 -->