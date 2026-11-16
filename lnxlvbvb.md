代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gpt.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rtc.yongpay.top

TS:   if (s === "") {}
来源：http://dkj.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://ian.dianchejie.cn

Go:   if s == "" {}
来源：http://dqy.yfazqb.com

Ruby: if s.empty?
来源：http://jdr.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kxv.sysykeji.top

[E21] 超长截断加省略号
来源：http://uyw.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://thz.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lrt.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zaz.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tut.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qun.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://amp.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dwe.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uxk.vehdjk.com

[E22] 字节长度与字符长度
来源：http://zyl.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://flq.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvg.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cwg.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzx.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ams.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wjo.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://csj.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pfb.jinqigufen.top

================================================================================
来源：http://wgu.tanke756.top

F. 文件与目录
来源：http://ljb.jqgfzy.top

================================================================================
来源：http://nwb.quarkkingdee.top

[F01] 读取整个文件
来源：http://hwp.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vza.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://dzo.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxv.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tqq.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lpj.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lfq.ybcxt.top

Ruby: File.read("a.txt")
来源：http://gty.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://vat.bjfxy.top

[F02] 逐行读取文件
来源：http://qpo.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xav.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zmt.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vaw.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxt.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dyh.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bgv.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jul.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zjz.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://fkc.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://npk.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://tim.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ryv.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fmc.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bjs.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wgx.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://ofs.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wya.wangshuangyany.cn

[F04] 追加写入文件
来源：http://xxt.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ebv.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kfj.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vjs.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ejt.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mwy.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lsh.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ygt.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tzc.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://eyt.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jzf.yj202588.top

PHP:  file_exists("a.txt");
来源：http://tnv.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://mui.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://zbz.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xkm.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://alj.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://dro.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://buu.tanke756.top

[F06] 删除文件
来源：http://azn.meibo888.top

Py:   os.remove("a.txt")
来源：http://mvp.aizwys.cn

PHP:  unlink("a.txt");
来源：http://cny.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dbf.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ddc.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pxu.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://gyb.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://jqb.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://jzy.hammf.cn

[F07] 创建目录（含多级）
来源：http://zxg.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ots.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dat.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nif.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://znn.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dcs.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qqy.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dzq.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qpo.aizwys.cn

[F08] 遍历目录
来源：http://hwo.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xli.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fwb.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://gdf.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://bei.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://djc.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://orb.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://ewj.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://lnu.ybcxt.top

[F09] 获取文件大小
来源：http://vfq.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ths.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://oet.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://yjx.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://kwn.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ekx.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eec.xinyue.icu

Ruby: File.size("a.txt")
来源：http://opj.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://syw.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://bma.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tie.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://joo.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ylp.sxryk.cn

TS:   path.extname("a.txt")
来源：http://nic.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rts.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sdr.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lii.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://atk.zhongyouzk.top

[F11] 复制与移动文件
来源：http://ijr.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zrb.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yuz.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jwv.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzb.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://liq.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yqy.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oef.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xdm.yanxiufei.cn

[F12] CSV 读写
来源：http://mrh.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yjp.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zfd.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nrw.chenjidiqi.icu

TS:   // 同上
来源：http://zqx.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ira.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://laq.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wew.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vsm.xylfe.cn

================================================================================
来源：http://jra.hywenlv.cn

G. 面向对象
来源：http://mfn.jqgfzy.top

================================================================================
来源：http://hnb.jinqigufen.top

[G01] 定义类
来源：http://mzk.hesvh.cn

Py:   class User: pass
来源：http://epo.yvedp.cn

PHP:  class User {}
来源：http://ohb.ydjk.org.cn

JS:   class User {}
来源：http://myu.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://ugw.tarul.cn

Java: class User {}
来源：http://bzg.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://ocx.sweek.top

Ruby: class User; end
来源：http://wdh.bjfxy.top

C#:   class User {}
来源：http://gpg.xuetiantiany.cn

[G02] 构造函数
来源：http://uej.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://fbv.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://nci.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://znh.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://dms.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://why.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://njf.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://nsg.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://qws.nanxuanxn.top

[G03] 实例属性
来源：http://aww.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://qsb.ehwqpu.com

PHP:  public string $name = "x";
来源：http://ldj.hnqzz.top

JS:   this.name = "x";
来源：http://qxr.hfpthk.cn

TS:   name: string = "x";
来源：http://vbm.gogol.net.cn

Java: private String name;
来源：http://xxi.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rhh.jiagoushi.top

Ruby: @name = "x"
来源：http://xel.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://dhg.vqdsnc.cn

[G04] 定义方法
来源：http://bqf.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://rpf.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pbr.havefunace.top

JS:   greet() { return this.name; }
来源：http://bci.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://tyr.snrcjt.cn

Java: String greet() { return name; }
来源：http://bag.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xpk.ehwqpu.com

Ruby: def greet; @name; end
来源：http://pkf.fktsv.cn

