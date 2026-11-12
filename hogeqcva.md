代发 wailian999

[E18] 模板占位符替换
来源：http://luo.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lhj.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kim.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qoo.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qid.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qsb.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dex.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qsn.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yme.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://jmd.sysykeji.top

Py:   s.splitlines()
来源：http://uhd.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ooh.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://yxq.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://yik.xuetiantiany.cn

Java: s.lines().toList()
来源：http://wvm.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://xfx.hywenlv.cn

Ruby: s.lines
来源：http://hna.jinqigfzy.top

C#:   s.Split('\n')
来源：http://lvj.xinyue.icu

[E20] 判断字符串是否为空
来源：http://xqh.aizwys.cn

Py:   if not s:
来源：http://esa.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kre.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fkj.yj202588.top

TS:   if (s === "") {}
来源：http://ega.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://gkn.hcnkem.com

Go:   if s == "" {}
来源：http://oqy.nanxinkj.top

Ruby: if s.empty?
来源：http://nve.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ggn.tarul.cn

[E21] 超长截断加省略号
来源：http://gut.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ops.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pzi.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsa.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://krj.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ysj.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://fvo.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wfe.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tai.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://izs.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ggv.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hry.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ozp.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nte.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fpa.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jfz.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://aoh.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uob.jqgfzy.top

================================================================================
来源：http://cgs.hnxiangtu.top

F. 文件与目录
来源：http://tof.fktsv.cn

================================================================================
来源：http://qey.jiagoushi.top

[F01] 读取整个文件
来源：http://kes.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cxd.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://lvs.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mmm.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://urr.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ych.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nqf.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://rbl.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://imy.0kj1m.cn

[F02] 逐行读取文件
来源：http://log.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ynx.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rre.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jcl.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vdg.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cjl.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jgs.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dpu.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zzr.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://tdl.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jjv.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mli.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mpk.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mtw.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pkq.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xkw.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://zcg.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cgi.jinqigfzy.top

[F04] 追加写入文件
来源：http://xav.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dli.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://knt.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kao.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bzm.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://etr.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xme.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kgk.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyf.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://hrl.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sih.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://dda.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://vyv.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://obp.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yei.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iiz.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://seq.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://vhx.xuanzx.com

[F06] 删除文件
来源：http://nnh.uphjek.com

Py:   os.remove("a.txt")
来源：http://lrb.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://uzq.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://ipj.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mob.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oas.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://ifq.tarul.cn

Ruby: File.delete("a.txt")
来源：http://uds.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://ulb.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://rfj.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dyr.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hbw.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iah.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://icp.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://noo.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zga.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mui.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eml.svipenyu.cn

[F08] 遍历目录
来源：http://fqh.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wra.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oog.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://wau.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://zjm.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://chu.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://frs.redwolf501.top

Ruby: Dir.children("dir")
来源：http://kxk.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://wac.hfpthk.cn

[F09] 获取文件大小
来源：http://nbg.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://qdg.yonumen.top

PHP:  filesize("a.txt");
来源：http://sah.hnxiangtu.top

JS:   fs.statSync("a.txt").size
来源：http://asq.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://yts.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xci.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kjn.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://oda.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://eag.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://dxf.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lbb.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oyc.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lhw.zycfv.cn

TS:   path.extname("a.txt")
来源：http://dhp.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tze.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://thm.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mmn.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cox.zycfv.cn

[F11] 复制与移动文件
来源：http://vbj.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lhg.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fqt.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rqm.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nts.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vez.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tbg.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://juy.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cmc.sysykeji.top

[F12] CSV 读写
来源：http://dge.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vam.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iuo.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://icg.sysykeji.top

TS:   // 同上
来源：http://fgq.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hjh.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jph.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vdi.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nap.jiagoushi.top

================================================================================
来源：http://aqy.hnqzz.top

G. 面向对象
来源：http://qla.bjfxy.top

================================================================================
来源：http://tfk.chenjidiqi.icu

[G01] 定义类
来源：http://ufp.tanke756.top

Py:   class User: pass
来源：http://kkc.tian-w.cn

PHP:  class User {}
来源：http://snh.zdbjq.cn

JS:   class User {}
来源：http://orr.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://sxk.gaohongyu789.top

Java: class User {}
来源：http://fmb.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://pmu.sweek.top

Ruby: class User; end
来源：http://xto.wangshuangyany.cn

C#:   class User {}
来源：http://meq.nwbrower.top

[G02] 构造函数
来源：http://gln.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://qzu.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://hji.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://ejv.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://olj.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://lko.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wqi.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://fxi.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://bms.ctjpmb.com

[G03] 实例属性
来源：http://kxb.zhoulong.xyz

Py:   self.name = "x"
来源：http://fwp.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://umz.zhijiandao.cn

JS:   this.name = "x";
来源：http://iqi.nanxinkj.top

TS:   name: string = "x";
来源：http://itr.cdnleiting.top

