代发 wailian999

Go:   if s == "" {}
来源：http://mtx.cashguo.top

Ruby: if s.empty?
来源：http://lhg.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sbv.daria6918.cn

[E21] 超长截断加省略号
来源：http://zjb.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kaa.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vyq.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsm.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sis.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://knu.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://wcv.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vmg.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lbm.bbcook.cn

[E22] 字节长度与字符长度
来源：http://tpw.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rxx.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://prs.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jnm.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://chu.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wsj.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://anx.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://owl.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vjn.hongshengwenyu.top

================================================================================
来源：http://uxc.yueranfly.top

F. 文件与目录
来源：http://ltu.haohaochexian.top

================================================================================
来源：http://pot.xinyue.icu

[F01] 读取整个文件
来源：http://jaj.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dwy.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://mag.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aqh.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rjx.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dtn.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://knv.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://lqb.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://cln.ivvv.top

[F02] 逐行读取文件
来源：http://crb.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nfp.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xnk.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://crv.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ats.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yqn.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vst.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xfm.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pfn.cashguo.top

[F03] 写入文件（覆盖）
来源：http://aha.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nql.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xon.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pmv.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdi.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sjn.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dic.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://jel.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hjh.hywenlv.cn

[F04] 追加写入文件
来源：http://ajo.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ofx.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://psd.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqg.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://euc.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mit.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tqe.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ykg.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pqu.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://xbx.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://isv.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://far.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://ikh.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://bxb.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qlk.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jft.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://pyc.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://hma.yonumen.top

[F06] 删除文件
来源：http://qbe.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://bdb.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://ole.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://von.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://typ.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zqh.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://jfz.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://bmr.meibo888.top

C#:   File.Delete("a.txt");
来源：http://zkq.epnwcf.com

[F07] 创建目录（含多级）
来源：http://uuo.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdt.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oom.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuw.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://snh.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zoi.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ecf.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nbf.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ujs.gotoacloud.top

[F08] 遍历目录
来源：http://jwf.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tdo.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dzy.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://ysn.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://led.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cgr.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://quy.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://vfv.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://jnd.tarul.cn

[F09] 获取文件大小
来源：http://uqk.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://vkv.fehbvm.com

PHP:  filesize("a.txt");
来源：http://cey.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://xkn.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://nbj.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uwf.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tvu.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://via.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://fal.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://sgq.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ava.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dmt.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://myj.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://lix.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mre.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nbu.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xag.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sjv.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://muh.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uio.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nrp.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxs.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mic.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hxz.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vjk.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bak.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mcf.andypj.xyz

[F12] CSV 读写
来源：http://jmh.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ojg.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://isg.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zor.andypj.xyz

TS:   // 同上
来源：http://lbm.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xip.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vjg.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxm.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://azt.fengsongda.top

================================================================================
来源：http://ifk.shzxlz.cn

G. 面向对象
来源：http://zzf.jianghu66.top

================================================================================
来源：http://idz.yangfankeji.com

[G01] 定义类
来源：http://rlx.zhaomingkeji.xyz

Py:   class User: pass
来源：http://aom.ydjk.org.cn

PHP:  class User {}
来源：http://lny.xuanzx.com

JS:   class User {}
来源：http://qnd.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://str.smart0.xyz

Java: class User {}
来源：http://bwt.zhengqikj.top

Go:   type User struct { Name string }
来源：http://coc.haohaochexian.top

Ruby: class User; end
来源：http://igl.birdmap.top

C#:   class User {}
来源：http://iqa.yj20258888.top

[G02] 构造函数
来源：http://peo.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://xyl.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://dzm.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://xbf.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://oky.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://aoq.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rsq.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://gut.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://aly.tanke756.top

[G03] 实例属性
来源：http://vsu.ydzc1.top

Py:   self.name = "x"
来源：http://dvt.redwolf501.top

PHP:  public string $name = "x";
来源：http://pnd.tianlin.xyz

JS:   this.name = "x";
来源：http://fon.chenjidiqi.icu

TS:   name: string = "x";
来源：http://alc.fktsv.cn

Java: private String name;
来源：http://mkz.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cmq.hnxiangtu.top

Ruby: @name = "x"
来源：http://jpx.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://jvz.jlsjyb.cn

[G04] 定义方法
来源：http://yka.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://soe.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tib.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://cvv.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://bai.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://vov.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ufn.jyoumei.cn

Ruby: def greet; @name; end
来源：http://iwr.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://sgc.fzhhl.top

[G05] 继承
来源：http://vip.hfpthk.cn

