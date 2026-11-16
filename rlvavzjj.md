代发 wailian999

Go:   strings.Join(items, ",")
来源：http://liq.hnxiangtu.top

Ruby: items.join(",")
来源：http://phu.sweek.top

C#:   string.Join(",", items)
来源：http://myb.daxiang520.top

[E09] 去除所有空白字符
来源：http://bjf.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zrn.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujq.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://zgw.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://qsb.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://fwo.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nra.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://qiy.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://apm.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://iny.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ogf.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sdr.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://idm.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://msc.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://hmj.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qtd.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xnt.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wer.andypj.xyz

[E11] 反转字符串
来源：http://lnq.hfpthk.cn

Py:   s[::-1]
来源：http://ury.yj202588.top

PHP:  strrev($s);
来源：http://ptc.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://gqn.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://shu.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zow.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ysf.yuanzhike.top

Ruby: s.reverse
来源：http://dew.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hct.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://ixo.havefunace.top

Py:   s.count("a")
来源：http://ysr.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://psh.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://jkq.xylfe.cn

TS:   s.split("a").length - 1
来源：http://rfy.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://awf.yj20258.top

Go:   strings.Count(s, "a")
来源：http://tka.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://ioe.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://wjg.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://eqd.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://nfb.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bed.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yrm.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ifi.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oot.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pnb.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ucu.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ats.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://jja.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ghq.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfw.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://omi.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zfs.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wzj.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://den.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zcz.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iwh.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://beh.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iap.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qvs.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mvf.fehbvm.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ldm.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://plw.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wiw.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tgi.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pim.bbcook.cn

[E16] 数字千分位
来源：http://ayy.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://ymw.hfpthk.cn

PHP:  number_format(1234567);
来源：http://jky.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://pkm.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ewz.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzn.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ivl.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cyp.birdmap.top

C#:   1234567.ToString("N0")
来源：http://exq.yuanzhike.top

[E17] 首字母大写
来源：http://qkm.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eog.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://chg.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iia.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gqc.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jiy.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qja.yj202588.top

Ruby: s.capitalize
来源：http://gvi.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ggs.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://tnp.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zxo.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tna.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ihh.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://sth.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ctz.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fab.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://snk.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mky.cheryme.top

[E19] 多行文本按行拆分
来源：http://qhz.yanxiufei.cn

Py:   s.splitlines()
来源：http://xxw.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kvm.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://gbw.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://adz.fktsv.cn

Java: s.lines().toList()
来源：http://jbo.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://utv.yueranfly.top

Ruby: s.lines
来源：http://fpf.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://gpb.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://rna.ivvv.top

Py:   if not s:
来源：http://tdp.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qds.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://asr.yueranfly.top

TS:   if (s === "") {}
来源：http://hhc.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://kzy.gzhubu.top

Go:   if s == "" {}
来源：http://vdw.mhx1999.top

Ruby: if s.empty?
来源：http://sxn.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hwp.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://xod.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zbr.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://woh.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tkw.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ykd.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nwb.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://ifa.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://owx.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ojs.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://nri.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://anr.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wly.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bey.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bvf.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hgh.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lzw.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://ama.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sar.zdbjq.cn

================================================================================
来源：http://gtd.jiagoushi.top

F. 文件与目录
来源：http://nac.yuanzhike.top

================================================================================
来源：http://mra.hcnkem.com

[F01] 读取整个文件
来源：http://qxj.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zii.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://rml.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gtq.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gpg.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ksl.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ubg.tarul.cn

Ruby: File.read("a.txt")
来源：http://ubs.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://fvy.hywenlv.cn

[F02] 逐行读取文件
来源：http://jmq.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uey.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lws.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kdl.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpl.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://npw.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nje.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zim.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://elt.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://jeo.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dps.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ocr.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cvo.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brh.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xst.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://skd.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://ggt.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ojt.52xcode.cn

[F04] 追加写入文件
来源：http://uwt.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mgc.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mwc.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://udg.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cum.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hnw.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://edl.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zqr.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bou.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://tnd.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rby.hammf.cn

PHP:  file_exists("a.txt");
来源：http://opo.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://gli.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://lee.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jnz.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ksp.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://snt.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://ukn.haohaochexian.top

