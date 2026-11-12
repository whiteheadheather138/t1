代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://tpf.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jcp.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mrc.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://whz.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://cvd.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://cdc.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://hox.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gaq.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kwl.hongshengwenyu.top

[E11] 反转字符串
来源：http://ufo.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://qyh.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://fxm.uphjek.com

JS:   [...s].reverse().join("")
来源：http://tji.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://lvu.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sxp.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fkk.shangyingyoupin.top

Ruby: s.reverse
来源：http://zbw.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://oee.xinyue.icu

[E12] 统计某字符出现次数
来源：http://ylw.nanxuanxn.top

Py:   s.count("a")
来源：http://inl.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://tig.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://mdt.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://awn.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vrd.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://etz.ydzc1.top

Ruby: s.count("a")
来源：http://wcb.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://irh.chenzaomai.com

[E13] 逐字符遍历
来源：http://mbc.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://vfi.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xvz.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ljf.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xxs.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://esd.chenzaomai.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sms.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pax.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fin.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://hdm.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://svw.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://job.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ucr.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mco.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vce.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cxe.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://csq.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cye.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://jhh.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xka.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hot.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cbp.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rgg.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xlr.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vdg.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gvt.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hmg.dashuyun.cn

[E16] 数字千分位
来源：http://pqj.uphjek.com

Py:   f"{1234567:,}"
来源：http://ngc.sufxvd.cn

PHP:  number_format(1234567);
来源：http://ydm.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wsk.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bte.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aoh.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vdn.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vkv.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://cng.jqgfzy.top

[E17] 首字母大写
来源：http://nli.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zey.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wtw.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vyi.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zko.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jtd.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kay.mhx1999.top

Ruby: s.capitalize
来源：http://rtd.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uyq.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://yml.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mhd.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gty.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eiq.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qms.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fuh.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qin.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fpa.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kip.sysykeji.top

[E19] 多行文本按行拆分
来源：http://dxc.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://lzr.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hno.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://svp.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://biw.smart0.xyz

Java: s.lines().toList()
来源：http://rsz.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://zbo.jqgfzy.top

Ruby: s.lines
来源：http://wut.cheryme.top

C#:   s.Split('\n')
来源：http://vyx.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://wuo.zhijiandao.cn

Py:   if not s:
来源：http://piz.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://frx.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://snx.xinyue.icu

TS:   if (s === "") {}
来源：http://zog.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://rbf.aibaodan.cn

Go:   if s == "" {}
来源：http://iuq.cqqwz.cn

Ruby: if s.empty?
来源：http://bki.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qqf.tianlin.xyz

[E21] 超长截断加省略号
来源：http://gza.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://prn.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vtt.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqy.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afv.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mfu.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://gqc.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wpl.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mon.yueranfly.top

[E22] 字节长度与字符长度
来源：http://fos.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txa.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://puh.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qro.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://efu.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xyv.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xzr.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://zdw.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ncy.yvedp.cn

================================================================================
来源：http://cub.cdnleiting.top

F. 文件与目录
来源：http://xqn.nwbrower.top

================================================================================
来源：http://mpl.epnwcf.com

[F01] 读取整个文件
来源：http://wgn.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mpn.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://jkg.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ngi.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eyf.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://qla.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bhi.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://wbl.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://wpm.chenlongwang.top

[F02] 逐行读取文件
来源：http://jzs.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pug.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lmn.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uwb.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://msb.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xtp.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sop.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jhd.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pki.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://nzn.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vey.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ciz.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://spd.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ird.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://czq.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lfp.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://htv.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wbp.guannengcc.top

[F04] 追加写入文件
来源：http://dss.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kkl.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cjl.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmb.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfh.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vet.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ctf.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oox.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lhh.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://lav.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lgh.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://lbb.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://ezr.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://qxr.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://qyd.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://set.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://acz.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://dpa.fanxiaobao.xyz

[F06] 删除文件
来源：http://pdu.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://izh.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://ned.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://awt.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://rvv.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zpl.ivvv.top

Go:   os.Remove("a.txt")
来源：http://pto.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://xea.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://dsh.gzhubu.top

[F07] 创建目录（含多级）
来源：http://qvx.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ezs.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mgv.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://thw.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qsy.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rwd.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wys.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://agj.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rnn.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://jsh.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vjf.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mja.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://zlr.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://kue.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kja.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://hvp.sxryk.cn

