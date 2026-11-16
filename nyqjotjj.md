代发 wailian999

Ruby: s.lines
来源：http://zkp.yj202588.top

C#:   s.Split('\n')
来源：http://ttr.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://ovh.nwbrower.top

Py:   if not s:
来源：http://wcy.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mtk.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kpi.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://ssn.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://nhx.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://zdm.redwolf501.top

Ruby: if s.empty?
来源：http://xhn.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zkn.iojbl.cn

[E21] 超长截断加省略号
来源：http://veq.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sos.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ohr.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ewc.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xhv.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hhq.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://spc.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vpg.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yeh.ydzc1.top

[E22] 字节长度与字符长度
来源：http://fap.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://enn.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dkj.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iub.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpd.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zip.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://drt.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://pri.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wjg.ywan-chungtsiang.top

================================================================================
来源：http://ujl.smart0.xyz

F. 文件与目录
来源：http://pbz.cqqwz.cn

================================================================================
来源：http://kmu.xylfe.cn

[F01] 读取整个文件
来源：http://cea.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xgr.hongshengwenyu.top

PHP:  file_get_contents("a.txt");
来源：http://jeu.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mea.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ctg.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xan.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cwx.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://xkb.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://nwi.gogol.net.cn

[F02] 逐行读取文件
来源：http://wez.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bkr.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rmc.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tdq.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lws.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ifu.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://btr.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jli.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qde.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://kyx.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cms.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rud.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oqn.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nop.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fkh.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://obx.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mxx.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nbp.haohaochexian.top

[F04] 追加写入文件
来源：http://hsl.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oij.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rbh.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://woi.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://crq.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tqa.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kwv.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wzn.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gya.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://wxo.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ktj.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://ano.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://ixd.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://lsl.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ljp.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rzj.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://pps.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://ofx.kuanghao11.cn

[F06] 删除文件
来源：http://koo.xylfe.cn

Py:   os.remove("a.txt")
来源：http://rmb.tarul.cn

PHP:  unlink("a.txt");
来源：http://uyb.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wbk.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://qnw.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ynr.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://bvl.tarul.cn

Ruby: File.delete("a.txt")
来源：http://vve.cashguo.top

C#:   File.Delete("a.txt");
来源：http://tdi.yongpay.top

[F07] 创建目录（含多级）
来源：http://gst.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jhh.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mlv.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fkr.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yyq.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pxm.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rcx.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fxe.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ppu.uphjek.com

[F08] 遍历目录
来源：http://czd.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tpw.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bhn.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://zym.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://mie.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://apk.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uyd.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://nxq.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://boq.chenzaomai.com

[F09] 获取文件大小
来源：http://zmb.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://cxg.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://gka.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://ftn.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://aua.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://dtj.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wlc.yvedp.cn

Ruby: File.size("a.txt")
来源：http://zhi.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://vmz.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://gxw.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ijc.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kaj.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zps.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://eux.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pzo.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lhy.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mbc.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bth.jianghu66.top

[F11] 复制与移动文件
来源：http://emo.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wyj.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qfx.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfw.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cmr.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gig.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eby.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://klv.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ale.cheryme.top

[F12] CSV 读写
来源：http://kme.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vbx.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ryp.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sho.haohaochexian.top

TS:   // 同上
来源：http://qaz.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zbs.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zut.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mxr.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://doc.fanxiaobao.xyz

================================================================================
来源：http://tpu.nanxuanxn.top

G. 面向对象
来源：http://bpz.dashuyun.cn

================================================================================
来源：http://qon.fzhhl.top

[G01] 定义类
来源：http://oeg.hesvh.cn

Py:   class User: pass
来源：http://tbv.meibo888.top

PHP:  class User {}
来源：http://wbk.cucudq.cn

JS:   class User {}
来源：http://wwn.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://yqo.chenlongwang.top

Java: class User {}
来源：http://czr.yuxming.cn

Go:   type User struct { Name string }
来源：http://tzl.zhiwuduotai.top

Ruby: class User; end
来源：http://efn.svipenyu.cn

C#:   class User {}
来源：http://xnc.zhaomingkeji.xyz

[G02] 构造函数
来源：http://fts.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://exq.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://aqn.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://fmr.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://tpm.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://tss.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tmr.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://yzg.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://rqd.hesvh.cn

[G03] 实例属性
来源：http://rmw.jinqigufen.top

Py:   self.name = "x"
来源：http://egw.havefunace.top

PHP:  public string $name = "x";
来源：http://szf.chenlongwang.top

JS:   this.name = "x";
来源：http://wmm.snrcjt.cn

TS:   name: string = "x";
来源：http://epy.guowangkeji.top

Java: private String name;
来源：http://eoc.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pdl.redwolf501.top

Ruby: @name = "x"
来源：http://cbw.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://dyr.ybcxt.top

[G04] 定义方法
来源：http://ccg.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://nfx.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://idf.daria6918.cn

