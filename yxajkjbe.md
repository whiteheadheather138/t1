代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aep.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zib.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dfq.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://atv.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wuu.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://fai.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vhh.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nwx.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lrz.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://eal.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://poy.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bze.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://khe.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mcb.jqgufenzy.top

[E16] 数字千分位
来源：http://iya.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://liq.xinyue.icu

PHP:  number_format(1234567);
来源：http://qxl.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rck.guannengcc.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ftm.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nyj.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://urw.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xsd.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://jzj.tanke756.top

[E17] 首字母大写
来源：http://ipp.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rmc.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://chi.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hmd.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wmq.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mcw.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lvc.iojbl.cn

Ruby: s.capitalize
来源：http://wab.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hns.gaohongyu789.top

[E18] 模板占位符替换
来源：http://czd.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oxy.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ofl.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pai.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://sdb.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gpp.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ayl.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bdo.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mqd.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://els.yfazqb.com

Py:   s.splitlines()
来源：http://zie.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jic.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://okf.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://fjt.zycfv.cn

Java: s.lines().toList()
来源：http://hen.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://unr.nwbrower.top

Ruby: s.lines
来源：http://gzm.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://wok.ybcxt.top

[E20] 判断字符串是否为空
来源：http://wni.fanxiaobao.xyz

Py:   if not s:
来源：http://fzq.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sgl.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oby.epnwcf.com

TS:   if (s === "") {}
来源：http://kpk.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://dfk.gogol.net.cn

Go:   if s == "" {}
来源：http://roi.shangyingyoupin.top

Ruby: if s.empty?
来源：http://rqa.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lba.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://tva.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zot.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mld.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ukj.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uwl.hfpthk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fji.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://dzp.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://how.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dnf.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://ywf.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xhw.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uap.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://plr.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qvk.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nep.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jff.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://eqp.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dvr.sysykeji.top

================================================================================
来源：http://oco.gaohongyu789.top

F. 文件与目录
来源：http://vac.zhiwuduotai.top

================================================================================
来源：http://sbo.dianchejie.cn

[F01] 读取整个文件
来源：http://uqm.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dff.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://ngi.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cct.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mqd.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vup.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yoe.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://lxj.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xmb.aibaodan.cn

[F02] 逐行读取文件
来源：http://qax.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ege.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qdh.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://byi.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpv.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kij.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://azi.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jku.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://noh.meibo888.top

[F03] 写入文件（覆盖）
来源：http://eem.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aln.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://heo.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eri.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lcn.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bvt.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://erd.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://sak.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://apn.feifeiyinyue.top

[F04] 追加写入文件
来源：http://zap.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gso.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sfy.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jjk.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xox.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ete.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jvr.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://axl.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fwm.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://ote.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imw.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://zcd.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://arc.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://cqj.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qye.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tus.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://gys.yongpay.top

C#:   File.Exists("a.txt")
来源：http://gwo.yueranfly.top

[F06] 删除文件
来源：http://bfm.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://lrm.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://qoo.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://rxj.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dqb.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rfc.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://vvs.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://oxe.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://kxj.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://uau.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqp.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ilm.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stc.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xhp.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dqg.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bcf.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dee.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vec.bjfxy.top

[F08] 遍历目录
来源：http://rix.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uoz.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dus.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://tkm.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://rnc.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://atc.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dqn.fzhhl.top

Ruby: Dir.children("dir")
来源：http://sfc.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://yes.xziqi.cn

[F09] 获取文件大小
来源：http://nxj.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://ikv.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://its.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://ngy.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://ooi.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://ptu.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vzl.mhx1999.top

Ruby: File.size("a.txt")
来源：http://dby.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://suz.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://rpo.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://krk.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://muj.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://djw.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://kmt.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zoi.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kmg.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://msn.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://suh.ctjpmb.com

[F11] 复制与移动文件
来源：http://jgt.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tun.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mrg.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fim.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzt.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mmg.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://chf.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yno.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tcz.pycfn.com

[F12] CSV 读写
来源：http://oej.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://avd.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lnx.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xbi.smart0.xyz

TS:   // 同上
来源：http://kii.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hjy.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nwd.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yzj.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jed.pycfn.com

================================================================================
来源：http://fib.jinyuanbaomall.cn

G. 面向对象
来源：http://zea.wangshuangyany.cn

================================================================================
来源：http://mta.zdbjq.cn

[G01] 定义类
来源：http://dat.fanxiaobao.xyz

Py:   class User: pass
来源：http://tbe.shuidangran.top

PHP:  class User {}
来源：http://ufw.snrcjt.cn

JS:   class User {}
来源：http://tqg.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://cnt.chenjidiqi.icu

