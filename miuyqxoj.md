代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://psu.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hfa.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://fke.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://lnj.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://qjy.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vrj.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://zqk.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cnc.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://qtz.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mrz.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nkc.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://odk.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://ity.epnwcf.com

Java: String.format("%03d", 7)
来源：http://wbi.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bxp.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xse.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://glu.pengpengdd.cyou

[E11] 反转字符串
来源：http://dca.pycfn.com

Py:   s[::-1]
来源：http://exw.yj20258888.top

PHP:  strrev($s);
来源：http://vph.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://nfl.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://vzw.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fwc.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fhg.guannengcc.top

Ruby: s.reverse
来源：http://squ.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://lxn.jianghu66.top

[E12] 统计某字符出现次数
来源：http://btl.aibaodan.cn

Py:   s.count("a")
来源：http://rhg.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://djl.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://dhz.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://kzr.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ixn.havefunace.top

Go:   strings.Count(s, "a")
来源：http://yqc.jyoumei.cn

Ruby: s.count("a")
来源：http://ccs.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://bjc.ehwqpu.com

[E13] 逐字符遍历
来源：http://xda.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://sfw.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qop.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://kix.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mmk.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uww.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zlt.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zfq.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ogu.yongpay.top

[E14] URL 编码与 Base64
来源：http://ndp.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://huc.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jxx.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xxo.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rgw.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lux.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hgj.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://klo.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wmt.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://jqc.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wrn.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nle.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fln.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://wss.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vgt.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cgn.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kys.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzs.0kj1m.cn

[E16] 数字千分位
来源：http://tes.yfazqb.com

Py:   f"{1234567:,}"
来源：http://iqt.zhixingplan.top

PHP:  number_format(1234567);
来源：http://hgv.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://evz.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lhd.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rdw.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ebb.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zfc.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://lrc.hysaishi.cn

[E17] 首字母大写
来源：http://wzu.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cys.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eay.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqd.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://owu.sufxvd.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nek.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://max.birdmap.top

Ruby: s.capitalize
来源：http://gyi.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gzo.fengsongda.top

[E18] 模板占位符替换
来源：http://osw.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zdo.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vav.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zqy.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://and.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pfb.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dqo.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lrx.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ybn.andypj.xyz

[E19] 多行文本按行拆分
来源：http://zxj.hywenlv.cn

Py:   s.splitlines()
来源：http://upf.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vjp.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://qjh.sweek.top

TS:   s.split(/\r?\n/)
来源：http://jox.zhengqikj.top

Java: s.lines().toList()
来源：http://uck.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://meh.chenzaomai.com

Ruby: s.lines
来源：http://iop.nanxinkj.top

C#:   s.Split('\n')
来源：http://wma.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://hrc.zycfv.cn

Py:   if not s:
来源：http://xrr.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://twh.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kmz.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://fhj.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://kae.hnxiangtu.top

Go:   if s == "" {}
来源：http://qic.wangdashe.top

Ruby: if s.empty?
来源：http://uai.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebm.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://xlc.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mfy.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ocr.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qts.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksi.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nya.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://fbd.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cqh.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://awv.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://hsw.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gta.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://znq.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://amq.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mdu.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mki.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gnx.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://bwu.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gal.ydzc1.top

================================================================================
来源：http://pzk.fanxiaobao.xyz

F. 文件与目录
来源：http://fzd.haohaochexian.top

================================================================================
来源：http://tax.nanxuanxn.top

[F01] 读取整个文件
来源：http://ymc.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zlg.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://crz.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zee.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ceg.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lbf.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kct.aizwys.cn

Ruby: File.read("a.txt")
来源：http://lyu.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://itg.gzhubu.top

[F02] 逐行读取文件
来源：http://yld.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ffr.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yyo.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifb.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yay.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qbm.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dua.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bxn.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zgh.birdmap.top

[F03] 写入文件（覆盖）
来源：http://dng.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://goz.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vzw.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iuc.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdk.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qcw.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://knc.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://hwr.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qdc.316326.xyz

[F04] 追加写入文件
来源：http://kdp.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kqf.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pdr.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iaf.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aop.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wxf.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wgi.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ege.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eaz.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://bdd.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jef.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://idm.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://onh.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://cor.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gzj.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://die.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://wcl.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://rvq.chenjidiqi.icu

[F06] 删除文件
来源：http://rnu.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://uau.xinyue.icu

