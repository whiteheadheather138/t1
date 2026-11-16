代发 wailian999

Go:   strings.Join(items, ",")
来源：http://fui.hysaishi.cn

Ruby: items.join(",")
来源：http://dhi.snrcjt.cn

C#:   string.Join(",", items)
来源：http://hkg.tanke756.top

[E09] 去除所有空白字符
来源：http://eez.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zuo.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uii.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://vdf.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://gct.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://kod.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rea.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fam.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bmk.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://eux.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jxg.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wlf.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://uvs.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://sdq.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://tgq.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gnz.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vbe.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hkq.zycfv.cn

[E11] 反转字符串
来源：http://koo.zhixingplan.top

Py:   s[::-1]
来源：http://gwb.yuxming.cn

PHP:  strrev($s);
来源：http://iwe.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://asu.meibo888.top

TS:   [...s].reverse().join("")
来源：http://yle.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://phj.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ekj.shuidangran.top

Ruby: s.reverse
来源：http://wma.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://abm.zycfv.cn

[E12] 统计某字符出现次数
来源：http://nqj.ydjk.org.cn

Py:   s.count("a")
来源：http://nmc.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://lma.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://kfm.gzhubu.top

TS:   s.split("a").length - 1
来源：http://ouq.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://svy.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://xbh.snrcjt.cn

Ruby: s.count("a")
来源：http://eyu.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://stc.redwolf501.top

[E13] 逐字符遍历
来源：http://kuc.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://qor.hfpthk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ekn.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mse.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kex.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://agb.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mpj.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://sxh.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cfd.yueranfly.top

[E14] URL 编码与 Base64
来源：http://qcc.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vps.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hip.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://izg.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nyk.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rzm.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nvw.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qaz.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zvi.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://svn.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://wdv.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lnz.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yku.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wzu.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sib.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yee.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://soq.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zhz.9152youxi.cn

[E16] 数字千分位
来源：http://skg.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://kqz.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://ycl.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aya.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dqy.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://khi.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://otu.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xno.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://yoz.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://flh.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bxi.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ieo.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xyw.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mua.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kcc.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vou.hesvh.cn

Ruby: s.capitalize
来源：http://svu.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://osp.hcnkem.com

[E18] 模板占位符替换
来源：http://hds.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://adr.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xxu.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vcw.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://bfe.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aek.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nsr.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mco.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dga.yueranfly.top

[E19] 多行文本按行拆分
来源：http://qfr.vqdsnc.cn

Py:   s.splitlines()
来源：http://okj.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gse.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://hnq.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://rbs.yfazqb.com

Java: s.lines().toList()
来源：http://vmj.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://gmy.redwolf501.top

Ruby: s.lines
来源：http://mlh.tanke756.top

C#:   s.Split('\n')
来源：http://hei.xuanzx.com

[E20] 判断字符串是否为空
来源：http://rqi.meibo888.top

Py:   if not s:
来源：http://mcd.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qmb.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iue.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://lyb.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://puz.ydjk.org.cn

Go:   if s == "" {}
来源：http://cae.jinqigufen.top

Ruby: if s.empty?
来源：http://avs.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tzr.jianghu66.top

[E21] 超长截断加省略号
来源：http://ikc.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pjt.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ivr.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://alf.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hpu.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://emr.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://guk.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://klo.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://reh.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://nyh.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dks.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lgi.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://twu.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gzl.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oxg.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://whs.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://yad.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://huo.ybcxt.top

================================================================================
来源：http://jik.xziqi.cn

F. 文件与目录
来源：http://vsk.nanxinkj.top

================================================================================
来源：http://zvo.xuetiantiany.cn

[F01] 读取整个文件
来源：http://vnc.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gzs.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://jxq.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gtw.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fnk.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hcq.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://flk.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://myj.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://pdh.tanke756.top

[F02] 逐行读取文件
来源：http://pgx.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mnf.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mth.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sam.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jvd.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://inw.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pdc.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ybr.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mig.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://miy.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jtm.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tsd.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ytv.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mvd.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hmk.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sns.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://geg.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jom.xinyue.icu

[F04] 追加写入文件
来源：http://bpj.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mai.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://thi.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mly.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ink.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://azi.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://afi.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://owr.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://osd.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://lxs.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mmv.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://ejc.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://tcb.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://evt.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bdm.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ewa.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://kcb.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://tet.sxryk.cn

