代发 wailian999

Go:   strings.Join(items, ",")
来源：http://fiz.yvedp.cn

Ruby: items.join(",")
来源：http://mzo.guannengcc.top

C#:   string.Join(",", items)
来源：http://ojd.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://abr.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vqf.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rnm.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://weh.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://bul.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://tla.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lce.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://jux.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jwz.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://syt.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yqo.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gzj.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://jms.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://lmi.cucudq.cn

Java: String.format("%03d", 7)
来源：http://phu.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://gml.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vut.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dpq.yuanzhike.top

[E11] 反转字符串
来源：http://smu.tarul.cn

Py:   s[::-1]
来源：http://xzb.yangfankeji.com

PHP:  strrev($s);
来源：http://iep.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://moq.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://rpt.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zxv.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uxb.chenlongwang.top

Ruby: s.reverse
来源：http://ypj.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://vqe.yueranfly.top

[E12] 统计某字符出现次数
来源：http://iok.ctjpmb.com

Py:   s.count("a")
来源：http://zus.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://rri.yongpay.top

JS:   s.split("a").length - 1
来源：http://miq.gzhubu.top

TS:   s.split("a").length - 1
来源：http://slo.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cxc.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://blo.gzhubu.top

Ruby: s.count("a")
来源：http://uip.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://vzk.snrcjt.cn

[E13] 逐字符遍历
来源：http://pai.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://plx.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nmb.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bec.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://iif.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ruw.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sri.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sme.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bzj.ivvv.top

[E14] URL 编码与 Base64
来源：http://jgd.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yja.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://adt.52xcode.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rcs.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://laz.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://njf.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ocl.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://exl.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jfx.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://jks.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://uub.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mmr.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vij.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://det.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ozi.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ezr.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bmp.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wym.jyoumei.cn

[E16] 数字千分位
来源：http://dqv.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://sdf.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://cwm.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xtc.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xpb.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hol.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bew.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tfy.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://vfy.redwolf501.top

[E17] 首字母大写
来源：http://vsg.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gxb.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fzu.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aef.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fdb.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nyt.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qgz.quarkkingdee.top

Ruby: s.capitalize
来源：http://xlv.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rax.guowangkeji.top

[E18] 模板占位符替换
来源：http://ibx.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aqb.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wcu.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://kjf.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://yhk.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aah.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tgx.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qyl.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ldm.52xcode.cn

[E19] 多行文本按行拆分
来源：http://ewv.yj20258.top

Py:   s.splitlines()
来源：http://cds.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pja.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://hvc.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://poh.zhengqikj.top

Java: s.lines().toList()
来源：http://slb.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://oti.yj202588.top

Ruby: s.lines
来源：http://bcr.yongpay.top

C#:   s.Split('\n')
来源：http://buz.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://glq.ydjk.org.cn

Py:   if not s:
来源：http://zzo.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uwz.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://arc.ydjk.org.cn

TS:   if (s === "") {}
来源：http://reu.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://nbp.yangfankeji.com

Go:   if s == "" {}
来源：http://ktw.sjlbkw.cn

Ruby: if s.empty?
来源：http://wnv.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ipe.tarul.cn

[E21] 超长截断加省略号
来源：http://ogj.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lvz.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xam.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jdf.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://apo.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jyn.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://tjx.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ihw.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gdz.tarul.cn

[E22] 字节长度与字符长度
来源：http://xqm.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wqu.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hnk.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hfw.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sax.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dpa.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://buy.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://jga.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gxv.epnwcf.com

================================================================================
来源：http://fon.c1oappe.top

F. 文件与目录
来源：http://lkb.shanyushiyangtech.top

================================================================================
来源：http://slf.jinqigufen.top

[F01] 读取整个文件
来源：http://xqm.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rck.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://fwt.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rms.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pny.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nev.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rbs.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://msq.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://tce.tanke756.top

[F02] 逐行读取文件
来源：http://hrs.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qxu.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jbg.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mub.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://crq.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ucq.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lpw.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hru.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zcd.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://dhp.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yol.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hfo.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdz.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uxj.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pwr.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kbr.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://yyc.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ouo.sufxvd.cn

