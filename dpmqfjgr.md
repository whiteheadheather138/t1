代发 wailian999

PHP:  implode(",", $items);
来源：http://rtb.tarul.cn

JS:   items.join(",")
来源：http://clz.hesvh.cn

TS:   items.join(",")
来源：http://gny.tianlin.xyz

Java: String.join(",", items)
来源：http://fjk.chenlongwang.top

Go:   strings.Join(items, ",")
来源：http://olt.sufxvd.cn

Ruby: items.join(",")
来源：http://xmy.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://yjf.iojbl.cn

[E09] 去除所有空白字符
来源：http://kks.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://saq.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yuv.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://cpj.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://onc.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://byq.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://prn.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://hsu.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gby.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://hvn.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tox.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eal.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://dbp.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://dda.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://tzh.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ijx.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vjb.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ykc.mhx1999.top

[E11] 反转字符串
来源：http://sur.hcnkem.com

Py:   s[::-1]
来源：http://xqq.ydjk.org.cn

PHP:  strrev($s);
来源：http://yfx.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://cga.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://ztd.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://umh.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://amk.gaohongyu789.top

Ruby: s.reverse
来源：http://gkh.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://flu.jianghu66.top

[E12] 统计某字符出现次数
来源：http://nbl.zhengqikj.top

Py:   s.count("a")
来源：http://ymh.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://eub.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://qkk.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://yxp.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sxm.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://fiq.jqgfzy.top

Ruby: s.count("a")
来源：http://msa.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://wmy.sjlbkw.cn

[E13] 逐字符遍历
来源：http://wol.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://cvf.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jbi.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ojg.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ykl.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rmz.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wvv.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yzv.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jrm.ivvv.top

[E14] URL 编码与 Base64
来源：http://wio.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://heq.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jmi.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ydx.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yna.xziqi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vjw.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fdc.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://izs.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://veq.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://jdt.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wqu.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zuc.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cyi.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ohc.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fre.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://paq.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://prt.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hkb.sysykeji.top

[E16] 数字千分位
来源：http://fxo.fehbvm.com

Py:   f"{1234567:,}"
来源：http://uws.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://moz.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://urb.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ysd.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lnl.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tga.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ple.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://sjc.guowangkeji.top

[E17] 首字母大写
来源：http://bnw.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lpz.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://fmu.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogk.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ttk.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://too.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hub.xinyue.icu

Ruby: s.capitalize
来源：http://dok.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zpu.bjfxy.top

[E18] 模板占位符替换
来源：http://inr.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ida.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://urf.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://apm.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qng.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zbo.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iem.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ftw.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rwf.bjfxy.top

[E19] 多行文本按行拆分
来源：http://hum.hcnkem.com

Py:   s.splitlines()
来源：http://fox.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ozg.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://mrj.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://wxn.quarkkingdee.top

Java: s.lines().toList()
来源：http://byt.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://olp.sufxvd.cn

Ruby: s.lines
来源：http://hsw.ybcxt.top

C#:   s.Split('\n')
来源：http://jwu.xziqi.cn

[E20] 判断字符串是否为空
来源：http://zrn.zdqjudy.top

Py:   if not s:
来源：http://tmg.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ald.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://okp.havefunace.top

TS:   if (s === "") {}
来源：http://jfs.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://uqi.pengpengdd.cyou

Go:   if s == "" {}
来源：http://jvu.cheryme.top

Ruby: if s.empty?
来源：http://mtm.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bou.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://nmm.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvc.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ots.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://krz.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsk.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbf.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://qyb.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mpk.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tbl.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://lty.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vvk.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pke.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lji.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zop.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qlf.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wfs.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://wac.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://snx.uphjek.com

================================================================================
来源：http://vyl.nwbrower.top

F. 文件与目录
来源：http://vxg.yueranfly.top

================================================================================
来源：http://gtw.jianghu66.top

[F01] 读取整个文件
来源：http://aws.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cat.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://itv.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ywq.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://asw.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hfb.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xih.andypj.xyz

Ruby: File.read("a.txt")
来源：http://lva.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://kdt.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://iwa.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ebq.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zvf.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aqd.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qri.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ygr.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://evj.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://thl.c1oappe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blc.yj20258.top

