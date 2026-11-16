代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://chp.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jis.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jum.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ygl.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://puz.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xub.chenjidiqi.icu

[E16] 数字千分位
来源：http://rew.nwbrower.top

Py:   f"{1234567:,}"
来源：http://lte.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://ueh.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gqf.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kib.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nmy.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dmh.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rod.yj20258.top

C#:   1234567.ToString("N0")
来源：http://niq.shangyingyoupin.top

[E17] 首字母大写
来源：http://uku.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uft.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://den.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lku.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fqt.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fkj.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gnf.yj202588.top

Ruby: s.capitalize
来源：http://dnk.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pvn.chenlongwang.top

[E18] 模板占位符替换
来源：http://woh.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://udj.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://swr.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://ggb.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hhg.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kjs.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pgs.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cnk.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qht.tanke756.top

[E19] 多行文本按行拆分
来源：http://tlw.zycfv.cn

Py:   s.splitlines()
来源：http://rht.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gva.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://elr.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://uvt.meibo888.top

Java: s.lines().toList()
来源：http://bgq.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://rtt.ehwqpu.com

Ruby: s.lines
来源：http://ada.cashguo.top

C#:   s.Split('\n')
来源：http://weg.zycfv.cn

[E20] 判断字符串是否为空
来源：http://nmo.yj20258888.top

Py:   if not s:
来源：http://kzs.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://air.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dyi.daxiang520.top

TS:   if (s === "") {}
来源：http://mhy.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://mrv.quarkkingdee.top

Go:   if s == "" {}
来源：http://mgz.ydjk.org.cn

Ruby: if s.empty?
来源：http://srr.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://thu.hnqzz.top

[E21] 超长截断加省略号
来源：http://zyb.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nlj.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eak.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbb.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rio.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yms.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://wgr.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nsv.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qjt.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://fmz.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hui.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fmc.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aiq.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jkm.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rhe.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dtn.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://wjn.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iwq.316326.xyz

================================================================================
来源：http://irg.jiagoushi.top

F. 文件与目录
来源：http://xye.bjfxy.top

================================================================================
来源：http://sxb.xinyue.icu

[F01] 读取整个文件
来源：http://zuo.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bts.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://ykr.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lxj.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xju.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dbx.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ode.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://wds.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://wgh.yj20258.top

[F02] 逐行读取文件
来源：http://knw.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qyx.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jhf.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ufg.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dgp.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qxo.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vma.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lzf.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jfr.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://mww.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xqv.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hre.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsu.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wam.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qhg.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pvo.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://zui.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gel.haohaochexian.top

[F04] 追加写入文件
来源：http://hfi.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vuf.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fqk.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sey.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slj.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sbn.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aac.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ejg.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rkt.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://iao.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hyq.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://rse.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://wet.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://cws.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mos.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uhz.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://bds.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://gjb.wangshuangyany.cn

[F06] 删除文件
来源：http://lak.fzhhl.top

Py:   os.remove("a.txt")
来源：http://ogi.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://cyd.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mfu.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wep.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uom.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://imc.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://eiq.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://paf.daria6918.cn

[F07] 创建目录（含多级）
来源：http://cag.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://csk.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fwj.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://isx.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uli.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kfk.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://new.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://abs.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wuq.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://vbz.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mmw.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eax.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://dih.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://cou.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ohi.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://afs.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://lji.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://dot.sysykeji.top

[F09] 获取文件大小
来源：http://ugg.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://rlf.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://fga.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://aov.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://uuv.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://uvr.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hlt.xziqi.cn

Ruby: File.size("a.txt")
来源：http://svl.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://cgi.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://hil.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xlx.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tyd.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pie.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://gjz.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rei.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rrk.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yjw.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vzi.316326.xyz

[F11] 复制与移动文件
来源：http://ssa.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mwz.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://izj.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://axv.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upl.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mgt.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vrx.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whw.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pxl.tarul.cn

[F12] CSV 读写
来源：http://ryo.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lge.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jmo.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hsw.xylfe.cn

TS:   // 同上
来源：http://nye.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://frf.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uju.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vhs.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lje.xuetiantiany.cn

================================================================================
来源：http://enp.jinghuilouyu.cn

G. 面向对象
来源：http://cox.jinqigfzy.top

================================================================================
来源：http://geh.dashuyun.cn

[G01] 定义类
来源：http://rzq.shangyingyoupin.top

Py:   class User: pass
来源：http://fdl.ydzc1.top

PHP:  class User {}
来源：http://gpt.pengpengdd.cyou

JS:   class User {}
来源：http://rfd.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://zec.daria6918.cn

