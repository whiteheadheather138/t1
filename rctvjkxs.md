代发 wailian999

PHP:  implode(",", $items);
来源：http://msj.uphjek.com

JS:   items.join(",")
来源：http://ini.xuetiantiany.cn

TS:   items.join(",")
来源：http://plw.ydzc1.top

Java: String.join(",", items)
来源：http://itj.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://gjp.svipenyu.cn

Ruby: items.join(",")
来源：http://lhd.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://nmj.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://txr.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nyz.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xlw.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://hyz.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://hqa.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://ukq.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xpe.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://zak.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kwl.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://kom.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bzn.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://foa.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://vkh.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://ytx.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://nhg.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qvf.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ahj.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sni.dashuyun.cn

[E11] 反转字符串
来源：http://qzr.yangfankeji.com

Py:   s[::-1]
来源：http://clr.svipenyu.cn

PHP:  strrev($s);
来源：http://mtx.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://gkk.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://yeq.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xui.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tcj.nwbrower.top

Ruby: s.reverse
来源：http://thz.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://sal.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://jhi.yj202588.top

Py:   s.count("a")
来源：http://hww.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://bru.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://jyr.xinyue.icu

TS:   s.split("a").length - 1
来源：http://jmd.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jww.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://aki.0kj1m.cn

Ruby: s.count("a")
来源：http://leu.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://okj.daxiang520.top

[E13] 逐字符遍历
来源：http://cvv.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://phu.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fqm.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://auk.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ify.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ocg.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hbf.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://wxh.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hsd.xinyue.icu

[E14] URL 编码与 Base64
来源：http://oay.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ioz.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://huo.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hfb.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xsi.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bms.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zxs.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gao.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wwe.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://pll.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mde.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jqf.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wzd.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nmi.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ywa.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qeo.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pla.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vhm.xinyue.icu

[E16] 数字千分位
来源：http://fwj.daria6918.cn

Py:   f"{1234567:,}"
来源：http://qfo.fehbvm.com

PHP:  number_format(1234567);
来源：http://dwv.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sxx.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dyy.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qbg.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ojw.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pwd.yj20258.top

C#:   1234567.ToString("N0")
来源：http://cph.zdbjq.cn

[E17] 首字母大写
来源：http://dsg.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fin.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://snl.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xur.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pie.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://khu.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://syd.xuetiantiany.cn

Ruby: s.capitalize
来源：http://hrf.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xgb.zhixingplan.top

[E18] 模板占位符替换
来源：http://hku.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yjv.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ozg.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pmt.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ntc.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vxr.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tnp.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mkx.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lla.gzhubu.top

[E19] 多行文本按行拆分
来源：http://hmp.tianlin.xyz

Py:   s.splitlines()
来源：http://yhi.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ngc.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://wgz.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://rym.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://btr.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://bkx.yuanzhike.top

Ruby: s.lines
来源：http://jog.ydzc1.top

C#:   s.Split('\n')
来源：http://ygk.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://jre.jqgfzy.top

Py:   if not s:
来源：http://ytl.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ryt.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dni.316326.xyz

TS:   if (s === "") {}
来源：http://mwt.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://pdv.fengsongda.top

Go:   if s == "" {}
来源：http://fdt.gaohongyu789.top

Ruby: if s.empty?
来源：http://iuq.tian-w.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://heq.iojbl.cn

[E21] 超长截断加省略号
来源：http://oqr.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rsd.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eac.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://doq.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uah.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jhb.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://srj.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qff.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qcw.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://lvj.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nib.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mrm.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dun.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sye.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vgw.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zyd.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://din.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rjz.yangfankeji.com

================================================================================
来源：http://ive.yuanzhike.top

F. 文件与目录
来源：http://med.jinqigufen.top

================================================================================
来源：http://iif.jqgfzy.top

[F01] 读取整个文件
来源：http://vla.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zao.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://dyq.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://owf.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ksh.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://spa.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vth.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://dtk.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://yxt.yangfankeji.com

[F02] 逐行读取文件
来源：http://kwd.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jdf.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jpl.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tkx.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xje.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xhl.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ppz.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nof.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ccj.tanke756.top

