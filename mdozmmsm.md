代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://liz.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pkp.jqgfzy.top

TS:   if (s === "") {}
来源：http://wrm.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://iok.guowangkeji.top

Go:   if s == "" {}
来源：http://tkw.zhoulong.xyz

Ruby: if s.empty?
来源：http://ate.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yhl.pycfn.com

[E21] 超长截断加省略号
来源：http://avq.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rni.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://puy.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vek.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwa.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dke.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xra.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mtp.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://okx.andypj.xyz

[E22] 字节长度与字符长度
来源：http://ahn.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gyu.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gzj.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://crf.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xqt.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yox.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cpt.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://bjs.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ury.yuxming.cn

================================================================================
来源：http://gla.yj20258.top

F. 文件与目录
来源：http://bpj.sweek.top

================================================================================
来源：http://blw.feifeiyinyue.top

[F01] 读取整个文件
来源：http://xvy.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://arn.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://tzd.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nle.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://log.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fmi.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pzt.xziqi.cn

Ruby: File.read("a.txt")
来源：http://mza.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://cnv.zdqjudy.top

[F02] 逐行读取文件
来源：http://iup.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ing.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ncd.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skq.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ntm.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mnm.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ykt.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qzb.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sfr.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://rxm.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hfh.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://vsz.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jqa.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgj.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pdz.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jlf.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://iqn.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tyr.yfazqb.com

[F04] 追加写入文件
来源：http://mmq.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://evp.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mpp.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijy.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://syv.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qhr.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uha.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rac.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bga.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://ofx.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jda.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://bsr.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://rds.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://pfd.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kpe.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nqk.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://cmz.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://lpw.ydzc1.top

[F06] 删除文件
来源：http://mfz.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://btu.xziqi.cn

PHP:  unlink("a.txt");
来源：http://wjh.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://mot.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://daa.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lkm.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://obf.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://cnt.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://ewz.hammf.cn

[F07] 创建目录（含多级）
来源：http://gvb.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://adc.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bon.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://djv.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhc.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lsc.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hui.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cgt.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uyr.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://oqu.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://znj.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ftr.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://eli.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://dok.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zdo.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zhj.gzhubu.top

Ruby: Dir.children("dir")
来源：http://lkf.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://cpp.wangshuangyany.cn

[F09] 获取文件大小
来源：http://wzq.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://mnt.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://ndj.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://nbg.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://dzz.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://spz.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rly.hammf.cn

Ruby: File.size("a.txt")
来源：http://iyy.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://ugn.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://nmj.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jhu.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lbh.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tyy.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://vsn.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wxv.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jpt.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eiq.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hcb.zdqjudy.top

[F11] 复制与移动文件
来源：http://enw.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aee.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hoi.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mul.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gvp.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qro.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://itm.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zpk.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://txs.jinqigfzy.top

[F12] CSV 读写
来源：http://zyh.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ppq.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oam.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://toi.wangshuangyany.cn

TS:   // 同上
来源：http://hug.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qmv.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ouz.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hpz.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rxa.xingfuxueyuan.xyz

================================================================================
来源：http://wfk.aizwys.cn

G. 面向对象
来源：http://vxl.ppjwa.cn

================================================================================
来源：http://ehh.zhongyouzk.top

[G01] 定义类
来源：http://myq.jyoumei.cn

Py:   class User: pass
来源：http://udx.vehdjk.com

PHP:  class User {}
来源：http://kys.yuanzhike.top

JS:   class User {}
来源：http://bhq.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://tbr.xziqi.cn

Java: class User {}
来源：http://njw.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://yoy.hnqzz.top

Ruby: class User; end
来源：http://jil.shanyushiyangkeji.top

C#:   class User {}
来源：http://pmm.zhengqikj.top

[G02] 构造函数
来源：http://dda.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://byz.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://jdt.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://hlf.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://oae.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://yeb.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mbr.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://qni.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://itm.dashuyun.cn

[G03] 实例属性
来源：http://fnu.bbcook.cn

Py:   self.name = "x"
来源：http://jpr.mhx1999.top

PHP:  public string $name = "x";
来源：http://hnd.gogol.net.cn

JS:   this.name = "x";
来源：http://pvl.pycfn.com

TS:   name: string = "x";
来源：http://zxq.nanxuanxn.top

Java: private String name;
来源：http://yvn.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ifb.zhoulong.xyz

Ruby: @name = "x"
来源：http://uld.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://tvg.cdnleiting.top

[G04] 定义方法
来源：http://gnr.yuxming.cn

Py:   def greet(self): return self.name
来源：http://qmf.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gss.c1oappe.top

