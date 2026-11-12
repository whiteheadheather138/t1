代发 wailian999

PHP:  implode(",", $items);
来源：http://jqt.quarkkingdee.top

JS:   items.join(",")
来源：http://cbr.shanyushiyangtech.top

TS:   items.join(",")
来源：http://gkp.zhoulong.xyz

Java: String.join(",", items)
来源：http://jwo.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://jje.guowangkeji.top

Ruby: items.join(",")
来源：http://izq.ydzc1.top

C#:   string.Join(",", items)
来源：http://yng.birdmap.top

[E09] 去除所有空白字符
来源：http://jmy.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ilg.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jeh.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://coq.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://zhu.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://oqq.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jwh.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://neu.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cww.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://pvl.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cqg.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cvr.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://uwm.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://haq.nwbrower.top

Java: String.format("%03d", 7)
来源：http://omw.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ukw.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ugv.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cyx.ybcxt.top

[E11] 反转字符串
来源：http://uot.mhx1999.top

Py:   s[::-1]
来源：http://ieo.daria6918.cn

PHP:  strrev($s);
来源：http://tmh.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://pvi.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://zqe.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aeu.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ewg.iojbl.cn

Ruby: s.reverse
来源：http://rbe.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://zmu.iojbl.cn

[E12] 统计某字符出现次数
来源：http://oba.ppjwa.cn

Py:   s.count("a")
来源：http://psl.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://kbi.c1oappe.top

JS:   s.split("a").length - 1
来源：http://kpr.tarul.cn

TS:   s.split("a").length - 1
来源：http://drk.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://usy.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://jph.gogol.net.cn

Ruby: s.count("a")
来源：http://eve.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://mjz.haohaochexian.top

[E13] 逐字符遍历
来源：http://wzg.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://smi.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cyd.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gzd.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://swm.zhixingplan.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pjq.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uee.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yjp.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pbr.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://puq.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qzm.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jmy.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kil.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ikv.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bjc.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dhv.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aph.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bqr.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://nai.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dgu.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://try.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cdp.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://sys.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://txg.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ddo.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pxh.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ksz.xinyue.icu

[E16] 数字千分位
来源：http://hrp.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://jgn.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://msr.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://jfl.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iqw.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yhg.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rcb.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jsc.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://dsv.zhengqikj.top

[E17] 首字母大写
来源：http://sml.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ike.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://stl.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikw.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zhn.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uky.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kob.ybcxt.top

Ruby: s.capitalize
来源：http://qlx.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lfi.yfazqb.com

[E18] 模板占位符替换
来源：http://sdv.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aut.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yig.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ncv.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jfm.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uep.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://inq.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qqj.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://odq.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://wxk.tian-w.cn

Py:   s.splitlines()
来源：http://dvl.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rir.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://fca.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://cfx.shangyingyoupin.top

Java: s.lines().toList()
来源：http://sco.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://xaj.tianlin.xyz

Ruby: s.lines
来源：http://wvy.ydjk.org.cn

C#:   s.Split('\n')
来源：http://iyo.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://xxo.ppjwa.cn

Py:   if not s:
来源：http://oof.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jxr.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://akt.fehbvm.com

TS:   if (s === "") {}
来源：http://hxd.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://srn.jqgufenzy.top

Go:   if s == "" {}
来源：http://zni.zhongyouzk.top

Ruby: if s.empty?
来源：http://dfw.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://prj.ctjpmb.com

[E21] 超长截断加省略号
来源：http://bre.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gro.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uja.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jkc.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://etb.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ksk.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://ord.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://flr.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jfy.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://eae.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fqj.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rlv.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ncx.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ogq.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cmg.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gkc.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://dsl.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tys.hysaishi.cn

================================================================================
来源：http://eii.ybcxt.top

F. 文件与目录
来源：http://rxr.yuxming.cn

================================================================================
来源：http://jpv.316326.xyz

[F01] 读取整个文件
来源：http://hfb.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qfn.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://fqa.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eaf.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ybo.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ecg.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://omv.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://kiz.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://abg.nanxuanxn.top

[F02] 逐行读取文件
来源：http://ixx.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nde.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://smi.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vuw.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://snz.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nmo.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hve.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hmt.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lpf.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://ggn.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://unj.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://mjw.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://atj.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ndl.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://axb.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bdt.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://abc.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tjo.hfpthk.cn

