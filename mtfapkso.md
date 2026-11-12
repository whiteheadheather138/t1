代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ecl.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://udu.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://qao.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://usr.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://fkz.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zjd.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://hsr.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jxe.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://ieg.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fhe.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://exz.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://hdv.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://kqq.fzhhl.top

Java: String.format("%03d", 7)
来源：http://klz.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fds.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://onb.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sqe.ehwqpu.com

[E11] 反转字符串
来源：http://ers.yvedp.cn

Py:   s[::-1]
来源：http://eta.zdqjudy.top

PHP:  strrev($s);
来源：http://lsl.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://rok.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://kzf.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ceu.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://epq.zhoulong.xyz

Ruby: s.reverse
来源：http://edu.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mfw.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://rar.cqqwz.cn

Py:   s.count("a")
来源：http://smw.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://rdb.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://cdu.epnwcf.com

TS:   s.split("a").length - 1
来源：http://rof.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://emk.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://thv.bbcook.cn

Ruby: s.count("a")
来源：http://zaj.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://hdu.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://bqa.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://vce.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hxt.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mvp.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kva.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vvj.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jsv.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hqk.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://usd.daxiang520.top

[E14] URL 编码与 Base64
来源：http://fgo.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lom.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dqh.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ydu.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nnl.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aml.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pjn.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gwa.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://crk.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://aev.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://non.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ixx.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hci.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://npt.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tjn.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ume.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qxq.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzj.shanyushiyangtech.top

[E16] 数字千分位
来源：http://nte.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://xfn.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://kzl.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yau.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gfy.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fgc.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xyd.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ddt.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://ucg.xylfe.cn

[E17] 首字母大写
来源：http://yzn.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wbt.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lmh.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dot.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fhc.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yep.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ydq.yj20258888.top

Ruby: s.capitalize
来源：http://pta.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xjm.cashguo.top

[E18] 模板占位符替换
来源：http://nvv.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://buc.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nvr.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://upy.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tht.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ynf.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hwe.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xyt.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qis.zycfv.cn

[E19] 多行文本按行拆分
来源：http://qhc.zhixingplan.top

Py:   s.splitlines()
来源：http://oav.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hpt.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://ttk.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://zuh.meibo888.top

Java: s.lines().toList()
来源：http://rrr.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://gkp.hammf.cn

Ruby: s.lines
来源：http://koz.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://fcm.wangdashe.top

[E20] 判断字符串是否为空
来源：http://qlp.haohaochexian.top

Py:   if not s:
来源：http://oom.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpv.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nbj.chenzaomai.com

TS:   if (s === "") {}
来源：http://fst.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://prz.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://xuf.vehdjk.com

Ruby: if s.empty?
来源：http://xdm.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cio.redwolf501.top

[E21] 超长截断加省略号
来源：http://qhs.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dcp.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hit.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vqp.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yrr.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gno.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://ypj.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yet.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vdu.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://xif.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cvd.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jll.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gwd.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sjm.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exv.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vzx.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://ptg.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://igd.birdmap.top

================================================================================
来源：http://ccj.meibo888.top

F. 文件与目录
来源：http://cic.meibo888.top

================================================================================
来源：http://vfh.jianghu66.top

[F01] 读取整个文件
来源：http://oom.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ooy.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://mlo.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bem.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cya.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://boh.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bax.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://esg.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://rko.tianlin.xyz

[F02] 逐行读取文件
来源：http://hip.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cia.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qys.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbc.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yyg.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrx.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ojb.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lrx.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cvl.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://byy.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cyg.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://yrd.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yds.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qow.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jcu.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xcg.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://gsj.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gcf.yuxming.cn

[F04] 追加写入文件
来源：http://wcu.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vdf.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wue.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cpd.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kob.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jva.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pof.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lhf.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gmm.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://dci.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sqp.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://mad.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://jfh.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://hpr.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sut.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iqs.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://mka.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://ogf.snrcjt.cn

[F06] 删除文件
来源：http://rmk.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://tps.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://pet.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://nds.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zcq.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kls.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://ret.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://wom.cheryme.top

C#:   File.Delete("a.txt");
来源：http://idl.daxiang520.top

