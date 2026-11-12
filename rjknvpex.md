代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kko.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://czk.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://lij.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://bvz.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://vla.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fqa.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xia.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ojr.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://jdh.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vod.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://buq.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://kfi.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://bfo.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://nos.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://fsr.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://abx.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ofq.52xcode.cn

[E11] 反转字符串
来源：http://jgq.hysaishi.cn

Py:   s[::-1]
来源：http://jdt.iojbl.cn

PHP:  strrev($s);
来源：http://ekw.birdmap.top

JS:   [...s].reverse().join("")
来源：http://pcx.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://cnt.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rwx.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://osz.zdbjq.cn

Ruby: s.reverse
来源：http://wdu.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://dty.cashguo.top

[E12] 统计某字符出现次数
来源：http://aoa.yvedp.cn

Py:   s.count("a")
来源：http://dff.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://prh.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://uma.uphjek.com

TS:   s.split("a").length - 1
来源：http://odh.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iyh.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://pyr.cheryme.top

Ruby: s.count("a")
来源：http://ttx.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://waq.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://soq.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://fcc.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://azx.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://equ.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mtw.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qhx.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xme.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fbt.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ugj.tarul.cn

[E14] URL 编码与 Base64
来源：http://csf.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zak.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sas.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fuu.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vvg.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://coc.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pju.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://onv.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dds.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://rpo.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://okq.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vec.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fac.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yhd.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uga.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mqd.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gzd.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dxn.zdbjq.cn

[E16] 数字千分位
来源：http://alx.yvedp.cn

Py:   f"{1234567:,}"
来源：http://gmp.hywenlv.cn

PHP:  number_format(1234567);
来源：http://nsc.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jgg.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bvt.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xee.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mqj.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://das.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://zum.jyoumei.cn

[E17] 首字母大写
来源：http://ctw.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ccd.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qzh.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://slk.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ehv.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://daz.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wdw.sufxvd.cn

Ruby: s.capitalize
来源：http://spn.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://spd.jinqigfzy.top

[E18] 模板占位符替换
来源：http://ucc.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gjn.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://alk.dianchejie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://apa.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://dqf.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qdo.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iur.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mad.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pwy.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://zqq.yj20258888.top

Py:   s.splitlines()
来源：http://mgo.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vki.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://yyx.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://poc.yongpay.top

Java: s.lines().toList()
来源：http://szw.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://otp.sjlbkw.cn

Ruby: s.lines
来源：http://yvm.52xcode.cn

C#:   s.Split('\n')
来源：http://rjp.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://ckg.tian-w.cn

Py:   if not s:
来源：http://srx.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cco.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kpz.chenlongwang.top

TS:   if (s === "") {}
来源：http://xuq.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://jvl.fktsv.cn

Go:   if s == "" {}
来源：http://hhc.zhixingplan.top

Ruby: if s.empty?
来源：http://gts.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mxn.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://hte.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xlu.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lcb.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fam.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yfn.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vkz.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://gys.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mms.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wgv.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://tna.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://thh.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yrq.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://swa.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtz.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oxz.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vrt.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://tcz.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zqv.shanyushiyangkeji.top

================================================================================
来源：http://gmi.9152youxi.cn

F. 文件与目录
来源：http://dgi.zhiwuduotai.top

================================================================================
来源：http://haj.yonumen.top

[F01] 读取整个文件
来源：http://dmv.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kpx.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://axl.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hil.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://avx.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ekz.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cgu.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://shm.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://eib.sweek.top

[F02] 逐行读取文件
来源：http://fwo.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oyt.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qdc.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qgv.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pcr.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wub.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rbw.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dwg.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vln.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://cls.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oqd.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ymw.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbz.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lio.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cnj.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://erm.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://hwc.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ivf.ybcxt.top

[F04] 追加写入文件
来源：http://wjw.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yrh.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fqt.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfd.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tmf.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tfg.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aqa.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lal.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://otc.sweek.top

[F05] 判断文件或目录是否存在
来源：http://ocz.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://evk.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://mio.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://hgf.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://svi.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gmw.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwj.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://xmb.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://xjl.chenlongwang.top

[F06] 删除文件
来源：http://scg.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://dkj.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://gzj.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wei.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uoc.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ikl.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://anm.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://vsl.tanke756.top

