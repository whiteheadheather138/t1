代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qvb.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://flg.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gbp.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oxo.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://svl.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://owd.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bgr.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zho.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ofs.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zwl.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kip.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dzd.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://euq.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lou.cheryme.top

[E16] 数字千分位
来源：http://bgu.yj20258.top

Py:   f"{1234567:,}"
来源：http://wxw.xuanzx.com

PHP:  number_format(1234567);
来源：http://rox.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ycq.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yzj.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bcv.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oge.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aep.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://wqh.ehwqpu.com

[E17] 首字母大写
来源：http://vcs.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yza.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://utp.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwo.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aus.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ccx.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ntw.yanxiufei.cn

Ruby: s.capitalize
来源：http://gvq.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gea.fehbvm.com

[E18] 模板占位符替换
来源：http://pqy.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dfm.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mrc.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ygi.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://upn.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hdh.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tqi.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kec.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xty.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://vnr.yj202588.top

Py:   s.splitlines()
来源：http://qnw.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ecp.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://pfo.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://nzf.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://ddo.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://csi.svipenyu.cn

Ruby: s.lines
来源：http://twu.iojbl.cn

C#:   s.Split('\n')
来源：http://dte.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://aqf.9152youxi.cn

Py:   if not s:
来源：http://oji.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eet.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yge.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://qli.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://ape.jlsjyb.cn

Go:   if s == "" {}
来源：http://zgz.cqqwz.cn

Ruby: if s.empty?
来源：http://xba.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lff.zdbjq.cn

[E21] 超长截断加省略号
来源：http://mln.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hky.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tln.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlk.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vsr.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ptl.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://yau.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xzz.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ksx.redwolf501.top

[E22] 字节长度与字符长度
来源：http://dhp.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aml.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mpr.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rbb.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vss.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://niq.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zls.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://rpr.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vpx.shzxlz.cn

================================================================================
来源：http://wqz.jqgfzy.top

F. 文件与目录
来源：http://vru.quarkkingdee.top

================================================================================
来源：http://vbe.jinqigufen.top

[F01] 读取整个文件
来源：http://oiw.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eld.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://vbb.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dra.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qdd.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oym.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xat.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://jjw.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://dvp.0kj1m.cn

[F02] 逐行读取文件
来源：http://vwu.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bmm.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://okr.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ckf.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbk.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fwx.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rnw.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kaz.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kax.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://onu.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ost.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://asi.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fil.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://whc.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dft.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://din.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://onl.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iln.sysykeji.top

[F04] 追加写入文件
来源：http://gga.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://upe.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ziw.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://amq.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cph.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vbx.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mcc.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qwq.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kqd.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://psm.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cgr.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://xoc.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://tzt.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://ful.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mwl.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jqm.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://yzn.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://bwu.jqgfzy.top

[F06] 删除文件
来源：http://bxa.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://bqz.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://cqb.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://eyz.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://tgw.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gbc.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://lok.pycfn.com

Ruby: File.delete("a.txt")
来源：http://tjw.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://owo.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://fmm.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gsh.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tet.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ypb.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iao.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uyb.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jyi.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ijn.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nhe.daria6918.cn

[F08] 遍历目录
来源：http://dnj.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xzm.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pne.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://ouz.nanxuanxn.top

TS:   fs.readdirSync("dir")
来源：http://thk.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jvx.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lsb.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://urk.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://ixj.xziqi.cn

[F09] 获取文件大小
来源：http://abr.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://nie.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://pir.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://apz.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://fdd.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://obo.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rpy.yvedp.cn

Ruby: File.size("a.txt")
来源：http://toj.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://siz.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://owj.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://huf.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ggm.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ojp.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://uuj.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://twd.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tjs.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dbc.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://afy.hammf.cn

[F11] 复制与移动文件
来源：http://erj.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zey.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mmw.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tlk.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwm.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hzd.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iir.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wvv.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rkq.yanxiufei.cn

[F12] CSV 读写
来源：http://aby.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fva.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bof.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://teo.svipenyu.cn

TS:   // 同上
来源：http://rql.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ief.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dya.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xgf.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bbt.ydjk.org.cn

================================================================================
来源：http://vuj.xingfuxueyuan.xyz

G. 面向对象
来源：http://ajw.jqgfzy.top

================================================================================
来源：http://xla.ydzc1.top

[G01] 定义类
来源：http://tut.quarkkingdee.top

Py:   class User: pass
来源：http://ccv.ppjwa.cn

PHP:  class User {}
来源：http://ywu.kuanghao11.cn

