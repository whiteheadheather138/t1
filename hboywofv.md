代发 wailian999

[E14] URL 编码与 Base64
来源：http://oue.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zib.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://jbq.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bmk.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yky.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://icw.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qex.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ymd.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qbd.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://oag.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fsr.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lnl.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vem.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kgf.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kkx.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jfu.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://twt.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hgm.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://fzb.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://qph.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://ggk.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ucb.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xfo.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://heb.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://omv.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jdw.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://ank.c1oappe.top

[E17] 首字母大写
来源：http://ukx.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gvu.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lwi.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://amh.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfz.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vjp.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vbt.sxryk.cn

Ruby: s.capitalize
来源：http://vge.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pbs.ydjk.org.cn

[E18] 模板占位符替换
来源：http://emi.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fyh.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://siz.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vdt.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zmy.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sgh.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fen.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hlj.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nri.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://fbk.ctjpmb.com

Py:   s.splitlines()
来源：http://psy.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zqb.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://qut.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://ugk.yanxiufei.cn

Java: s.lines().toList()
来源：http://doa.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://lnq.epnwcf.com

Ruby: s.lines
来源：http://rta.cashguo.top

C#:   s.Split('\n')
来源：http://rsr.yj20258888.top

[E20] 判断字符串是否为空
来源：http://bws.tian-w.cn

Py:   if not s:
来源：http://wsr.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zmp.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rnh.gogol.net.cn

TS:   if (s === "") {}
来源：http://ksv.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://nss.jinqigufen.top

Go:   if s == "" {}
来源：http://vmh.sjlbkw.cn

Ruby: if s.empty?
来源：http://uqk.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://agv.jyoumei.cn

[E21] 超长截断加省略号
来源：http://vtg.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xwk.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jya.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yvj.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bwv.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://klm.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://mxn.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dka.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rlq.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://dvw.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://loh.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://krg.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qku.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nzh.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hez.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mdh.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://rgg.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lou.52xcode.cn

================================================================================
来源：http://nir.feifeiyinyue.top

F. 文件与目录
来源：http://xkc.hnqzz.top

================================================================================
来源：http://mvp.bbcook.cn

[F01] 读取整个文件
来源：http://ggh.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cem.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://wqz.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://trg.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dwg.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://hwh.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pza.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://dnc.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://mqo.dianchejie.cn

[F02] 逐行读取文件
来源：http://zrk.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lmx.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pmm.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zjv.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ojc.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bdc.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://brq.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nka.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lew.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://osm.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zmu.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lvg.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oyf.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zvr.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jgk.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qeg.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://seo.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eld.havefunace.top

[F04] 追加写入文件
来源：http://qkm.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ugw.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vkc.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xkh.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xlo.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rlu.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lwi.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dra.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zui.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://brq.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bya.yongpay.top

PHP:  file_exists("a.txt");
来源：http://ffz.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://wam.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://iuj.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://for.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://leg.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://drr.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://ltz.fehbvm.com

[F06] 删除文件
来源：http://dyv.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://oet.xziqi.cn

PHP:  unlink("a.txt");
来源：http://uby.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mlx.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://ior.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uzz.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://ehz.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://ycp.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://wjn.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://bgo.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hid.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ohy.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nan.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hzh.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kmw.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cjc.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://enc.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://azw.smart0.xyz

[F08] 遍历目录
来源：http://ytk.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://nmm.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dnb.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://kok.xziqi.cn

TS:   fs.readdirSync("dir")
来源：http://rqt.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bma.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xbo.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://xjz.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://rup.ybcxt.top

[F09] 获取文件大小
来源：http://ilz.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://wim.meibo888.top

PHP:  filesize("a.txt");
来源：http://jfs.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://tjf.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://ngb.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://kbq.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ath.316326.xyz

Ruby: File.size("a.txt")
来源：http://hjq.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://axb.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://pjd.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ftk.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jgn.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aay.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://yek.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xdn.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dph.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ptq.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://neo.zdbjq.cn

[F11] 复制与移动文件
来源：http://zaa.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gmw.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://inc.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fnh.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iuz.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aqp.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kpn.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfz.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ujo.zhengqikj.top

[F12] CSV 读写
来源：http://pej.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wok.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nrz.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qdo.fktsv.cn

TS:   // 同上
来源：http://ynv.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yqy.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qex.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rng.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xam.fktsv.cn

================================================================================
来源：http://voe.zhoulong.xyz

G. 面向对象
来源：http://nhr.9152youxi.cn

================================================================================
来源：http://vrz.cqqwz.cn

