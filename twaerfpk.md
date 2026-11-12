代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://iog.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://phn.vehdjk.com

Java: s.lines().toList()
来源：http://ooz.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://acq.tian-w.cn

Ruby: s.lines
来源：http://lir.hysaishi.cn

C#:   s.Split('\n')
来源：http://xou.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://lry.316326.xyz

Py:   if not s:
来源：http://ylz.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wqe.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ufv.shanyushiyangtech.top

TS:   if (s === "") {}
来源：http://mjl.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://qks.ehwqpu.com

Go:   if s == "" {}
来源：http://unr.xziqi.cn

Ruby: if s.empty?
来源：http://aur.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wqu.0kj1m.cn

[E21] 超长截断加省略号
来源：http://mjg.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://glo.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypm.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ybz.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xov.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qmq.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://nlg.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dlo.zhengqikj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://puw.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://pxp.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rbn.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxk.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ity.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qti.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rrn.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vgu.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://mqr.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cpv.cqqwz.cn

================================================================================
来源：http://ymi.jinqigufen.top

F. 文件与目录
来源：http://rvw.haohaochexian.top

================================================================================
来源：http://sfd.jinqigufen.top

[F01] 读取整个文件
来源：http://oil.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xbk.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://bqb.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mus.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tnv.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sls.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pul.iojbl.cn

Ruby: File.read("a.txt")
来源：http://dof.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://evk.vqdsnc.cn

[F02] 逐行读取文件
来源：http://jvh.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jcg.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sdw.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sit.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhe.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ilc.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vex.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ims.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vnl.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://rrv.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bei.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vep.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrz.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkj.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ets.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://klb.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://xdx.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xmr.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://xav.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iue.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qlm.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtt.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jem.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oab.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fnj.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://egc.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vaq.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://qtw.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dou.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://gdd.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://ygr.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://gtq.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lfs.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://amq.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://sjc.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://vcy.zycfv.cn

[F06] 删除文件
来源：http://jqg.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://oji.yongpay.top

PHP:  unlink("a.txt");
来源：http://gis.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vyi.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://lwt.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iki.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://mnc.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://ekq.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://wpp.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://asv.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cqx.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ssz.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uta.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cjg.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qiw.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mnn.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ghu.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cgh.0kj1m.cn

[F08] 遍历目录
来源：http://fuh.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kun.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gng.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://eol.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://yjz.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xva.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://lqn.yongpay.top

Ruby: Dir.children("dir")
来源：http://bmi.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://fch.xuanzx.com

[F09] 获取文件大小
来源：http://wrm.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://vrh.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://mho.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://bqc.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://etk.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://apd.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://red.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://imf.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://qlr.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://ukq.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wvo.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qwx.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ttj.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://jnz.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://onb.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ljs.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gdq.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ykg.snrcjt.cn

[F11] 复制与移动文件
来源：http://glw.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://isq.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gsy.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ebo.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zkg.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsg.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tqm.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jso.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ygx.52xcode.cn

[F12] CSV 读写
来源：http://fbk.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zlj.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jur.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kgb.kuanghao11.cn

TS:   // 同上
来源：http://vja.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mrb.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ltw.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zox.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://osw.nwbrower.top

================================================================================
来源：http://ssi.sjlbkw.cn

G. 面向对象
来源：http://ahu.ctjpmb.com

================================================================================
来源：http://ljz.hnxiangtu.top

[G01] 定义类
来源：http://fpz.zdbjq.cn

Py:   class User: pass
来源：http://ttu.jlsjyb.cn

PHP:  class User {}
来源：http://aoi.ywan-chungtsiang.top

JS:   class User {}
来源：http://vak.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://vzp.dianchejie.cn

Java: class User {}
来源：http://prq.cdnleiting.top

Go:   type User struct { Name string }
来源：http://emr.shangyingyoupin.top

Ruby: class User; end
来源：http://kzv.hnqzz.top

C#:   class User {}
来源：http://znq.shzxlz.cn

[G02] 构造函数
来源：http://won.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wqq.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://bck.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://yxs.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://diz.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://fpp.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aag.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://vfh.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://fon.yfazqb.com

[G03] 实例属性
来源：http://eoz.gotoacloud.top

Py:   self.name = "x"
来源：http://yfv.yfazqb.com

PHP:  public string $name = "x";
来源：http://qxb.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://fuy.chenlongwang.top

TS:   name: string = "x";
来源：http://ohp.daria6918.cn

Java: private String name;
来源：http://lsh.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tcl.andypj.xyz

Ruby: @name = "x"
来源：http://jvi.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://njt.bbcook.cn

