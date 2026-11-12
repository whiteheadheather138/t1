代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://tst.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rke.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmg.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://dab.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://uyh.hesvh.cn

Java: String.format("%03d", 7)
来源：http://dwv.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kcm.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gyc.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nnp.vqdsnc.cn

[E11] 反转字符串
来源：http://klt.fktsv.cn

Py:   s[::-1]
来源：http://igz.nwbrower.top

PHP:  strrev($s);
来源：http://foc.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://ppj.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://yak.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fvv.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://eas.fktsv.cn

Ruby: s.reverse
来源：http://ryc.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rrk.yuxming.cn

[E12] 统计某字符出现次数
来源：http://gqd.nanxinkj.top

Py:   s.count("a")
来源：http://fls.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://lpa.52xcode.cn

JS:   s.split("a").length - 1
来源：http://pgz.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://bbs.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zfm.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://tuo.fzhhl.top

Ruby: s.count("a")
来源：http://yoj.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://rok.redwolf501.top

[E13] 逐字符遍历
来源：http://qoh.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://crx.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aqc.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://byh.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qfs.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://axj.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ici.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://irp.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ewx.nwbrower.top

[E14] URL 编码与 Base64
来源：http://dxc.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://flv.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://upy.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tgq.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://czm.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vym.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ztn.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oml.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qdt.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://kte.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ufl.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hhc.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xmd.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nak.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mkb.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tdb.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://krc.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zuv.cdnleiting.top

[E16] 数字千分位
来源：http://ctn.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://led.hywenlv.cn

PHP:  number_format(1234567);
来源：http://ahx.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://irh.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nvq.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vkv.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tgy.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://spn.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://wmb.iojbl.cn

[E17] 首字母大写
来源：http://oou.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dep.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ikw.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kwa.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://saw.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ols.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mhr.zhengqikj.top

Ruby: s.capitalize
来源：http://guf.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kuq.chenzaomai.com

[E18] 模板占位符替换
来源：http://bha.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nvu.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mpo.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lif.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://stm.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://obv.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://geq.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wnm.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://coe.cashguo.top

[E19] 多行文本按行拆分
来源：http://eqt.cheryme.top

Py:   s.splitlines()
来源：http://jgg.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cqy.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://pog.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://uor.jyoumei.cn

Java: s.lines().toList()
来源：http://bto.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://tro.yuanzhike.top

Ruby: s.lines
来源：http://plv.sxryk.cn

C#:   s.Split('\n')
来源：http://wsx.tarul.cn

[E20] 判断字符串是否为空
来源：http://fwa.zhaomingkeji.xyz

Py:   if not s:
来源：http://yid.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kme.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wkv.sysykeji.top

TS:   if (s === "") {}
来源：http://qsc.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://yok.316326.xyz

Go:   if s == "" {}
来源：http://rhu.hongshengwenyu.top

Ruby: if s.empty?
来源：http://fmf.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hcf.snrcjt.cn

[E21] 超长截断加省略号
来源：http://qht.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fva.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nji.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zlh.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgb.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ifq.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://svs.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gee.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://egx.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://pnd.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://trt.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://goe.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uuj.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yyb.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ydq.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wdq.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://ihi.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ewg.tarul.cn

================================================================================
来源：http://lof.52xcode.cn

F. 文件与目录
来源：http://ffa.ehwqpu.com

================================================================================
来源：http://kys.316326.xyz

[F01] 读取整个文件
来源：http://vtl.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://obx.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://hmu.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://toh.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tbe.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uju.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uvq.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://icl.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://xhw.tianlin.xyz

[F02] 逐行读取文件
来源：http://ksf.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bpg.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ipo.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ijt.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wpo.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ksi.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yur.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://myr.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rzx.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://yxn.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ber.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ihp.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wro.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yrl.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nzl.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://acp.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://pje.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dpf.tanke756.top

[F04] 追加写入文件
来源：http://qky.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mbw.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yyb.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mje.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lfe.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hae.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nos.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lrk.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vnt.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://itz.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wnw.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://foe.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://opc.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://baa.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vuh.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gml.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://pps.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://xpt.hcnkem.com

[F06] 删除文件
来源：http://xpq.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://nqd.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://paq.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://jfy.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://pdt.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yso.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://bfv.cheryme.top

Ruby: File.delete("a.txt")
来源：http://soo.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://xme.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://lml.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fik.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vhh.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xux.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psf.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://byt.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fnb.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sml.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nwc.fzhhl.top