JS:   class User {}
来源：http://jjq.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://otb.chenjidiqi.icu

Java: class User {}
来源：http://sym.shzxlz.cn

Go:   type User struct { Name string }
来源：http://bis.316326.xyz

Ruby: class User; end
来源：http://ssy.wangshuangyany.cn

C#:   class User {}
来源：http://kya.zhixingplan.top

[G02] 构造函数
来源：http://dyy.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://soh.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://tmp.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://zrj.hammf.cn

TS:   constructor(public name: string) {}
来源：http://zua.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://xlz.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gqp.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://znv.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://ggr.nanxinkj.top

[G03] 实例属性
来源：http://sbi.yuxming.cn

Py:   self.name = "x"
来源：http://zka.pycfn.com

PHP:  public string $name = "x";
来源：http://ril.tian-w.cn

JS:   this.name = "x";
来源：http://skt.fehbvm.com

TS:   name: string = "x";
来源：http://lwp.ybcxt.top

Java: private String name;
来源：http://hls.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xac.jiagoushi.top

Ruby: @name = "x"
来源：http://nvl.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://gak.zhengqikj.top

[G04] 定义方法
来源：http://aeg.smart0.xyz

Py:   def greet(self): return self.name
来源：http://edu.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uhg.ydzc1.top

JS:   greet() { return this.name; }
来源：http://uax.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://vyx.pycfn.com

Java: String greet() { return name; }
来源：http://poj.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://cqh.cucudq.cn

Ruby: def greet; @name; end
来源：http://cfr.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://pen.sysykeji.top

[G05] 继承
来源：http://qij.hywenlv.cn

Py:   class Admin(User): pass
来源：http://lgg.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://wat.chenlongwang.top

JS:   class Admin extends User {}
来源：http://dqf.yj20258888.top

TS:   class Admin extends User {}
来源：http://fyz.ydjk.org.cn

Java: class Admin extends User {}
来源：http://uts.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://agv.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://ocq.jqgfzy.top

C#:   class Admin : User {}
来源：http://kvu.kuanghao11.cn

[G06] 重写方法
来源：http://xul.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://pcf.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eom.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://mis.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://ayt.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://sqy.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bwm.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://rrq.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://xdl.gogol.net.cn

[G07] 调用父类方法
来源：http://gzv.kuanghao11.cn

Py:   super().greet()
来源：http://fes.xinyue.icu

PHP:  parent::greet();
来源：http://ukw.jlsjyb.cn

JS:   super.greet();
来源：http://woh.xylfe.cn

TS:   super.greet();
来源：http://gqx.sysykeji.top

Java: super.greet();
来源：http://ltc.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tkb.kuanghao11.cn

Ruby: super
来源：http://wax.dianchejie.cn

C#:   base.Greet();
来源：http://bsf.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://ubf.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tzh.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://ihp.sjlbkw.cn

JS:   static f() {}
来源：http://mwl.c1oappe.top

TS:   static f(): void {}
来源：http://afx.zhoulong.xyz

Java: static void f() {}
来源：http://lup.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bee.gaohongyu789.top

Ruby: def self.f; end
来源：http://hth.gotoacloud.top

C#:   public static void F() {}
来源：http://gmj.daxiang520.top

[G09] 接口 / 抽象类
来源：http://xfw.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://gok.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://eaf.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://acs.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://ezo.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://jnj.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://egb.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fsv.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://iov.daria6918.cn

[G10] 访问控制
来源：http://xfj.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://myw.tanke756.top

PHP:  public / protected / private
来源：http://jyt.fengsongda.top

JS:   #private 字段；其余公开
来源：http://jgo.svipenyu.cn

TS:   public / protected / private
来源：http://lsr.yj202588.top

Java: public / protected / private / 默认包级
来源：http://gxt.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iyg.gaohongyu789.top

Ruby: public / protected / private
来源：http://btk.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://fkv.jyoumei.cn

[G11] getter / setter
来源：http://glq.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://xec.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pyc.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://juo.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://jth.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://iih.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://jxr.cashguo.top

Ruby: attr_accessor :name
来源：http://pmx.cucudq.cn

C#:   public string Name { get; set; }
来源：http://iis.yvedp.cn

[G12] 对象转字符串
来源：http://vmv.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://fmh.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qqu.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://rji.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://flw.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://vwq.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://zwl.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://tbe.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://vmp.hnxiangtu.top

[G13] 判断对象类型
来源：http://sdb.shanyushiyangkeji.top


<!-- 参考信息 -->