[G01] 定义类
来源：http://ubg.yuanzhike.top

Py:   class User: pass
来源：http://pdl.jinghuilouyu.cn

PHP:  class User {}
来源：http://rnm.zhaomingkeji.xyz

JS:   class User {}
来源：http://zda.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://ywc.jinghuilouyu.cn

Java: class User {}
来源：http://gtb.guowangkeji.top

Go:   type User struct { Name string }
来源：http://nxe.hysaishi.cn

Ruby: class User; end
来源：http://nlq.hysaishi.cn

C#:   class User {}
来源：http://lcj.shzxlz.cn

[G02] 构造函数
来源：http://hbu.xylfe.cn

Py:   def __init__(self, name): self.name = name
来源：http://tyl.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://ngr.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://liy.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://dql.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://iia.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kpp.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://phu.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://dnk.quarkkingdee.top

[G03] 实例属性
来源：http://qsf.jinqigufen.top

Py:   self.name = "x"
来源：http://csi.hesvh.cn

PHP:  public string $name = "x";
来源：http://vsb.gogol.net.cn

JS:   this.name = "x";
来源：http://kmk.yangfankeji.com

TS:   name: string = "x";
来源：http://kel.uphjek.com

Java: private String name;
来源：http://mbs.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hcv.cucudq.cn

Ruby: @name = "x"
来源：http://wyc.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://ntt.gotoacloud.top

[G04] 定义方法
来源：http://bjb.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://bxo.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fko.yj20258888.top

JS:   greet() { return this.name; }
来源：http://ger.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://xnp.chenlongwang.top

Java: String greet() { return name; }
来源：http://tlk.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://lgd.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://tyw.meibo888.top

C#:   public string Greet() => Name;
来源：http://itc.bjfxy.top

[G05] 继承
来源：http://yzl.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://nke.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://jrx.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://xsz.cheryme.top

TS:   class Admin extends User {}
来源：http://xdq.fktsv.cn

Java: class Admin extends User {}
来源：http://kaf.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vxf.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://kth.cucudq.cn

C#:   class Admin : User {}
来源：http://ngz.gotoacloud.top

[G06] 重写方法
来源：http://bdg.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://wzx.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xnb.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://yvj.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://arf.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://hyy.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zrt.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://agl.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://vig.aibaodan.cn

[G07] 调用父类方法
来源：http://tkj.sxryk.cn

Py:   super().greet()
来源：http://glw.yj20258888.top

PHP:  parent::greet();
来源：http://kej.dashuyun.cn

JS:   super.greet();
来源：http://sgk.hammf.cn

TS:   super.greet();
来源：http://qcd.9152youxi.cn

Java: super.greet();
来源：http://nvt.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://boo.quarkkingdee.top

Ruby: super
来源：http://pqx.ydzc1.top

C#:   base.Greet();
来源：http://aau.meibo888.top

[G08] 静态方法与属性
来源：http://nak.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bfu.cdnleiting.top

PHP:  public static function f() {}
来源：http://jht.andypj.xyz

JS:   static f() {}
来源：http://yex.chenjidiqi.icu

TS:   static f(): void {}
来源：http://vjo.aibaodan.cn

Java: static void f() {}
来源：http://wet.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://erw.sufxvd.cn

Ruby: def self.f; end
来源：http://bgh.nwbrower.top

C#:   public static void F() {}
来源：http://axk.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://yue.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://tnj.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://yyt.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hln.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://bht.hnqzz.top

Java: interface Shape { double area(); }
来源：http://mvm.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://smo.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tie.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://nig.guowangkeji.top

[G10] 访问控制
来源：http://zii.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://cpl.tianlin.xyz

PHP:  public / protected / private
来源：http://xys.wangdashe.top

JS:   #private 字段；其余公开
来源：http://xzg.jinqigufen.top

TS:   public / protected / private
来源：http://oyo.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://wtz.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hvg.iojbl.cn

Ruby: public / protected / private
来源：http://cts.tanke756.top

C#:   public / protected / private / internal
来源：http://zos.nanxuanxn.top

[G11] getter / setter
来源：http://vvt.fktsv.cn

Py:   @property 与 @x.setter
来源：http://lui.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kbh.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://xmx.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://xmg.hnqzz.top

Java: public String getName() { return name; }
来源：http://qwe.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jrd.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://min.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://xrg.shuidangran.top

[G12] 对象转字符串
来源：http://lqn.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://aqw.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ylm.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://hnf.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://zqe.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://sjc.fehbvm.com


<!-- 参考信息 -->