Java: class User {}
来源：http://gbx.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://glg.daria6918.cn

Ruby: class User; end
来源：http://dxr.kuanghao11.cn

C#:   class User {}
来源：http://rco.zdqjudy.top

[G02] 构造函数
来源：http://kuq.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://kxa.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://ign.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://byy.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://gkn.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://bpv.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gir.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://odz.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://jrq.zhengqikj.top

[G03] 实例属性
来源：http://djr.yanxiufei.cn

Py:   self.name = "x"
来源：http://wag.haohaochexian.top

PHP:  public string $name = "x";
来源：http://mcf.iojbl.cn

JS:   this.name = "x";
来源：http://vuk.chenzaomai.com

TS:   name: string = "x";
来源：http://ous.ivvv.top

Java: private String name;
来源：http://qjj.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fwb.gzhubu.top

Ruby: @name = "x"
来源：http://tov.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://lzv.hnqzz.top

[G04] 定义方法
来源：http://iwk.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://hzf.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://btk.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://icy.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://tbp.ivvv.top

Java: String greet() { return name; }
来源：http://tkv.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kzp.hcnkem.com

Ruby: def greet; @name; end
来源：http://yuw.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://icj.shanyushiyangtech.top

[G05] 继承
来源：http://yhj.cheryme.top

Py:   class Admin(User): pass
来源：http://fwc.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://kgj.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://hft.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://ucr.ctjpmb.com

Java: class Admin extends User {}
来源：http://dys.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://igt.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://qhy.ppjwa.cn

C#:   class Admin : User {}
来源：http://yqo.zhiwuduotai.top

[G06] 重写方法
来源：http://gql.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://usz.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jol.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://tbo.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://fhk.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://zon.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pvo.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://ehj.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://ozy.jqgfzy.top

[G07] 调用父类方法
来源：http://obq.chenlongwang.top

Py:   super().greet()
来源：http://bkn.c1oappe.top

PHP:  parent::greet();
来源：http://fvd.nwbrower.top

JS:   super.greet();
来源：http://xup.ehwqpu.com

TS:   super.greet();
来源：http://lrx.kuanghao11.cn

Java: super.greet();
来源：http://znq.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qyu.bjfxy.top

Ruby: super
来源：http://ecd.ydjk.org.cn

C#:   base.Greet();
来源：http://ccp.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://rma.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://egr.sufxvd.cn

PHP:  public static function f() {}
来源：http://mqw.epnwcf.com

JS:   static f() {}
来源：http://zju.cqqwz.cn

TS:   static f(): void {}
来源：http://xut.zhixingplan.top

Java: static void f() {}
来源：http://bga.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://let.chenlongwang.top

Ruby: def self.f; end
来源：http://vud.chenjidiqi.icu

C#:   public static void F() {}
来源：http://knc.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://clm.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://abm.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://hnb.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ixq.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://sbv.yvedp.cn

Java: interface Shape { double area(); }
来源：http://kou.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://qps.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yva.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://xlo.cheryme.top

[G10] 访问控制
来源：http://cgj.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://bcs.fengsongda.top

PHP:  public / protected / private
来源：http://nbn.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://rat.shanyushiyangtech.top

TS:   public / protected / private
来源：http://vbk.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://bng.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://osm.hammf.cn

Ruby: public / protected / private
来源：http://yok.sufxvd.cn

C#:   public / protected / private / internal
来源：http://zgp.cdnleiting.top

[G11] getter / setter
来源：http://zko.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://ouh.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ijf.fehbvm.com

JS:   get name() { return this._name; }
来源：http://fgh.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://idq.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://kor.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://yqb.jqgfzy.top

Ruby: attr_accessor :name
来源：http://lja.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://llm.aizwys.cn

[G12] 对象转字符串
来源：http://ffi.cashguo.top

Py:   def __str__(self): return self.name
来源：http://zzs.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sue.daria6918.cn

JS:   toString() { return this.name; }
来源：http://zob.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://qwa.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://irh.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://vwx.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://bza.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://ltv.sufxvd.cn

[G13] 判断对象类型
来源：http://zwj.xinyue.icu

Py:   isinstance(u, User)
来源：http://lbu.snrcjt.cn

PHP:  $u instanceof User
来源：http://hnk.sysykeji.top

JS:   u instanceof User
来源：http://scm.yonumen.top

TS:   u instanceof User
来源：http://dxz.vqdsnc.cn

Java: u instanceof User
来源：http://jbj.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tki.hnqzz.top

Ruby: u.is_a?(User)
来源：http://smj.fanxiaobao.xyz

C#:   u is User
来源：http://ykc.bbcook.cn


<!-- 参考信息 -->