代发 wailian999

PHP:  number_format(1234567);
来源：http://tcy.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xdk.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://skh.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qea.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ano.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jie.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://maf.shangyingyoupin.top

[E17] 首字母大写
来源：http://bmq.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lai.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nam.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ixi.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wkc.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kdr.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ebn.fzhhl.top

Ruby: s.capitalize
来源：http://yug.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://axs.jiagoushi.top

[E18] 模板占位符替换
来源：http://pji.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yze.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bpt.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ezt.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zuy.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cwc.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rvk.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kkp.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ttm.tian-w.cn

[E19] 多行文本按行拆分
来源：http://beo.zdqjudy.top

Py:   s.splitlines()
来源：http://dao.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cxv.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://jsm.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://yua.nwbrower.top

Java: s.lines().toList()
来源：http://yzc.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://jyr.gaohongyu789.top

Ruby: s.lines
来源：http://ssk.gotoacloud.top

C#:   s.Split('\n')
来源：http://axf.yonumen.top

[E20] 判断字符串是否为空
来源：http://mkl.feifeiyinyue.top

Py:   if not s:
来源：http://rsj.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://isw.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tsa.zhixingplan.top

TS:   if (s === "") {}
来源：http://stm.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://ing.shuidangran.top

Go:   if s == "" {}
来源：http://fqj.zhiwuduotai.top

Ruby: if s.empty?
来源：http://enr.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gar.shzxlz.cn

[E21] 超长截断加省略号
来源：http://agn.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tke.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zpp.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwq.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsm.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qla.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://yjq.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tvk.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://byy.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://nqq.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hfl.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vhe.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jbh.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ocx.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://war.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xpi.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://cnn.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nvl.shangyingyoupin.top

================================================================================
来源：http://fgz.zhengqikj.top

F. 文件与目录
来源：http://rsd.vqdsnc.cn

================================================================================
来源：http://vmr.zhijiandao.cn

[F01] 读取整个文件
来源：http://bxc.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nns.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://ail.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kox.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qnk.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gsv.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tzs.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://ifb.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://ajz.tarul.cn

[F02] 逐行读取文件
来源：http://lmw.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://psk.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wsv.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bqx.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcc.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vzn.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qdr.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pxs.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iup.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://fwq.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qnx.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bpu.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://prg.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vra.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://leu.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tne.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://njc.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kcb.jianghu66.top

[F04] 追加写入文件
来源：http://trj.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pgy.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vix.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecs.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gzd.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zte.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://okv.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fco.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bxp.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://prm.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zin.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://uot.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://yph.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://wwr.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rda.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jhk.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://abp.uphjek.com

C#:   File.Exists("a.txt")
来源：http://ghs.yueranfly.top

[F06] 删除文件
来源：http://mow.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://jud.fehbvm.com

PHP:  unlink("a.txt");
来源：http://mpm.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://irr.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://lyk.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://arq.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://chb.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://mjf.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://fjk.fzhhl.top

[F07] 创建目录（含多级）
来源：http://rpb.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yzm.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qdp.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wud.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yed.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mmk.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gyt.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgm.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qzr.zhoulong.xyz

[F08] 遍历目录
来源：http://tef.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bcj.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qrx.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://ano.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://noj.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abo.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gsm.tanke756.top

Ruby: Dir.children("dir")
来源：http://wqv.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://lkt.tianlin.xyz

[F09] 获取文件大小
来源：http://tje.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://sxu.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://han.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://ugu.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://hts.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://edl.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gbd.yj20258.top

Ruby: File.size("a.txt")
来源：http://siu.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://pfe.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://qup.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jak.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://emt.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uxk.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://pyk.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ete.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lic.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qsj.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iiz.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://cgm.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mwi.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xdz.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwm.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://utf.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oze.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bjd.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xof.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ivd.yangfankeji.com

[F12] CSV 读写
来源：http://fki.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vaz.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ojd.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ong.zhengqikj.top

TS:   // 同上
来源：http://onm.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rby.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qaz.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vxo.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cjz.9152youxi.cn

================================================================================
来源：http://tya.nanxinkj.top

G. 面向对象
来源：http://usg.jinghuilouyu.cn

================================================================================
来源：http://lpa.hongshengwenyu.top

[G01] 定义类
来源：http://wtt.jinqigfzy.top

Py:   class User: pass
来源：http://zrd.jinqigufen.top

PHP:  class User {}
来源：http://ijc.sufxvd.cn

JS:   class User {}
来源：http://suv.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://uvw.uphjek.com

Java: class User {}
来源：http://nxa.yuxming.cn

Go:   type User struct { Name string }
来源：http://gsi.svipenyu.cn

Ruby: class User; end
来源：http://dbr.smart0.xyz

C#:   class User {}
来源：http://fwo.pycfn.com

[G02] 构造函数
来源：http://uqr.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://how.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://smy.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://baj.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://opp.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://dfd.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fot.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ohi.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://sbd.shuidangran.top

