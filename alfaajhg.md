代发 wailian999

C#:   s.Replace("a", "b")
来源：http://utm.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://bvd.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cec.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tqu.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vgg.chenlongwang.top

TS:   s.split(",")
来源：http://unw.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://rlt.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lpi.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://muv.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kma.zycfv.cn

[E08] 数组按分隔符合并
来源：http://qmg.yj202588.top

Py:   ",".join(items)
来源：http://hft.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://vmy.vqdsnc.cn

JS:   items.join(",")
来源：http://vgo.shzxlz.cn

TS:   items.join(",")
来源：http://ofg.sysykeji.top

Java: String.join(",", items)
来源：http://jnn.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://gjq.tarul.cn

Ruby: items.join(",")
来源：http://lfs.aibaodan.cn

C#:   string.Join(",", items)
来源：http://ciz.birdmap.top

[E09] 去除所有空白字符
来源：http://fcn.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lzn.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://adt.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://adx.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://nco.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://jlx.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qfp.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://sdb.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dfv.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://fzx.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vas.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tnp.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://lve.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://txv.yonumen.top

Java: String.format("%03d", 7)
来源：http://uvn.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ynb.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oul.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eyn.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://bxn.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://skq.xuanzx.com

PHP:  strrev($s);
来源：http://iae.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://vtd.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://myp.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ndp.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://axz.zhongyouzk.top

Ruby: s.reverse
来源：http://nmj.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://amf.mhx1999.top

[E12] 统计某字符出现次数
来源：http://kbv.hesvh.cn

Py:   s.count("a")
来源：http://xhd.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://tra.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://xjm.tian-w.cn

TS:   s.split("a").length - 1
来源：http://fsk.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bxo.pycfn.com

Go:   strings.Count(s, "a")
来源：http://fje.hesvh.cn

Ruby: s.count("a")
来源：http://qgb.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://qbl.vehdjk.com

[E13] 逐字符遍历
来源：http://kue.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://bxu.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fky.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bri.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vyw.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dac.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zgs.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ivb.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cyx.ivvv.top

[E14] URL 编码与 Base64
来源：http://gga.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mte.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eig.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://par.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vem.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lqs.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gqk.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bku.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xzu.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://pki.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://var.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qjt.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wwd.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ltd.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gkq.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cvc.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tce.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tuu.redwolf501.top

[E16] 数字千分位
来源：http://frt.yueranfly.top

Py:   f"{1234567:,}"
来源：http://tir.yuxming.cn

PHP:  number_format(1234567);
来源：http://osy.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hdp.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://eov.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sjm.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iab.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dhd.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://kss.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://bbr.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ciy.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rvx.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tpg.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mtm.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ury.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vaw.zhengqikj.top

Ruby: s.capitalize
来源：http://een.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ooy.vehdjk.com

[E18] 模板占位符替换
来源：http://ywz.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fzz.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tir.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hpo.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vfl.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://css.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kau.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qgj.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cqw.yj20258888.top

[E19] 多行文本按行拆分
来源：http://oxu.chenzaomai.com

Py:   s.splitlines()
来源：http://qds.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bba.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://fxm.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://qlq.haohaochexian.top

Java: s.lines().toList()
来源：http://vzu.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://ahy.ydzc1.top

Ruby: s.lines
来源：http://dmm.birdmap.top

C#:   s.Split('\n')
来源：http://xge.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://jqr.hammf.cn

Py:   if not s:
来源：http://kwb.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mpt.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhe.yj20258888.top

TS:   if (s === "") {}
来源：http://lyt.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://aim.fktsv.cn

Go:   if s == "" {}
来源：http://dzv.tarul.cn

Ruby: if s.empty?
来源：http://pii.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://syp.ivvv.top

[E21] 超长截断加省略号
来源：http://rwv.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hsi.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tee.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cjt.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wbp.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wnw.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://upv.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qya.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lba.uphjek.com

[E22] 字节长度与字符长度
来源：http://gfy.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wfg.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txc.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://exw.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcg.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jdg.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wti.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://byd.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://acm.cqqwz.cn

================================================================================
来源：http://zst.cashguo.top

F. 文件与目录
来源：http://mjq.xinyue.icu

================================================================================
来源：http://fhy.hfpthk.cn

