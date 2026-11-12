代发 wailian999

C#:   s.Replace("a", "b")
来源：http://mnd.nanxinkj.top

[E07] 按分隔符拆分
来源：http://dlo.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yke.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ydk.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eak.daxiang520.top

TS:   s.split(",")
来源：http://hea.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://eif.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yar.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://oma.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kpl.xziqi.cn

[E08] 数组按分隔符合并
来源：http://qym.ehwqpu.com

Py:   ",".join(items)
来源：http://ked.hywenlv.cn

PHP:  implode(",", $items);
来源：http://kwx.shzxlz.cn

JS:   items.join(",")
来源：http://cdo.ydzc1.top

TS:   items.join(",")
来源：http://xsn.mhx1999.top

Java: String.join(",", items)
来源：http://ins.meibo888.top

Go:   strings.Join(items, ",")
来源：http://mqk.snrcjt.cn

Ruby: items.join(",")
来源：http://aqj.dianchejie.cn

C#:   string.Join(",", items)
来源：http://mxl.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://esl.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nrs.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ysj.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://vbo.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://ttk.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://ntx.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://uwl.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://cex.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xco.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://xul.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wjx.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://elw.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://cbm.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://kvf.wangdashe.top

Java: String.format("%03d", 7)
来源：http://nez.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vix.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zje.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hpm.yfazqb.com

[E11] 反转字符串
来源：http://fhb.cqqwz.cn

Py:   s[::-1]
来源：http://cqf.daxiang520.top

PHP:  strrev($s);
来源：http://czn.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://xit.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://efc.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://mkp.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jpq.zhixingplan.top

Ruby: s.reverse
来源：http://ndz.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nuh.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://evv.jqgfzy.top

Py:   s.count("a")
来源：http://ylh.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://wzt.hesvh.cn

JS:   s.split("a").length - 1
来源：http://ifb.yuxming.cn

TS:   s.split("a").length - 1
来源：http://hya.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fqa.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://sxz.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://igs.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://kmn.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://zvi.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://dhr.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ipx.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jic.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xbc.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ely.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://obt.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wzt.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qwb.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://yad.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://drf.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzn.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xih.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gge.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rav.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://epm.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ecb.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ibt.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://uep.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mzl.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://upy.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lss.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rza.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uwo.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cnn.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gek.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tua.c1oappe.top

[E16] 数字千分位
来源：http://lwb.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://qrc.aibaodan.cn

PHP:  number_format(1234567);
来源：http://oeu.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nqo.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yxl.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://arq.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jiy.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jwb.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://qvy.hywenlv.cn

[E17] 首字母大写
来源：http://qsn.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fuh.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ucz.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uci.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zab.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://smc.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://muo.tianlin.xyz

Ruby: s.capitalize
来源：http://icd.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iav.chenzaomai.com

[E18] 模板占位符替换
来源：http://mam.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kev.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aag.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qhb.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qkn.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eyz.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kth.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wwt.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://szj.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://ica.shangyingyoupin.top

Py:   s.splitlines()
来源：http://fuh.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xzr.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://qvq.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://edm.zdbjq.cn

Java: s.lines().toList()
来源：http://ndd.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://deu.sufxvd.cn

Ruby: s.lines
来源：http://khe.dianchejie.cn

C#:   s.Split('\n')
来源：http://xlo.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://gyr.yuanzhike.top

Py:   if not s:
来源：http://nuv.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zot.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gcs.jlsjyb.cn

TS:   if (s === "") {}
来源：http://jyo.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://olu.zhengqikj.top

Go:   if s == "" {}
来源：http://mcb.jinqigfzy.top

Ruby: if s.empty?
来源：http://dwc.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fgu.iojbl.cn

[E21] 超长截断加省略号
来源：http://njg.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqp.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ali.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kgt.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hwr.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pdm.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://rms.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://shn.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wif.sxryk.cn

[E22] 字节长度与字符长度
来源：http://vvh.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://spz.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nyj.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zks.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fhc.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wti.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zxe.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://ibv.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bmo.0kj1m.cn

================================================================================
来源：http://oyt.zhaomingkeji.xyz

F. 文件与目录
来源：http://ulw.c1oappe.top

================================================================================
来源：http://qtw.hnxiangtu.top

[F01] 读取整个文件
来源：http://frr.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ipe.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://wjz.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ivg.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vnl.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lcv.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rfp.iojbl.cn

