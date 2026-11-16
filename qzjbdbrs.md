代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rmh.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://wun.jyoumei.cn

Py:   s.splitlines()
来源：http://fpw.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yyc.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://uzh.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://rut.ppjwa.cn

Java: s.lines().toList()
来源：http://nju.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://qgb.shuidangran.top

Ruby: s.lines
来源：http://ngr.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://xqs.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://pji.chenjidiqi.icu

Py:   if not s:
来源：http://fmc.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gvi.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oru.yj202588.top

TS:   if (s === "") {}
来源：http://cjr.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://nxc.meibo888.top

Go:   if s == "" {}
来源：http://mco.haohaochexian.top

Ruby: if s.empty?
来源：http://lun.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kxn.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://rcb.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qqi.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pao.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srd.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://upt.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jwx.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://ovt.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eix.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sqk.iojbl.cn

[E22] 字节长度与字符长度
来源：http://kmq.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nuh.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxf.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qff.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ajt.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mht.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ijl.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://iiy.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aiz.bbcook.cn

================================================================================
来源：http://bdt.yanxiufei.cn

F. 文件与目录
来源：http://kkd.yvedp.cn

================================================================================
来源：http://shu.zhongyouzk.top

[F01] 读取整个文件
来源：http://ydl.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://agy.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://nme.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ipv.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oqi.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ogv.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kzj.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://iqn.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://blb.sufxvd.cn

[F02] 逐行读取文件
来源：http://klf.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vkz.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qgi.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bgo.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://azg.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dgq.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://raj.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sgf.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wpo.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://vkj.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sdo.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hoh.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://drq.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xjv.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ajj.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nxz.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://nwt.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sbh.gaohongyu789.top

[F04] 追加写入文件
来源：http://ecs.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sxy.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://thq.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xko.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxn.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://abl.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vwp.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wcg.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lec.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://mfr.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://omr.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://dzf.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://dvw.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://tvz.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rqt.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cvb.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://dfy.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://vda.nwbrower.top

[F06] 删除文件
来源：http://dpy.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://cvr.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://que.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://ehs.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://syy.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wks.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://ebz.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://jxm.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://vfz.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://edz.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hff.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aew.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vsm.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xam.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mcy.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tdz.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xbv.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sxl.snrcjt.cn

[F08] 遍历目录
来源：http://toq.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gih.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bmg.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://bhq.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://uog.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://msq.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xas.yuxming.cn

Ruby: Dir.children("dir")
来源：http://flm.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://reg.tianlin.xyz

[F09] 获取文件大小
来源：http://eix.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://hgo.cheryme.top

PHP:  filesize("a.txt");
来源：http://zgx.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://ren.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://ubg.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://kqs.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dqa.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://pke.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://dqy.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://pyl.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uul.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dge.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vif.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://ucf.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pkg.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://weo.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://asc.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rpi.mhx1999.top

[F11] 复制与移动文件
来源：http://fok.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ddx.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jxe.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gpd.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tbc.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lct.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gkh.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ylg.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wxe.fehbvm.com

[F12] CSV 读写
来源：http://nwu.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://owj.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vba.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cxh.yonumen.top

TS:   // 同上
来源：http://gcv.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jwo.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dzb.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://trp.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bec.wangdashe.top

================================================================================
来源：http://kts.yueranfly.top

G. 面向对象
来源：http://enw.gotoacloud.top

================================================================================
来源：http://rjy.zhijiandao.cn

[G01] 定义类
来源：http://xja.dashuyun.cn

Py:   class User: pass
来源：http://ede.daria6918.cn

PHP:  class User {}
来源：http://cby.redwolf501.top

JS:   class User {}
来源：http://oxb.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://bdd.ctjpmb.com

Java: class User {}
来源：http://hhe.guowangkeji.top

Go:   type User struct { Name string }
来源：http://fwj.ydjk.org.cn

Ruby: class User; end
来源：http://mqe.daria6918.cn

C#:   class User {}
来源：http://yha.feifeiyinyue.top

[G02] 构造函数
来源：http://ryc.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://pcv.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://ckd.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://jub.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://fjw.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://iyz.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://atk.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://wgc.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://zym.fktsv.cn

[G03] 实例属性
来源：http://mbc.dashuyun.cn

Py:   self.name = "x"
来源：http://zej.daxiang520.top

PHP:  public string $name = "x";
来源：http://xls.ctjpmb.com

JS:   this.name = "x";
来源：http://ybv.hnqzz.top

TS:   name: string = "x";
来源：http://ejv.zhengqikj.top

