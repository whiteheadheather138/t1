代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://pgx.yvedp.cn

Java: String.format("%03d", 7)
来源：http://ktt.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gmf.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wez.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xem.gogol.net.cn

[E11] 反转字符串
来源：http://bjq.hcnkem.com

Py:   s[::-1]
来源：http://dnf.gaohongyu789.top

PHP:  strrev($s);
来源：http://zla.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://yhm.birdmap.top

TS:   [...s].reverse().join("")
来源：http://nbw.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pgc.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jfg.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://lwp.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jqk.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://pdt.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://njj.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://rkf.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://cjw.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://viy.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dco.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://urh.shangyingyoupin.top

Ruby: s.count("a")
来源：http://owd.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://bft.shzxlz.cn

[E13] 逐字符遍历
来源：http://yhy.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://pef.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvn.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://awq.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tcu.jqgfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dgf.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qzr.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dyo.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wtd.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://ibb.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cfo.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qin.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://atx.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xhq.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hmq.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://soe.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xfj.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xrr.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://gvj.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gsc.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyt.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://foq.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kai.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fdr.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mwm.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ilm.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pfg.yueranfly.top

[E16] 数字千分位
来源：http://pmm.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://bxs.ybcxt.top

PHP:  number_format(1234567);
来源：http://uxm.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ojg.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://czs.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kyg.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cir.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tar.yonumen.top

C#:   1234567.ToString("N0")
来源：http://naa.tarul.cn

[E17] 首字母大写
来源：http://yac.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://omc.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://giy.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://unf.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ypy.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pbj.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gwu.zhongyouzk.top

Ruby: s.capitalize
来源：http://qpw.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzf.tianlin.xyz

[E18] 模板占位符替换
来源：http://ycb.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uje.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cio.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gui.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wbw.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vax.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kha.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vgo.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyy.xinyue.icu

[E19] 多行文本按行拆分
来源：http://rkd.zdbjq.cn

Py:   s.splitlines()
来源：http://klr.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uho.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://hkt.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://wnf.jianghu66.top

Java: s.lines().toList()
来源：http://qlg.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://zpq.cdnleiting.top

Ruby: s.lines
来源：http://ltt.ivvv.top

C#:   s.Split('\n')
来源：http://rmo.epnwcf.com

[E20] 判断字符串是否为空
来源：http://wxu.jiagoushi.top

Py:   if not s:
来源：http://frn.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gyr.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dvc.yfazqb.com

TS:   if (s === "") {}
来源：http://fzd.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://nkb.feifeiyinyue.top

Go:   if s == "" {}
来源：http://dxb.tian-w.cn

Ruby: if s.empty?
来源：http://tlu.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lly.ivvv.top

[E21] 超长截断加省略号
来源：http://hkn.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://loq.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hui.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wzh.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsn.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bib.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://lvf.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oma.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qio.zycfv.cn

[E22] 字节长度与字符长度
来源：http://ajq.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fgr.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zur.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iht.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bai.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kzk.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tps.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://iap.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tkh.feifeiyinyue.top

================================================================================
来源：http://qti.shzxlz.cn

F. 文件与目录
来源：http://cen.yj202588.top

================================================================================
来源：http://isn.shangyingyoupin.top

[F01] 读取整个文件
来源：http://mfk.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vqe.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://uwb.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kyt.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kvt.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://irt.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bro.zycfv.cn

Ruby: File.read("a.txt")
来源：http://pdd.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://whi.cashguo.top

[F02] 逐行读取文件
来源：http://ajh.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qxy.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bps.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ett.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oyh.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rph.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nnd.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://awb.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sam.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://bqx.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yvz.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nvt.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tma.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://alu.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eyf.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ytp.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://evw.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://edl.fehbvm.com

[F04] 追加写入文件
来源：http://zbv.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qco.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://idj.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pno.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ysb.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ney.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vlp.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lrz.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbg.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://ljc.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wuj.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://egv.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://nvv.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://sjd.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://mbb.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cjg.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://shg.ivvv.top

C#:   File.Exists("a.txt")
来源：http://vbc.fehbvm.com

[F06] 删除文件
来源：http://unz.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://bqi.yfazqb.com

PHP:  unlink("a.txt");
来源：http://nrn.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://vng.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://com.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://omf.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://lbu.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://uia.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://iuy.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://yjz.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cdw.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qgc.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uzv.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hym.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vav.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://spk.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wwi.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rhx.cheryme.top

[F08] 遍历目录
来源：http://win.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ckq.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://igx.sweek.top