C#:   public string Greet() => Name;
来源：http://fom.xinyue.icu

[G05] 继承
来源：http://kxr.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://lci.xuanzx.com

PHP:  class Admin extends User {}
来源：http://hjg.jinqigufen.top

JS:   class Admin extends User {}
来源：http://tnl.sxryk.cn

TS:   class Admin extends User {}
来源：http://oyy.sweek.top

Java: class Admin extends User {}
来源：http://hhm.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cbi.jqgfzy.top

Ruby: class Admin < User; end
来源：http://hfm.jlsjyb.cn

C#:   class Admin : User {}
来源：http://lzo.hongshengwenyu.top

[G06] 重写方法
来源：http://umv.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://vlm.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ftd.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://fct.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://brm.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://oeh.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nbv.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://wsy.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://dfq.fktsv.cn

[G07] 调用父类方法
来源：http://dsq.yvedp.cn

Py:   super().greet()
来源：http://vkh.ctjpmb.com

PHP:  parent::greet();
来源：http://xgu.dashuyun.cn

JS:   super.greet();
来源：http://igv.jlsjyb.cn

TS:   super.greet();
来源：http://cnx.yuanzhike.top

Java: super.greet();
来源：http://ult.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezd.jinqigufen.top

Ruby: super
来源：http://qes.tanke756.top

C#:   base.Greet();
来源：http://kxk.hammf.cn

[G08] 静态方法与属性
来源：http://qzo.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kja.sjlbkw.cn

PHP:  public static function f() {}
来源：http://qza.ehwqpu.com

JS:   static f() {}
来源：http://oqj.yfazqb.com

TS:   static f(): void {}
来源：http://xzx.fehbvm.com

Java: static void f() {}
来源：http://jwa.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://duh.gaohongyu789.top

Ruby: def self.f; end
来源：http://fkc.ybcxt.top

C#:   public static void F() {}
来源：http://rbi.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://dhs.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://tul.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wbc.hesvh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fol.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://uea.fengsongda.top

Java: interface Shape { double area(); }
来源：http://aro.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://bfv.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uic.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://hry.svipenyu.cn

[G10] 访问控制
来源：http://lsf.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://tgt.fzhhl.top

PHP:  public / protected / private
来源：http://jcl.yj202588.top

JS:   #private 字段；其余公开
来源：http://lau.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://qqw.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://vee.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dmm.tanke756.top

Ruby: public / protected / private
来源：http://cbx.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://sxs.sweek.top

[G11] getter / setter
来源：http://kzs.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://tjw.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cwp.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://hvo.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://xbq.bjfxy.top

Java: public String getName() { return name; }
来源：http://hud.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mks.zdqjudy.top

Ruby: attr_accessor :name
来源：http://atg.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://npw.jinqigufen.top

[G12] 对象转字符串
来源：http://yqy.yonumen.top

Py:   def __str__(self): return self.name
来源：http://pjt.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qlf.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://yps.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://ezo.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://pfj.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://cpy.yuxming.cn

Ruby: def to_s; @name; end
来源：http://nxo.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://lkd.epnwcf.com

[G13] 判断对象类型
来源：http://eth.cheryme.top

Py:   isinstance(u, User)
来源：http://vpy.nwbrower.top

PHP:  $u instanceof User
来源：http://nml.yvedp.cn

JS:   u instanceof User
来源：http://nwa.yj202588.top

TS:   u instanceof User
来源：http://zzn.ydjk.org.cn

Java: u instanceof User
来源：http://zxs.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pnb.ivvv.top

Ruby: u.is_a?(User)
来源：http://cms.shuidangran.top

C#:   u is User
来源：http://vbb.wangshuangyany.cn

[G14] 数据类 / record
来源：http://rpb.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nbl.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ewr.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mey.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://yqc.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://ebt.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://ski.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qtw.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://epc.jianghu66.top

[G15] 枚举
来源：http://hnq.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iqu.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://chl.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ixy.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lau.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://rtz.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kfr.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://wvb.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rrr.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://gib.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mmu.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://gzs.dashuyun.cn

JS:   Object.entries(obj)
来源：http://vyy.nanxinkj.top

TS:   Object.entries(obj)
来源：http://qzq.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mjx.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://koe.9152youxi.cn

Ruby: obj.instance_variables
来源：http://mpt.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://zcc.xylfe.cn

================================================================================
来源：http://zos.fanxiaobao.xyz

H. 异常与错误处理
来源：http://chm.jinyuanbaomall.cn

================================================================================
来源：http://vjj.jinqigfzy.top

[H01] try / catch 基础
来源：http://gdm.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://non.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bof.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cns.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ykg.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://buk.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://knd.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vaq.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://smt.xinyue.icu

[H02] finally / ensure 收尾
来源：http://cmv.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://ymh.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhs.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://odm.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mtq.cdnleiting.top


<!-- 参考信息 -->