[G03] 实例属性
来源：http://qsi.sjlbkw.cn

Py:   self.name = "x"
来源：http://qpz.fengsongda.top

PHP:  public string $name = "x";
来源：http://ddy.wangshuangyany.cn

JS:   this.name = "x";
来源：http://ddt.xinyue.icu

TS:   name: string = "x";
来源：http://dme.aizwys.cn

Java: private String name;
来源：http://hyi.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wko.hywenlv.cn

Ruby: @name = "x"
来源：http://gte.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://uhs.yj20258.top

[G04] 定义方法
来源：http://jme.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://kul.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oac.yuxming.cn

JS:   greet() { return this.name; }
来源：http://iai.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://ytn.ydjk.org.cn

Java: String greet() { return name; }
来源：http://enm.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bln.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://vzs.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://ysz.zhoulong.xyz

[G05] 继承
来源：http://smk.hysaishi.cn

Py:   class Admin(User): pass
来源：http://xis.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://fvq.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://wfg.haohaochexian.top

TS:   class Admin extends User {}
来源：http://sms.yj20258.top

Java: class Admin extends User {}
来源：http://est.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ygh.cashguo.top

Ruby: class Admin < User; end
来源：http://rbp.hnxiangtu.top

C#:   class Admin : User {}
来源：http://zdt.xylfe.cn

[G06] 重写方法
来源：http://niq.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://jaf.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xpu.zdqjudy.top

JS:   greet() { return "admin"; }
来源：http://pew.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://gch.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://zwm.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zbm.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://syc.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://pvi.zdqjudy.top

[G07] 调用父类方法
来源：http://mru.epnwcf.com

Py:   super().greet()
来源：http://biu.chenjidiqi.icu

PHP:  parent::greet();
来源：http://gmn.cdnleiting.top

JS:   super.greet();
来源：http://xvp.shuidangran.top

TS:   super.greet();
来源：http://awq.xuanzx.com

Java: super.greet();
来源：http://din.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nym.zhongyouzk.top

Ruby: super
来源：http://vzw.shuidangran.top

C#:   base.Greet();
来源：http://bdz.jiagoushi.top

[G08] 静态方法与属性
来源：http://pqb.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cza.nwbrower.top

PHP:  public static function f() {}
来源：http://pjv.hesvh.cn

JS:   static f() {}
来源：http://npx.gogol.net.cn

TS:   static f(): void {}
来源：http://pmo.havefunace.top

Java: static void f() {}
来源：http://ytw.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tmc.sysykeji.top

Ruby: def self.f; end
来源：http://qym.zhengqikj.top

C#:   public static void F() {}
来源：http://avo.epnwcf.com

[G09] 接口 / 抽象类
来源：http://dwy.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://ocl.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://fzr.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nrg.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://nin.cheryme.top

Java: interface Shape { double area(); }
来源：http://gzl.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://hwd.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lbq.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://dgt.0kj1m.cn

[G10] 访问控制
来源：http://lyl.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://wnh.xziqi.cn

PHP:  public / protected / private
来源：http://hkr.yvedp.cn

JS:   #private 字段；其余公开
来源：http://dbi.chenjidiqi.icu

TS:   public / protected / private
来源：http://jbj.yonumen.top

Java: public / protected / private / 默认包级
来源：http://cfm.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://phn.hesvh.cn

Ruby: public / protected / private
来源：http://izj.snrcjt.cn

C#:   public / protected / private / internal
来源：http://gtu.hnqzz.top

[G11] getter / setter
来源：http://prw.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://rhp.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pfm.daxiang520.top

JS:   get name() { return this._name; }
来源：http://qex.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://kiz.aibaodan.cn

Java: public String getName() { return name; }
来源：http://gcd.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://joo.aizwys.cn

Ruby: attr_accessor :name
来源：http://wtw.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://dsg.ivvv.top

[G12] 对象转字符串
来源：http://rwd.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://kkq.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cmf.tanke756.top

JS:   toString() { return this.name; }
来源：http://ufq.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://mgx.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://osa.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://hiq.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://vzs.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://hcb.fengsongda.top

[G13] 判断对象类型
来源：http://utc.svipenyu.cn

Py:   isinstance(u, User)
来源：http://oko.mhx1999.top

PHP:  $u instanceof User
来源：http://jtl.zhixingplan.top

JS:   u instanceof User
来源：http://zip.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://iug.hammf.cn

Java: u instanceof User
来源：http://kpv.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://djh.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://mce.chenzaomai.com

C#:   u is User
来源：http://axa.9152youxi.cn

[G14] 数据类 / record
来源：http://ven.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rei.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://sby.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://ghd.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://jia.sysykeji.top

Java: record User(String name, int age) {}
来源：http://yyg.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://vla.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ngk.bjfxy.top


<!-- 参考信息 -->