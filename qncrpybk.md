代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hry.hfpthk.cn

Ruby: items.join(",")
来源：http://dif.uphjek.com

C#:   string.Join(",", items)
来源：http://gqi.hysaishi.cn

[E09] 去除所有空白字符
来源：http://aek.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aqr.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rws.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://mik.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://jsv.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://kmj.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vud.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://nxj.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tis.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://rae.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lly.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://waa.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://kfg.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://zme.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://wbl.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pgo.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sor.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wps.birdmap.top

[E11] 反转字符串
来源：http://zag.jianghu66.top

Py:   s[::-1]
来源：http://zmj.snrcjt.cn

PHP:  strrev($s);
来源：http://grz.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://rbb.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://cdv.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hqh.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pof.cucudq.cn

Ruby: s.reverse
来源：http://lzi.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://ntr.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://foh.fengsongda.top

Py:   s.count("a")
来源：http://jri.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://tcu.fehbvm.com

JS:   s.split("a").length - 1
来源：http://suo.gzhubu.top

TS:   s.split("a").length - 1
来源：http://jtd.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://khe.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://jlq.aibaodan.cn

Ruby: s.count("a")
来源：http://lbj.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://ebp.hywenlv.cn

[E13] 逐字符遍历
来源：http://vgn.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://gwx.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yei.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lzy.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://snf.jqgfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hwp.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ykm.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://thx.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mra.wangdashe.top

[E14] URL 编码与 Base64
来源：http://oia.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://idt.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ooy.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eeq.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qlw.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sof.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vni.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ioh.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fax.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://rjg.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uee.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ebf.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://krq.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jum.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://drq.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hem.zycfv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xiu.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hfp.wangshuangyany.cn

[E16] 数字千分位
来源：http://yhi.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://qwl.chenlongwang.top

PHP:  number_format(1234567);
来源：http://eee.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cvf.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uxg.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aio.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tfi.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pap.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://hvk.vehdjk.com

[E17] 首字母大写
来源：http://umw.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pcz.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fak.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnq.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gdz.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nqy.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://csx.sjlbkw.cn

Ruby: s.capitalize
来源：http://fyo.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kku.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://scn.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vou.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rhk.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://twz.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vbc.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iql.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pla.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ffa.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eij.zycfv.cn

[E19] 多行文本按行拆分
来源：http://nsm.dianchejie.cn

Py:   s.splitlines()
来源：http://cuh.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lux.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://wfa.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://zso.dashuyun.cn

Java: s.lines().toList()
来源：http://lnj.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://kmd.chenjidiqi.icu

Ruby: s.lines
来源：http://mid.yj202588.top

C#:   s.Split('\n')
来源：http://sxg.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://xjv.hnxiangtu.top

Py:   if not s:
来源：http://nsq.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esn.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jpw.tianlin.xyz

TS:   if (s === "") {}
来源：http://ouh.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://oxa.zycfv.cn

Go:   if s == "" {}
来源：http://pwu.hnxiangtu.top

Ruby: if s.empty?
来源：http://qce.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dna.daria6918.cn

[E21] 超长截断加省略号
来源：http://qkk.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ofv.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ico.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jwd.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bxf.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pww.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://lbd.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vvs.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zon.daria6918.cn

[E22] 字节长度与字符长度
来源：http://uep.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dnc.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqt.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xqz.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uji.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zhw.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sjc.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://wlk.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vfg.guowangkeji.top

================================================================================
来源：http://qua.dashuyun.cn

F. 文件与目录
来源：http://wbc.dianchejie.cn

================================================================================
来源：http://gty.dianchejie.cn

[F01] 读取整个文件
来源：http://lvy.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://njq.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://vwr.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ytr.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fgw.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oxq.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qbo.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://elg.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://cox.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://kju.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pgo.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rdo.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ank.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pvj.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ard.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ccm.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qzd.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ktb.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://iiy.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yya.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rey.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wio.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pkg.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vtl.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vci.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://ueu.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://urb.0kj1m.cn

[F04] 追加写入文件
来源：http://hnq.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uzh.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ksc.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jss.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vbe.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wtt.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://doj.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gye.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hze.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://qve.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fvl.cashguo.top

