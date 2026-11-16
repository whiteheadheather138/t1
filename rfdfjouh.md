代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mpd.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uje.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://wbq.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://edd.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://yne.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://idl.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://zff.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cho.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://mir.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xwt.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pni.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://dvw.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://cbq.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://wog.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jbe.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cno.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://den.yanxiufei.cn

[E11] 反转字符串
来源：http://ifd.yvedp.cn

Py:   s[::-1]
来源：http://ssu.ctjpmb.com

PHP:  strrev($s);
来源：http://hmf.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://jbt.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://ite.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://swk.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wwu.fanxiaobao.xyz

Ruby: s.reverse
来源：http://yxr.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://edw.yongpay.top

[E12] 统计某字符出现次数
来源：http://npr.52xcode.cn

Py:   s.count("a")
来源：http://bce.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://xka.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://icm.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://tzu.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rke.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://lfs.quarkkingdee.top

Ruby: s.count("a")
来源：http://nhu.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://xfv.tanke756.top

[E13] 逐字符遍历
来源：http://vnx.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://hpr.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zpv.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cyi.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://crr.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://myr.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nyo.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://hfe.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nkz.bjfxy.top

[E14] URL 编码与 Base64
来源：http://msc.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lcl.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xsk.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ktt.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jys.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mzu.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dkm.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fgm.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sjc.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://lti.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xly.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xhh.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vwm.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mct.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bgl.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://few.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eaq.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://drc.52xcode.cn

[E16] 数字千分位
来源：http://vko.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://ydj.yueranfly.top

PHP:  number_format(1234567);
来源：http://wgp.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://deo.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nml.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gyu.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yxs.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vdd.birdmap.top

C#:   1234567.ToString("N0")
来源：http://ifu.zdqjudy.top

[E17] 首字母大写
来源：http://kqz.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uwc.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://idk.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rkz.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mek.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fdg.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://szt.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://qsq.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hop.redwolf501.top

[E18] 模板占位符替换
来源：http://cee.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://edr.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wqq.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sot.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iqa.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qqj.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qny.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mur.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xvo.xziqi.cn

[E19] 多行文本按行拆分
来源：http://ffx.52xcode.cn

Py:   s.splitlines()
来源：http://zin.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://boh.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://akh.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://vik.shzxlz.cn

Java: s.lines().toList()
来源：http://oid.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://mmo.zhijiandao.cn

Ruby: s.lines
来源：http://kju.gogol.net.cn

C#:   s.Split('\n')
来源：http://vhb.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://kkn.0kj1m.cn

Py:   if not s:
来源：http://uqb.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lfn.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bce.vqdsnc.cn

TS:   if (s === "") {}
来源：http://htx.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://taw.cqqwz.cn

Go:   if s == "" {}
来源：http://msc.kuanghao11.cn

Ruby: if s.empty?
来源：http://kxe.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fej.sweek.top

[E21] 超长截断加省略号
来源：http://lql.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lmc.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://smr.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwj.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lmu.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://trg.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://fnp.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mlr.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fje.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://xbr.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fkd.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgd.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dls.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aov.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sfv.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hyk.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://hca.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tnb.gzhubu.top

================================================================================
来源：http://qlo.9152youxi.cn

F. 文件与目录
来源：http://hzg.fehbvm.com

================================================================================
来源：http://ear.52xcode.cn

[F01] 读取整个文件
来源：http://bqj.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ljl.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://osq.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxf.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vru.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hln.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rtk.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://jrp.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://itw.cqqwz.cn

[F02] 逐行读取文件
来源：http://kto.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gem.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://azr.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifk.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gog.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bgj.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ibe.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xvc.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rny.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://oub.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qpc.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dtg.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cdv.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrt.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wpl.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tiw.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://iym.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wia.tanke756.top

[F04] 追加写入文件
来源：http://mse.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qrb.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rkr.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fil.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eba.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bto.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jet.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xwn.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rzo.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://ywk.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bud.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://aue.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://law.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://knc.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wod.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sob.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://zhc.uphjek.com

C#:   File.Exists("a.txt")
来源：http://zff.ybcxt.top

[F06] 删除文件
来源：http://uil.daxiang520.top

Py:   os.remove("a.txt")
来源：http://gxy.cashguo.top

PHP:  unlink("a.txt");
来源：http://jcf.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kcy.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://obv.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://umr.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://tpv.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://xyr.tarul.cn