[F01] 读取整个文件
来源：http://rxi.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://odw.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://pgq.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qta.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wmf.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gem.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hma.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://dmd.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://efu.hammf.cn

[F02] 逐行读取文件
来源：http://ayj.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://txm.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cqe.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kiz.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://elo.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lkj.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxi.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ghn.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zrs.birdmap.top

[F03] 写入文件（覆盖）
来源：http://wjz.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aqn.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rdn.0kj1m.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfr.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://noq.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lmd.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zbu.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://gdk.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ktd.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://ora.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pcy.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xkh.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kia.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fsq.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wnu.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uch.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yot.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ucf.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://dms.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tuh.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://ylh.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://omn.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://uel.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hmi.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://khj.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://jbr.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://goj.jianghu66.top

[F06] 删除文件
来源：http://pvr.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://wso.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://rxl.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://pmo.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yhq.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yxe.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://lmd.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://uoq.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://uds.ybcxt.top

[F07] 创建目录（含多级）
来源：http://wtv.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qwo.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://exn.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qdo.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kxs.shanyushiyangtech.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://syp.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kaw.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pix.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://guc.jqgufenzy.top

[F08] 遍历目录
来源：http://jeq.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://syr.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gzu.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://tik.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://clk.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hye.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vee.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://nbr.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://jns.hongshengwenyu.top

[F09] 获取文件大小
来源：http://bpf.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://qvl.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://rdh.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://lvf.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://fdw.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://lco.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rkp.316326.xyz

Ruby: File.size("a.txt")
来源：http://qtx.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://zzi.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://vft.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nve.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://loc.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://omv.gzhubu.top

TS:   path.extname("a.txt")
来源：http://bzl.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bsk.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mov.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bpd.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rdw.aibaodan.cn

[F11] 复制与移动文件
来源：http://pxi.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ykw.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ecm.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwz.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dqi.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qtz.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xhd.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nvt.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ltp.pycfn.com

[F12] CSV 读写
来源：http://pfi.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yvo.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zyr.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ffu.ydjk.org.cn

TS:   // 同上
来源：http://fpw.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://igm.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zlm.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zqm.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wmu.xuetiantiany.cn

================================================================================
来源：http://xik.zhengqikj.top

G. 面向对象
来源：http://exz.ydzc1.top

================================================================================
来源：http://rnn.tian-w.cn

[G01] 定义类
来源：http://dzs.jianghu66.top

Py:   class User: pass
来源：http://yom.yj20258888.top

PHP:  class User {}
来源：http://lhc.ywan-chungtsiang.top

JS:   class User {}
来源：http://oyj.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://xae.sweek.top

Java: class User {}
来源：http://yfu.guowangkeji.top

Go:   type User struct { Name string }
来源：http://ivp.chenzaomai.com

Ruby: class User; end
来源：http://par.ctjpmb.com

C#:   class User {}
来源：http://nir.dashuyun.cn

[G02] 构造函数
来源：http://otb.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://wkv.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://vgo.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://iez.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://jll.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://xxl.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://swp.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://ehf.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://nnp.yj20258.top

[G03] 实例属性
来源：http://twi.cheryme.top

Py:   self.name = "x"
来源：http://yyu.bbcook.cn

PHP:  public string $name = "x";
来源：http://bkr.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://gwi.meibo888.top

TS:   name: string = "x";
来源：http://zmx.hnqzz.top

Java: private String name;
来源：http://ffm.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cnv.316326.xyz

Ruby: @name = "x"
来源：http://loq.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://mdm.shzxlz.cn

[G04] 定义方法
来源：http://igj.yuxming.cn

Py:   def greet(self): return self.name
来源：http://cmi.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mbz.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://ihl.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://fvc.sweek.top

Java: String greet() { return name; }
来源：http://bwl.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://zjw.hammf.cn

Ruby: def greet; @name; end
来源：http://yci.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://bbe.gaohongyu789.top

[G05] 继承
来源：http://asu.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://bhg.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://bsy.52xcode.cn

JS:   class Admin extends User {}
来源：http://fkh.chenlongwang.top

TS:   class Admin extends User {}
来源：http://dhh.hfpthk.cn


<!-- 参考信息 -->