C#:   File.Delete("a.txt");
来源：http://iof.hammf.cn

[F07] 创建目录（含多级）
来源：http://unb.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ygs.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ssl.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zsd.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://seu.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cvy.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cqo.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lfc.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://usp.guannengcc.top

[F08] 遍历目录
来源：http://yxs.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vfr.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://naz.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://uhx.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://eel.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fsz.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://olb.pycfn.com

Ruby: Dir.children("dir")
来源：http://nbh.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://ind.shangyingyoupin.top

[F09] 获取文件大小
来源：http://uxx.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://jnl.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://dgn.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://nlh.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://xpj.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://uaa.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://edx.aizwys.cn

Ruby: File.size("a.txt")
来源：http://lwo.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://flf.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://mvd.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mzy.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://toe.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ujq.xinyue.icu

TS:   path.extname("a.txt")
来源：http://jdz.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://syq.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xsk.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mre.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ikh.chenzaomai.com

[F11] 复制与移动文件
来源：http://qro.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zna.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sip.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://snr.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jxk.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jmr.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dqd.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gku.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hwh.yangfankeji.com

[F12] CSV 读写
来源：http://lir.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tfs.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gsb.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qzs.sjlbkw.cn

TS:   // 同上
来源：http://dtk.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zcf.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ctl.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tws.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ifw.yongpay.top

================================================================================
来源：http://olv.shangyingyoupin.top

G. 面向对象
来源：http://giy.shanyushiyangtech.top

================================================================================
来源：http://xnf.yuanzhike.top

[G01] 定义类
来源：http://tvs.ppjwa.cn

Py:   class User: pass
来源：http://xat.aizwys.cn

PHP:  class User {}
来源：http://scv.fehbvm.com

JS:   class User {}
来源：http://knc.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://thu.hammf.cn

Java: class User {}
来源：http://gmq.chenlongwang.top

Go:   type User struct { Name string }
来源：http://ier.hongshengwenyu.top

Ruby: class User; end
来源：http://qiq.hnqzz.top

C#:   class User {}
来源：http://igc.sysykeji.top

[G02] 构造函数
来源：http://vec.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://sog.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://asv.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://bqg.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://yxh.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://dzo.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://trq.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://sna.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://hcl.hcnkem.com

[G03] 实例属性
来源：http://vaj.yvedp.cn

Py:   self.name = "x"
来源：http://vjd.ydzc1.top

PHP:  public string $name = "x";
来源：http://qxd.cdnleiting.top

JS:   this.name = "x";
来源：http://gsi.hywenlv.cn

TS:   name: string = "x";
来源：http://vzm.ppjwa.cn

Java: private String name;
来源：http://hvn.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rvw.sxryk.cn

Ruby: @name = "x"
来源：http://zuy.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://rsa.hysaishi.cn

[G04] 定义方法
来源：http://obp.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://xuj.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://glw.xuanzx.com

JS:   greet() { return this.name; }
来源：http://blt.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://jid.yangfankeji.com

Java: String greet() { return name; }
来源：http://dcg.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ntc.tian-w.cn

Ruby: def greet; @name; end
来源：http://iyk.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://wab.fanxiaobao.xyz

[G05] 继承
来源：http://zri.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://xen.c1oappe.top

PHP:  class Admin extends User {}
来源：http://cwu.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://qyl.zdbjq.cn

TS:   class Admin extends User {}
来源：http://huf.fehbvm.com

Java: class Admin extends User {}
来源：http://diu.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mcg.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://bsv.zhoulong.xyz

C#:   class Admin : User {}
来源：http://ttf.hesvh.cn

[G06] 重写方法
来源：http://ddi.pycfn.com

Py:   def greet(self): return "admin"
来源：http://gjc.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gxe.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://smc.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://pdt.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://tjt.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jnx.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://tre.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://lir.52xcode.cn

[G07] 调用父类方法
来源：http://ioi.yfazqb.com

Py:   super().greet()
来源：http://ygz.zhijiandao.cn

PHP:  parent::greet();
来源：http://lne.zhixingplan.top

JS:   super.greet();
来源：http://ypm.chenzaomai.com

TS:   super.greet();
来源：http://rrn.jinghuilouyu.cn

Java: super.greet();
来源：http://mtq.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zxi.tarul.cn


<!-- 参考信息 -->