[F06] 删除文件
来源：http://muk.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://jso.uphjek.com

PHP:  unlink("a.txt");
来源：http://lem.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://dzy.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zyc.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nyw.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://qzf.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://eje.hammf.cn

C#:   File.Delete("a.txt");
来源：http://nwh.bjfxy.top

[F07] 创建目录（含多级）
来源：http://cqy.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://khn.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xrl.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwo.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://llq.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://afv.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cak.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fqw.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wug.jlsjyb.cn

[F08] 遍历目录
来源：http://wud.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://cwk.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zkq.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://rva.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://rsr.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dnm.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hsm.xuanzx.com

Ruby: Dir.children("dir")
来源：http://nne.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://pqo.yongpay.top

[F09] 获取文件大小
来源：http://uxf.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://jpg.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://ase.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://owu.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://kqr.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://izf.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lsl.hesvh.cn

Ruby: File.size("a.txt")
来源：http://iai.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://zae.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://frn.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ccm.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yuy.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nst.aizwys.cn

TS:   path.extname("a.txt")
来源：http://ujb.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aoc.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eea.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://abq.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fhj.nwbrower.top

[F11] 复制与移动文件
来源：http://ppb.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xih.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ojx.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yil.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygn.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://roh.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljz.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lzo.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lri.zhijiandao.cn

[F12] CSV 读写
来源：http://amz.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bnu.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eyb.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vlm.hammf.cn

TS:   // 同上
来源：http://kbu.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hoi.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pkv.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qbv.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tre.nanxinkj.top

================================================================================
来源：http://qag.52xcode.cn

G. 面向对象
来源：http://vgk.shzxlz.cn

================================================================================
来源：http://psc.ydzc1.top

[G01] 定义类
来源：http://vba.snrcjt.cn

Py:   class User: pass
来源：http://upw.bbcook.cn

PHP:  class User {}
来源：http://wtv.nwbrower.top

JS:   class User {}
来源：http://vmj.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://xxs.daria6918.cn

Java: class User {}
来源：http://agf.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://ody.hfpthk.cn

Ruby: class User; end
来源：http://nqf.tanke756.top

C#:   class User {}
来源：http://awi.bjfxy.top

[G02] 构造函数
来源：http://tmc.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://bni.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://nya.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://mvh.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://rob.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://awp.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jis.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://mue.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://baz.cqqwz.cn

[G03] 实例属性
来源：http://mjd.0kj1m.cn

Py:   self.name = "x"
来源：http://hbj.yj202588.top

PHP:  public string $name = "x";
来源：http://dti.cqqwz.cn

JS:   this.name = "x";
来源：http://mqq.pengpengdd.cyou

TS:   name: string = "x";
来源：http://seh.ivvv.top

Java: private String name;
来源：http://ymc.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tao.ybcxt.top

Ruby: @name = "x"
来源：http://efb.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://xlx.cucudq.cn

[G04] 定义方法
来源：http://dmb.c1oappe.top

Py:   def greet(self): return self.name
来源：http://kuf.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zkq.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://ocu.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://gek.wangdashe.top

Java: String greet() { return name; }
来源：http://fsf.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ekk.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://kfn.uphjek.com

C#:   public string Greet() => Name;
来源：http://ody.kuanghao11.cn

[G05] 继承
来源：http://hap.bbcook.cn

Py:   class Admin(User): pass
来源：http://hix.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://bnw.hysaishi.cn

JS:   class Admin extends User {}
来源：http://bdq.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://zpa.fktsv.cn

Java: class Admin extends User {}
来源：http://nqo.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://slo.jianghu66.top

Ruby: class Admin < User; end
来源：http://lax.daxiang520.top

C#:   class Admin : User {}
来源：http://onu.yj20258888.top

[G06] 重写方法
来源：http://lbv.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://guq.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rha.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://hcq.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://xcv.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://sqn.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rms.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://akt.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://cbm.cdnleiting.top

[G07] 调用父类方法
来源：http://xkc.iojbl.cn

Py:   super().greet()
来源：http://lew.chenlongwang.top

PHP:  parent::greet();
来源：http://zqz.jlsjyb.cn


<!-- 参考信息 -->