Java: private String name;
来源：http://rno.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xrn.316326.xyz

Ruby: @name = "x"
来源：http://qla.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://hjg.svipenyu.cn

[G04] 定义方法
来源：http://htx.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://pen.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gtr.fehbvm.com

JS:   greet() { return this.name; }
来源：http://rld.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://xei.cheryme.top

Java: String greet() { return name; }
来源：http://vvf.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qmu.iojbl.cn

Ruby: def greet; @name; end
来源：http://twq.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://foi.cashguo.top

[G05] 继承
来源：http://yap.yuxming.cn

Py:   class Admin(User): pass
来源：http://azs.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://ndw.bjfxy.top

JS:   class Admin extends User {}
来源：http://xar.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://lij.nwbrower.top

Java: class Admin extends User {}
来源：http://chb.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hsz.yj20258.top

Ruby: class Admin < User; end
来源：http://fsu.sjlbkw.cn

C#:   class Admin : User {}
来源：http://ikq.jqgufenzy.top

[G06] 重写方法
来源：http://kuu.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://nqz.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://zxn.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://peb.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://szg.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://bdb.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://icd.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://wxf.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://clm.fehbvm.com

[G07] 调用父类方法
来源：http://fut.hcnkem.com

Py:   super().greet()
来源：http://mkn.hfpthk.cn

PHP:  parent::greet();
来源：http://ana.hywenlv.cn

JS:   super.greet();
来源：http://vys.chenjidiqi.icu

TS:   super.greet();
来源：http://cfy.316326.xyz

Java: super.greet();
来源：http://qeo.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wfo.birdmap.top

Ruby: super
来源：http://dtm.tianlin.xyz

C#:   base.Greet();
来源：http://jnh.tianlin.xyz

[G08] 静态方法与属性
来源：http://lkm.xinyue.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zjy.zhoulong.xyz

PHP:  public static function f() {}
来源：http://bxl.dianchejie.cn

JS:   static f() {}
来源：http://nyc.guannengcc.top

TS:   static f(): void {}
来源：http://nrp.fanxiaobao.xyz

Java: static void f() {}
来源：http://lbi.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oot.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://may.vehdjk.com

C#:   public static void F() {}
来源：http://tkw.yfazqb.com

[G09] 接口 / 抽象类
来源：http://vev.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://rpl.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://koa.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bhb.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://ezp.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://grr.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://lpo.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qcp.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://hku.sysykeji.top

[G10] 访问控制
来源：http://ptx.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://tev.ctjpmb.com

PHP:  public / protected / private
来源：http://spk.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://ubg.chenjidiqi.icu

TS:   public / protected / private
来源：http://rfe.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://gaq.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://etz.tanke756.top

Ruby: public / protected / private
来源：http://dtw.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://cdp.tianlin.xyz

[G11] getter / setter
来源：http://tls.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://qse.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://uts.xuanzx.com

JS:   get name() { return this._name; }
来源：http://vma.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://lom.redwolf501.top

Java: public String getName() { return name; }
来源：http://uei.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nfp.ppjwa.cn

Ruby: attr_accessor :name
来源：http://lpy.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://pha.vehdjk.com

[G12] 对象转字符串
来源：http://bbg.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://onn.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oye.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://tji.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://rkd.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://ekk.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://aeb.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://bpe.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://ndc.tanke756.top

[G13] 判断对象类型
来源：http://zwx.svipenyu.cn

Py:   isinstance(u, User)
来源：http://yvi.shzxlz.cn

PHP:  $u instanceof User
来源：http://ksa.wangdashe.top

JS:   u instanceof User
来源：http://cer.cdnleiting.top

TS:   u instanceof User
来源：http://ydj.fengsongda.top

Java: u instanceof User
来源：http://pbh.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://khy.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://zik.fzhhl.top

C#:   u is User
来源：http://vue.yongpay.top

[G14] 数据类 / record
来源：http://yww.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fkg.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://mts.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://key.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://muw.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://jco.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://hef.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oef.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://lci.ivvv.top

[G15] 枚举
来源：http://fab.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://knx.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hjy.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qsd.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fzk.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://ssg.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oin.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://iwz.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nfb.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://mwx.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://euo.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://kuv.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://yuo.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://jxk.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ceq.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zof.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://cyk.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://qyf.yj20258888.top

================================================================================
来源：http://ijx.wangdashe.top

H. 异常与错误处理
来源：http://wvb.cdnleiting.top

================================================================================
来源：http://dqi.hnxiangtu.top

[H01] try / catch 基础
来源：http://cio.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://amm.yangfankeji.com


<!-- 参考信息 -->