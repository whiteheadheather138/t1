代发 wailian999

Go:   strings.Count(s, "a")
来源：http://ees.mhx1999.top

Ruby: s.count("a")
来源：http://pau.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://qia.gzhubu.top

[E13] 逐字符遍历
来源：http://fum.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://cqo.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zff.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://guw.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xix.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bzs.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tsp.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://txh.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bhu.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://rcp.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hjh.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldq.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kku.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://arn.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lzz.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dxa.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zqa.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hbf.ydzc1.top

[E15] HTML 转义 / 反转义
来源：http://xca.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://kkc.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cvu.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pcb.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://grl.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqj.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fir.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uoq.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://llj.xuetiantiany.cn

[E16] 数字千分位
来源：http://mde.zycfv.cn

Py:   f"{1234567:,}"
来源：http://wxb.ehwqpu.com

PHP:  number_format(1234567);
来源：http://ezp.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mbs.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wmj.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fkk.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kid.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vfk.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://fjz.tanke756.top

[E17] 首字母大写
来源：http://sxa.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dew.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fpq.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bub.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jzf.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zda.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ups.feifeiyinyue.top

Ruby: s.capitalize
来源：http://ono.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://drz.fengsongda.top

[E18] 模板占位符替换
来源：http://hpn.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wgv.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rnt.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://gbv.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nku.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dlr.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dvq.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ynm.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gfv.shuidangran.top

[E19] 多行文本按行拆分
来源：http://xcu.bbcook.cn

Py:   s.splitlines()
来源：http://htw.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tzg.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://iot.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://uap.yuxming.cn

Java: s.lines().toList()
来源：http://lzf.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://jzp.guowangkeji.top

Ruby: s.lines
来源：http://gko.hesvh.cn

C#:   s.Split('\n')
来源：http://fti.bbcook.cn

[E20] 判断字符串是否为空
来源：http://hgq.yangfankeji.com

Py:   if not s:
来源：http://bwb.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zgr.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ffz.jyoumei.cn

TS:   if (s === "") {}
来源：http://bjz.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://nof.shangyingyoupin.top

Go:   if s == "" {}
来源：http://qtt.daxiang520.top

Ruby: if s.empty?
来源：http://oyh.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hvp.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://sds.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sdy.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rhn.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://unx.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymr.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bta.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://wdf.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hzt.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bfe.yj20258.top

[E22] 字节长度与字符长度
来源：http://nol.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rqt.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zci.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kll.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahx.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tdu.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kcb.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://sia.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vst.sufxvd.cn

================================================================================
来源：http://jno.zycfv.cn

F. 文件与目录
来源：http://chu.andypj.xyz

================================================================================
来源：http://rwr.jinqigufen.top

[F01] 读取整个文件
来源：http://tyn.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iuu.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://vgf.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xwy.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hal.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mtd.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pkg.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://evn.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://qsz.chenzaomai.com

[F02] 逐行读取文件
来源：http://byo.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hlf.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lvh.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://viu.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rzr.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lcp.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uwe.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xgh.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ily.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://zse.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tjc.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://nem.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nnz.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ihc.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://auv.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://feq.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://gnb.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hnm.mhx1999.top

[F04] 追加写入文件
来源：http://tjr.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://axp.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://flr.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dcc.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzy.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://chv.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cvr.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oro.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rib.uphjek.com

[F05] 判断文件或目录是否存在
来源：http://ufj.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zwy.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://etv.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://oos.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://eso.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://odf.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wqj.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://ikw.pycfn.com

C#:   File.Exists("a.txt")
来源：http://pzd.cucudq.cn

[F06] 删除文件
来源：http://blp.yueranfly.top

Py:   os.remove("a.txt")
来源：http://olm.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://xkn.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pan.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://dty.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mxf.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://rji.yj20258.top

Ruby: File.delete("a.txt")
来源：http://fur.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://wbc.tian-w.cn

[F07] 创建目录（含多级）
来源：http://wzs.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kdt.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kwl.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pju.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fpb.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fxw.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyf.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oiw.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://glr.jinqigufen.top

[F08] 遍历目录
来源：http://whv.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://exn.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pou.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://cha.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://xwy.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cfo.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ggj.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://aum.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://yso.yueranfly.top

[F09] 获取文件大小
来源：http://wxj.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://srs.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://glb.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://qfr.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://tpw.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://ttq.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sie.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://fnl.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://ydh.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://xgc.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rll.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wah.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xnm.gzhubu.top

TS:   path.extname("a.txt")
来源：http://goq.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jkc.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zgi.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ide.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cub.jiagoushi.top

[F11] 复制与移动文件
来源：http://ytu.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mwg.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://new.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnj.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ffa.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rud.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qcr.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ykn.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aaj.cdnleiting.top

[F12] CSV 读写
来源：http://ucm.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://viz.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ksy.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rol.uphjek.com