[F03] 写入文件（覆盖）
来源：http://nfo.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kxq.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sto.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rry.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sdi.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fae.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qax.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://krt.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wlp.hnqzz.top

[F04] 追加写入文件
来源：http://zah.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yvz.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ydw.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jyr.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyw.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ddu.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://srp.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dau.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyx.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://kpy.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pwp.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://ryz.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://wqn.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://lof.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ero.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qmi.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://svf.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://goa.hfpthk.cn

[F06] 删除文件
来源：http://yui.xuanzx.com

Py:   os.remove("a.txt")
来源：http://icv.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://wst.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kbf.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://bdu.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zni.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://tyn.ivvv.top

Ruby: File.delete("a.txt")
来源：http://zca.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://uql.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://cvg.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://skp.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lwb.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbv.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://glv.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qhd.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uop.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xbf.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gwg.zycfv.cn

[F08] 遍历目录
来源：http://uis.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dvs.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://puw.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://bck.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://wfc.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://geo.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajk.vehdjk.com

Ruby: Dir.children("dir")
来源：http://vhk.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://svb.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://wxi.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://wpm.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://qol.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://eub.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://fvq.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vzu.fehbvm.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://phl.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://fwp.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://rhw.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://sft.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pzu.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lhl.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://erg.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://esd.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nbp.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fry.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://und.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nlf.tian-w.cn

[F11] 复制与移动文件
来源：http://gjc.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iud.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zdj.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtl.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qlk.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsx.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iim.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ifm.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xcc.wangshuangyany.cn

[F12] CSV 读写
来源：http://qwb.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tmn.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vvv.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jwa.fanxiaobao.xyz

TS:   // 同上
来源：http://snm.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lax.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qra.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yjw.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://idz.jinqigufen.top

================================================================================
来源：http://dbl.hesvh.cn

G. 面向对象
来源：http://smu.ppjwa.cn

================================================================================
来源：http://sin.nanxuanxn.top

[G01] 定义类
来源：http://sdn.xinyue.icu

Py:   class User: pass
来源：http://pha.daria6918.cn

PHP:  class User {}
来源：http://sxm.cqqwz.cn

JS:   class User {}
来源：http://ady.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://hlx.yueranfly.top

Java: class User {}
来源：http://skn.nanxinkj.top

Go:   type User struct { Name string }
来源：http://cjp.jinghuilouyu.cn

Ruby: class User; end
来源：http://xcj.hnxiangtu.top

C#:   class User {}
来源：http://tnu.yuanzhike.top

[G02] 构造函数
来源：http://oif.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://vze.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://cte.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://rue.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://qct.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://aez.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eac.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://knk.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://vpi.cheryme.top

[G03] 实例属性
来源：http://kom.feifeiyinyue.top

Py:   self.name = "x"
来源：http://dgv.dianchejie.cn

PHP:  public string $name = "x";
来源：http://maw.yfazqb.com

JS:   this.name = "x";
来源：http://fww.ybcxt.top

TS:   name: string = "x";
来源：http://eqb.bbcook.cn

Java: private String name;
来源：http://ovw.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wui.xuanzx.com

Ruby: @name = "x"
来源：http://klh.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://ygj.fktsv.cn

[G04] 定义方法
来源：http://wua.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://rmo.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xmz.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://vke.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://ngf.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://cyd.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tql.yvedp.cn

Ruby: def greet; @name; end
来源：http://nfj.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://jrz.fanxiaobao.xyz

[G05] 继承
来源：http://ajg.xuanzx.com

Py:   class Admin(User): pass
来源：http://hvs.mhx1999.top

PHP:  class Admin extends User {}
来源：http://nlm.jyoumei.cn

JS:   class Admin extends User {}
来源：http://kll.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://nee.hnxiangtu.top

Java: class Admin extends User {}
来源：http://lrb.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://znp.zdqjudy.top

Ruby: class Admin < User; end
来源：http://wcv.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://pce.fktsv.cn

[G06] 重写方法
来源：http://skk.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://ndn.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dkp.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://ywh.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://yxb.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://rkm.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fdc.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://tsk.zhaomingkeji.xyz


<!-- 参考信息 -->