Java: class User {}
来源：http://uwm.snrcjt.cn

Go:   type User struct { Name string }
来源：http://uli.ywan-chungtsiang.top

Ruby: class User; end
来源：http://iin.sufxvd.cn

C#:   class User {}
来源：http://edq.yfazqb.com

[G02] 构造函数
来源：http://szu.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://vzl.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://xvn.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://uqq.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://wpr.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://xsw.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sna.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://xoq.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://xzy.yj20258888.top

[G03] 实例属性
来源：http://wli.fengsongda.top

Py:   self.name = "x"
来源：http://tdx.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://xto.haohaochexian.top

JS:   this.name = "x";
来源：http://zfa.havefunace.top

TS:   name: string = "x";
来源：http://efz.ppjwa.cn

Java: private String name;
来源：http://vtb.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lcj.jinqigufen.top

Ruby: @name = "x"
来源：http://msq.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://lyh.dashuyun.cn

[G04] 定义方法
来源：http://ryc.sweek.top

Py:   def greet(self): return self.name
来源：http://hyg.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fll.gzhubu.top

JS:   greet() { return this.name; }
来源：http://tsw.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://uxk.jyoumei.cn

Java: String greet() { return name; }
来源：http://wum.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fub.fktsv.cn

Ruby: def greet; @name; end
来源：http://cvf.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://qcd.redwolf501.top

[G05] 继承
来源：http://efh.xylfe.cn

Py:   class Admin(User): pass
来源：http://twq.tian-w.cn

PHP:  class Admin extends User {}
来源：http://wjw.bbcook.cn

JS:   class Admin extends User {}
来源：http://ziw.aibaodan.cn

TS:   class Admin extends User {}
来源：http://wma.gaohongyu789.top

Java: class Admin extends User {}
来源：http://mcd.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jxq.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://ldn.ybcxt.top

C#:   class Admin : User {}
来源：http://byb.gotoacloud.top

[G06] 重写方法
来源：http://gse.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://xel.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gxo.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://zfd.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://vqz.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://qdp.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jnr.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://qxv.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://hxh.meibo888.top

[G07] 调用父类方法
来源：http://ywp.vehdjk.com

Py:   super().greet()
来源：http://fre.cucudq.cn

PHP:  parent::greet();
来源：http://uir.nwbrower.top

JS:   super.greet();
来源：http://mhl.cucudq.cn

TS:   super.greet();
来源：http://eci.ivvv.top

Java: super.greet();
来源：http://umk.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hsg.xylfe.cn

Ruby: super
来源：http://yay.feifeiyinyue.top

C#:   base.Greet();
来源：http://sjj.sufxvd.cn

[G08] 静态方法与属性
来源：http://ajy.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xie.bbcook.cn

PHP:  public static function f() {}
来源：http://kka.nanxinkj.top

JS:   static f() {}
来源：http://dbn.tian-w.cn

TS:   static f(): void {}
来源：http://dfi.yuxming.cn

Java: static void f() {}
来源：http://guz.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://bph.52xcode.cn

Ruby: def self.f; end
来源：http://rir.hesvh.cn

C#:   public static void F() {}
来源：http://icd.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://nxi.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://wck.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://nkx.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qbr.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://fqz.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://odl.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://jxw.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cmq.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://xsu.guowangkeji.top

[G10] 访问控制
来源：http://udp.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://bjp.nanxuanxn.top

PHP:  public / protected / private
来源：http://uid.fengsongda.top

JS:   #private 字段；其余公开
来源：http://aef.zdqjudy.top

TS:   public / protected / private
来源：http://hgw.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://gui.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://zud.sjlbkw.cn

Ruby: public / protected / private
来源：http://vtf.hesvh.cn

C#:   public / protected / private / internal
来源：http://bti.feifeiyinyue.top

[G11] getter / setter
来源：http://okn.gzhubu.top

Py:   @property 与 @x.setter
来源：http://gfs.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kvd.gotoacloud.top

JS:   get name() { return this._name; }
来源：http://cto.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://nyh.zdqjudy.top

Java: public String getName() { return name; }
来源：http://jhj.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dsx.gzhubu.top

Ruby: attr_accessor :name
来源：http://jbj.andypj.xyz

C#:   public string Name { get; set; }
来源：http://mwa.bjfxy.top

[G12] 对象转字符串
来源：http://vkr.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://ggy.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fqd.smart0.xyz

JS:   toString() { return this.name; }
来源：http://lys.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://jxx.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://zzu.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zda.tanke756.top

Ruby: def to_s; @name; end
来源：http://qrt.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://gxc.tianlin.xyz

[G13] 判断对象类型
来源：http://zyq.epnwcf.com


<!-- 参考信息 -->