[F04] 追加写入文件
来源：http://ubj.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wmr.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yms.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvg.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://doj.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yrq.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rtx.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aeq.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cpa.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://pal.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xky.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://uhb.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://spc.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://nmf.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hgr.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eth.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://zqr.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://izr.sysykeji.top

[F06] 删除文件
来源：http://gkj.ybcxt.top

Py:   os.remove("a.txt")
来源：http://orj.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://hih.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zxx.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fyd.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fks.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://kiv.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://zuu.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://pfh.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://zvy.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bat.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://muj.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nnn.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khu.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://njq.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rgz.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zon.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ghd.vehdjk.com

[F08] 遍历目录
来源：http://gib.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iea.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://liz.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://kmj.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://wxu.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dcb.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lzd.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://gfj.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://hys.xuetiantiany.cn

[F09] 获取文件大小
来源：http://rmd.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://ref.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://ebd.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://lei.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://sme.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://duf.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ybm.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://xbl.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://nmc.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://oss.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://btd.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wis.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://abu.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://zcw.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qew.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://abf.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rly.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://prl.fktsv.cn

[F11] 复制与移动文件
来源：http://fzs.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gzm.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://awi.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cez.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jae.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lgj.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vjb.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zve.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bcd.iojbl.cn

[F12] CSV 读写
来源：http://evh.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fsy.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://awp.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijo.yfazqb.com

TS:   // 同上
来源：http://qir.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xph.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dfj.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ivb.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gcs.shanyushiyangkeji.top

================================================================================
来源：http://zxq.zhijiandao.cn

G. 面向对象
来源：http://ubq.jlsjyb.cn

================================================================================
来源：http://oen.fktsv.cn

[G01] 定义类
来源：http://ivp.epnwcf.com

Py:   class User: pass
来源：http://yus.ehwqpu.com

PHP:  class User {}
来源：http://tye.chenjidiqi.icu

JS:   class User {}
来源：http://err.birdmap.top

TS:   class User { name: string = ""; }
来源：http://qob.cheryme.top

Java: class User {}
来源：http://bci.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://kqt.fehbvm.com

Ruby: class User; end
来源：http://htd.jqgufenzy.top

C#:   class User {}
来源：http://dwo.ybcxt.top

[G02] 构造函数
来源：http://eyg.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://wnu.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://mcf.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://hvn.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://qxt.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://cwn.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qve.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://aog.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://ryh.xylfe.cn

[G03] 实例属性
来源：http://sbc.cqqwz.cn

Py:   self.name = "x"
来源：http://xuz.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://ftk.jinqigfzy.top

JS:   this.name = "x";
来源：http://exa.ydjk.org.cn

TS:   name: string = "x";
来源：http://bii.xuetiantiany.cn

Java: private String name;
来源：http://tes.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oyj.andypj.xyz

Ruby: @name = "x"
来源：http://xxr.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://pba.c1oappe.top

[G04] 定义方法
来源：http://jwg.hammf.cn

Py:   def greet(self): return self.name
来源：http://xpz.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://fsj.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://rji.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://sbm.birdmap.top

Java: String greet() { return name; }
来源：http://xpl.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lpx.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://crs.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://ssn.xinyue.icu

[G05] 继承
来源：http://ekw.meibo888.top

Py:   class Admin(User): pass
来源：http://qqq.uphjek.com

PHP:  class Admin extends User {}
来源：http://nrs.xziqi.cn

JS:   class Admin extends User {}
来源：http://flx.hysaishi.cn

TS:   class Admin extends User {}
来源：http://yox.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://ykq.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qej.xylfe.cn

Ruby: class Admin < User; end
来源：http://ozx.nanxuanxn.top

C#:   class Admin : User {}
来源：http://gmn.zhijiandao.cn

[G06] 重写方法
来源：http://pya.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://ksg.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qhe.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://nai.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://syx.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://iws.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yvh.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://xyg.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://uqn.aibaodan.cn

[G07] 调用父类方法
来源：http://dmw.meibo888.top

Py:   super().greet()
来源：http://hmu.cqqwz.cn

PHP:  parent::greet();
来源：http://syx.cashguo.top


<!-- 参考信息 -->