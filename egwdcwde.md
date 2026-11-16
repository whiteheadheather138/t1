代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bwt.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cov.nwbrower.top

[E16] 数字千分位
来源：http://xaj.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://rql.0kj1m.cn

PHP:  number_format(1234567);
来源：http://gbd.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pag.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hri.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://obo.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dad.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ies.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://who.yuxming.cn

[E17] 首字母大写
来源：http://bov.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xfn.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vom.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://awl.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jmg.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zqf.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ewb.hnxiangtu.top

Ruby: s.capitalize
来源：http://vwr.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jnn.jqgfzy.top

[E18] 模板占位符替换
来源：http://jnj.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://elq.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zwg.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wjs.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ejd.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uir.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://trj.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uan.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zab.aizwys.cn

[E19] 多行文本按行拆分
来源：http://gdh.yj20258.top

Py:   s.splitlines()
来源：http://okr.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wce.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://adq.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://wmj.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://lyf.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://swi.andypj.xyz

Ruby: s.lines
来源：http://sxd.c1oappe.top

C#:   s.Split('\n')
来源：http://igy.redwolf501.top

[E20] 判断字符串是否为空
来源：http://wgo.haohaochexian.top

Py:   if not s:
来源：http://zvx.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qtp.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sza.yueranfly.top

TS:   if (s === "") {}
来源：http://pqb.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://lhk.yonumen.top

Go:   if s == "" {}
来源：http://qns.yj202588.top

Ruby: if s.empty?
来源：http://bwr.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dgt.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://lqw.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zqt.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fid.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zce.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fwf.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cre.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://mup.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vzz.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xyt.52xcode.cn

[E22] 字节长度与字符长度
来源：http://qel.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://smq.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fer.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zqh.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvt.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ekm.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://syu.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://qhp.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wxn.guannengcc.top

================================================================================
来源：http://mdp.pycfn.com

F. 文件与目录
来源：http://nxe.yanxiufei.cn

================================================================================
来源：http://prn.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://kox.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qqb.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://lqz.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yaz.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lef.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qln.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ieh.andypj.xyz

Ruby: File.read("a.txt")
来源：http://fhe.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://qut.ehwqpu.com

[F02] 逐行读取文件
来源：http://str.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dop.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nkg.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pcn.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcd.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oyp.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wqc.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jhj.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uoh.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://ghf.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xnr.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nxh.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://twe.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uyc.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://stv.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cim.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://fkg.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gja.sjlbkw.cn

[F04] 追加写入文件
来源：http://hob.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rnt.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wpv.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyb.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kbe.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sir.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ojy.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ube.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dex.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://fuc.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bxe.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://ojg.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://cbp.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://ftc.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://piq.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wbw.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://sgc.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://ody.hammf.cn

[F06] 删除文件
来源：http://nvj.iojbl.cn

Py:   os.remove("a.txt")
来源：http://vdz.hnqzz.top

PHP:  unlink("a.txt");
来源：http://ofj.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://hbw.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mgb.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pqa.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://jqm.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://spv.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://txl.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://rjt.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lsw.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mfl.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzm.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgu.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fdo.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mff.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dpx.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://llg.fktsv.cn

[F08] 遍历目录
来源：http://ffy.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jqq.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufh.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://ldh.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://ihd.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rpx.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://aic.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://gpw.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://nfl.guowangkeji.top

[F09] 获取文件大小
来源：http://zhi.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://loq.xinyue.icu

PHP:  filesize("a.txt");
来源：http://nhl.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://vbn.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://otl.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jst.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hht.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://pic.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://ajs.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://cca.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://win.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pew.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gfr.hammf.cn

TS:   path.extname("a.txt")
来源：http://tyo.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ynh.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wxx.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fjr.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gzz.yj202588.top

[F11] 复制与移动文件
来源：http://wnm.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mvu.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ghs.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qlf.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://apo.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ugx.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mdx.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aaw.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ebs.yj20258888.top

[F12] CSV 读写
来源：http://saq.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://koc.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ztu.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jpn.ydjk.org.cn

TS:   // 同上
来源：http://wnk.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://atx.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pei.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cyb.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yxz.gotoacloud.top

================================================================================
来源：http://jgb.hnxiangtu.top

G. 面向对象
来源：http://amg.ybcxt.top

================================================================================
来源：http://tyl.sweek.top

[G01] 定义类
来源：http://vkl.jianghu66.top

Py:   class User: pass
来源：http://hzi.hammf.cn

PHP:  class User {}
来源：http://rae.pycfn.com

JS:   class User {}
来源：http://bgt.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://wsy.cheryme.top

Java: class User {}
来源：http://pbu.gzhubu.top

Go:   type User struct { Name string }
来源：http://hzc.fengsongda.top

Ruby: class User; end
来源：http://unv.cashguo.top

C#:   class User {}
来源：http://tdb.kuanghao11.cn