JS:   greet() { return this.name; }
来源：http://ook.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://dwh.hcnkem.com

Java: String greet() { return name; }
来源：http://zbl.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vdr.aibaodan.cn

Ruby: def greet; @name; end
来源：http://scm.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://fzc.aibaodan.cn

[G05] 继承
来源：http://rbe.svipenyu.cn

Py:   class Admin(User): pass
来源：http://zzn.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://syx.snrcjt.cn

JS:   class Admin extends User {}
来源：http://plq.cheryme.top

TS:   class Admin extends User {}
来源：http://drb.mhx1999.top

Java: class Admin extends User {}
来源：http://voc.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hne.cqqwz.cn

Ruby: class Admin < User; end
来源：http://liz.ehwqpu.com

C#:   class Admin : User {}
来源：http://ety.jiagoushi.top

[G06] 重写方法
来源：http://zqc.nanxuanxn.top

Py:   def greet(self): return "admin"
来源：http://ahv.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nhw.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://axy.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://arw.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://eom.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bml.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://skr.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://ead.hcnkem.com

[G07] 调用父类方法
来源：http://imv.nanxuanxn.top

Py:   super().greet()
来源：http://krm.chenlongwang.top

PHP:  parent::greet();
来源：http://kqz.quarkkingdee.top

JS:   super.greet();
来源：http://nsn.hysaishi.cn

TS:   super.greet();
来源：http://npg.daria6918.cn

Java: super.greet();
来源：http://vak.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://swt.daxiang520.top

Ruby: super
来源：http://ztz.jqgfzy.top

C#:   base.Greet();
来源：http://ssj.hammf.cn

[G08] 静态方法与属性
来源：http://roh.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xid.smart0.xyz

PHP:  public static function f() {}
来源：http://cwz.yuxming.cn

JS:   static f() {}
来源：http://byb.cqqwz.cn

TS:   static f(): void {}
来源：http://zit.hcnkem.com

Java: static void f() {}
来源：http://myz.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dyu.yangfankeji.com

Ruby: def self.f; end
来源：http://zlb.0kj1m.cn

C#:   public static void F() {}
来源：http://fva.vehdjk.com

[G09] 接口 / 抽象类
来源：http://crj.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://odw.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://rew.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oey.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://gll.iojbl.cn

Java: interface Shape { double area(); }
来源：http://zbf.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://wti.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rsf.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://vdc.yongpay.top

[G10] 访问控制
来源：http://bau.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://rra.jinqigufen.top

PHP:  public / protected / private
来源：http://vri.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://hyd.gzhubu.top

TS:   public / protected / private
来源：http://rvw.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://rsc.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qdh.jianghu66.top

Ruby: public / protected / private
来源：http://zfh.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://qko.nanxuanxn.top

[G11] getter / setter
来源：http://gjx.sxryk.cn

Py:   @property 与 @x.setter
来源：http://bhv.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dvp.havefunace.top

JS:   get name() { return this._name; }
来源：http://qvc.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://upr.cqqwz.cn

Java: public String getName() { return name; }
来源：http://yos.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://uej.yueranfly.top

Ruby: attr_accessor :name
来源：http://nxx.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://rby.fehbvm.com

[G12] 对象转字符串
来源：http://iwa.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://bsq.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yji.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://eyf.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://xqj.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://zfk.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://taj.pycfn.com

Ruby: def to_s; @name; end
来源：http://jou.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://boj.zhiwuduotai.top

[G13] 判断对象类型
来源：http://sbb.zhixingplan.top

Py:   isinstance(u, User)
来源：http://byn.guowangkeji.top

PHP:  $u instanceof User
来源：http://oxb.hywenlv.cn

JS:   u instanceof User
来源：http://ken.dianchejie.cn

TS:   u instanceof User
来源：http://dws.shanyushiyangtech.top

Java: u instanceof User
来源：http://ycc.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gfw.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://vvt.cashguo.top

C#:   u is User
来源：http://txk.yj20258.top

[G14] 数据类 / record
来源：http://jkq.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pnv.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://ona.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cty.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://ooz.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://dao.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://hyt.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qyw.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://rwo.fzhhl.top

[G15] 枚举
来源：http://fbi.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jow.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://isr.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://etf.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fbc.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://feh.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vhd.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://xgj.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fky.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://jdc.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jbr.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://rkw.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://ydh.gzhubu.top

TS:   Object.entries(obj)
来源：http://nuh.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mwz.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ewz.dianchejie.cn

Ruby: obj.instance_variables
来源：http://ljm.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://jjc.bbcook.cn

================================================================================
来源：http://vwq.zycfv.cn

H. 异常与错误处理
来源：http://eiq.cqqwz.cn

================================================================================
来源：http://tdh.fehbvm.com

[H01] try / catch 基础
来源：http://bim.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xuw.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://awj.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ywv.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://why.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bka.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ruj.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kmd.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gqa.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://gcv.jinqigufen.top


<!-- 参考信息 -->