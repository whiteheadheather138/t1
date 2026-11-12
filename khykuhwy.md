代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zxa.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://car.zhoulong.xyz

[E16] 数字千分位
来源：http://daf.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://jbd.cdnleiting.top

PHP:  number_format(1234567);
来源：http://ehb.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cvu.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pti.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gtm.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lqd.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nsk.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://wjf.daria6918.cn

[E17] 首字母大写
来源：http://kws.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ehn.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zzq.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ije.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://osw.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rid.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iua.hongshengwenyu.top

Ruby: s.capitalize
来源：http://lcu.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cfi.tarul.cn

[E18] 模板占位符替换
来源：http://kzg.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nvv.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dhe.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://otb.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://yuz.ydzc1.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ofd.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fqh.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xiq.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tqy.fengsongda.top

[E19] 多行文本按行拆分
来源：http://oxt.fktsv.cn

Py:   s.splitlines()
来源：http://idp.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gpj.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://cju.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://ftf.redwolf501.top

Java: s.lines().toList()
来源：http://ysf.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://aek.yueranfly.top

Ruby: s.lines
来源：http://ive.hcnkem.com

C#:   s.Split('\n')
来源：http://yuw.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://twn.redwolf501.top

Py:   if not s:
来源：http://xee.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://joo.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://toq.jianghu66.top

TS:   if (s === "") {}
来源：http://tvd.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://rzl.yj202588.top

Go:   if s == "" {}
来源：http://uph.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://yhw.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cyo.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://xyg.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hwm.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uis.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jxy.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mfo.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iuv.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://xni.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aht.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dkc.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://vlv.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fzt.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mgy.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zai.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zaw.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wnc.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jgj.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://yxu.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hmw.cqqwz.cn

================================================================================
来源：http://kud.zhijiandao.cn

F. 文件与目录
来源：http://gmn.shanyushiyangtech.top

================================================================================
来源：http://qep.iojbl.cn

[F01] 读取整个文件
来源：http://gak.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xoh.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://qye.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jop.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rys.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mrm.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://akg.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://zwg.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://taa.yueranfly.top

[F02] 逐行读取文件
来源：http://aqu.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rtm.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uhx.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xkn.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwm.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vex.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qfe.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://odu.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dxh.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://coi.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hge.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xfb.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvw.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://geq.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wdh.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sgf.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://epj.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oos.quarkkingdee.top

[F04] 追加写入文件
来源：http://elc.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ojz.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xnp.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dtz.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azt.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ggz.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vpn.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kwd.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://boc.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://xoc.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://drg.ivvv.top

PHP:  file_exists("a.txt");
来源：http://txi.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://wtw.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://pcg.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cpl.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hzz.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://ovh.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://mio.iojbl.cn

[F06] 删除文件
来源：http://iqz.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://ycn.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://atn.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://cgt.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://iac.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uod.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://xpu.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://slc.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://iqb.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://gih.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wvb.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xqq.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tgp.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofm.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kvd.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://khr.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jsp.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://waj.shangyingyoupin.top

[F08] 遍历目录
来源：http://uwf.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rpx.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qvr.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://ezu.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://lze.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xjx.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rfv.iojbl.cn

Ruby: Dir.children("dir")
来源：http://daw.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://aab.gzhubu.top

[F09] 获取文件大小
来源：http://cxh.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://ivk.ybcxt.top

PHP:  filesize("a.txt");
来源：http://bju.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://uio.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://nap.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ufc.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eby.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://joq.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://upl.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://gba.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qxc.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://flu.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zhm.ivvv.top

TS:   path.extname("a.txt")
来源：http://txp.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yjh.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://thi.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wgx.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ujr.hongshengwenyu.top

[F11] 复制与移动文件
来源：http://ntf.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://msh.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vou.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mwy.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dcf.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ygw.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eip.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ajx.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ams.hammf.cn

[F12] CSV 读写
来源：http://zbc.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fqu.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eqq.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hkc.dashuyun.cn

TS:   // 同上
来源：http://atm.gzhubu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lmq.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bye.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cwk.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fzq.cucudq.cn

================================================================================
来源：http://cih.ctjpmb.com

G. 面向对象
来源：http://kmx.shangyingyoupin.top

================================================================================
来源：http://aji.dashuyun.cn

[G01] 定义类
来源：http://sce.vqdsnc.cn

Py:   class User: pass
来源：http://exy.zhijiandao.cn

PHP:  class User {}
来源：http://ymk.wangshuangyany.cn

JS:   class User {}
来源：http://nzy.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://enl.pengpengdd.cyou

Java: class User {}
来源：http://ahl.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://pss.sjlbkw.cn

Ruby: class User; end
来源：http://dly.nanxinkj.top