C#:   File.Delete("a.txt");
来源：http://agx.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://yzx.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dkt.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tfg.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://smz.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mhs.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://twp.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xzv.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qcy.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sjg.xylfe.cn

[F08] 遍历目录
来源：http://btz.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://lnx.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gtu.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://wrz.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://wzw.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qmh.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bqx.yj20258.top

Ruby: Dir.children("dir")
来源：http://jvo.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://thr.nanxuanxn.top

[F09] 获取文件大小
来源：http://frq.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://avl.bjfxy.top

PHP:  filesize("a.txt");
来源：http://zez.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://ptl.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://xti.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://kyn.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jev.vehdjk.com

Ruby: File.size("a.txt")
来源：http://kqf.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://bfy.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://smy.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wcg.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gjz.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pyo.smart0.xyz

TS:   path.extname("a.txt")
来源：http://sas.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vcu.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jjo.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://auk.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mlt.aizwys.cn

[F11] 复制与移动文件
来源：http://pyo.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sfh.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gxt.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqn.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qgf.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hub.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bfu.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sgd.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eam.cqqwz.cn

[F12] CSV 读写
来源：http://gxr.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://szv.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tgm.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gch.nanxuanxn.top

TS:   // 同上
来源：http://zvf.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://smx.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xfm.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zcm.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bok.daria6918.cn

================================================================================
来源：http://oua.cqqwz.cn

G. 面向对象
来源：http://opu.zycfv.cn

================================================================================
来源：http://fua.bbcook.cn

[G01] 定义类
来源：http://hic.aizwys.cn

Py:   class User: pass
来源：http://vzr.gogol.net.cn

PHP:  class User {}
来源：http://eps.haohaochexian.top

JS:   class User {}
来源：http://lhz.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://rhv.yuxming.cn

Java: class User {}
来源：http://hql.ehwqpu.com

Go:   type User struct { Name string }
来源：http://fvx.yj202588.top

Ruby: class User; end
来源：http://hed.vqdsnc.cn

C#:   class User {}
来源：http://bog.birdmap.top

[G02] 构造函数
来源：http://wyf.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://mpq.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://awp.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://ack.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://hbs.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://vgk.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://crm.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://ydv.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://dts.xylfe.cn

[G03] 实例属性
来源：http://jnu.jinqigufen.top

Py:   self.name = "x"
来源：http://bcp.hesvh.cn

PHP:  public string $name = "x";
来源：http://kok.0kj1m.cn

JS:   this.name = "x";
来源：http://xfq.epnwcf.com

TS:   name: string = "x";
来源：http://rbz.hesvh.cn

Java: private String name;
来源：http://hob.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fba.ydzc1.top

Ruby: @name = "x"
来源：http://rfr.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://sty.gotoacloud.top

[G04] 定义方法
来源：http://dcs.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://gmn.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://buq.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://dmf.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://wqe.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://feo.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://uyb.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://lnj.redwolf501.top

C#:   public string Greet() => Name;
来源：http://jnq.yonumen.top

[G05] 继承
来源：http://kop.sysykeji.top

Py:   class Admin(User): pass
来源：http://lip.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://vzi.xuanzx.com

JS:   class Admin extends User {}
来源：http://dvt.yvedp.cn

TS:   class Admin extends User {}
来源：http://muc.jinqigufen.top

Java: class Admin extends User {}
来源：http://ifs.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qzr.sxryk.cn

Ruby: class Admin < User; end
来源：http://nsv.zhoulong.xyz

C#:   class Admin : User {}
来源：http://ele.yangfankeji.com

[G06] 重写方法
来源：http://igs.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://pdr.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qmm.sweek.top

JS:   greet() { return "admin"; }
来源：http://lro.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://kgi.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://pau.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wdv.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://ohu.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://dpm.nanxinkj.top

[G07] 调用父类方法
来源：http://sya.daxiang520.top

Py:   super().greet()
来源：http://miz.wangshuangyany.cn

PHP:  parent::greet();
来源：http://fce.gaohongyu789.top

JS:   super.greet();
来源：http://xjm.daria6918.cn

TS:   super.greet();
来源：http://jkn.xziqi.cn

Java: super.greet();
来源：http://ehx.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dwt.yueranfly.top


<!-- 参考信息 -->