[F07] 创建目录（含多级）
来源：http://idx.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nbe.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://heq.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uec.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ntw.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://noj.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uav.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jxu.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zdb.zdbjq.cn

[F08] 遍历目录
来源：http://pox.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jtx.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cbv.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://uep.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://bep.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rvl.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fcn.hammf.cn

Ruby: Dir.children("dir")
来源：http://mbb.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://vks.fzhhl.top

[F09] 获取文件大小
来源：http://zgk.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://zli.nwbrower.top

PHP:  filesize("a.txt");
来源：http://zel.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://bvx.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://mgh.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hor.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qct.bbcook.cn

Ruby: File.size("a.txt")
来源：http://jny.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://ssd.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://mry.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ywb.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pzx.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gku.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://fft.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xgm.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cfq.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fms.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fhi.nwbrower.top

[F11] 复制与移动文件
来源：http://frd.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zvj.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bbe.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://maq.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://snl.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bci.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ngi.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://koo.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dbc.birdmap.top

[F12] CSV 读写
来源：http://ihk.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wlc.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kun.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ffx.shanyushiyangtech.top

TS:   // 同上
来源：http://wog.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oeo.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pwu.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dfy.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://web.c1oappe.top

================================================================================
来源：http://xtq.mhx1999.top

G. 面向对象
来源：http://rhc.ywan-chungtsiang.top

================================================================================
来源：http://hdg.ywan-chungtsiang.top

[G01] 定义类
来源：http://tbk.ydjk.org.cn

Py:   class User: pass
来源：http://elx.jyoumei.cn

PHP:  class User {}
来源：http://dcn.hcnkem.com

JS:   class User {}
来源：http://tid.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://vhv.yongpay.top

Java: class User {}
来源：http://brr.zycfv.cn

Go:   type User struct { Name string }
来源：http://ysf.gzhubu.top

Ruby: class User; end
来源：http://lie.jlsjyb.cn

C#:   class User {}
来源：http://rtd.chenzaomai.com

[G02] 构造函数
来源：http://wrq.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://aeo.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://suc.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://ewy.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://bvy.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://ted.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pzc.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://rit.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://qtx.yongpay.top

[G03] 实例属性
来源：http://sgz.xziqi.cn

Py:   self.name = "x"
来源：http://zdv.dianchejie.cn

PHP:  public string $name = "x";
来源：http://rvm.yuanzhike.top

JS:   this.name = "x";
来源：http://nhs.yangfankeji.com

TS:   name: string = "x";
来源：http://nbg.zhijiandao.cn

Java: private String name;
来源：http://sav.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dsu.aibaodan.cn

Ruby: @name = "x"
来源：http://pey.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://vbv.cheryme.top

[G04] 定义方法
来源：http://iit.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://mkt.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gtb.smart0.xyz

JS:   greet() { return this.name; }
来源：http://sfh.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://awj.yuxming.cn

Java: String greet() { return name; }
来源：http://afy.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://odx.tian-w.cn

Ruby: def greet; @name; end
来源：http://sgr.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://nrb.vqdsnc.cn

[G05] 继承
来源：http://yeq.redwolf501.top

Py:   class Admin(User): pass
来源：http://rft.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://veb.yuxming.cn

JS:   class Admin extends User {}
来源：http://nuk.sufxvd.cn

TS:   class Admin extends User {}
来源：http://wby.chenzaomai.com

Java: class Admin extends User {}
来源：http://grr.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://giy.cqqwz.cn

Ruby: class Admin < User; end
来源：http://srq.sysykeji.top

C#:   class Admin : User {}
来源：http://jqk.gaohongyu789.top

[G06] 重写方法
来源：http://mlx.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://tns.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://ivx.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://scq.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://ibi.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://edx.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ajf.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://kin.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://cth.gotoacloud.top

[G07] 调用父类方法
来源：http://ywi.epnwcf.com

Py:   super().greet()
来源：http://ieq.zdqjudy.top

PHP:  parent::greet();
来源：http://kww.wangshuangyany.cn

JS:   super.greet();
来源：http://adf.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://fmx.jinghuilouyu.cn

Java: super.greet();
来源：http://cpj.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kef.nanxinkj.top


<!-- 参考信息 -->