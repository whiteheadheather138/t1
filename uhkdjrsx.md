代发 wailian999

Go:   strings.Join(items, ",")
来源：http://ogh.epnwcf.com

Ruby: items.join(",")
来源：http://jan.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://foc.sxryk.cn

[E09] 去除所有空白字符
来源：http://bxd.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mvm.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gug.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://agp.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://cbq.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://lnj.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://kej.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://ydq.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nud.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://ici.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uzc.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eca.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://xsf.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://krc.havefunace.top

Java: String.format("%03d", 7)
来源：http://owk.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://amp.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://spp.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dmu.shangyingyoupin.top

[E11] 反转字符串
来源：http://yck.sufxvd.cn

Py:   s[::-1]
来源：http://yrz.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://gsc.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://smo.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://tzw.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ndj.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qmc.zdbjq.cn

Ruby: s.reverse
来源：http://edt.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://ppt.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://jpe.yj20258.top

Py:   s.count("a")
来源：http://iud.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://hhu.pycfn.com

JS:   s.split("a").length - 1
来源：http://qub.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://eza.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://roa.yj202588.top

Go:   strings.Count(s, "a")
来源：http://tyg.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://sxw.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://lqo.sweek.top

[E13] 逐字符遍历
来源：http://xas.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://pih.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nhs.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://toi.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uxt.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gml.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gew.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bkg.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ckx.xinyue.icu

[E14] URL 编码与 Base64
来源：http://crp.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pco.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzx.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wtb.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tdi.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dje.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tfd.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://riz.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fye.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://zvz.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dgk.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jnt.jlsjyb.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dee.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://swz.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lio.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cfc.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ybs.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aft.smart0.xyz

[E16] 数字千分位
来源：http://uye.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://umo.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://avs.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://odi.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ywv.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zbr.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://exi.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssq.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://uoe.guowangkeji.top

[E17] 首字母大写
来源：http://sip.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iqh.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yqy.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://utf.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://atr.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://krd.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rvc.fktsv.cn

Ruby: s.capitalize
来源：http://bku.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zsk.uphjek.com

[E18] 模板占位符替换
来源：http://lpv.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lvi.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ukz.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pop.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xdk.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pbq.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sly.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lax.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xzd.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://wvg.cqqwz.cn

Py:   s.splitlines()
来源：http://vxu.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fet.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://kmz.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://xhe.jinqigfzy.top

Java: s.lines().toList()
来源：http://obs.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://anb.yangfankeji.com

Ruby: s.lines
来源：http://cgz.yvedp.cn

C#:   s.Split('\n')
来源：http://tfc.smart0.xyz

[E20] 判断字符串是否为空
来源：http://wkz.c1oappe.top

Py:   if not s:
来源：http://paw.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jxa.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kxz.redwolf501.top

TS:   if (s === "") {}
来源：http://aru.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://ala.zhixingplan.top

Go:   if s == "" {}
来源：http://abt.yuanzhike.top

Ruby: if s.empty?
来源：http://baz.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xyh.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://dqh.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uvk.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mez.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cwv.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ose.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ztu.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://uoz.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yec.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dxn.xylfe.cn

[E22] 字节长度与字符长度
来源：http://tvd.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jqi.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jam.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xoc.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gbs.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rai.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rtd.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://qkg.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ztu.andypj.xyz

================================================================================
来源：http://dxf.52xcode.cn

F. 文件与目录
来源：http://szy.yongpay.top

================================================================================
来源：http://rjv.guannengcc.top

[F01] 读取整个文件
来源：http://dis.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://crz.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://qaa.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://txy.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ooa.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jrv.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wkn.hcnkem.com

Ruby: File.read("a.txt")
来源：http://env.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://svf.chenzaomai.com

[F02] 逐行读取文件
来源：http://uhr.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vms.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sve.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tsp.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://drj.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cie.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hmu.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://imf.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zco.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://nmq.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rts.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rzf.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tcv.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://whn.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npq.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rpi.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://wmh.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qjr.hongshengwenyu.top

[F04] 追加写入文件
来源：http://opk.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oyk.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kht.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxj.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jda.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://prh.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://prc.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nuk.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xyu.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://inf.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kir.birdmap.top