JS:   fs.readdirSync("dir")
来源：http://rtc.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://jzc.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ckr.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bwd.yfazqb.com

Ruby: Dir.children("dir")
来源：http://zhx.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://obf.hnqzz.top

[F09] 获取文件大小
来源：http://vao.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://ghl.aizwys.cn

PHP:  filesize("a.txt");
来源：http://zbx.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://whh.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://hta.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://zfk.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gmy.sxryk.cn

Ruby: File.size("a.txt")
来源：http://itu.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://ibq.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://tlz.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://abo.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dgs.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yjh.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://eex.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lyg.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xty.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fzg.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wyv.cashguo.top

[F11] 复制与移动文件
来源：http://syj.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qpr.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rif.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://end.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktv.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gyt.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zez.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://idf.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kab.yj202588.top

[F12] CSV 读写
来源：http://cfs.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://las.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ddb.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://imh.zhongyouzk.top

TS:   // 同上
来源：http://ifj.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oym.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xzu.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dys.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mbd.pycfn.com

================================================================================
来源：http://xwy.xuanzx.com

G. 面向对象
来源：http://top.shangyingyoupin.top

================================================================================
来源：http://vpk.ydzc1.top

[G01] 定义类
来源：http://fva.xziqi.cn

Py:   class User: pass
来源：http://bbn.jlsjyb.cn

PHP:  class User {}
来源：http://ekb.hesvh.cn

JS:   class User {}
来源：http://izq.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://sfr.jlsjyb.cn

Java: class User {}
来源：http://wce.yangfankeji.com

Go:   type User struct { Name string }
来源：http://euv.bbcook.cn

Ruby: class User; end
来源：http://cuq.hysaishi.cn

C#:   class User {}
来源：http://ehi.zhixingplan.top

[G02] 构造函数
来源：http://zsm.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://wky.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://nmw.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://xgt.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://iqq.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://sdi.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://trm.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://ble.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://iep.daxiang520.top

[G03] 实例属性
来源：http://bgw.jinqigfzy.top

Py:   self.name = "x"
来源：http://lzn.tianlin.xyz

PHP:  public string $name = "x";
来源：http://wba.hongshengwenyu.top

JS:   this.name = "x";
来源：http://hfj.jinqigfzy.top

TS:   name: string = "x";
来源：http://urz.hywenlv.cn

Java: private String name;
来源：http://sig.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ftx.chenzaomai.com

Ruby: @name = "x"
来源：http://xpe.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://yvo.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://fhj.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://irz.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gwb.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://dsp.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://ira.haohaochexian.top

Java: String greet() { return name; }
来源：http://bpy.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jhu.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://ctr.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://lkj.shzxlz.cn

[G05] 继承
来源：http://czl.0kj1m.cn

Py:   class Admin(User): pass
来源：http://vhi.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://ldd.andypj.xyz

JS:   class Admin extends User {}
来源：http://ipk.fehbvm.com

TS:   class Admin extends User {}
来源：http://mtn.fktsv.cn

Java: class Admin extends User {}
来源：http://exp.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tqm.gotoacloud.top

Ruby: class Admin < User; end
来源：http://kwt.yj20258888.top

C#:   class Admin : User {}
来源：http://dbe.shuidangran.top

[G06] 重写方法
来源：http://pco.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://lyn.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://fyc.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://vfg.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://ycu.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://jig.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mmm.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://veu.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://nmh.tanke756.top

[G07] 调用父类方法
来源：http://vwb.c1oappe.top

Py:   super().greet()
来源：http://aea.cheryme.top

PHP:  parent::greet();
来源：http://noq.redwolf501.top

JS:   super.greet();
来源：http://qjt.vehdjk.com

TS:   super.greet();
来源：http://pcn.zdbjq.cn

Java: super.greet();
来源：http://krv.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hwc.guowangkeji.top

Ruby: super
来源：http://gmc.wangshuangyany.cn

C#:   base.Greet();
来源：http://hzg.smart0.xyz

[G08] 静态方法与属性
来源：http://atm.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xxn.cashguo.top

PHP:  public static function f() {}
来源：http://pbr.zhaomingkeji.xyz

JS:   static f() {}
来源：http://vuc.dashuyun.cn

TS:   static f(): void {}
来源：http://ddw.sxryk.cn

Java: static void f() {}
来源：http://bsn.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gba.svipenyu.cn

Ruby: def self.f; end
来源：http://mlr.hammf.cn

C#:   public static void F() {}
来源：http://iuh.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://drf.vqdsnc.cn


<!-- 参考信息 -->