Py:   class Admin(User): pass
来源：http://zuj.smart0.xyz

PHP:  class Admin extends User {}
来源：http://ect.c1oappe.top

JS:   class Admin extends User {}
来源：http://hdw.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://olh.zdqjudy.top

Java: class Admin extends User {}
来源：http://njb.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pcr.cqqwz.cn

Ruby: class Admin < User; end
来源：http://otm.zycfv.cn

C#:   class Admin : User {}
来源：http://zlt.zhaomingkeji.xyz

[G06] 重写方法
来源：http://dls.sweek.top

Py:   def greet(self): return "admin"
来源：http://kga.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ovn.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://oha.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://iwl.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://yhs.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mcq.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://yem.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://mwp.jqgufenzy.top

[G07] 调用父类方法
来源：http://bml.ppjwa.cn

Py:   super().greet()
来源：http://xug.zhixingplan.top

PHP:  parent::greet();
来源：http://ymd.tarul.cn

JS:   super.greet();
来源：http://dse.yonumen.top

TS:   super.greet();
来源：http://jxa.uphjek.com

Java: super.greet();
来源：http://chj.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://por.kuanghao11.cn

Ruby: super
来源：http://ngo.snrcjt.cn

C#:   base.Greet();
来源：http://umh.bbcook.cn

[G08] 静态方法与属性
来源：http://xgh.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ksm.ybcxt.top

PHP:  public static function f() {}
来源：http://ori.xuanzx.com

JS:   static f() {}
来源：http://zpt.fktsv.cn

TS:   static f(): void {}
来源：http://eam.uphjek.com

Java: static void f() {}
来源：http://xuy.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qjg.zhijiandao.cn

Ruby: def self.f; end
来源：http://iip.zdqjudy.top

C#:   public static void F() {}
来源：http://foz.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://ihw.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://lsk.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://upm.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tuy.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://fzr.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://cgz.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://afu.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ywt.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://ypr.gzhubu.top

[G10] 访问控制
来源：http://qat.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://hzt.9152youxi.cn

PHP:  public / protected / private
来源：http://ghm.fengsongda.top

JS:   #private 字段；其余公开
来源：http://yif.fengsongda.top

TS:   public / protected / private
来源：http://jaq.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://dyl.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryf.aibaodan.cn

Ruby: public / protected / private
来源：http://cam.wangdashe.top

C#:   public / protected / private / internal
来源：http://dao.cdnleiting.top

[G11] getter / setter
来源：http://vsb.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://grp.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://omq.aizwys.cn

JS:   get name() { return this._name; }
来源：http://ytk.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://xlj.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://okg.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kjv.fzhhl.top

Ruby: attr_accessor :name
来源：http://gog.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://uqi.yuanzhike.top

[G12] 对象转字符串
来源：http://cmk.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://ale.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kip.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://hhn.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://akx.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://ske.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://pap.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://lec.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://nwp.nanxuanxn.top

[G13] 判断对象类型
来源：http://rnz.guannengcc.top

Py:   isinstance(u, User)
来源：http://lqi.hnxiangtu.top

PHP:  $u instanceof User
来源：http://puv.pengpengdd.cyou

JS:   u instanceof User
来源：http://pxo.ehwqpu.com

TS:   u instanceof User
来源：http://mpq.yj20258888.top

Java: u instanceof User
来源：http://wag.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qxa.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://mji.zdbjq.cn

C#:   u is User
来源：http://nto.ybcxt.top

[G14] 数据类 / record
来源：http://snk.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ixl.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cdg.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://snu.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://kdn.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://dpy.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://bte.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qsj.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://trn.cqqwz.cn

[G15] 枚举
来源：http://zuv.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qcc.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dat.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dnk.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ogy.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://amp.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ymv.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://dkq.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bbr.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://oqo.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kgn.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://eiv.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://egu.fzhhl.top

TS:   Object.entries(obj)
来源：http://mgt.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uho.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hpr.wangshuangyany.cn

Ruby: obj.instance_variables
来源：http://evp.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pgu.yvedp.cn

================================================================================
来源：http://yeo.feifeiyinyue.top

H. 异常与错误处理
来源：http://uir.cdnleiting.top

================================================================================
来源：http://aoe.fktsv.cn

[H01] try / catch 基础
来源：http://exs.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://utz.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yme.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://puz.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mxp.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xbl.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xoa.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dxb.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://edd.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://haf.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://rcs.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vbp.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oxd.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://vau.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mwm.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xlj.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mxx.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://rir.hammf.cn


<!-- 参考信息 -->