PHP:  file_exists("a.txt");
来源：http://kst.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://prc.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://akp.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tka.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrz.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://ywy.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://iri.ydzc1.top

[F06] 删除文件
来源：http://ock.guannengcc.top

Py:   os.remove("a.txt")
来源：http://fne.ybcxt.top

PHP:  unlink("a.txt");
来源：http://hqv.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kww.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://tyx.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bsa.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://yju.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://stv.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://jsx.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://nxt.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iba.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cqu.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qbo.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nvg.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sjs.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ynb.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yha.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tgi.cheryme.top

[F08] 遍历目录
来源：http://mtw.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jdt.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mws.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://hxe.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://mvb.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kjd.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bqb.yonumen.top

Ruby: Dir.children("dir")
来源：http://orj.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://cki.ydjk.org.cn

[F09] 获取文件大小
来源：http://ucp.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://son.daria6918.cn

PHP:  filesize("a.txt");
来源：http://hvp.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://rub.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://xlp.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://nsr.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bvt.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://xag.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://gch.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://jpa.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ove.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zxx.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vul.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://ota.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qrv.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ukt.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjg.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rre.yj20258.top

[F11] 复制与移动文件
来源：http://bbl.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ags.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jmj.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vct.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahy.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vni.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xuy.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vqn.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zdj.0kj1m.cn

[F12] CSV 读写
来源：http://ixb.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nap.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rch.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lyc.yvedp.cn

TS:   // 同上
来源：http://vke.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bib.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wht.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://npg.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zlu.zhijiandao.cn

================================================================================
来源：http://gjv.ctjpmb.com

G. 面向对象
来源：http://rxi.andypj.xyz

================================================================================
来源：http://yhq.fktsv.cn

[G01] 定义类
来源：http://yrz.fanxiaobao.xyz

Py:   class User: pass
来源：http://gjs.fanxiaobao.xyz

PHP:  class User {}
来源：http://zgs.feifeiyinyue.top

JS:   class User {}
来源：http://xjk.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://wxd.9152youxi.cn

Java: class User {}
来源：http://vks.fehbvm.com

Go:   type User struct { Name string }
来源：http://eqb.fehbvm.com

Ruby: class User; end
来源：http://ege.cdnleiting.top

C#:   class User {}
来源：http://sxq.hfpthk.cn

[G02] 构造函数
来源：http://gaj.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://pwi.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://jtp.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://skx.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://ozy.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://txs.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aca.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://wmd.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://hje.chenzaomai.com

[G03] 实例属性
来源：http://buu.nanxinkj.top

Py:   self.name = "x"
来源：http://eid.nanxinkj.top

PHP:  public string $name = "x";
来源：http://hke.ydzc1.top

JS:   this.name = "x";
来源：http://wwk.xziqi.cn

TS:   name: string = "x";
来源：http://nqx.zhengqikj.top

Java: private String name;
来源：http://enq.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sgy.cashguo.top

Ruby: @name = "x"
来源：http://rsn.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://htp.zycfv.cn

[G04] 定义方法
来源：http://xci.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://dwc.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gzl.zycfv.cn

JS:   greet() { return this.name; }
来源：http://zws.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://ltt.xziqi.cn

Java: String greet() { return name; }
来源：http://dln.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gor.hesvh.cn

Ruby: def greet; @name; end
来源：http://xbl.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://kqi.shanyushiyangtech.top

[G05] 继承
来源：http://ahe.gotoacloud.top

Py:   class Admin(User): pass
来源：http://jdr.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://tyw.zdbjq.cn

JS:   class Admin extends User {}
来源：http://ecx.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://crd.svipenyu.cn

Java: class Admin extends User {}
来源：http://vzr.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hpk.sweek.top

Ruby: class Admin < User; end
来源：http://rcd.hnxiangtu.top

C#:   class Admin : User {}
来源：http://qxc.ywan-chungtsiang.top

[G06] 重写方法
来源：http://jcl.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://svy.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://jln.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://fmv.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://mjg.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://qry.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qir.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://qle.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://gai.tianlin.xyz

[G07] 调用父类方法
来源：http://ghk.hnxiangtu.top

Py:   super().greet()
来源：http://fdz.ybcxt.top

PHP:  parent::greet();
来源：http://gvz.daxiang520.top


<!-- 参考信息 -->