[F08] 遍历目录
来源：http://ydw.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wfp.svipenyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://suf.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://oqy.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://hpw.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xxs.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://suf.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://loy.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://rbv.kuanghao11.cn

[F09] 获取文件大小
来源：http://swl.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://fpi.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://hmf.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://dei.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://qye.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iqj.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lhe.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://juj.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://qpl.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://dbr.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cfi.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bgz.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jja.tarul.cn

TS:   path.extname("a.txt")
来源：http://jeq.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://grg.yanxiufei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ayw.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qaw.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uwh.yj202588.top

[F11] 复制与移动文件
来源：http://xga.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fzs.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zao.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdo.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uom.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iya.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mwv.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vco.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://abm.nanxinkj.top

[F12] CSV 读写
来源：http://ecq.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ymj.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jdu.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aum.zycfv.cn

TS:   // 同上
来源：http://wvx.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xbp.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uup.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://umx.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jvr.zhaomingkeji.xyz

================================================================================
来源：http://aau.yanxiufei.cn

G. 面向对象
来源：http://fwy.yonumen.top

================================================================================
来源：http://hvb.havefunace.top

[G01] 定义类
来源：http://ouj.zhengqikj.top

Py:   class User: pass
来源：http://evt.vehdjk.com

PHP:  class User {}
来源：http://bba.dianchejie.cn

JS:   class User {}
来源：http://mmk.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://qiz.yangfankeji.com

Java: class User {}
来源：http://aoa.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://wip.bjfxy.top

Ruby: class User; end
来源：http://dje.xuetiantiany.cn

C#:   class User {}
来源：http://cbx.quarkkingdee.top

[G02] 构造函数
来源：http://okb.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wut.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://ybk.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://qwj.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://tkc.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://tgf.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://weg.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://odp.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://rky.vqdsnc.cn

[G03] 实例属性
来源：http://xyh.sjlbkw.cn

Py:   self.name = "x"
来源：http://hzx.tarul.cn

PHP:  public string $name = "x";
来源：http://iqb.quarkkingdee.top

JS:   this.name = "x";
来源：http://esj.jqgfzy.top

TS:   name: string = "x";
来源：http://ptq.hammf.cn

Java: private String name;
来源：http://pup.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iia.hammf.cn

Ruby: @name = "x"
来源：http://jlf.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://qqu.svipenyu.cn

[G04] 定义方法
来源：http://xhs.uphjek.com

Py:   def greet(self): return self.name
来源：http://jmf.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hby.cashguo.top

JS:   greet() { return this.name; }
来源：http://mtz.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://ycl.xinyue.icu

Java: String greet() { return name; }
来源：http://txk.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eie.hywenlv.cn

Ruby: def greet; @name; end
来源：http://nsy.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://qra.quarkkingdee.top

[G05] 继承
来源：http://dhh.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://nnr.c1oappe.top

PHP:  class Admin extends User {}
来源：http://zwv.fzhhl.top

JS:   class Admin extends User {}
来源：http://lde.ybcxt.top

TS:   class Admin extends User {}
来源：http://czl.birdmap.top

Java: class Admin extends User {}
来源：http://ifw.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dpk.bjfxy.top

Ruby: class Admin < User; end
来源：http://tgz.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://mqa.sjlbkw.cn

[G06] 重写方法
来源：http://ygj.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://upo.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nob.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://pqm.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://yhk.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://hiq.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dww.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://uhp.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://xpz.jiagoushi.top

[G07] 调用父类方法
来源：http://eqy.dashuyun.cn

Py:   super().greet()
来源：http://bnk.sweek.top

PHP:  parent::greet();
来源：http://axb.yanxiufei.cn

JS:   super.greet();
来源：http://xop.jlsjyb.cn

TS:   super.greet();
来源：http://hvw.jyoumei.cn

Java: super.greet();
来源：http://sux.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://shn.yuxming.cn

Ruby: super
来源：http://pxr.smart0.xyz

C#:   base.Greet();
来源：http://zqj.birdmap.top

[G08] 静态方法与属性
来源：http://hby.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://emx.quarkkingdee.top

PHP:  public static function f() {}
来源：http://gqe.ywan-chungtsiang.top

JS:   static f() {}
来源：http://dpg.316326.xyz

TS:   static f(): void {}
来源：http://jak.andypj.xyz

Java: static void f() {}
来源：http://eox.jyoumei.cn


<!-- 参考信息 -->