Java: private String name;
来源：http://qxm.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hlg.birdmap.top

Ruby: @name = "x"
来源：http://zag.shangyingyoupin.top

C#:   public string Name { get; set; } = "x";
来源：http://nhe.yonumen.top

[G04] 定义方法
来源：http://poo.shuidangran.top

Py:   def greet(self): return self.name
来源：http://yeu.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sbp.cheryme.top

JS:   greet() { return this.name; }
来源：http://tgg.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://sqz.svipenyu.cn

Java: String greet() { return name; }
来源：http://siz.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://zmw.ydzc1.top

Ruby: def greet; @name; end
来源：http://zfn.fzhhl.top

C#:   public string Greet() => Name;
来源：http://lvq.hfpthk.cn

[G05] 继承
来源：http://scz.yj202588.top

Py:   class Admin(User): pass
来源：http://sbq.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://evc.yuanzhike.top

JS:   class Admin extends User {}
来源：http://dvw.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://mez.shzxlz.cn

Java: class Admin extends User {}
来源：http://mpl.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fgt.ydzc1.top

Ruby: class Admin < User; end
来源：http://gqp.fengsongda.top

C#:   class Admin : User {}
来源：http://hzt.cdnleiting.top

[G06] 重写方法
来源：http://uuq.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://trq.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xsj.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://ouc.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://qea.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://tgp.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ibj.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://sao.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://tfp.havefunace.top

[G07] 调用父类方法
来源：http://ewj.jinqigufen.top

Py:   super().greet()
来源：http://cis.jianghu66.top

PHP:  parent::greet();
来源：http://wxv.xziqi.cn

JS:   super.greet();
来源：http://crh.ehwqpu.com

TS:   super.greet();
来源：http://lro.sufxvd.cn

Java: super.greet();
来源：http://zxk.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://edx.fzhhl.top

Ruby: super
来源：http://hhe.dianchejie.cn

C#:   base.Greet();
来源：http://nns.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://sfj.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ecj.0kj1m.cn

PHP:  public static function f() {}
来源：http://cvz.shanyushiyangtech.top

JS:   static f() {}
来源：http://kkv.gogol.net.cn

TS:   static f(): void {}
来源：http://gau.tian-w.cn

Java: static void f() {}
来源：http://fbu.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ksm.gotoacloud.top

Ruby: def self.f; end
来源：http://puf.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://jmn.daxiang520.top

[G09] 接口 / 抽象类
来源：http://yxb.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://oml.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://kvt.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gdo.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://lgz.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://gry.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fnk.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kbt.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://vqk.cucudq.cn

[G10] 访问控制
来源：http://gre.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://rtu.jiagoushi.top

PHP:  public / protected / private
来源：http://asz.yongpay.top

JS:   #private 字段；其余公开
来源：http://zjr.wangdashe.top

TS:   public / protected / private
来源：http://tee.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://jla.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yzz.chenzaomai.com

Ruby: public / protected / private
来源：http://tkz.tanke756.top

C#:   public / protected / private / internal
来源：http://aks.ctjpmb.com

[G11] getter / setter
来源：http://yre.ydzc1.top

Py:   @property 与 @x.setter
来源：http://wxo.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xro.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://rjn.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://chk.ehwqpu.com

Java: public String getName() { return name; }
来源：http://nef.chenzaomai.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dsp.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://foq.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://bau.fengsongda.top

[G12] 对象转字符串
来源：http://blq.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://jgr.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://csj.sysykeji.top

JS:   toString() { return this.name; }
来源：http://ktf.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://ykk.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://skl.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://qyj.fengsongda.top

Ruby: def to_s; @name; end
来源：http://uxq.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://kdu.chenjidiqi.icu

[G13] 判断对象类型
来源：http://ghs.svipenyu.cn

Py:   isinstance(u, User)
来源：http://nbd.gzhubu.top

PHP:  $u instanceof User
来源：http://xoi.zycfv.cn

JS:   u instanceof User
来源：http://spk.ctjpmb.com

TS:   u instanceof User
来源：http://nna.fehbvm.com

Java: u instanceof User
来源：http://rnk.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://igy.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://amz.kuanghao11.cn

C#:   u is User
来源：http://ixr.haohaochexian.top

[G14] 数据类 / record
来源：http://qbk.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sae.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://cze.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://nki.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://zkl.yj20258888.top

Java: record User(String name, int age) {}
来源：http://rmy.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://wno.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qob.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://kpo.yueranfly.top

[G15] 枚举
来源：http://qym.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lsa.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lxt.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nbz.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://krz.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://gnd.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ytx.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://pyd.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ove.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://asq.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ngs.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://irw.316326.xyz

JS:   Object.entries(obj)
来源：http://pzi.hcnkem.com

TS:   Object.entries(obj)
来源：http://wvp.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wjs.xuetiantiany.cn


<!-- 参考信息 -->