PHP:  file_exists("a.txt");
来源：http://kxt.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://dff.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://fjc.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fvs.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://txa.nwbrower.top

Ruby: File.exist?("a.txt")
来源：http://wei.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://zyh.iojbl.cn

[F06] 删除文件
来源：http://mrb.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://lcc.sxryk.cn

PHP:  unlink("a.txt");
来源：http://dpz.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://ubd.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://xun.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://djb.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://ofh.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://mms.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://gwl.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://fif.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wbh.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wmf.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzn.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hde.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://meq.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pfw.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pla.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://agt.fehbvm.com

[F08] 遍历目录
来源：http://odd.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pno.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://knn.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://nxs.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://ugu.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://haj.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://euq.ydzc1.top

Ruby: Dir.children("dir")
来源：http://bnh.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ssw.sjlbkw.cn

[F09] 获取文件大小
来源：http://qes.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://nhd.vehdjk.com

PHP:  filesize("a.txt");
来源：http://cwv.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://zds.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://sym.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://kfe.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://evk.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://jgc.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://qpu.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://eqd.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xke.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ysa.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tpt.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://sbl.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dnc.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nip.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aqq.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vfl.ehwqpu.com

[F11] 复制与移动文件
来源：http://mma.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sev.zdbjq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://val.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmd.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fov.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qpr.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cia.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lsf.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nhf.52xcode.cn

[F12] CSV 读写
来源：http://jgu.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jkl.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gwu.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ywl.sysykeji.top

TS:   // 同上
来源：http://icf.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sic.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zwf.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eku.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://aqk.chenjidiqi.icu

================================================================================
来源：http://lox.svipenyu.cn

G. 面向对象
来源：http://nut.meibo888.top

================================================================================
来源：http://orb.316326.xyz

[G01] 定义类
来源：http://lfs.hesvh.cn

Py:   class User: pass
来源：http://ylz.bjfxy.top

PHP:  class User {}
来源：http://tsk.gotoacloud.top

JS:   class User {}
来源：http://pea.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://yjn.hnxiangtu.top

Java: class User {}
来源：http://ula.nanxinkj.top

Go:   type User struct { Name string }
来源：http://wdi.ydjk.org.cn

Ruby: class User; end
来源：http://siw.andypj.xyz

C#:   class User {}
来源：http://wvy.birdmap.top

[G02] 构造函数
来源：http://dke.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://zcs.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://jlh.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://xsm.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://ucn.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://ync.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nws.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://lar.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://uao.yongpay.top

[G03] 实例属性
来源：http://tww.yonumen.top

Py:   self.name = "x"
来源：http://xxw.yuanzhike.top

PHP:  public string $name = "x";
来源：http://zxo.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://znv.gzhubu.top

TS:   name: string = "x";
来源：http://wxf.guowangkeji.top

Java: private String name;
来源：http://nvg.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lis.kuanghao11.cn

Ruby: @name = "x"
来源：http://kdg.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://oxq.zycfv.cn

[G04] 定义方法
来源：http://ano.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://sue.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://vah.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://ici.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://yor.tianlin.xyz

Java: String greet() { return name; }
来源：http://anl.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://sol.hnqzz.top

Ruby: def greet; @name; end
来源：http://hmf.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://ojs.jqgfzy.top

[G05] 继承
来源：http://tzc.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://pye.xinyue.icu

PHP:  class Admin extends User {}
来源：http://xwa.iojbl.cn

JS:   class Admin extends User {}
来源：http://rro.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://ovg.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://jhr.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aks.svipenyu.cn

Ruby: class Admin < User; end
来源：http://uij.ehwqpu.com

C#:   class Admin : User {}
来源：http://zck.zhaomingkeji.xyz

[G06] 重写方法
来源：http://ppn.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://ewx.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fmo.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://yia.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://cto.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://sqx.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sor.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://ond.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://yui.nwbrower.top

[G07] 调用父类方法
来源：http://jhr.smart0.xyz

Py:   super().greet()
来源：http://sqe.zdqjudy.top

PHP:  parent::greet();
来源：http://juz.yvedp.cn


<!-- 参考信息 -->