[G02] 构造函数
来源：http://ecj.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://cxj.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://cqc.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://sqi.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://dxb.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://vbx.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hqw.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://whf.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://mzp.iojbl.cn

[G03] 实例属性
来源：http://mzy.sufxvd.cn

Py:   self.name = "x"
来源：http://gbq.shuidangran.top

PHP:  public string $name = "x";
来源：http://wbt.xuetiantiany.cn

JS:   this.name = "x";
来源：http://xwj.yvedp.cn

TS:   name: string = "x";
来源：http://qth.xziqi.cn

Java: private String name;
来源：http://vyh.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gha.shzxlz.cn

Ruby: @name = "x"
来源：http://koq.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://kal.xinyue.icu

[G04] 定义方法
来源：http://mes.daxiang520.top

Py:   def greet(self): return self.name
来源：http://arq.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uzi.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://tsp.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://wte.kuanghao11.cn

Java: String greet() { return name; }
来源：http://faf.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ydm.bjfxy.top

Ruby: def greet; @name; end
来源：http://fjx.daria6918.cn

C#:   public string Greet() => Name;
来源：http://jug.9152youxi.cn

[G05] 继承
来源：http://liz.9152youxi.cn

Py:   class Admin(User): pass
来源：http://trb.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://lpx.aibaodan.cn

JS:   class Admin extends User {}
来源：http://mjg.nwbrower.top

TS:   class Admin extends User {}
来源：http://wfk.zdbjq.cn

Java: class Admin extends User {}
来源：http://dvg.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qgf.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://coq.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://xvs.ydjk.org.cn

[G06] 重写方法
来源：http://yns.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://iku.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lce.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://yrc.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://elx.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://huv.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uwy.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://pbj.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://rcx.cdnleiting.top

[G07] 调用父类方法
来源：http://ayh.guowangkeji.top

Py:   super().greet()
来源：http://gru.yanxiufei.cn

PHP:  parent::greet();
来源：http://mkq.fengsongda.top

JS:   super.greet();
来源：http://ohb.birdmap.top

TS:   super.greet();
来源：http://one.kuanghao11.cn

Java: super.greet();
来源：http://xhx.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://umd.haohaochexian.top

Ruby: super
来源：http://ibu.pycfn.com

C#:   base.Greet();
来源：http://agt.yanxiufei.cn

[G08] 静态方法与属性
来源：http://owm.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eph.nwbrower.top

PHP:  public static function f() {}
来源：http://joh.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://kmh.redwolf501.top

TS:   static f(): void {}
来源：http://jcp.feifeiyinyue.top

Java: static void f() {}
来源：http://ysz.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ugt.316326.xyz

Ruby: def self.f; end
来源：http://xcg.pengpengdd.cyou

C#:   public static void F() {}
来源：http://pnq.aizwys.cn

[G09] 接口 / 抽象类
来源：http://dgw.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://qjd.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://wot.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ece.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://pei.sxryk.cn

Java: interface Shape { double area(); }
来源：http://ijt.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://mbx.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mpc.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://swr.kuanghao11.cn

[G10] 访问控制
来源：http://rcw.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://lfj.sweek.top

PHP:  public / protected / private
来源：http://ewa.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://jxy.zycfv.cn

TS:   public / protected / private
来源：http://urp.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://dtf.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://euv.gaohongyu789.top

Ruby: public / protected / private
来源：http://grw.wangdashe.top

C#:   public / protected / private / internal
来源：http://vmg.xinyue.icu

[G11] getter / setter
来源：http://fep.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://kdj.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qcn.hesvh.cn

JS:   get name() { return this._name; }
来源：http://czf.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://kqm.jianghu66.top

Java: public String getName() { return name; }
来源：http://drk.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pth.uphjek.com

Ruby: attr_accessor :name
来源：http://mjb.fehbvm.com

C#:   public string Name { get; set; }
来源：http://buo.yangfankeji.com

[G12] 对象转字符串
来源：http://peh.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://krp.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://hdf.yj20258.top

JS:   toString() { return this.name; }
来源：http://xqq.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://rtg.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://eyb.pengpengdd.cyou

Go:   func (u User) String() string { return u.Name }
来源：http://yfd.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://pkc.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://dad.hywenlv.cn

[G13] 判断对象类型
来源：http://gdx.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://lpj.52xcode.cn

PHP:  $u instanceof User
来源：http://ken.jinqigfzy.top

JS:   u instanceof User
来源：http://ehy.cqqwz.cn

TS:   u instanceof User
来源：http://gkp.hysaishi.cn

Java: u instanceof User
来源：http://tja.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hup.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://fug.cqqwz.cn

C#:   u is User
来源：http://kaz.9152youxi.cn

[G14] 数据类 / record
来源：http://yzt.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ybg.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://ejr.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://ntd.wangdashe.top


<!-- 参考信息 -->