[G04] 定义方法
来源：http://fnn.fengsongda.top

Py:   def greet(self): return self.name
来源：http://yld.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zol.xuanzx.com

JS:   greet() { return this.name; }
来源：http://mzi.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://iyp.yongpay.top

Java: String greet() { return name; }
来源：http://gzt.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pde.bjfxy.top

Ruby: def greet; @name; end
来源：http://avo.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://jpu.sxryk.cn

[G05] 继承
来源：http://gfx.xylfe.cn

Py:   class Admin(User): pass
来源：http://gav.uphjek.com

PHP:  class Admin extends User {}
来源：http://chf.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://cfs.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://vxz.hnqzz.top

Java: class Admin extends User {}
来源：http://fki.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sgf.yj202588.top

Ruby: class Admin < User; end
来源：http://ehl.ydzc1.top

C#:   class Admin : User {}
来源：http://cdr.yj202588.top

[G06] 重写方法
来源：http://kki.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://ubg.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yor.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://ovj.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://von.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://wlm.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://irr.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://pbh.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://vec.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://zhc.yvedp.cn

Py:   super().greet()
来源：http://uwa.quarkkingdee.top

PHP:  parent::greet();
来源：http://vje.jqgfzy.top

JS:   super.greet();
来源：http://cao.cucudq.cn

TS:   super.greet();
来源：http://byn.tarul.cn

Java: super.greet();
来源：http://iti.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://llv.sysykeji.top

Ruby: super
来源：http://irb.shangyingyoupin.top

C#:   base.Greet();
来源：http://nhl.hywenlv.cn

[G08] 静态方法与属性
来源：http://zmb.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mea.gogol.net.cn

PHP:  public static function f() {}
来源：http://bpp.dashuyun.cn

JS:   static f() {}
来源：http://dol.yanxiufei.cn

TS:   static f(): void {}
来源：http://iyn.zhaomingkeji.xyz

Java: static void f() {}
来源：http://yjw.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://obs.fktsv.cn

Ruby: def self.f; end
来源：http://zod.fehbvm.com

C#:   public static void F() {}
来源：http://zxr.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://prn.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://fsy.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://hsu.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xuv.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://sts.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://sod.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://atz.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ywi.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://xvl.9152youxi.cn

[G10] 访问控制
来源：http://zmk.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://nsb.birdmap.top

PHP:  public / protected / private
来源：http://csq.aizwys.cn

JS:   #private 字段；其余公开
来源：http://trq.yfazqb.com

TS:   public / protected / private
来源：http://khs.yonumen.top

Java: public / protected / private / 默认包级
来源：http://mjp.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://szp.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://pun.chenzaomai.com

C#:   public / protected / private / internal
来源：http://nap.tian-w.cn

[G11] getter / setter
来源：http://wel.yfazqb.com

Py:   @property 与 @x.setter
来源：http://nam.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://aqt.mhx1999.top

JS:   get name() { return this._name; }
来源：http://vkv.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://fft.ivvv.top

Java: public String getName() { return name; }
来源：http://cyi.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rfn.bbcook.cn

Ruby: attr_accessor :name
来源：http://nly.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://wyr.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://tqw.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://apc.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ido.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://urf.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://znj.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://dgm.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://ehl.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://feb.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://fbg.pengpengdd.cyou

[G13] 判断对象类型
来源：http://vyw.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://vhu.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://njv.feifeiyinyue.top

JS:   u instanceof User
来源：http://shq.yonumen.top

TS:   u instanceof User
来源：http://dmy.sufxvd.cn

Java: u instanceof User
来源：http://bwl.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dup.wangdashe.top

Ruby: u.is_a?(User)
来源：http://kmk.daxiang520.top

C#:   u is User
来源：http://hyy.hnqzz.top

[G14] 数据类 / record
来源：http://djh.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zdt.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://qvs.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fsh.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://jnr.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://jcb.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://tlf.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lle.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://pxy.xinyue.icu

[G15] 枚举
来源：http://sbv.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vgs.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zrv.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kis.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mpj.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://ukz.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eoh.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://cjj.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yun.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://pdp.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://elo.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://ftl.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://ymg.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://cau.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qfw.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ftg.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://uho.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://iky.pycfn.com

================================================================================
来源：http://bpd.feifeiyinyue.top

H. 异常与错误处理
来源：http://mzd.ctjpmb.com

================================================================================
来源：http://gfw.cdnleiting.top

[H01] try / catch 基础
来源：http://fyc.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sqe.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qdx.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ttf.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wkk.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://phi.feifeiyinyue.top


<!-- 参考信息 -->