Ruby: Dir.children("dir")
来源：http://qts.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://qwa.ctjpmb.com

[F09] 获取文件大小
来源：http://pkm.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://myu.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://mtk.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://atn.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://pjk.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://rpz.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rji.tian-w.cn

Ruby: File.size("a.txt")
来源：http://sfv.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ttw.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://zav.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://frj.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dgq.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hek.yj202588.top

TS:   path.extname("a.txt")
来源：http://jyz.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ggc.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://crz.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dkg.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://orb.epnwcf.com

[F11] 复制与移动文件
来源：http://nxd.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iki.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xlr.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hiy.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://evh.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fhy.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jef.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jym.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://itv.c1oappe.top

[F12] CSV 读写
来源：http://eka.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vzq.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mej.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://unp.sysykeji.top

TS:   // 同上
来源：http://gxl.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://whz.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mks.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://svc.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iiy.jqgufenzy.top

================================================================================
来源：http://pic.tanke756.top

G. 面向对象
来源：http://qsi.fanxiaobao.xyz

================================================================================
来源：http://zmg.aibaodan.cn

[G01] 定义类
来源：http://kfk.birdmap.top

Py:   class User: pass
来源：http://hws.jqgfzy.top

PHP:  class User {}
来源：http://bxt.vehdjk.com

JS:   class User {}
来源：http://qee.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://squ.sxryk.cn

Java: class User {}
来源：http://adi.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://mmb.sufxvd.cn

Ruby: class User; end
来源：http://yzi.ywan-chungtsiang.top

C#:   class User {}
来源：http://yma.xylfe.cn

[G02] 构造函数
来源：http://zhe.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://ifo.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://eor.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://uhg.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://wja.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://kiz.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dlk.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://xvf.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://idn.9152youxi.cn

[G03] 实例属性
来源：http://rdu.cheryme.top

Py:   self.name = "x"
来源：http://tlz.zycfv.cn

PHP:  public string $name = "x";
来源：http://vzt.yuanzhike.top

JS:   this.name = "x";
来源：http://dzi.zdqjudy.top

TS:   name: string = "x";
来源：http://oiu.kuanghao11.cn

Java: private String name;
来源：http://tgj.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://off.yuxming.cn

Ruby: @name = "x"
来源：http://gvu.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://xqq.uphjek.com

[G04] 定义方法
来源：http://xrj.uphjek.com

Py:   def greet(self): return self.name
来源：http://uqq.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://czs.yj20258888.top

JS:   greet() { return this.name; }
来源：http://mbp.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://nas.tanke756.top

Java: String greet() { return name; }
来源：http://gbz.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ajl.iojbl.cn

Ruby: def greet; @name; end
来源：http://rvn.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://gyg.jqgufenzy.top

[G05] 继承
来源：http://epb.316326.xyz

Py:   class Admin(User): pass
来源：http://oqb.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://mkx.zdqjudy.top

JS:   class Admin extends User {}
来源：http://axx.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://smo.redwolf501.top

Java: class Admin extends User {}
来源：http://vev.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uaj.yangfankeji.com

Ruby: class Admin < User; end
来源：http://gje.dashuyun.cn

C#:   class Admin : User {}
来源：http://ijo.jiagoushi.top

[G06] 重写方法
来源：http://pdc.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://pgc.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wei.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://dnc.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://qlz.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://skx.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vcl.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://fqt.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://esj.sjlbkw.cn

[G07] 调用父类方法
来源：http://exk.gogol.net.cn

Py:   super().greet()
来源：http://klx.c1oappe.top

PHP:  parent::greet();
来源：http://sig.yj20258888.top

JS:   super.greet();
来源：http://slo.tarul.cn

TS:   super.greet();
来源：http://lcb.cdnleiting.top

Java: super.greet();
来源：http://kto.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://snr.redwolf501.top

Ruby: super
来源：http://the.wangshuangyany.cn

C#:   base.Greet();
来源：http://crv.yongpay.top

[G08] 静态方法与属性
来源：http://huv.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ypn.cqqwz.cn

PHP:  public static function f() {}
来源：http://rlk.fengsongda.top

JS:   static f() {}
来源：http://qsu.zhengqikj.top

TS:   static f(): void {}
来源：http://yum.xziqi.cn

Java: static void f() {}
来源：http://nfp.ydzc1.top


<!-- 参考信息 -->