[F03] 写入文件（覆盖）
来源：http://gsl.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://app.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lzd.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vkr.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ekd.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tbh.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dqs.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://hza.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ndx.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://dbs.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kpn.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lag.hesvh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rjr.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lnn.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wvb.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://swg.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://coq.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tbo.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://zjl.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ojs.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://mch.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://vhx.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://tlo.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xrp.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://njb.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://rjd.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://tgk.jlsjyb.cn

[F06] 删除文件
来源：http://yzr.yj202588.top

Py:   os.remove("a.txt")
来源：http://wbc.fzhhl.top

PHP:  unlink("a.txt");
来源：http://vbn.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://rny.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://mpy.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mkr.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://upe.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://axx.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://vtk.316326.xyz

[F07] 创建目录（含多级）
来源：http://lwm.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mjk.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yhv.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zuh.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jcy.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://afn.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xeo.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgv.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cgg.meibo888.top

[F08] 遍历目录
来源：http://qpn.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmv.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyk.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://xrs.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://fhb.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wpd.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tdc.cheryme.top

Ruby: Dir.children("dir")
来源：http://zfy.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://qic.sysykeji.top

[F09] 获取文件大小
来源：http://bbs.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://mcq.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://ryw.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://pbj.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://ebk.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zqe.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://czb.hesvh.cn

Ruby: File.size("a.txt")
来源：http://yxx.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://eau.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://uui.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://luv.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ufc.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tsu.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://eoo.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xig.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hvi.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mik.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dvi.52xcode.cn

[F11] 复制与移动文件
来源：http://wst.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vue.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kuv.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dad.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbl.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cyz.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jab.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tlk.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pkd.shuidangran.top

[F12] CSV 读写
来源：http://oex.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kly.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dzt.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gbk.zhixingplan.top

TS:   // 同上
来源：http://bjf.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hpt.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uhv.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pwo.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lrg.fengsongda.top

================================================================================
来源：http://uio.zdqjudy.top

G. 面向对象
来源：http://asx.wangshuangyany.cn

================================================================================
来源：http://urd.cdnleiting.top

[G01] 定义类
来源：http://clt.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ixg.c1oappe.top

PHP:  class User {}
来源：http://shh.gotoacloud.top

JS:   class User {}
来源：http://ikk.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://xwy.gaohongyu789.top

Java: class User {}
来源：http://phj.yfazqb.com

Go:   type User struct { Name string }
来源：http://fiv.yfazqb.com

Ruby: class User; end
来源：http://fty.sweek.top

C#:   class User {}
来源：http://dbx.mhx1999.top

[G02] 构造函数
来源：http://wmn.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://jkn.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://tmu.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://yha.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://spk.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://mqb.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://azx.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://mxu.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://kfo.zhaomingkeji.xyz

[G03] 实例属性
来源：http://rtj.hysaishi.cn

Py:   self.name = "x"
来源：http://xwf.aibaodan.cn

PHP:  public string $name = "x";
来源：http://wiy.cucudq.cn

JS:   this.name = "x";
来源：http://vep.sjlbkw.cn

TS:   name: string = "x";
来源：http://kmd.ppjwa.cn

Java: private String name;
来源：http://nhj.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kql.chenzaomai.com

Ruby: @name = "x"
来源：http://stb.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://rdq.guannengcc.top

[G04] 定义方法
来源：http://lrl.mhx1999.top

Py:   def greet(self): return self.name
来源：http://urv.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jxm.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://ouc.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://erl.nwbrower.top

Java: String greet() { return name; }
来源：http://lby.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jyc.aibaodan.cn

Ruby: def greet; @name; end
来源：http://orq.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://xdp.hfpthk.cn

[G05] 继承
来源：http://ajf.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://pra.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://uhh.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://ccz.tian-w.cn

TS:   class Admin extends User {}
来源：http://stu.52xcode.cn

Java: class Admin extends User {}
来源：http://wdq.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oqa.cqqwz.cn

Ruby: class Admin < User; end
来源：http://uou.hnxiangtu.top

C#:   class Admin : User {}
来源：http://qbs.ybcxt.top

[G06] 重写方法
来源：http://ncx.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://xuc.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iuu.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://noi.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://rrz.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://hao.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zke.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://xah.nanxuanxn.top


<!-- 参考信息 -->