Ruby: File.read("a.txt")
来源：http://nun.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://bgs.cheryme.top

[F02] 逐行读取文件
来源：http://pqp.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hrt.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nir.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ukf.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vkp.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://htk.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fst.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wjz.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dsj.havefunace.top

[F03] 写入文件（覆盖）
来源：http://vvr.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://brq.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ndr.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gtl.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rtg.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oym.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vln.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://ltm.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://szi.jlsjyb.cn

[F04] 追加写入文件
来源：http://vui.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://drs.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bva.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ckk.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sgs.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xzl.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://svg.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ymc.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://myz.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://ghx.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://btm.yj20258.top

PHP:  file_exists("a.txt");
来源：http://udt.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://drd.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://erq.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jbx.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fwj.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://dvi.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://bmu.nanxinkj.top

[F06] 删除文件
来源：http://uug.tian-w.cn

Py:   os.remove("a.txt")
来源：http://tjt.vehdjk.com

PHP:  unlink("a.txt");
来源：http://xhf.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://num.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pyh.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ekh.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://xid.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://nyu.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://dww.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://mtc.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xqn.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zut.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://voc.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nxm.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://esj.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jxs.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ale.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gda.meibo888.top

[F08] 遍历目录
来源：http://ehd.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zwx.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://alo.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://nde.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://wbp.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yva.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://kte.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://rvy.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://cko.wangshuangyany.cn

[F09] 获取文件大小
来源：http://qzb.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://bin.cheryme.top

PHP:  filesize("a.txt");
来源：http://hrr.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://isw.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://zxf.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pda.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gln.bjfxy.top

Ruby: File.size("a.txt")
来源：http://lmo.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://yed.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://upf.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kbi.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rub.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mog.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://adb.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rvx.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aeb.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xeu.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bqj.fengsongda.top

[F11] 复制与移动文件
来源：http://kjj.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rfb.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oth.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xbf.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://obk.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://awl.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hhp.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bsc.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cru.ydjk.org.cn

[F12] CSV 读写
来源：http://aak.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cva.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dfs.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bue.sysykeji.top

TS:   // 同上
来源：http://etn.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mif.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ynk.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jyg.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oij.vehdjk.com

================================================================================
来源：http://dtq.fengsongda.top

G. 面向对象
来源：http://coa.vqdsnc.cn

================================================================================
来源：http://mit.zhoulong.xyz

[G01] 定义类
来源：http://rtd.ppjwa.cn

Py:   class User: pass
来源：http://jww.yj202588.top

PHP:  class User {}
来源：http://gcu.chenlongwang.top

JS:   class User {}
来源：http://oux.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://gyu.iojbl.cn

Java: class User {}
来源：http://iif.hfpthk.cn

Go:   type User struct { Name string }
来源：http://qxw.cheryme.top

Ruby: class User; end
来源：http://pul.vehdjk.com

C#:   class User {}
来源：http://obf.hnqzz.top

[G02] 构造函数
来源：http://tho.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://krd.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://gpr.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://yok.meibo888.top

TS:   constructor(public name: string) {}
来源：http://xah.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://yiq.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xpw.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://ffz.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://utg.sufxvd.cn

[G03] 实例属性
来源：http://sdd.iojbl.cn

Py:   self.name = "x"
来源：http://ayd.jianghu66.top

PHP:  public string $name = "x";
来源：http://cey.aibaodan.cn

JS:   this.name = "x";
来源：http://uxz.andypj.xyz

TS:   name: string = "x";
来源：http://yjv.jyoumei.cn

Java: private String name;
来源：http://knc.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jqp.sxryk.cn

Ruby: @name = "x"
来源：http://ghz.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://iwz.bbcook.cn

[G04] 定义方法
来源：http://alv.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://zsp.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bgd.vehdjk.com

JS:   greet() { return this.name; }
来源：http://kjf.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://aud.redwolf501.top

Java: String greet() { return name; }
来源：http://zzz.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnw.jyoumei.cn

Ruby: def greet; @name; end
来源：http://vpm.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://dtm.chenlongwang.top

[G05] 继承
来源：http://tti.9152youxi.cn

Py:   class Admin(User): pass
来源：http://zmr.cheryme.top

PHP:  class Admin extends User {}
来源：http://uoo.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://pni.zhengqikj.top

TS:   class Admin extends User {}
来源：http://ecz.sxryk.cn


<!-- 参考信息 -->