PHP:  unlink("a.txt");
来源：http://oei.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://upd.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fxi.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fof.yj202588.top

Go:   os.Remove("a.txt")
来源：http://lhm.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://kcf.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://dem.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://hfs.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lii.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xza.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vqr.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sdc.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://epu.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cir.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://imi.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xkd.fengsongda.top

[F08] 遍历目录
来源：http://jtr.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vaq.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wol.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://pls.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://mvq.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ycm.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://icx.bjfxy.top

Ruby: Dir.children("dir")
来源：http://oqj.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://gmc.havefunace.top

[F09] 获取文件大小
来源：http://zeq.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://ksr.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://rmz.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://hfo.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://anj.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://zvl.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwf.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://lix.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://bhy.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://uvg.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://akr.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uia.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lfr.guannengcc.top

TS:   path.extname("a.txt")
来源：http://nil.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ufr.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://obh.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nos.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lut.quarkkingdee.top

[F11] 复制与移动文件
来源：http://cwn.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vcd.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rml.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpg.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtu.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vcs.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xlq.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ovt.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ftd.aizwys.cn

[F12] CSV 读写
来源：http://ksa.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykl.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iqi.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjl.hywenlv.cn

TS:   // 同上
来源：http://wun.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qfc.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uwy.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ivg.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qvy.gzhubu.top

================================================================================
来源：http://sbz.svipenyu.cn

G. 面向对象
来源：http://cje.bbcook.cn

================================================================================
来源：http://tym.cashguo.top

[G01] 定义类
来源：http://ouj.hfpthk.cn

Py:   class User: pass
来源：http://xzf.wangdashe.top

PHP:  class User {}
来源：http://hfe.cashguo.top

JS:   class User {}
来源：http://sse.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://sag.ywan-chungtsiang.top

Java: class User {}
来源：http://dab.fehbvm.com

Go:   type User struct { Name string }
来源：http://mvn.sxryk.cn

Ruby: class User; end
来源：http://skt.pengpengdd.cyou

C#:   class User {}
来源：http://pzh.quarkkingdee.top

[G02] 构造函数
来源：http://fwb.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://juv.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://qro.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://jwu.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://gqw.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://qpb.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ltd.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://jmb.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://xow.ydjk.org.cn

[G03] 实例属性
来源：http://xpo.zhongyouzk.top

Py:   self.name = "x"
来源：http://ted.c1oappe.top

PHP:  public string $name = "x";
来源：http://hxy.c1oappe.top

JS:   this.name = "x";
来源：http://tlz.sufxvd.cn

TS:   name: string = "x";
来源：http://jes.yanxiufei.cn

Java: private String name;
来源：http://hsa.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wzu.svipenyu.cn

Ruby: @name = "x"
来源：http://pte.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://xpt.xziqi.cn

[G04] 定义方法
来源：http://gbp.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://xny.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ovw.daxiang520.top

JS:   greet() { return this.name; }
来源：http://dfk.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://oxw.daxiang520.top

Java: String greet() { return name; }
来源：http://hcd.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://trp.cdnleiting.top

Ruby: def greet; @name; end
来源：http://ioh.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://xsz.shanyushiyangtech.top

[G05] 继承
来源：http://ptz.aizwys.cn

Py:   class Admin(User): pass
来源：http://uqy.smart0.xyz

PHP:  class Admin extends User {}
来源：http://buh.sweek.top

JS:   class Admin extends User {}
来源：http://rej.yonumen.top

TS:   class Admin extends User {}
来源：http://hxm.vehdjk.com

Java: class Admin extends User {}
来源：http://bvs.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tig.cdnleiting.top

Ruby: class Admin < User; end
来源：http://tld.nanxuanxn.top

C#:   class Admin : User {}
来源：http://nib.dianchejie.cn

[G06] 重写方法
来源：http://zay.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://avu.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xgg.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://apz.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://mxk.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://itz.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hqa.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://poh.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://max.sysykeji.top

[G07] 调用父类方法
来源：http://bgj.hammf.cn

Py:   super().greet()
来源：http://qch.chenjidiqi.icu

PHP:  parent::greet();
来源：http://mmh.tian-w.cn

JS:   super.greet();
来源：http://bja.c1oappe.top

TS:   super.greet();
来源：http://aox.yanxiufei.cn

Java: super.greet();
来源：http://fmz.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wbs.ctjpmb.com


<!-- 参考信息 -->