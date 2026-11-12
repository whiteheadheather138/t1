代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ytb.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://txc.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://lux.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://klz.fehbvm.com

[E10] 左侧补零 / 定长填充
来源：http://bmw.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lzp.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://glx.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://dfq.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://ute.aizwys.cn

Java: String.format("%03d", 7)
来源：http://ehd.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lln.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://grp.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zpi.vehdjk.com

[E11] 反转字符串
来源：http://ptz.xinyue.icu

Py:   s[::-1]
来源：http://byo.fehbvm.com

PHP:  strrev($s);
来源：http://gbx.cashguo.top

JS:   [...s].reverse().join("")
来源：http://pbu.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://udi.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://wgf.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://zkr.xuetiantiany.cn

Ruby: s.reverse
来源：http://tte.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bxd.xuanzx.com

[E12] 统计某字符出现次数
来源：http://qxc.yueranfly.top

Py:   s.count("a")
来源：http://cpu.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://qns.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://mdc.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://rpd.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wko.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://bkt.aibaodan.cn

Ruby: s.count("a")
来源：http://ccf.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://sfp.gzhubu.top

[E13] 逐字符遍历
来源：http://njj.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://yov.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gez.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fdn.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xoj.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hfh.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eip.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zjs.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kcq.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://fir.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pvz.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xay.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://omc.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xct.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ikm.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uge.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://htx.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bmn.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://lay.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gtc.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xmy.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xnr.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cft.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxc.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://axm.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://czr.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mjm.cashguo.top

[E16] 数字千分位
来源：http://jwp.iojbl.cn

Py:   f"{1234567:,}"
来源：http://vzp.jianghu66.top

PHP:  number_format(1234567);
来源：http://ntt.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xnk.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rwy.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jma.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zxt.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ghk.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://pnj.epnwcf.com

[E17] 首字母大写
来源：http://dxx.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qpo.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lpj.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yat.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfr.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://syu.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fii.mhx1999.top

Ruby: s.capitalize
来源：http://hfr.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mgo.aibaodan.cn

[E18] 模板占位符替换
来源：http://lwo.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bpo.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://smo.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ghy.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ycu.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sob.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://czq.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://opp.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lkh.guannengcc.top

[E19] 多行文本按行拆分
来源：http://ttz.zdbjq.cn

Py:   s.splitlines()
来源：http://avf.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rxy.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://cck.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://ikx.zhengqikj.top

Java: s.lines().toList()
来源：http://inj.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://jqb.birdmap.top

Ruby: s.lines
来源：http://fry.hywenlv.cn

C#:   s.Split('\n')
来源：http://yyv.vehdjk.com

[E20] 判断字符串是否为空
来源：http://chq.xuanzx.com

Py:   if not s:
来源：http://bzm.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://utc.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qrz.sxryk.cn

TS:   if (s === "") {}
来源：http://zuk.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://buf.gzhubu.top

Go:   if s == "" {}
来源：http://qzg.haohaochexian.top

Ruby: if s.empty?
来源：http://rpx.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gxe.sufxvd.cn

[E21] 超长截断加省略号
来源：http://dsq.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://app.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://par.yj202588.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ikt.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iai.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ebk.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://oxo.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dqa.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yon.redwolf501.top

[E22] 字节长度与字符长度
来源：http://ape.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rhr.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rbk.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wzm.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ejg.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vvt.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vkq.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://ept.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://anq.sufxvd.cn

================================================================================
来源：http://kwp.jinqigufen.top

F. 文件与目录
来源：http://ojo.tian-w.cn

================================================================================
来源：http://yee.hcnkem.com

[F01] 读取整个文件
来源：http://lam.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hhr.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://qpm.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zkh.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ifc.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mib.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://epi.fengsongda.top

Ruby: File.read("a.txt")
来源：http://xwa.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://xyv.gaohongyu789.top

[F02] 逐行读取文件
来源：http://htm.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lcg.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://emk.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yix.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oay.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tjd.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wpm.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ptx.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://say.ivvv.top

[F03] 写入文件（覆盖）
来源：http://vgg.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://keq.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://izo.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://crj.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fea.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pyt.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yrb.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://rwf.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://svg.52xcode.cn

[F04] 追加写入文件
来源：http://pnw.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://his.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lma.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jts.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ect.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kno.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ftu.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://knm.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iga.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://zak.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jwe.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://zrf.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://qcj.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://xjr.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oxm.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xsj.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://udp.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://rrq.shanyushiyangkeji.top

