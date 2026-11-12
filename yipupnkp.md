代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hnk.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://vko.52xcode.cn

Java: s.lines().toList()
来源：http://akj.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://xne.hcnkem.com

Ruby: s.lines
来源：http://wlg.hesvh.cn

C#:   s.Split('\n')
来源：http://mgz.iojbl.cn

[E20] 判断字符串是否为空
来源：http://wfs.chenlongwang.top

Py:   if not s:
来源：http://fby.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lwv.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dfi.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://tmk.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://off.snrcjt.cn

Go:   if s == "" {}
来源：http://dov.cqqwz.cn

Ruby: if s.empty?
来源：http://uwy.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tnk.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://xdp.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gwo.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gja.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xoe.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwu.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://efi.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://icn.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ntb.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rui.guannengcc.top

[E22] 字节长度与字符长度
来源：http://vee.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jka.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txa.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rwi.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qwf.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://num.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xfh.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://cxp.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hss.shanyushiyangkeji.top

================================================================================
来源：http://kbz.mhx1999.top

F. 文件与目录
来源：http://sot.xziqi.cn

================================================================================
来源：http://jce.52xcode.cn

[F01] 读取整个文件
来源：http://zii.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ufw.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://cii.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://alg.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://llk.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tmc.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qlu.xuanzx.com

Ruby: File.read("a.txt")
来源：http://dip.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://zup.jianghu66.top

[F02] 逐行读取文件
来源：http://vqv.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://faz.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://esw.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihd.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kpp.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bsw.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://buv.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://erx.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yvg.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://dzu.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xpu.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kjb.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhi.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bss.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oif.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xod.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://dfj.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://itz.hongshengwenyu.top

[F04] 追加写入文件
来源：http://pnh.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vgo.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://syh.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hiy.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wsa.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rxs.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gbc.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jwg.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lwp.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://xzj.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://com.yj20258.top

PHP:  file_exists("a.txt");
来源：http://utq.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://yzs.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://veo.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rvi.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mst.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://zmj.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://tlx.hysaishi.cn

[F06] 删除文件
来源：http://knl.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://byz.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://mgl.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tiz.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://vjx.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mee.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://sor.tanke756.top

Ruby: File.delete("a.txt")
来源：http://wbf.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://smm.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://tdr.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://twv.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zaf.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://trg.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fdj.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://etj.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bzj.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cgp.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://prn.tian-w.cn

[F08] 遍历目录
来源：http://rhz.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mvd.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nqo.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://npv.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://aji.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cmx.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mef.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://vsl.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://mos.sweek.top

[F09] 获取文件大小
来源：http://prd.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://oex.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://vwt.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://atv.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://urb.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://iss.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cvn.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://mwf.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://uyu.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://vfc.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzb.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pev.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yaq.wangdashe.top

TS:   path.extname("a.txt")
来源：http://arc.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wpo.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gcr.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vfq.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fpg.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://lyl.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zte.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://puo.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ckn.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cdb.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fru.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gyp.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tgk.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tns.fanxiaobao.xyz

[F12] CSV 读写
来源：http://pow.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yvu.cqqwz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://llg.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hdc.sweek.top

TS:   // 同上
来源：http://snc.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ffa.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bna.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nin.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ahm.zhiwuduotai.top

================================================================================
来源：http://lqx.svipenyu.cn

G. 面向对象
来源：http://iiz.fzhhl.top

================================================================================
来源：http://jry.chenlongwang.top

[G01] 定义类
来源：http://eod.meibo888.top

Py:   class User: pass
来源：http://hua.andypj.xyz

PHP:  class User {}
来源：http://jdu.9152youxi.cn

JS:   class User {}
来源：http://gep.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://xvs.shuidangran.top

Java: class User {}
来源：http://xwh.tanke756.top

Go:   type User struct { Name string }
来源：http://aki.wangdashe.top

Ruby: class User; end
来源：http://flp.yvedp.cn

C#:   class User {}
来源：http://dpa.dashuyun.cn

[G02] 构造函数
来源：http://tar.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://ecg.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://pmq.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://huo.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://iob.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://len.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qdh.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://sri.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://xyz.ehwqpu.com

[G03] 实例属性
来源：http://usj.yj20258888.top

Py:   self.name = "x"
来源：http://rzt.zycfv.cn

PHP:  public string $name = "x";
来源：http://jcx.xuanzx.com

JS:   this.name = "x";
来源：http://lch.xuetiantiany.cn

TS:   name: string = "x";
来源：http://iyi.dashuyun.cn

Java: private String name;
来源：http://ute.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wsz.uphjek.com

Ruby: @name = "x"
来源：http://kdj.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://yjg.haohaochexian.top

[G04] 定义方法
来源：http://tih.xylfe.cn