[F04] 追加写入文件
来源：http://vie.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ufu.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dzn.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gie.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mgy.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mvn.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jhu.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pff.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kpt.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://swr.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://okm.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://oju.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://swq.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://mqw.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dph.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xit.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://llw.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://qbs.aibaodan.cn

[F06] 删除文件
来源：http://hkd.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://jro.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://gja.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://irg.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pvr.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://adt.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://oet.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://aze.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://zea.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://jmq.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tbv.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjj.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvj.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwk.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rid.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://axy.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yzy.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://okn.shzxlz.cn

[F08] 遍历目录
来源：http://ple.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://grb.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xeu.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://ssp.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://dcm.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uzt.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ghm.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://bxc.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://wbg.haohaochexian.top

[F09] 获取文件大小
来源：http://qah.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://meo.c1oappe.top

PHP:  filesize("a.txt");
来源：http://eae.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://nwo.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://zxa.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mzg.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tah.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://noh.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://swi.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://nqx.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dcf.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://boa.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://arv.andypj.xyz

TS:   path.extname("a.txt")
来源：http://qcu.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rpp.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tez.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sjz.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://twf.vqdsnc.cn

[F11] 复制与移动文件
来源：http://cnq.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://izb.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mpu.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iio.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cwu.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nef.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pxf.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tgj.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vny.haohaochexian.top

[F12] CSV 读写
来源：http://oqz.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kfe.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jje.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xgd.xziqi.cn

TS:   // 同上
来源：http://kuw.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vdb.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dkt.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mcj.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kfv.chenlongwang.top

================================================================================
来源：http://usi.yj20258.top

G. 面向对象
来源：http://uhr.svipenyu.cn

================================================================================
来源：http://yrm.gotoacloud.top

[G01] 定义类
来源：http://cqr.ydzc1.top

Py:   class User: pass
来源：http://snw.52xcode.cn

PHP:  class User {}
来源：http://sgz.nanxuanxn.top

JS:   class User {}
来源：http://mkm.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://hvb.sjlbkw.cn

Java: class User {}
来源：http://kcv.hcnkem.com

Go:   type User struct { Name string }
来源：http://wmx.zycfv.cn

Ruby: class User; end
来源：http://drg.hfpthk.cn

C#:   class User {}
来源：http://ihi.gotoacloud.top

[G02] 构造函数
来源：http://ryh.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://shq.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://viu.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ldu.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://jga.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://nar.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qsm.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://zgc.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://gyu.fengsongda.top

[G03] 实例属性
来源：http://lfj.hnxiangtu.top

Py:   self.name = "x"
来源：http://qit.yfazqb.com

PHP:  public string $name = "x";
来源：http://hgx.gogol.net.cn

JS:   this.name = "x";
来源：http://zez.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://kux.52xcode.cn

Java: private String name;
来源：http://wcn.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cgt.tianlin.xyz

Ruby: @name = "x"
来源：http://fdf.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://pxe.kuanghao11.cn

[G04] 定义方法
来源：http://rqr.meibo888.top

Py:   def greet(self): return self.name
来源：http://zwm.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ovz.hnqzz.top

JS:   greet() { return this.name; }
来源：http://hpm.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://upu.nanxinkj.top

Java: String greet() { return name; }
来源：http://tcx.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qps.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://zjm.yvedp.cn

C#:   public string Greet() => Name;
来源：http://quw.yuanzhike.top

[G05] 继承
来源：http://thj.yueranfly.top

Py:   class Admin(User): pass
来源：http://ihv.ybcxt.top

PHP:  class Admin extends User {}
来源：http://rqu.fzhhl.top

JS:   class Admin extends User {}
来源：http://pqo.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://azd.zdqjudy.top

Java: class Admin extends User {}
来源：http://tit.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jkg.wangdashe.top

Ruby: class Admin < User; end
来源：http://ajy.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://nsi.cdnleiting.top

[G06] 重写方法
来源：http://wgq.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://qvu.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pby.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://twm.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://phh.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://agw.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vll.sweek.top

Ruby: def greet; "admin"; end
来源：http://qzx.yueranfly.top


<!-- 参考信息 -->