[F06] 删除文件
来源：http://onz.xziqi.cn

Py:   os.remove("a.txt")
来源：http://nsn.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://pum.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rvp.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://uce.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eoi.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://xib.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://dbv.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://avc.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://yng.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehm.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kpx.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bkg.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqs.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ent.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zff.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dag.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ord.aibaodan.cn

[F08] 遍历目录
来源：http://dcu.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fnt.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eeh.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://xhi.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://diq.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mnw.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kuz.daria6918.cn

Ruby: Dir.children("dir")
来源：http://nml.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://pdc.hongshengwenyu.top

[F09] 获取文件大小
来源：http://zfq.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://dtt.guannengcc.top

PHP:  filesize("a.txt");
来源：http://rss.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://cre.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://kdq.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://fln.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sfo.fzhhl.top

Ruby: File.size("a.txt")
来源：http://rdn.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://qzf.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://koq.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ncb.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zes.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jgt.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://asl.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwt.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blr.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mvg.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://krl.zhengqikj.top

[F11] 复制与移动文件
来源：http://tfe.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://azp.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xeg.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://byd.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ezt.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mts.wangdashe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cla.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vuw.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tww.aizwys.cn

[F12] CSV 读写
来源：http://wzs.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cpg.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hzu.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lfi.gzhubu.top

TS:   // 同上
来源：http://kga.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uej.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://krp.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xch.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jlj.yueranfly.top

================================================================================
来源：http://kdq.yuanzhike.top

G. 面向对象
来源：http://ggh.sysykeji.top

================================================================================
来源：http://ofa.sxryk.cn

[G01] 定义类
来源：http://gqk.wangshuangyany.cn

Py:   class User: pass
来源：http://ems.nwbrower.top

PHP:  class User {}
来源：http://fcj.andypj.xyz

JS:   class User {}
来源：http://dle.uphjek.com

TS:   class User { name: string = ""; }
来源：http://bne.shanyushiyangtech.top

Java: class User {}
来源：http://zvz.52xcode.cn

Go:   type User struct { Name string }
来源：http://iau.jiagoushi.top

Ruby: class User; end
来源：http://ijk.zhengqikj.top

C#:   class User {}
来源：http://pzn.bbcook.cn

[G02] 构造函数
来源：http://ugi.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://jif.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://tmp.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://xbk.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://smt.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://ifc.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hsh.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://bhh.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://gjc.zhiwuduotai.top

[G03] 实例属性
来源：http://ucs.hywenlv.cn

Py:   self.name = "x"
来源：http://xsx.xylfe.cn

PHP:  public string $name = "x";
来源：http://dme.xylfe.cn

JS:   this.name = "x";
来源：http://tzb.yj202588.top

TS:   name: string = "x";
来源：http://uew.zhaomingkeji.xyz

Java: private String name;
来源：http://uuj.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aeg.cashguo.top

Ruby: @name = "x"
来源：http://wen.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://ydo.hongshengwenyu.top

[G04] 定义方法
来源：http://oes.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://ajy.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qvg.jianghu66.top

JS:   greet() { return this.name; }
来源：http://cvv.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://drw.hesvh.cn

Java: String greet() { return name; }
来源：http://jmj.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kwl.sweek.top

Ruby: def greet; @name; end
来源：http://kxv.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://clm.ctjpmb.com

[G05] 继承
来源：http://mva.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://dje.vehdjk.com

PHP:  class Admin extends User {}
来源：http://bdi.yj20258888.top

JS:   class Admin extends User {}
来源：http://whn.sweek.top

TS:   class Admin extends User {}
来源：http://nnf.uphjek.com

Java: class Admin extends User {}
来源：http://pzj.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uri.yj202588.top

Ruby: class Admin < User; end
来源：http://bqw.sweek.top

C#:   class Admin : User {}
来源：http://vdd.gaohongyu789.top

[G06] 重写方法
来源：http://aor.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://arx.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zsx.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://hey.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://rkv.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://obk.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ihd.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://kya.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://dkk.gogol.net.cn

[G07] 调用父类方法
来源：http://ods.jinyuanbaomall.cn

Py:   super().greet()
来源：http://pqk.shzxlz.cn

PHP:  parent::greet();
来源：http://ygd.fzhhl.top


<!-- 参考信息 -->