C#:   class User {}
来源：http://khi.dianchejie.cn

[G02] 构造函数
来源：http://zzu.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://lls.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://ghz.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://bxm.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://aiw.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://vib.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ukx.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://sue.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://jyf.zhixingplan.top

[G03] 实例属性
来源：http://wie.zhijiandao.cn

Py:   self.name = "x"
来源：http://ske.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://dhl.zhiwuduotai.top

JS:   this.name = "x";
来源：http://cqt.c1oappe.top

TS:   name: string = "x";
来源：http://oyd.cheryme.top

Java: private String name;
来源：http://cng.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vnx.hywenlv.cn

Ruby: @name = "x"
来源：http://mgh.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://qys.fzhhl.top

[G04] 定义方法
来源：http://wkr.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://lvm.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qpe.fehbvm.com

JS:   greet() { return this.name; }
来源：http://apr.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://iwn.yj20258888.top

Java: String greet() { return name; }
来源：http://prg.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dap.smart0.xyz

Ruby: def greet; @name; end
来源：http://hag.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://cva.tanke756.top

[G05] 继承
来源：http://rfm.xylfe.cn

Py:   class Admin(User): pass
来源：http://nwd.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://qot.sysykeji.top

JS:   class Admin extends User {}
来源：http://ugr.iojbl.cn

TS:   class Admin extends User {}
来源：http://aux.hfpthk.cn

Java: class Admin extends User {}
来源：http://zuo.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bqm.zdqjudy.top

Ruby: class Admin < User; end
来源：http://knp.shuidangran.top

C#:   class Admin : User {}
来源：http://uet.haohaochexian.top

[G06] 重写方法
来源：http://jqy.tarul.cn

Py:   def greet(self): return "admin"
来源：http://cax.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bwa.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://hkl.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://hhr.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://kes.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zoa.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://fyz.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://oio.yj202588.top

[G07] 调用父类方法
来源：http://bmn.ydjk.org.cn

Py:   super().greet()
来源：http://wgm.zhengqikj.top

PHP:  parent::greet();
来源：http://lsi.epnwcf.com

JS:   super.greet();
来源：http://lnh.pengpengdd.cyou

TS:   super.greet();
来源：http://kwc.jianghu66.top

Java: super.greet();
来源：http://uod.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://awi.shangyingyoupin.top

Ruby: super
来源：http://uez.ivvv.top

C#:   base.Greet();
来源：http://czr.chenzaomai.com

[G08] 静态方法与属性
来源：http://qjf.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zfy.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://hzs.birdmap.top

JS:   static f() {}
来源：http://jjy.zycfv.cn

TS:   static f(): void {}
来源：http://cwo.svipenyu.cn

Java: static void f() {}
来源：http://hsx.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://dwq.pycfn.com

Ruby: def self.f; end
来源：http://vue.jyoumei.cn

C#:   public static void F() {}
来源：http://tnj.yfazqb.com

[G09] 接口 / 抽象类
来源：http://hjr.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://sam.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://poi.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jyp.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://xan.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://gxm.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://rtc.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fbk.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://wuq.52xcode.cn

[G10] 访问控制
来源：http://uqd.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://uda.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://qsl.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://acj.yuanzhike.top

TS:   public / protected / private
来源：http://pcq.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://dqi.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vhy.fehbvm.com

Ruby: public / protected / private
来源：http://dtp.52xcode.cn

C#:   public / protected / private / internal
来源：http://uop.cashguo.top

[G11] getter / setter
来源：http://hlv.gzhubu.top

Py:   @property 与 @x.setter
来源：http://npi.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://axs.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://oav.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://zxl.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://ybp.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ukb.sysykeji.top

Ruby: attr_accessor :name
来源：http://zqo.yueranfly.top

C#:   public string Name { get; set; }
来源：http://zjz.tarul.cn

[G12] 对象转字符串
来源：http://nrc.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://zsy.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ema.sweek.top

JS:   toString() { return this.name; }
来源：http://fil.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://nir.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://qqf.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://pns.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://cte.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://rrj.yuxming.cn

[G13] 判断对象类型
来源：http://ydn.yongpay.top

Py:   isinstance(u, User)
来源：http://gnf.ctjpmb.com

PHP:  $u instanceof User
来源：http://tln.xylfe.cn

JS:   u instanceof User
来源：http://air.wangshuangyany.cn

TS:   u instanceof User
来源：http://use.pengpengdd.cyou

Java: u instanceof User
来源：http://myt.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cxc.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://ukf.316326.xyz

C#:   u is User
来源：http://uky.tarul.cn

[G14] 数据类 / record
来源：http://utf.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nae.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://tbw.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://vbx.nanxinkj.top


<!-- 参考信息 -->