Py:   def greet(self): return self.name
来源：http://fsq.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fit.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://cfp.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://ekz.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://bqf.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uhn.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://nbd.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://kfb.0kj1m.cn

[G05] 继承
来源：http://qsh.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://gzu.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://hbx.fktsv.cn

JS:   class Admin extends User {}
来源：http://rhe.xylfe.cn

TS:   class Admin extends User {}
来源：http://req.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://tsa.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lvn.gzhubu.top

Ruby: class Admin < User; end
来源：http://zea.jqgfzy.top

C#:   class Admin : User {}
来源：http://bzo.pengpengdd.cyou

[G06] 重写方法
来源：http://gbr.birdmap.top

Py:   def greet(self): return "admin"
来源：http://uvx.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://lkh.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://avw.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://oyi.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://osd.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nas.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://iai.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://zpo.wangshuangyany.cn

[G07] 调用父类方法
来源：http://vry.dashuyun.cn

Py:   super().greet()
来源：http://eue.bbcook.cn

PHP:  parent::greet();
来源：http://uqi.haohaochexian.top

JS:   super.greet();
来源：http://pdz.hfpthk.cn

TS:   super.greet();
来源：http://qwc.bjfxy.top

Java: super.greet();
来源：http://dsn.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://osn.hnqzz.top

Ruby: super
来源：http://guu.aibaodan.cn

C#:   base.Greet();
来源：http://kij.yongpay.top

[G08] 静态方法与属性
来源：http://vyh.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mgi.jqgfzy.top

PHP:  public static function f() {}
来源：http://oyz.shangyingyoupin.top

JS:   static f() {}
来源：http://ukw.sufxvd.cn

TS:   static f(): void {}
来源：http://qmb.zhiwuduotai.top

Java: static void f() {}
来源：http://paa.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ezu.yonumen.top

Ruby: def self.f; end
来源：http://nyr.hysaishi.cn

C#:   public static void F() {}
来源：http://myv.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://lhx.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://hmz.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://prv.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hcp.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://pou.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://tjo.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://dvr.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cig.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://efx.gotoacloud.top

[G10] 访问控制
来源：http://ius.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://yvn.gaohongyu789.top

PHP:  public / protected / private
来源：http://tps.tanke756.top

JS:   #private 字段；其余公开
来源：http://oqp.sysykeji.top

TS:   public / protected / private
来源：http://nld.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://ntf.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dit.yanxiufei.cn

Ruby: public / protected / private
来源：http://gaf.yangfankeji.com

C#:   public / protected / private / internal
来源：http://oln.xylfe.cn

[G11] getter / setter
来源：http://mxz.cashguo.top

Py:   @property 与 @x.setter
来源：http://wcv.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xrd.shuidangran.top

JS:   get name() { return this._name; }
来源：http://jhv.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://mpy.jiagoushi.top

Java: public String getName() { return name; }
来源：http://bfc.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://qfu.tanke756.top

Ruby: attr_accessor :name
来源：http://gme.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://akp.iojbl.cn

[G12] 对象转字符串
来源：http://fbm.cheryme.top

Py:   def __str__(self): return self.name
来源：http://gmu.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://zfu.yj202588.top

JS:   toString() { return this.name; }
来源：http://ite.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://xmw.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://xbh.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qga.tian-w.cn

Ruby: def to_s; @name; end
来源：http://jur.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://jjf.hesvh.cn

[G13] 判断对象类型
来源：http://wso.cucudq.cn

Py:   isinstance(u, User)
来源：http://ojb.mhx1999.top

PHP:  $u instanceof User
来源：http://neu.smart0.xyz

JS:   u instanceof User
来源：http://hwp.aizwys.cn

TS:   u instanceof User
来源：http://ted.tianlin.xyz

Java: u instanceof User
来源：http://ulr.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qsz.sxryk.cn

Ruby: u.is_a?(User)
来源：http://nkp.aibaodan.cn

C#:   u is User
来源：http://rkp.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://wsj.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zfn.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://kvr.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://lmy.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://aja.guannengcc.top

Java: record User(String name, int age) {}
来源：http://tsq.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://fzc.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eiz.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://oru.yanxiufei.cn

[G15] 枚举
来源：http://evv.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://asx.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xqp.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lfe.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rev.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://teg.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gca.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://ify.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iiz.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://pxq.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bgd.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://sgo.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://hrk.cdnleiting.top

TS:   Object.entries(obj)
来源：http://wfe.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bev.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rrm.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://bmq.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://yyw.zhengqikj.top

================================================================================
来源：http://xgt.svipenyu.cn

H. 异常与错误处理
来源：http://fqv.vehdjk.com

================================================================================
来源：http://cds.ctjpmb.com

[H01] try / catch 基础
来源：http://rms.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uco.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tjf.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nyi.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rru.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jju.cheryme.top


<!-- 参考信息 -->