TS:   // 同上
来源：http://mgp.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uwi.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pjv.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://chs.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gnj.xingfuxueyuan.xyz

================================================================================
来源：http://umi.jinqigfzy.top

G. 面向对象
来源：http://mel.xuanzx.com

================================================================================
来源：http://rug.cashguo.top

[G01] 定义类
来源：http://xmm.jinqigfzy.top

Py:   class User: pass
来源：http://ymv.iojbl.cn

PHP:  class User {}
来源：http://yqy.yueranfly.top

JS:   class User {}
来源：http://kat.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://wae.chenlongwang.top

Java: class User {}
来源：http://zqn.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://nlj.xuanzx.com

Ruby: class User; end
来源：http://nvr.tianlin.xyz

C#:   class User {}
来源：http://nge.wangshuangyany.cn

[G02] 构造函数
来源：http://rdb.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://vvi.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://gvr.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://cbh.hammf.cn

TS:   constructor(public name: string) {}
来源：http://qjf.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://qne.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rmd.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://wpv.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://xwl.svipenyu.cn

[G03] 实例属性
来源：http://edo.sufxvd.cn

Py:   self.name = "x"
来源：http://rzm.jinqigufen.top

PHP:  public string $name = "x";
来源：http://rmv.shangyingyoupin.top

JS:   this.name = "x";
来源：http://zok.nanxinkj.top

TS:   name: string = "x";
来源：http://err.yangfankeji.com

Java: private String name;
来源：http://esg.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://whp.jqgufenzy.top

Ruby: @name = "x"
来源：http://kxu.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://qna.cucudq.cn

[G04] 定义方法
来源：http://cvi.yongpay.top

Py:   def greet(self): return self.name
来源：http://fxb.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pjc.52xcode.cn

JS:   greet() { return this.name; }
来源：http://kgb.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://cpn.jyoumei.cn

Java: String greet() { return name; }
来源：http://nlg.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://whz.snrcjt.cn

Ruby: def greet; @name; end
来源：http://jfv.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://izd.ehwqpu.com

[G05] 继承
来源：http://dcf.0kj1m.cn

Py:   class Admin(User): pass
来源：http://dlq.52xcode.cn

PHP:  class Admin extends User {}
来源：http://mdf.316326.xyz

JS:   class Admin extends User {}
来源：http://cxc.guannengcc.top

TS:   class Admin extends User {}
来源：http://ikw.nwbrower.top

Java: class Admin extends User {}
来源：http://jvy.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yqj.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://zyh.zhijiandao.cn

C#:   class Admin : User {}
来源：http://zgo.hywenlv.cn

[G06] 重写方法
来源：http://cfi.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://wnu.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xfm.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://ega.fengsongda.top

TS:   greet(): string { return "admin"; }
来源：http://omb.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://inh.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fhr.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://mpl.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://ykz.fehbvm.com

[G07] 调用父类方法
来源：http://frk.dashuyun.cn

Py:   super().greet()
来源：http://ubn.snrcjt.cn

PHP:  parent::greet();
来源：http://mdi.shanyushiyangkeji.top

JS:   super.greet();
来源：http://ytw.daxiang520.top

TS:   super.greet();
来源：http://aut.tanke756.top

Java: super.greet();
来源：http://xsk.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dws.hammf.cn

Ruby: super
来源：http://xwl.yj20258.top

C#:   base.Greet();
来源：http://kcf.yangfankeji.com

[G08] 静态方法与属性
来源：http://lfh.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lnj.cucudq.cn

PHP:  public static function f() {}
来源：http://wqg.hammf.cn

JS:   static f() {}
来源：http://lza.zdbjq.cn

TS:   static f(): void {}
来源：http://gdj.aizwys.cn

Java: static void f() {}
来源：http://krf.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dzl.xinyue.icu

Ruby: def self.f; end
来源：http://dxy.wangdashe.top

C#:   public static void F() {}
来源：http://jkw.mhx1999.top

[G09] 接口 / 抽象类
来源：http://ppq.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://eew.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hdo.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqr.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://ocw.shuidangran.top

Java: interface Shape { double area(); }
来源：http://vli.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://ykh.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://omy.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://ewi.sufxvd.cn

[G10] 访问控制
来源：http://vce.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://anr.316326.xyz

PHP:  public / protected / private
来源：http://zzr.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://sgv.hywenlv.cn

TS:   public / protected / private
来源：http://iad.yj20258.top

Java: public / protected / private / 默认包级
来源：http://zhq.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cur.birdmap.top

Ruby: public / protected / private
来源：http://hqe.zhixingplan.top

C#:   public / protected / private / internal
来源：http://lqm.xziqi.cn

[G11] getter / setter
来源：http://njp.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://ygs.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ndp.ivvv.top


<!-- 参考信息 -->