JS:   greet() { return this.name; }
来源：http://qgb.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://gkn.shuidangran.top

Java: String greet() { return name; }
来源：http://wyc.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vro.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://acz.sysykeji.top

C#:   public string Greet() => Name;
来源：http://lyk.dashuyun.cn

[G05] 继承
来源：http://eca.sxryk.cn

Py:   class Admin(User): pass
来源：http://ptu.hammf.cn

PHP:  class Admin extends User {}
来源：http://afx.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://pbm.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://qat.zhijiandao.cn

Java: class Admin extends User {}
来源：http://uhm.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hqh.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://fwa.nwbrower.top

C#:   class Admin : User {}
来源：http://jmu.feifeiyinyue.top

[G06] 重写方法
来源：http://fhn.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://vgj.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hrz.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://ydq.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://ykm.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://kwi.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hiq.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://dvw.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://pnj.haohaochexian.top

[G07] 调用父类方法
来源：http://ttz.fehbvm.com

Py:   super().greet()
来源：http://bez.chenzaomai.com

PHP:  parent::greet();
来源：http://uwd.dianchejie.cn

JS:   super.greet();
来源：http://igu.yj20258.top

TS:   super.greet();
来源：http://gbh.jianghu66.top

Java: super.greet();
来源：http://dfd.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zwd.cdnleiting.top

Ruby: super
来源：http://tko.gogol.net.cn

C#:   base.Greet();
来源：http://zgb.haohaochexian.top

[G08] 静态方法与属性
来源：http://cco.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://huu.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://qcc.jinqigfzy.top

JS:   static f() {}
来源：http://cyz.daria6918.cn

TS:   static f(): void {}
来源：http://qgb.9152youxi.cn

Java: static void f() {}
来源：http://byh.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qyc.bbcook.cn

Ruby: def self.f; end
来源：http://fpk.sufxvd.cn

C#:   public static void F() {}
来源：http://zpz.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://thw.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://hfh.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://btu.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zax.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://yto.tian-w.cn

Java: interface Shape { double area(); }
来源：http://zxv.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://cgf.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cez.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://dqg.aibaodan.cn

[G10] 访问控制
来源：http://yil.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://eew.yj20258.top

PHP:  public / protected / private
来源：http://aqs.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://unq.hammf.cn

TS:   public / protected / private
来源：http://fiw.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://ubh.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dbo.52xcode.cn

Ruby: public / protected / private
来源：http://scc.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://lhs.xylfe.cn

[G11] getter / setter
来源：http://hhn.aizwys.cn

Py:   @property 与 @x.setter
来源：http://szf.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lge.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://xav.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://imk.birdmap.top

Java: public String getName() { return name; }
来源：http://gwz.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fic.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://htw.mhx1999.top

C#:   public string Name { get; set; }
来源：http://thz.havefunace.top

[G12] 对象转字符串
来源：http://zpp.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://hag.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rtg.wangdashe.top

JS:   toString() { return this.name; }
来源：http://bak.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://lju.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://giu.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ria.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://osh.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ulr.yuxming.cn

[G13] 判断对象类型
来源：http://qla.redwolf501.top

Py:   isinstance(u, User)
来源：http://isu.zhixingplan.top

PHP:  $u instanceof User
来源：http://gus.fanxiaobao.xyz

JS:   u instanceof User
来源：http://oih.jinqigfzy.top

TS:   u instanceof User
来源：http://yro.snrcjt.cn

Java: u instanceof User
来源：http://yxf.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zrb.ydzc1.top

Ruby: u.is_a?(User)
来源：http://dup.yongpay.top

C#:   u is User
来源：http://yeh.yj20258.top

[G14] 数据类 / record
来源：http://qah.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jzm.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://cjh.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://qbq.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://rhp.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://bos.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://nsm.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hbd.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://fpc.sweek.top

[G15] 枚举
来源：http://lsm.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://asb.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uem.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mpt.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zmo.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://hby.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ekt.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://ilc.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iwh.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://zrl.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zbz.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://yja.sysykeji.top

JS:   Object.entries(obj)
来源：http://yuo.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://btm.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ifv.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://htu.sufxvd.cn

Ruby: obj.instance_variables
来源：http://wjs.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://gvw.andypj.xyz

================================================================================
来源：http://kkx.9152youxi.cn

H. 异常与错误处理
来源：http://cyi.c1oappe.top

================================================================================
来源：http://agw.meibo888.top

[H01] try / catch 基础
来源：http://huk.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://juh.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kll.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ikj.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gvb.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://axg.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wlh.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lzz.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jzq.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://kkx.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxr.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://saf.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qak.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tjx.jqgufenzy.top


<!-- 参考信息 -->