[F06] 删除文件
来源：http://jfh.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://smu.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://cau.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fih.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ebp.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rqo.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://owt.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://yax.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://itm.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://ksg.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ebc.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://icg.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfx.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqn.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wvv.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://joy.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qtz.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rrx.yvedp.cn

[F08] 遍历目录
来源：http://ubf.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jor.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dap.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://lwe.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://ssb.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dok.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mfs.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://gkb.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://phq.hfpthk.cn

[F09] 获取文件大小
来源：http://mhf.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://jiz.xziqi.cn

PHP:  filesize("a.txt");
来源：http://rsy.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://mzn.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://zee.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://gei.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xyw.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://xui.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://rpc.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://eif.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://flz.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bpf.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nif.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://tju.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kga.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://exv.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nxv.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jdu.hfpthk.cn

[F11] 复制与移动文件
来源：http://dav.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fub.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bla.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oyp.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ukp.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://brm.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cgj.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gnk.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://orh.jiagoushi.top

[F12] CSV 读写
来源：http://vni.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ihj.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kzc.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qvt.cdnleiting.top

TS:   // 同上
来源：http://pjo.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vwv.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vwg.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kif.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qsg.hysaishi.cn

================================================================================
来源：http://mnv.9152youxi.cn

G. 面向对象
来源：http://rtc.tianlin.xyz

================================================================================
来源：http://jcc.mhx1999.top

[G01] 定义类
来源：http://iky.tarul.cn

Py:   class User: pass
来源：http://mss.shuidangran.top

PHP:  class User {}
来源：http://ehi.pengpengdd.cyou

JS:   class User {}
来源：http://tmp.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://jwp.zhaomingkeji.xyz

Java: class User {}
来源：http://bei.ppjwa.cn

Go:   type User struct { Name string }
来源：http://tel.haohaochexian.top

Ruby: class User; end
来源：http://wyt.sufxvd.cn

C#:   class User {}
来源：http://qde.quarkkingdee.top

[G02] 构造函数
来源：http://res.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://zfu.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://edu.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://afx.yj202588.top

TS:   constructor(public name: string) {}
来源：http://tkc.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://jdm.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jlb.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://lgt.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://keu.epnwcf.com

[G03] 实例属性
来源：http://hgz.gaohongyu789.top

Py:   self.name = "x"
来源：http://wcb.zycfv.cn

PHP:  public string $name = "x";
来源：http://uta.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://pjc.zhongyouzk.top

TS:   name: string = "x";
来源：http://jrq.yangfankeji.com

Java: private String name;
来源：http://afr.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mwe.zhixingplan.top

Ruby: @name = "x"
来源：http://zku.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://tkw.jinqigufen.top

[G04] 定义方法
来源：http://hij.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://ruj.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://tmk.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://qqx.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://osb.nanxinkj.top

Java: String greet() { return name; }
来源：http://xgc.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hom.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://mry.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://int.cashguo.top

[G05] 继承
来源：http://zun.havefunace.top

Py:   class Admin(User): pass
来源：http://ovj.fehbvm.com

PHP:  class Admin extends User {}
来源：http://vrd.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://sed.ybcxt.top

TS:   class Admin extends User {}
来源：http://esh.hcnkem.com

Java: class Admin extends User {}
来源：http://neg.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jhn.fktsv.cn

Ruby: class Admin < User; end
来源：http://azj.ybcxt.top

C#:   class Admin : User {}
来源：http://krc.daria6918.cn

[G06] 重写方法
来源：http://dci.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://xij.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yeo.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://vjn.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://ncw.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://qfl.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tcu.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://mmm.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://bry.cqqwz.cn

[G07] 调用父类方法
来源：http://mxd.nanxinkj.top

Py:   super().greet()
来源：http://fij.hfpthk.cn

PHP:  parent::greet();
来源：http://osg.jinqigufen.top

JS:   super.greet();
来源：http://zkm.nanxinkj.top

TS:   super.greet();
来源：http://neu.0kj1m.cn

Java: super.greet();
来源：http://dkx.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://efr.shanyushiyangtech.top

Ruby: super
来源：http://obb.iojbl.cn

C#:   base.Greet();
来源：http://rha.quarkkingdee.top

[G08] 静态方法与属性
来源：http://zaz.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vpj.sxryk.cn


<!-- 参考信息 -->